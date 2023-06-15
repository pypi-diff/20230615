# Comparing `tmp/deepomatic-rpc-0.8.8.tar.gz` & `tmp/deepomatic-rpc-0.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/deepomatic-rpc-0.8.8.tar", last modified: Mon Jun  7 17:42:23 2021, max compression
+gzip compressed data, was "dist/deepomatic-rpc-0.8.9.tar", last modified: Tue Aug  3 14:07:04 2021, max compression
```

## Comparing `deepomatic-rpc-0.8.8.tar` & `deepomatic-rpc-0.8.9.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-07 17:42:23.000000 deepomatic-rpc-0.8.8/
--rw-r--r--   0 root         (0) root         (0)    12037 2021-06-07 17:42:23.000000 deepomatic-rpc-0.8.8/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-07 17:42:23.000000 deepomatic-rpc-0.8.8/deepomatic/
--rw-r--r--   0 root         (0) root         (0)      170 2019-03-07 11:41:56.000000 deepomatic-rpc-0.8.8/deepomatic/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-07 17:42:23.000000 deepomatic-rpc-0.8.8/deepomatic/rpc/
--rw-rw-r--   0 root         (0) root         (0)      304 2021-06-07 17:20:34.000000 deepomatic-rpc-0.8.8/deepomatic/rpc/version.py
--rw-r--r--   0 root         (0) root         (0)      360 2019-04-01 11:57:21.000000 deepomatic-rpc-0.8.8/deepomatic/rpc/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-07 17:42:23.000000 deepomatic-rpc-0.8.8/deepomatic/rpc/grpc/
--rw-r--r--   0 root         (0) root         (0)      530 2020-10-14 10:01:19.000000 deepomatic-rpc-0.8.8/deepomatic/rpc/grpc/workflow_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2020-10-14 10:01:19.000000 deepomatic-rpc-0.8.8/deepomatic/rpc/grpc/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1288 2019-04-01 11:57:21.000000 deepomatic-rpc-0.8.8/deepomatic/rpc/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-07 17:42:23.000000 deepomatic-rpc-0.8.8/deepomatic/rpc/buffers/
--rw-r--r--   0 root         (0) root         (0)        0 2021-06-07 17:42:22.000000 deepomatic-rpc-0.8.8/deepomatic/rpc/buffers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-07 17:42:23.000000 deepomatic-rpc-0.8.8/deepomatic/rpc/buffers/protobuf/
--rw-r--r--   0 root         (0) root         (0)        0 2021-06-07 17:42:22.000000 deepomatic-rpc-0.8.8/deepomatic/rpc/buffers/protobuf/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-07 17:42:23.000000 deepomatic-rpc-0.8.8/deepomatic/rpc/buffers/protobuf/workflows/
--rw-r--r--   0 root         (0) root         (0)     4941 2021-06-07 17:42:22.000000 deepomatic-rpc-0.8.8/deepomatic/rpc/buffers/protobuf/workflows/WorkflowExecution_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    24704 2021-06-07 17:42:22.000000 deepomatic-rpc-0.8.8/deepomatic/rpc/buffers/protobuf/workflows/Workflow_pb2.py
--rw-r--r--   0 root         (0) root         (0)    15974 2021-06-07 17:42:22.000000 deepomatic-rpc-0.8.8/deepomatic/rpc/buffers/protobuf/workflows/WorkflowExecution_pb2.py
--rw-r--r--   0 root         (0) root         (0)        0 2021-06-07 17:42:22.000000 deepomatic-rpc-0.8.8/deepomatic/rpc/buffers/protobuf/workflows/__init__.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-06-07 17:42:22.000000 deepomatic-rpc-0.8.8/deepomatic/rpc/buffers/protobuf/workflows/Workflow_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-07 17:42:23.000000 deepomatic-rpc-0.8.8/deepomatic/rpc/buffers/protobuf/common/
--rw-r--r--   0 root         (0) root         (0)     3027 2021-06-07 17:42:22.000000 deepomatic-rpc-0.8.8/deepomatic/rpc/buffers/protobuf/common/Error_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-06-07 17:42:22.000000 deepomatic-rpc-0.8.8/deepomatic/rpc/buffers/protobuf/common/Image_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)        0 2021-06-07 17:42:22.000000 deepomatic-rpc-0.8.8/deepomatic/rpc/buffers/protobuf/common/__init__.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-06-07 17:42:22.000000 deepomatic-rpc-0.8.8/deepomatic/rpc/buffers/protobuf/common/Error_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     5088 2021-06-07 17:42:22.000000 deepomatic-rpc-0.8.8/deepomatic/rpc/buffers/protobuf/common/Image_pb2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-07 17:42:23.000000 deepomatic-rpc-0.8.8/deepomatic/rpc/buffers/protobuf/cli/
--rw-r--r--   0 root         (0) root         (0)      159 2021-06-07 17:42:22.000000 deepomatic-rpc-0.8.8/deepomatic/rpc/buffers/protobuf/cli/Message_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)        0 2021-06-07 17:42:22.000000 deepomatic-rpc-0.8.8/deepomatic/rpc/buffers/protobuf/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5277 2021-06-07 17:42:22.000000 deepomatic-rpc-0.8.8/deepomatic/rpc/buffers/protobuf/cli/Message_pb2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-07 17:42:23.000000 deepomatic-rpc-0.8.8/deepomatic/rpc/buffers/protobuf/nn/
--rw-r--r--   0 root         (0) root         (0)      159 2021-06-07 17:42:22.000000 deepomatic-rpc-0.8.8/deepomatic/rpc/buffers/protobuf/nn/Message_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-06-07 17:42:22.000000 deepomatic-rpc-0.8.8/deepomatic/rpc/buffers/protobuf/nn/Preprocessing_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    49868 2021-06-07 17:42:22.000000 deepomatic-rpc-0.8.8/deepomatic/rpc/buffers/protobuf/nn/Postprocessing_pb2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-07 17:42:23.000000 deepomatic-rpc-0.8.8/deepomatic/rpc/buffers/protobuf/nn/frameworks/
--rw-r--r--   0 root         (0) root         (0)      159 2021-06-07 17:42:22.000000 deepomatic-rpc-0.8.8/deepomatic/rpc/buffers/protobuf/nn/frameworks/Caffe_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)        0 2021-06-07 17:42:22.000000 deepomatic-rpc-0.8.8/deepomatic/rpc/buffers/protobuf/nn/frameworks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7818 2021-06-07 17:42:22.000000 deepomatic-rpc-0.8.8/deepomatic/rpc/buffers/protobuf/nn/frameworks/Caffe_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4720 2021-06-07 17:42:22.000000 deepomatic-rpc-0.8.8/deepomatic/rpc/buffers/protobuf/nn/Result_pb2.py
--rw-r--r--   0 root         (0) root         (0)    24311 2021-06-07 17:42:22.000000 deepomatic-rpc-0.8.8/deepomatic/rpc/buffers/protobuf/nn/Preprocessing_pb2.py
--rw-r--r--   0 root         (0) root         (0)    14567 2021-06-07 17:42:22.000000 deepomatic-rpc-0.8.8/deepomatic/rpc/buffers/protobuf/nn/Command_pb2.py
--rw-r--r--   0 root         (0) root         (0)        0 2021-06-07 17:42:22.000000 deepomatic-rpc-0.8.8/deepomatic/rpc/buffers/protobuf/nn/__init__.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-06-07 17:42:22.000000 deepomatic-rpc-0.8.8/deepomatic/rpc/buffers/protobuf/nn/Postprocessing_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-06-07 17:42:22.000000 deepomatic-rpc-0.8.8/deepomatic/rpc/buffers/protobuf/nn/Command_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-06-07 17:42:22.000000 deepomatic-rpc-0.8.8/deepomatic/rpc/buffers/protobuf/nn/Result_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-07 17:42:23.000000 deepomatic-rpc-0.8.8/deepomatic/rpc/buffers/protobuf/nn/v07/
--rw-r--r--   0 root         (0) root         (0)    20640 2021-06-07 17:42:22.000000 deepomatic-rpc-0.8.8/deepomatic/rpc/buffers/protobuf/nn/v07/Results_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-06-07 17:42:22.000000 deepomatic-rpc-0.8.8/deepomatic/rpc/buffers/protobuf/nn/v07/Results_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     4861 2021-06-07 17:42:22.000000 deepomatic-rpc-0.8.8/deepomatic/rpc/buffers/protobuf/nn/v07/Commands_pb2.py
--rw-r--r--   0 root         (0) root         (0)        0 2021-06-07 17:42:22.000000 deepomatic-rpc-0.8.8/deepomatic/rpc/buffers/protobuf/nn/v07/__init__.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-06-07 17:42:22.000000 deepomatic-rpc-0.8.8/deepomatic/rpc/buffers/protobuf/nn/v07/Inputs_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     7434 2021-06-07 17:42:22.000000 deepomatic-rpc-0.8.8/deepomatic/rpc/buffers/protobuf/nn/v07/Inputs_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-06-07 17:42:22.000000 deepomatic-rpc-0.8.8/deepomatic/rpc/buffers/protobuf/nn/v07/Workflows_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    14190 2021-06-07 17:42:22.000000 deepomatic-rpc-0.8.8/deepomatic/rpc/buffers/protobuf/nn/v07/Workflows_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-06-07 17:42:22.000000 deepomatic-rpc-0.8.8/deepomatic/rpc/buffers/protobuf/nn/v07/Commands_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     3812 2021-06-07 17:42:22.000000 deepomatic-rpc-0.8.8/deepomatic/rpc/buffers/protobuf/nn/Message_pb2.py
--rw-r--r--   0 root         (0) root         (0)      218 2019-04-01 11:57:21.000000 deepomatic-rpc-0.8.8/deepomatic/rpc/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-07 17:42:23.000000 deepomatic-rpc-0.8.8/deepomatic/rpc/amqp/
--rw-r--r--   0 root         (0) root         (0)      401 2020-02-07 17:54:29.000000 deepomatic-rpc-0.8.8/deepomatic/rpc/amqp/exceptions.py
--rw-r--r--   0 root         (0) root         (0)    26340 2020-02-07 17:54:29.000000 deepomatic-rpc-0.8.8/deepomatic/rpc/amqp/client.py
--rw-r--r--   0 root         (0) root         (0)      221 2020-02-07 17:54:29.000000 deepomatic-rpc-0.8.8/deepomatic/rpc/amqp/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13305 2020-02-07 17:54:29.000000 deepomatic-rpc-0.8.8/deepomatic/rpc/amqp/entities.py
--rw-r--r--   0 root         (0) root         (0)     3189 2019-04-01 11:57:21.000000 deepomatic-rpc-0.8.8/deepomatic/rpc/response.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-07 17:42:23.000000 deepomatic-rpc-0.8.8/deepomatic/rpc/helpers/
--rw-r--r--   0 root         (0) root         (0)     1031 2019-09-27 13:38:53.000000 deepomatic-rpc-0.8.8/deepomatic/rpc/helpers/v07_proto.py
--rw-r--r--   0 root         (0) root         (0)      229 2019-04-01 11:57:21.000000 deepomatic-rpc-0.8.8/deepomatic/rpc/helpers/common.py
--rw-r--r--   0 root         (0) root         (0)        0 2019-04-01 11:57:21.000000 deepomatic-rpc-0.8.8/deepomatic/rpc/helpers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2618 2019-04-01 11:57:21.000000 deepomatic-rpc-0.8.8/deepomatic/rpc/helpers/proto.py
--rw-r--r--   0 root         (0) root         (0)       38 2021-06-07 17:42:23.000000 deepomatic-rpc-0.8.8/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-07 17:42:23.000000 deepomatic-rpc-0.8.8/deepomatic_rpc.egg-info/
--rw-r--r--   0 root         (0) root         (0)       69 2021-06-07 17:42:23.000000 deepomatic-rpc-0.8.8/deepomatic_rpc.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2021-06-07 17:42:23.000000 deepomatic-rpc-0.8.8/deepomatic_rpc.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)    12037 2021-06-07 17:42:23.000000 deepomatic-rpc-0.8.8/deepomatic_rpc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       11 2021-06-07 17:42:23.000000 deepomatic-rpc-0.8.8/deepomatic_rpc.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-06-07 17:42:23.000000 deepomatic-rpc-0.8.8/deepomatic_rpc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     2876 2021-06-07 17:42:23.000000 deepomatic-rpc-0.8.8/deepomatic_rpc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2019-04-01 11:57:21.000000 deepomatic-rpc-0.8.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)       20 2020-10-14 10:01:19.000000 deepomatic-rpc-0.8.8/requirements.txt
--rw-r--r--   0 root         (0) root         (0)     9358 2020-02-18 17:31:26.000000 deepomatic-rpc-0.8.8/README.md
--rwxrwxr-x   0 root         (0) root         (0)     1988 2021-06-07 17:17:48.000000 deepomatic-rpc-0.8.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-03 14:07:04.000000 deepomatic-rpc-0.8.9/
+-rw-r--r--   0 root         (0) root         (0)       38 2021-08-03 14:07:04.000000 deepomatic-rpc-0.8.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)        1 2021-05-24 15:03:49.000000 deepomatic-rpc-0.8.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     9358 2021-05-24 15:03:49.000000 deepomatic-rpc-0.8.9/README.md
+-rw-r--r--   0 root         (0) root         (0)    12037 2021-08-03 14:07:04.000000 deepomatic-rpc-0.8.9/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-03 14:07:04.000000 deepomatic-rpc-0.8.9/deepomatic_rpc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2876 2021-08-03 14:07:04.000000 deepomatic-rpc-0.8.9/deepomatic_rpc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2021-08-03 14:07:04.000000 deepomatic-rpc-0.8.9/deepomatic_rpc.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2021-08-03 14:07:04.000000 deepomatic-rpc-0.8.9/deepomatic_rpc.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)    12037 2021-08-03 14:07:04.000000 deepomatic-rpc-0.8.9/deepomatic_rpc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        1 2021-08-03 14:07:04.000000 deepomatic-rpc-0.8.9/deepomatic_rpc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       69 2021-08-03 14:07:04.000000 deepomatic-rpc-0.8.9/deepomatic_rpc.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2021-05-24 15:03:49.000000 deepomatic-rpc-0.8.9/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-03 14:07:04.000000 deepomatic-rpc-0.8.9/deepomatic/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-03 14:07:04.000000 deepomatic-rpc-0.8.9/deepomatic/rpc/
+-rw-r--r--   0 root         (0) root         (0)      218 2021-05-24 15:03:49.000000 deepomatic-rpc-0.8.9/deepomatic/rpc/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-03 14:07:04.000000 deepomatic-rpc-0.8.9/deepomatic/rpc/grpc/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-05-24 15:03:49.000000 deepomatic-rpc-0.8.9/deepomatic/rpc/grpc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      530 2021-05-24 15:03:49.000000 deepomatic-rpc-0.8.9/deepomatic/rpc/grpc/workflow_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-03 14:07:04.000000 deepomatic-rpc-0.8.9/deepomatic/rpc/helpers/
+-rw-r--r--   0 root         (0) root         (0)      229 2021-05-24 15:03:49.000000 deepomatic-rpc-0.8.9/deepomatic/rpc/helpers/common.py
+-rw-r--r--   0 root         (0) root         (0)        0 2021-05-24 15:03:49.000000 deepomatic-rpc-0.8.9/deepomatic/rpc/helpers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2618 2021-05-24 15:03:49.000000 deepomatic-rpc-0.8.9/deepomatic/rpc/helpers/proto.py
+-rw-r--r--   0 root         (0) root         (0)     1031 2021-05-24 15:03:49.000000 deepomatic-rpc-0.8.9/deepomatic/rpc/helpers/v07_proto.py
+-rw-r--r--   0 root         (0) root         (0)      304 2021-08-03 13:47:59.000000 deepomatic-rpc-0.8.9/deepomatic/rpc/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-03 14:07:04.000000 deepomatic-rpc-0.8.9/deepomatic/rpc/amqp/
+-rw-r--r--   0 root         (0) root         (0)      221 2021-05-24 15:03:51.000000 deepomatic-rpc-0.8.9/deepomatic/rpc/amqp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13305 2021-05-24 15:03:51.000000 deepomatic-rpc-0.8.9/deepomatic/rpc/amqp/entities.py
+-rw-r--r--   0 root         (0) root         (0)    26340 2021-05-24 15:03:51.000000 deepomatic-rpc-0.8.9/deepomatic/rpc/amqp/client.py
+-rw-r--r--   0 root         (0) root         (0)      401 2021-05-24 15:03:51.000000 deepomatic-rpc-0.8.9/deepomatic/rpc/amqp/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     3189 2021-05-24 15:03:49.000000 deepomatic-rpc-0.8.9/deepomatic/rpc/response.py
+-rw-r--r--   0 root         (0) root         (0)     1288 2021-05-24 15:03:49.000000 deepomatic-rpc-0.8.9/deepomatic/rpc/client.py
+-rw-r--r--   0 root         (0) root         (0)      360 2021-05-24 15:03:49.000000 deepomatic-rpc-0.8.9/deepomatic/rpc/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-03 14:07:04.000000 deepomatic-rpc-0.8.9/deepomatic/rpc/buffers/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-08-03 14:07:01.000000 deepomatic-rpc-0.8.9/deepomatic/rpc/buffers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-03 14:07:04.000000 deepomatic-rpc-0.8.9/deepomatic/rpc/buffers/protobuf/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-03 14:07:04.000000 deepomatic-rpc-0.8.9/deepomatic/rpc/buffers/protobuf/workflows/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-08-03 14:07:01.000000 deepomatic-rpc-0.8.9/deepomatic/rpc/buffers/protobuf/workflows/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4941 2021-08-03 14:07:01.000000 deepomatic-rpc-0.8.9/deepomatic/rpc/buffers/protobuf/workflows/WorkflowExecution_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    24704 2021-08-03 14:07:01.000000 deepomatic-rpc-0.8.9/deepomatic/rpc/buffers/protobuf/workflows/Workflow_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    15974 2021-08-03 14:07:01.000000 deepomatic-rpc-0.8.9/deepomatic/rpc/buffers/protobuf/workflows/WorkflowExecution_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-08-03 14:07:01.000000 deepomatic-rpc-0.8.9/deepomatic/rpc/buffers/protobuf/workflows/Workflow_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-03 14:07:04.000000 deepomatic-rpc-0.8.9/deepomatic/rpc/buffers/protobuf/cli/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-08-03 14:07:01.000000 deepomatic-rpc-0.8.9/deepomatic/rpc/buffers/protobuf/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5277 2021-08-03 14:07:01.000000 deepomatic-rpc-0.8.9/deepomatic/rpc/buffers/protobuf/cli/Message_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-08-03 14:07:01.000000 deepomatic-rpc-0.8.9/deepomatic/rpc/buffers/protobuf/cli/Message_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)        0 2021-08-03 14:07:01.000000 deepomatic-rpc-0.8.9/deepomatic/rpc/buffers/protobuf/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-03 14:07:04.000000 deepomatic-rpc-0.8.9/deepomatic/rpc/buffers/protobuf/nn/
+-rw-r--r--   0 root         (0) root         (0)    14567 2021-08-03 14:07:01.000000 deepomatic-rpc-0.8.9/deepomatic/rpc/buffers/protobuf/nn/Command_pb2.py
+-rw-r--r--   0 root         (0) root         (0)        0 2021-08-03 14:07:01.000000 deepomatic-rpc-0.8.9/deepomatic/rpc/buffers/protobuf/nn/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4720 2021-08-03 14:07:01.000000 deepomatic-rpc-0.8.9/deepomatic/rpc/buffers/protobuf/nn/Result_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     3812 2021-08-03 14:07:01.000000 deepomatic-rpc-0.8.9/deepomatic/rpc/buffers/protobuf/nn/Message_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-08-03 14:07:01.000000 deepomatic-rpc-0.8.9/deepomatic/rpc/buffers/protobuf/nn/Preprocessing_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-08-03 14:07:01.000000 deepomatic-rpc-0.8.9/deepomatic/rpc/buffers/protobuf/nn/Message_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-03 14:07:04.000000 deepomatic-rpc-0.8.9/deepomatic/rpc/buffers/protobuf/nn/v07/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-08-03 14:07:01.000000 deepomatic-rpc-0.8.9/deepomatic/rpc/buffers/protobuf/nn/v07/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7434 2021-08-03 14:07:01.000000 deepomatic-rpc-0.8.9/deepomatic/rpc/buffers/protobuf/nn/v07/Inputs_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    14190 2021-08-03 14:07:01.000000 deepomatic-rpc-0.8.9/deepomatic/rpc/buffers/protobuf/nn/v07/Workflows_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-08-03 14:07:01.000000 deepomatic-rpc-0.8.9/deepomatic/rpc/buffers/protobuf/nn/v07/Inputs_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    23323 2021-08-03 14:07:01.000000 deepomatic-rpc-0.8.9/deepomatic/rpc/buffers/protobuf/nn/v07/Results_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-08-03 14:07:01.000000 deepomatic-rpc-0.8.9/deepomatic/rpc/buffers/protobuf/nn/v07/Workflows_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     4861 2021-08-03 14:07:01.000000 deepomatic-rpc-0.8.9/deepomatic/rpc/buffers/protobuf/nn/v07/Commands_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-08-03 14:07:01.000000 deepomatic-rpc-0.8.9/deepomatic/rpc/buffers/protobuf/nn/v07/Results_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-08-03 14:07:01.000000 deepomatic-rpc-0.8.9/deepomatic/rpc/buffers/protobuf/nn/v07/Commands_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    24311 2021-08-03 14:07:01.000000 deepomatic-rpc-0.8.9/deepomatic/rpc/buffers/protobuf/nn/Preprocessing_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    58826 2021-08-03 14:07:01.000000 deepomatic-rpc-0.8.9/deepomatic/rpc/buffers/protobuf/nn/Postprocessing_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-08-03 14:07:01.000000 deepomatic-rpc-0.8.9/deepomatic/rpc/buffers/protobuf/nn/Postprocessing_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-08-03 14:07:01.000000 deepomatic-rpc-0.8.9/deepomatic/rpc/buffers/protobuf/nn/Command_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-03 14:07:04.000000 deepomatic-rpc-0.8.9/deepomatic/rpc/buffers/protobuf/nn/frameworks/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-08-03 14:07:01.000000 deepomatic-rpc-0.8.9/deepomatic/rpc/buffers/protobuf/nn/frameworks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7818 2021-08-03 14:07:01.000000 deepomatic-rpc-0.8.9/deepomatic/rpc/buffers/protobuf/nn/frameworks/Caffe_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-08-03 14:07:01.000000 deepomatic-rpc-0.8.9/deepomatic/rpc/buffers/protobuf/nn/frameworks/Caffe_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-08-03 14:07:01.000000 deepomatic-rpc-0.8.9/deepomatic/rpc/buffers/protobuf/nn/Result_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-03 14:07:04.000000 deepomatic-rpc-0.8.9/deepomatic/rpc/buffers/protobuf/common/
+-rw-r--r--   0 root         (0) root         (0)      159 2021-08-03 14:07:01.000000 deepomatic-rpc-0.8.9/deepomatic/rpc/buffers/protobuf/common/Image_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)        0 2021-08-03 14:07:01.000000 deepomatic-rpc-0.8.9/deepomatic/rpc/buffers/protobuf/common/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6420 2021-08-03 14:07:01.000000 deepomatic-rpc-0.8.9/deepomatic/rpc/buffers/protobuf/common/Image_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     3027 2021-08-03 14:07:01.000000 deepomatic-rpc-0.8.9/deepomatic/rpc/buffers/protobuf/common/Error_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2021-08-03 14:07:01.000000 deepomatic-rpc-0.8.9/deepomatic/rpc/buffers/protobuf/common/Error_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)      170 2021-05-24 15:03:49.000000 deepomatic-rpc-0.8.9/deepomatic/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     1988 2021-08-03 13:47:59.000000 deepomatic-rpc-0.8.9/setup.py
```

### Comparing `deepomatic-rpc-0.8.8/PKG-INFO` & `deepomatic-rpc-0.8.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepomatic-rpc
-Version: 0.8.8
+Version: 0.8.9
 Summary: Deepomatic RPC python client
 Home-page: https://www.deepomatic.com
 Author: deepomatic
 Author-email: support@deepomatic.com
 License: UNLICENSED
 Project-URL: Product, https://www.deepomatic.com
 Description: # Table of contents
```

### Comparing `deepomatic-rpc-0.8.8/deepomatic/rpc/grpc/workflow_client.py` & `deepomatic-rpc-0.8.9/deepomatic/rpc/grpc/workflow_client.py`

 * *Files identical despite different names*

### Comparing `deepomatic-rpc-0.8.8/deepomatic/rpc/client.py` & `deepomatic-rpc-0.8.9/deepomatic/rpc/client.py`

 * *Files identical despite different names*

### Comparing `deepomatic-rpc-0.8.8/deepomatic/rpc/buffers/protobuf/workflows/WorkflowExecution_pb2_grpc.py` & `deepomatic-rpc-0.8.9/deepomatic/rpc/buffers/protobuf/workflows/WorkflowExecution_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `deepomatic-rpc-0.8.8/deepomatic/rpc/buffers/protobuf/workflows/Workflow_pb2.py` & `deepomatic-rpc-0.8.9/deepomatic/rpc/buffers/protobuf/workflows/Workflow_pb2.py`

 * *Files identical despite different names*

### Comparing `deepomatic-rpc-0.8.8/deepomatic/rpc/buffers/protobuf/workflows/WorkflowExecution_pb2.py` & `deepomatic-rpc-0.8.9/deepomatic/rpc/buffers/protobuf/workflows/WorkflowExecution_pb2.py`

 * *Files identical despite different names*

### Comparing `deepomatic-rpc-0.8.8/deepomatic/rpc/buffers/protobuf/common/Error_pb2.py` & `deepomatic-rpc-0.8.9/deepomatic/rpc/buffers/protobuf/common/Error_pb2.py`

 * *Files identical despite different names*

### Comparing `deepomatic-rpc-0.8.8/deepomatic/rpc/buffers/protobuf/common/Image_pb2.py` & `deepomatic-rpc-0.8.9/deepomatic/rpc/buffers/protobuf/common/Image_pb2.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='buffers/protobuf/common/Image.proto',
   package='buffers.protobuf.common',
   syntax='proto3',
   serialized_options=None,
   create_key=_descriptor._internal_create_key,
-  serialized_pb=b'\n#buffers/protobuf/common/Image.proto\x12\x17\x62uffers.protobuf.common\"\x1d\n\x05Point\x12\t\n\x01x\x18\x01 \x01(\x02\x12\t\n\x01y\x18\x02 \x01(\x02\">\n\x04\x42\x42ox\x12\x0c\n\x04xmin\x18\x01 \x01(\x02\x12\x0c\n\x04xmax\x18\x02 \x01(\x02\x12\x0c\n\x04ymin\x18\x03 \x01(\x02\x12\x0c\n\x04ymax\x18\x04 \x01(\x02\x62\x06proto3'
+  serialized_pb=b'\n#buffers/protobuf/common/Image.proto\x12\x17\x62uffers.protobuf.common\"\x1d\n\x05Point\x12\t\n\x01x\x18\x01 \x01(\x02\x12\t\n\x01y\x18\x02 \x01(\x02\">\n\x04\x42\x42ox\x12\x0c\n\x04xmin\x18\x01 \x01(\x02\x12\x0c\n\x04xmax\x18\x02 \x01(\x02\x12\x0c\n\x04ymin\x18\x03 \x01(\x02\x12\x0c\n\x04ymax\x18\x04 \x01(\x02\"9\n\x07Polygon\x12.\n\x06points\x18\x01 \x03(\x0b\x32\x1e.buffers.protobuf.common.Pointb\x06proto3'
 )
 
 
 
 
 _POINT = _descriptor.Descriptor(
   name='Point',
@@ -112,16 +112,50 @@
   extension_ranges=[],
   oneofs=[
   ],
   serialized_start=95,
   serialized_end=157,
 )
 
+
+_POLYGON = _descriptor.Descriptor(
+  name='Polygon',
+  full_name='buffers.protobuf.common.Polygon',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='points', full_name='buffers.protobuf.common.Polygon.points', index=0,
+      number=1, type=11, cpp_type=10, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=159,
+  serialized_end=216,
+)
+
+_POLYGON.fields_by_name['points'].message_type = _POINT
 DESCRIPTOR.message_types_by_name['Point'] = _POINT
 DESCRIPTOR.message_types_by_name['BBox'] = _BBOX
+DESCRIPTOR.message_types_by_name['Polygon'] = _POLYGON
 _sym_db.RegisterFileDescriptor(DESCRIPTOR)
 
 Point = _reflection.GeneratedProtocolMessageType('Point', (_message.Message,), {
   'DESCRIPTOR' : _POINT,
   '__module__' : 'buffers.protobuf.common.Image_pb2'
   # @@protoc_insertion_point(class_scope:buffers.protobuf.common.Point)
   })
@@ -130,9 +164,16 @@
 BBox = _reflection.GeneratedProtocolMessageType('BBox', (_message.Message,), {
   'DESCRIPTOR' : _BBOX,
   '__module__' : 'buffers.protobuf.common.Image_pb2'
   # @@protoc_insertion_point(class_scope:buffers.protobuf.common.BBox)
   })
 _sym_db.RegisterMessage(BBox)
 
+Polygon = _reflection.GeneratedProtocolMessageType('Polygon', (_message.Message,), {
+  'DESCRIPTOR' : _POLYGON,
+  '__module__' : 'buffers.protobuf.common.Image_pb2'
+  # @@protoc_insertion_point(class_scope:buffers.protobuf.common.Polygon)
+  })
+_sym_db.RegisterMessage(Polygon)
+
 
 # @@protoc_insertion_point(module_scope)
```

### Comparing `deepomatic-rpc-0.8.8/deepomatic/rpc/buffers/protobuf/cli/Message_pb2.py` & `deepomatic-rpc-0.8.9/deepomatic/rpc/buffers/protobuf/cli/Message_pb2.py`

 * *Files identical despite different names*

### Comparing `deepomatic-rpc-0.8.8/deepomatic/rpc/buffers/protobuf/nn/Postprocessing_pb2.py` & `deepomatic-rpc-0.8.9/deepomatic/rpc/buffers/protobuf/nn/Postprocessing_pb2.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='buffers/protobuf/nn/Postprocessing.proto',
   package='buffers.protobuf.nn.postprocessing',
   syntax='proto3',
   serialized_options=None,
   create_key=_descriptor._internal_create_key,
-  serialized_pb=b'\n(buffers/protobuf/nn/Postprocessing.proto\x12\"buffers.protobuf.nn.postprocessing\"#\n\x10RawTensorsOutput\x12\x0f\n\x07tensors\x18\x01 \x03(\t\"=\n\x0eStandardOutput\x12\x14\n\x0c\x62oxes_tensor\x18\x01 \x01(\t\x12\x15\n\rscores_tensor\x18\x02 \x01(\t\"W\n\x0e\x41nchoredOutput\x12\x16\n\x0e\x61nchors_tensor\x18\x01 \x01(\t\x12\x16\n\x0eoffsets_tensor\x18\x02 \x01(\t\x12\x15\n\rscores_tensor\x18\x03 \x01(\t\"S\n\x0c\x44irectOutput\x12\x14\n\x0c\x62oxes_tensor\x18\x01 \x01(\t\x12\x15\n\rscores_tensor\x18\x02 \x01(\t\x12\x16\n\x0e\x63lasses_tensor\x18\x03 \x01(\t\"4\n\nYoloOutput\x12\x15\n\routput_tensor\x18\x01 \x01(\t\x12\x0f\n\x07\x61nchors\x18\x02 \x03(\x02\"7\n\x0cYoloV3Output\x12\x16\n\x0eoutput_tensors\x18\x01 \x03(\t\x12\x0f\n\x07\x61nchors\x18\x02 \x03(\x02\"\xfd\x03\n\x0ePostProcessing\x12M\n\x0f\x61nchored_output\x18\x01 \x01(\x0b\x32\x32.buffers.protobuf.nn.postprocessing.AnchoredOutputH\x00\x12I\n\rdirect_output\x18\x02 \x01(\x0b\x32\x30.buffers.protobuf.nn.postprocessing.DirectOutputH\x00\x12\x45\n\x0byolo_output\x18\x03 \x01(\x0b\x32..buffers.protobuf.nn.postprocessing.YoloOutputH\x00\x12I\n\ryolov3_output\x18\x04 \x01(\x0b\x32\x30.buffers.protobuf.nn.postprocessing.YoloV3OutputH\x00\x12N\n\x0etensors_output\x18\x05 \x01(\x0b\x32\x34.buffers.protobuf.nn.postprocessing.RawTensorsOutputH\x00\x12M\n\x0fstandard_output\x18\x06 \x01(\x0b\x32\x32.buffers.protobuf.nn.postprocessing.StandardOutputH\x00\x12\x18\n\x10\x65xpand_batch_dim\x18\x0f \x01(\x08\x42\x06\n\x04type\"^\n\x0fPostProcessings\x12K\n\x0fpostprocessings\x18\x01 \x03(\x0b\x32\x32.buffers.protobuf.nn.postprocessing.PostProcessing\"\xf2\x01\n\x0cLabelsOutput\x12\x46\n\x06labels\x18\x01 \x03(\x0b\x32\x36.buffers.protobuf.nn.postprocessing.LabelsOutput.Label\x12\x11\n\texclusive\x18\x02 \x01(\x08\x12\x45\n\x03roi\x18\x03 \x01(\x0e\x32\x38.buffers.protobuf.nn.postprocessing.LabelsOutput.ROIType\x1a!\n\x05Label\x12\n\n\x02id\x18\x01 \x01(\r\x12\x0c\n\x04name\x18\x02 \x01(\t\"\x1d\n\x07ROIType\x12\x08\n\x04NONE\x10\x00\x12\x08\n\x04\x42\x42OX\x10\x01\" \n\nTextOutput\x12\x12\n\ncharacters\x18\x01 \x03(\t\"\xeb\x01\n\x07Outputs\x12\x46\n\x07outputs\x18\x01 \x03(\x0b\x32\x35.buffers.protobuf.nn.postprocessing.Outputs.OutputMix\x1a\x97\x01\n\tOutputMix\x12\x42\n\x06labels\x18\x01 \x01(\x0b\x32\x30.buffers.protobuf.nn.postprocessing.LabelsOutputH\x00\x12>\n\x04text\x18\x02 \x01(\x0b\x32..buffers.protobuf.nn.postprocessing.TextOutputH\x00\x42\x06\n\x04type\";\n\x0e\x43lassification\x12\x15\n\routput_tensor\x18\x01 \x01(\t\x12\x12\n\nthresholds\x18\x02 \x03(\x01\"\xcd\x04\n\tDetection\x12K\n\noutput_mix\x18\x01 \x01(\x0b\x32\x37.buffers.protobuf.nn.postprocessing.Detection.OutputMix\x12\x12\n\nthresholds\x18\x02 \x03(\x01\x12\x15\n\rnms_threshold\x18\x03 \x01(\x01\x12\x19\n\x11\x64iscard_threshold\x18\x04 \x01(\x01\x12\x1c\n\x14normalize_wrt_tensor\x18\x05 \x01(\t\x1a\x8e\x03\n\tOutputMix\x12M\n\x0f\x61nchored_output\x18\x01 \x01(\x0b\x32\x32.buffers.protobuf.nn.postprocessing.AnchoredOutputH\x00\x12I\n\rdirect_output\x18\x02 \x01(\x0b\x32\x30.buffers.protobuf.nn.postprocessing.DirectOutputH\x00\x12\x45\n\x0byolo_output\x18\x03 \x01(\x0b\x32..buffers.protobuf.nn.postprocessing.YoloOutputH\x00\x12I\n\ryolov3_output\x18\x04 \x01(\x0b\x32\x30.buffers.protobuf.nn.postprocessing.YoloV3OutputH\x00\x12M\n\x0fstandard_output\x18\x05 \x01(\x0b\x32\x32.buffers.protobuf.nn.postprocessing.StandardOutputH\x00\x42\x06\n\x04type\"\x05\n\x03OCR\"\x81\x03\n\x19PostprocessingsDeprecated\x12r\n\x0fpostprocessings\x18\x01 \x03(\x0b\x32Y.buffers.protobuf.nn.postprocessing.PostprocessingsDeprecated.PostprocessingMixDeprecated\x1a\xef\x01\n\x1bPostprocessingMixDeprecated\x12L\n\x0e\x63lassification\x18\x01 \x01(\x0b\x32\x32.buffers.protobuf.nn.postprocessing.ClassificationH\x00\x12\x42\n\tdetection\x18\x02 \x01(\x0b\x32-.buffers.protobuf.nn.postprocessing.DetectionH\x00\x12\x36\n\x03ocr\x18\x03 \x01(\x0b\x32\'.buffers.protobuf.nn.postprocessing.OCRH\x00\x42\x06\n\x04typeb\x06proto3'
+  serialized_pb=b'\n(buffers/protobuf/nn/Postprocessing.proto\x12\"buffers.protobuf.nn.postprocessing\"#\n\x10RawTensorsOutput\x12\x0f\n\x07tensors\x18\x01 \x03(\t\"=\n\x0eStandardOutput\x12\x14\n\x0c\x62oxes_tensor\x18\x01 \x01(\t\x12\x15\n\rscores_tensor\x18\x02 \x01(\t\"w\n\x1aInstanceSegmentationOutput\x12\x14\n\x0c\x62oxes_tensor\x18\x01 \x01(\t\x12\x15\n\rscores_tensor\x18\x02 \x01(\t\x12\x16\n\x0e\x63lasses_tensor\x18\x03 \x01(\t\x12\x14\n\x0cmasks_tensor\x18\x04 \x01(\t\"W\n\x0e\x41nchoredOutput\x12\x16\n\x0e\x61nchors_tensor\x18\x01 \x01(\t\x12\x16\n\x0eoffsets_tensor\x18\x02 \x01(\t\x12\x15\n\rscores_tensor\x18\x03 \x01(\t\"S\n\x0c\x44irectOutput\x12\x14\n\x0c\x62oxes_tensor\x18\x01 \x01(\t\x12\x15\n\rscores_tensor\x18\x02 \x01(\t\x12\x16\n\x0e\x63lasses_tensor\x18\x03 \x01(\t\"4\n\nYoloOutput\x12\x15\n\routput_tensor\x18\x01 \x01(\t\x12\x0f\n\x07\x61nchors\x18\x02 \x03(\x02\"7\n\x0cYoloV3Output\x12\x16\n\x0eoutput_tensors\x18\x01 \x03(\t\x12\x0f\n\x07\x61nchors\x18\x02 \x03(\x02\"\xe5\x04\n\x0ePostProcessing\x12M\n\x0f\x61nchored_output\x18\x01 \x01(\x0b\x32\x32.buffers.protobuf.nn.postprocessing.AnchoredOutputH\x00\x12I\n\rdirect_output\x18\x02 \x01(\x0b\x32\x30.buffers.protobuf.nn.postprocessing.DirectOutputH\x00\x12\x45\n\x0byolo_output\x18\x03 \x01(\x0b\x32..buffers.protobuf.nn.postprocessing.YoloOutputH\x00\x12I\n\ryolov3_output\x18\x04 \x01(\x0b\x32\x30.buffers.protobuf.nn.postprocessing.YoloV3OutputH\x00\x12N\n\x0etensors_output\x18\x05 \x01(\x0b\x32\x34.buffers.protobuf.nn.postprocessing.RawTensorsOutputH\x00\x12M\n\x0fstandard_output\x18\x06 \x01(\x0b\x32\x32.buffers.protobuf.nn.postprocessing.StandardOutputH\x00\x12\x66\n\x1cinstance_segmentation_output\x18\x07 \x01(\x0b\x32>.buffers.protobuf.nn.postprocessing.InstanceSegmentationOutputH\x00\x12\x18\n\x10\x65xpand_batch_dim\x18\x0f \x01(\x08\x42\x06\n\x04type\"^\n\x0fPostProcessings\x12K\n\x0fpostprocessings\x18\x01 \x03(\x0b\x32\x32.buffers.protobuf.nn.postprocessing.PostProcessing\"\xfc\x01\n\x0cLabelsOutput\x12\x46\n\x06labels\x18\x01 \x03(\x0b\x32\x36.buffers.protobuf.nn.postprocessing.LabelsOutput.Label\x12\x11\n\texclusive\x18\x02 \x01(\x08\x12\x45\n\x03roi\x18\x03 \x01(\x0e\x32\x38.buffers.protobuf.nn.postprocessing.LabelsOutput.ROIType\x1a!\n\x05Label\x12\n\n\x02id\x18\x01 \x01(\r\x12\x0c\n\x04name\x18\x02 \x01(\t\"\'\n\x07ROIType\x12\x08\n\x04NONE\x10\x00\x12\x08\n\x04\x42\x42OX\x10\x01\x12\x08\n\x04MASK\x10\x02\" \n\nTextOutput\x12\x12\n\ncharacters\x18\x01 \x03(\t\"\xeb\x01\n\x07Outputs\x12\x46\n\x07outputs\x18\x01 \x03(\x0b\x32\x35.buffers.protobuf.nn.postprocessing.Outputs.OutputMix\x1a\x97\x01\n\tOutputMix\x12\x42\n\x06labels\x18\x01 \x01(\x0b\x32\x30.buffers.protobuf.nn.postprocessing.LabelsOutputH\x00\x12>\n\x04text\x18\x02 \x01(\x0b\x32..buffers.protobuf.nn.postprocessing.TextOutputH\x00\x42\x06\n\x04type\";\n\x0e\x43lassification\x12\x15\n\routput_tensor\x18\x01 \x01(\t\x12\x12\n\nthresholds\x18\x02 \x03(\x01\"\xcd\x04\n\tDetection\x12K\n\noutput_mix\x18\x01 \x01(\x0b\x32\x37.buffers.protobuf.nn.postprocessing.Detection.OutputMix\x12\x12\n\nthresholds\x18\x02 \x03(\x01\x12\x15\n\rnms_threshold\x18\x03 \x01(\x01\x12\x19\n\x11\x64iscard_threshold\x18\x04 \x01(\x01\x12\x1c\n\x14normalize_wrt_tensor\x18\x05 \x01(\t\x1a\x8e\x03\n\tOutputMix\x12M\n\x0f\x61nchored_output\x18\x01 \x01(\x0b\x32\x32.buffers.protobuf.nn.postprocessing.AnchoredOutputH\x00\x12I\n\rdirect_output\x18\x02 \x01(\x0b\x32\x30.buffers.protobuf.nn.postprocessing.DirectOutputH\x00\x12\x45\n\x0byolo_output\x18\x03 \x01(\x0b\x32..buffers.protobuf.nn.postprocessing.YoloOutputH\x00\x12I\n\ryolov3_output\x18\x04 \x01(\x0b\x32\x30.buffers.protobuf.nn.postprocessing.YoloV3OutputH\x00\x12M\n\x0fstandard_output\x18\x05 \x01(\x0b\x32\x32.buffers.protobuf.nn.postprocessing.StandardOutputH\x00\x42\x06\n\x04type\"\x05\n\x03OCR\"\x8a\x02\n\x0cSegmentation\x12N\n\noutput_mix\x18\x01 \x01(\x0b\x32:.buffers.protobuf.nn.postprocessing.Segmentation.OutputMix\x12\x12\n\nthresholds\x18\x02 \x03(\x01\x12\x19\n\x11\x64iscard_threshold\x18\x03 \x01(\x01\x1a{\n\tOutputMix\x12\x66\n\x1cinstance_segmentation_output\x18\x01 \x01(\x0b\x32>.buffers.protobuf.nn.postprocessing.InstanceSegmentationOutputH\x00\x42\x06\n\x04type\"\x81\x03\n\x19PostprocessingsDeprecated\x12r\n\x0fpostprocessings\x18\x01 \x03(\x0b\x32Y.buffers.protobuf.nn.postprocessing.PostprocessingsDeprecated.PostprocessingMixDeprecated\x1a\xef\x01\n\x1bPostprocessingMixDeprecated\x12L\n\x0e\x63lassification\x18\x01 \x01(\x0b\x32\x32.buffers.protobuf.nn.postprocessing.ClassificationH\x00\x12\x42\n\tdetection\x18\x02 \x01(\x0b\x32-.buffers.protobuf.nn.postprocessing.DetectionH\x00\x12\x36\n\x03ocr\x18\x03 \x01(\x0b\x32\'.buffers.protobuf.nn.postprocessing.OCRH\x00\x42\x06\n\x04typeb\x06proto3'
 )
 
 
 
 _LABELSOUTPUT_ROITYPE = _descriptor.EnumDescriptor(
   name='ROIType',
   full_name='buffers.protobuf.nn.postprocessing.LabelsOutput.ROIType',
@@ -37,19 +37,24 @@
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
       name='BBOX', index=1, number=1,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
+    _descriptor.EnumValueDescriptor(
+      name='MASK', index=2, number=2,
+      serialized_options=None,
+      type=None,
+      create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=1287,
-  serialized_end=1316,
+  serialized_start=1512,
+  serialized_end=1551,
 )
 _sym_db.RegisterEnumDescriptor(_LABELSOUTPUT_ROITYPE)
 
 
 _RAWTENSORSOUTPUT = _descriptor.Descriptor(
   name='RawTensorsOutput',
   full_name='buffers.protobuf.nn.postprocessing.RawTensorsOutput',
@@ -117,14 +122,67 @@
   oneofs=[
   ],
   serialized_start=117,
   serialized_end=178,
 )
 
 
+_INSTANCESEGMENTATIONOUTPUT = _descriptor.Descriptor(
+  name='InstanceSegmentationOutput',
+  full_name='buffers.protobuf.nn.postprocessing.InstanceSegmentationOutput',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='boxes_tensor', full_name='buffers.protobuf.nn.postprocessing.InstanceSegmentationOutput.boxes_tensor', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='scores_tensor', full_name='buffers.protobuf.nn.postprocessing.InstanceSegmentationOutput.scores_tensor', index=1,
+      number=2, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='classes_tensor', full_name='buffers.protobuf.nn.postprocessing.InstanceSegmentationOutput.classes_tensor', index=2,
+      number=3, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='masks_tensor', full_name='buffers.protobuf.nn.postprocessing.InstanceSegmentationOutput.masks_tensor', index=3,
+      number=4, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=180,
+  serialized_end=299,
+)
+
+
 _ANCHOREDOUTPUT = _descriptor.Descriptor(
   name='AnchoredOutput',
   full_name='buffers.protobuf.nn.postprocessing.AnchoredOutput',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
@@ -158,16 +216,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=180,
-  serialized_end=267,
+  serialized_start=301,
+  serialized_end=388,
 )
 
 
 _DIRECTOUTPUT = _descriptor.Descriptor(
   name='DirectOutput',
   full_name='buffers.protobuf.nn.postprocessing.DirectOutput',
   filename=None,
@@ -204,16 +262,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=269,
-  serialized_end=352,
+  serialized_start=390,
+  serialized_end=473,
 )
 
 
 _YOLOOUTPUT = _descriptor.Descriptor(
   name='YoloOutput',
   full_name='buffers.protobuf.nn.postprocessing.YoloOutput',
   filename=None,
@@ -243,16 +301,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=354,
-  serialized_end=406,
+  serialized_start=475,
+  serialized_end=527,
 )
 
 
 _YOLOV3OUTPUT = _descriptor.Descriptor(
   name='YoloV3Output',
   full_name='buffers.protobuf.nn.postprocessing.YoloV3Output',
   filename=None,
@@ -282,16 +340,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=408,
-  serialized_end=463,
+  serialized_start=529,
+  serialized_end=584,
 )
 
 
 _POSTPROCESSING = _descriptor.Descriptor(
   name='PostProcessing',
   full_name='buffers.protobuf.nn.postprocessing.PostProcessing',
   filename=None,
@@ -338,15 +396,22 @@
       name='standard_output', full_name='buffers.protobuf.nn.postprocessing.PostProcessing.standard_output', index=5,
       number=6, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='expand_batch_dim', full_name='buffers.protobuf.nn.postprocessing.PostProcessing.expand_batch_dim', index=6,
+      name='instance_segmentation_output', full_name='buffers.protobuf.nn.postprocessing.PostProcessing.instance_segmentation_output', index=6,
+      number=7, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='expand_batch_dim', full_name='buffers.protobuf.nn.postprocessing.PostProcessing.expand_batch_dim', index=7,
       number=15, type=8, cpp_type=7, label=1,
       has_default_value=False, default_value=False,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
@@ -361,16 +426,16 @@
   oneofs=[
     _descriptor.OneofDescriptor(
       name='type', full_name='buffers.protobuf.nn.postprocessing.PostProcessing.type',
       index=0, containing_type=None,
       create_key=_descriptor._internal_create_key,
     fields=[]),
   ],
-  serialized_start=466,
-  serialized_end=975,
+  serialized_start=587,
+  serialized_end=1200,
 )
 
 
 _POSTPROCESSINGS = _descriptor.Descriptor(
   name='PostProcessings',
   full_name='buffers.protobuf.nn.postprocessing.PostProcessings',
   filename=None,
@@ -393,16 +458,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=977,
-  serialized_end=1071,
+  serialized_start=1202,
+  serialized_end=1296,
 )
 
 
 _LABELSOUTPUT_LABEL = _descriptor.Descriptor(
   name='Label',
   full_name='buffers.protobuf.nn.postprocessing.LabelsOutput.Label',
   filename=None,
@@ -432,16 +497,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1252,
-  serialized_end=1285,
+  serialized_start=1477,
+  serialized_end=1510,
 )
 
 _LABELSOUTPUT = _descriptor.Descriptor(
   name='LabelsOutput',
   full_name='buffers.protobuf.nn.postprocessing.LabelsOutput',
   filename=None,
   file=DESCRIPTOR,
@@ -478,16 +543,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1074,
-  serialized_end=1316,
+  serialized_start=1299,
+  serialized_end=1551,
 )
 
 
 _TEXTOUTPUT = _descriptor.Descriptor(
   name='TextOutput',
   full_name='buffers.protobuf.nn.postprocessing.TextOutput',
   filename=None,
@@ -510,16 +575,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1318,
-  serialized_end=1350,
+  serialized_start=1553,
+  serialized_end=1585,
 )
 
 
 _OUTPUTS_OUTPUTMIX = _descriptor.Descriptor(
   name='OutputMix',
   full_name='buffers.protobuf.nn.postprocessing.Outputs.OutputMix',
   filename=None,
@@ -554,16 +619,16 @@
   oneofs=[
     _descriptor.OneofDescriptor(
       name='type', full_name='buffers.protobuf.nn.postprocessing.Outputs.OutputMix.type',
       index=0, containing_type=None,
       create_key=_descriptor._internal_create_key,
     fields=[]),
   ],
-  serialized_start=1437,
-  serialized_end=1588,
+  serialized_start=1672,
+  serialized_end=1823,
 )
 
 _OUTPUTS = _descriptor.Descriptor(
   name='Outputs',
   full_name='buffers.protobuf.nn.postprocessing.Outputs',
   filename=None,
   file=DESCRIPTOR,
@@ -585,16 +650,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1353,
-  serialized_end=1588,
+  serialized_start=1588,
+  serialized_end=1823,
 )
 
 
 _CLASSIFICATION = _descriptor.Descriptor(
   name='Classification',
   full_name='buffers.protobuf.nn.postprocessing.Classification',
   filename=None,
@@ -624,16 +689,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1590,
-  serialized_end=1649,
+  serialized_start=1825,
+  serialized_end=1884,
 )
 
 
 _DETECTION_OUTPUTMIX = _descriptor.Descriptor(
   name='OutputMix',
   full_name='buffers.protobuf.nn.postprocessing.Detection.OutputMix',
   filename=None,
@@ -689,16 +754,16 @@
   oneofs=[
     _descriptor.OneofDescriptor(
       name='type', full_name='buffers.protobuf.nn.postprocessing.Detection.OutputMix.type',
       index=0, containing_type=None,
       create_key=_descriptor._internal_create_key,
     fields=[]),
   ],
-  serialized_start=1843,
-  serialized_end=2241,
+  serialized_start=2078,
+  serialized_end=2476,
 )
 
 _DETECTION = _descriptor.Descriptor(
   name='Detection',
   full_name='buffers.protobuf.nn.postprocessing.Detection',
   filename=None,
   file=DESCRIPTOR,
@@ -748,16 +813,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1652,
-  serialized_end=2241,
+  serialized_start=1887,
+  serialized_end=2476,
 )
 
 
 _OCR = _descriptor.Descriptor(
   name='OCR',
   full_name='buffers.protobuf.nn.postprocessing.OCR',
   filename=None,
@@ -773,16 +838,98 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2243,
-  serialized_end=2248,
+  serialized_start=2478,
+  serialized_end=2483,
+)
+
+
+_SEGMENTATION_OUTPUTMIX = _descriptor.Descriptor(
+  name='OutputMix',
+  full_name='buffers.protobuf.nn.postprocessing.Segmentation.OutputMix',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='instance_segmentation_output', full_name='buffers.protobuf.nn.postprocessing.Segmentation.OutputMix.instance_segmentation_output', index=0,
+      number=1, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+    _descriptor.OneofDescriptor(
+      name='type', full_name='buffers.protobuf.nn.postprocessing.Segmentation.OutputMix.type',
+      index=0, containing_type=None,
+      create_key=_descriptor._internal_create_key,
+    fields=[]),
+  ],
+  serialized_start=2629,
+  serialized_end=2752,
+)
+
+_SEGMENTATION = _descriptor.Descriptor(
+  name='Segmentation',
+  full_name='buffers.protobuf.nn.postprocessing.Segmentation',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='output_mix', full_name='buffers.protobuf.nn.postprocessing.Segmentation.output_mix', index=0,
+      number=1, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='thresholds', full_name='buffers.protobuf.nn.postprocessing.Segmentation.thresholds', index=1,
+      number=2, type=1, cpp_type=5, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='discard_threshold', full_name='buffers.protobuf.nn.postprocessing.Segmentation.discard_threshold', index=2,
+      number=3, type=1, cpp_type=5, label=1,
+      has_default_value=False, default_value=float(0),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[_SEGMENTATION_OUTPUTMIX, ],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=2486,
+  serialized_end=2752,
 )
 
 
 _POSTPROCESSINGSDEPRECATED_POSTPROCESSINGMIXDEPRECATED = _descriptor.Descriptor(
   name='PostprocessingMixDeprecated',
   full_name='buffers.protobuf.nn.postprocessing.PostprocessingsDeprecated.PostprocessingMixDeprecated',
   filename=None,
@@ -824,16 +971,16 @@
   oneofs=[
     _descriptor.OneofDescriptor(
       name='type', full_name='buffers.protobuf.nn.postprocessing.PostprocessingsDeprecated.PostprocessingMixDeprecated.type',
       index=0, containing_type=None,
       create_key=_descriptor._internal_create_key,
     fields=[]),
   ],
-  serialized_start=2397,
-  serialized_end=2636,
+  serialized_start=2901,
+  serialized_end=3140,
 )
 
 _POSTPROCESSINGSDEPRECATED = _descriptor.Descriptor(
   name='PostprocessingsDeprecated',
   full_name='buffers.protobuf.nn.postprocessing.PostprocessingsDeprecated',
   filename=None,
   file=DESCRIPTOR,
@@ -855,24 +1002,25 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2251,
-  serialized_end=2636,
+  serialized_start=2755,
+  serialized_end=3140,
 )
 
 _POSTPROCESSING.fields_by_name['anchored_output'].message_type = _ANCHOREDOUTPUT
 _POSTPROCESSING.fields_by_name['direct_output'].message_type = _DIRECTOUTPUT
 _POSTPROCESSING.fields_by_name['yolo_output'].message_type = _YOLOOUTPUT
 _POSTPROCESSING.fields_by_name['yolov3_output'].message_type = _YOLOV3OUTPUT
 _POSTPROCESSING.fields_by_name['tensors_output'].message_type = _RAWTENSORSOUTPUT
 _POSTPROCESSING.fields_by_name['standard_output'].message_type = _STANDARDOUTPUT
+_POSTPROCESSING.fields_by_name['instance_segmentation_output'].message_type = _INSTANCESEGMENTATIONOUTPUT
 _POSTPROCESSING.oneofs_by_name['type'].fields.append(
   _POSTPROCESSING.fields_by_name['anchored_output'])
 _POSTPROCESSING.fields_by_name['anchored_output'].containing_oneof = _POSTPROCESSING.oneofs_by_name['type']
 _POSTPROCESSING.oneofs_by_name['type'].fields.append(
   _POSTPROCESSING.fields_by_name['direct_output'])
 _POSTPROCESSING.fields_by_name['direct_output'].containing_oneof = _POSTPROCESSING.oneofs_by_name['type']
 _POSTPROCESSING.oneofs_by_name['type'].fields.append(
@@ -883,14 +1031,17 @@
 _POSTPROCESSING.fields_by_name['yolov3_output'].containing_oneof = _POSTPROCESSING.oneofs_by_name['type']
 _POSTPROCESSING.oneofs_by_name['type'].fields.append(
   _POSTPROCESSING.fields_by_name['tensors_output'])
 _POSTPROCESSING.fields_by_name['tensors_output'].containing_oneof = _POSTPROCESSING.oneofs_by_name['type']
 _POSTPROCESSING.oneofs_by_name['type'].fields.append(
   _POSTPROCESSING.fields_by_name['standard_output'])
 _POSTPROCESSING.fields_by_name['standard_output'].containing_oneof = _POSTPROCESSING.oneofs_by_name['type']
+_POSTPROCESSING.oneofs_by_name['type'].fields.append(
+  _POSTPROCESSING.fields_by_name['instance_segmentation_output'])
+_POSTPROCESSING.fields_by_name['instance_segmentation_output'].containing_oneof = _POSTPROCESSING.oneofs_by_name['type']
 _POSTPROCESSINGS.fields_by_name['postprocessings'].message_type = _POSTPROCESSING
 _LABELSOUTPUT_LABEL.containing_type = _LABELSOUTPUT
 _LABELSOUTPUT.fields_by_name['labels'].message_type = _LABELSOUTPUT_LABEL
 _LABELSOUTPUT.fields_by_name['roi'].enum_type = _LABELSOUTPUT_ROITYPE
 _LABELSOUTPUT_ROITYPE.containing_type = _LABELSOUTPUT
 _OUTPUTS_OUTPUTMIX.fields_by_name['labels'].message_type = _LABELSOUTPUT
 _OUTPUTS_OUTPUTMIX.fields_by_name['text'].message_type = _TEXTOUTPUT
@@ -920,14 +1071,20 @@
 _DETECTION_OUTPUTMIX.oneofs_by_name['type'].fields.append(
   _DETECTION_OUTPUTMIX.fields_by_name['yolov3_output'])
 _DETECTION_OUTPUTMIX.fields_by_name['yolov3_output'].containing_oneof = _DETECTION_OUTPUTMIX.oneofs_by_name['type']
 _DETECTION_OUTPUTMIX.oneofs_by_name['type'].fields.append(
   _DETECTION_OUTPUTMIX.fields_by_name['standard_output'])
 _DETECTION_OUTPUTMIX.fields_by_name['standard_output'].containing_oneof = _DETECTION_OUTPUTMIX.oneofs_by_name['type']
 _DETECTION.fields_by_name['output_mix'].message_type = _DETECTION_OUTPUTMIX
+_SEGMENTATION_OUTPUTMIX.fields_by_name['instance_segmentation_output'].message_type = _INSTANCESEGMENTATIONOUTPUT
+_SEGMENTATION_OUTPUTMIX.containing_type = _SEGMENTATION
+_SEGMENTATION_OUTPUTMIX.oneofs_by_name['type'].fields.append(
+  _SEGMENTATION_OUTPUTMIX.fields_by_name['instance_segmentation_output'])
+_SEGMENTATION_OUTPUTMIX.fields_by_name['instance_segmentation_output'].containing_oneof = _SEGMENTATION_OUTPUTMIX.oneofs_by_name['type']
+_SEGMENTATION.fields_by_name['output_mix'].message_type = _SEGMENTATION_OUTPUTMIX
 _POSTPROCESSINGSDEPRECATED_POSTPROCESSINGMIXDEPRECATED.fields_by_name['classification'].message_type = _CLASSIFICATION
 _POSTPROCESSINGSDEPRECATED_POSTPROCESSINGMIXDEPRECATED.fields_by_name['detection'].message_type = _DETECTION
 _POSTPROCESSINGSDEPRECATED_POSTPROCESSINGMIXDEPRECATED.fields_by_name['ocr'].message_type = _OCR
 _POSTPROCESSINGSDEPRECATED_POSTPROCESSINGMIXDEPRECATED.containing_type = _POSTPROCESSINGSDEPRECATED
 _POSTPROCESSINGSDEPRECATED_POSTPROCESSINGMIXDEPRECATED.oneofs_by_name['type'].fields.append(
   _POSTPROCESSINGSDEPRECATED_POSTPROCESSINGMIXDEPRECATED.fields_by_name['classification'])
 _POSTPROCESSINGSDEPRECATED_POSTPROCESSINGMIXDEPRECATED.fields_by_name['classification'].containing_oneof = _POSTPROCESSINGSDEPRECATED_POSTPROCESSINGMIXDEPRECATED.oneofs_by_name['type']
@@ -936,26 +1093,28 @@
 _POSTPROCESSINGSDEPRECATED_POSTPROCESSINGMIXDEPRECATED.fields_by_name['detection'].containing_oneof = _POSTPROCESSINGSDEPRECATED_POSTPROCESSINGMIXDEPRECATED.oneofs_by_name['type']
 _POSTPROCESSINGSDEPRECATED_POSTPROCESSINGMIXDEPRECATED.oneofs_by_name['type'].fields.append(
   _POSTPROCESSINGSDEPRECATED_POSTPROCESSINGMIXDEPRECATED.fields_by_name['ocr'])
 _POSTPROCESSINGSDEPRECATED_POSTPROCESSINGMIXDEPRECATED.fields_by_name['ocr'].containing_oneof = _POSTPROCESSINGSDEPRECATED_POSTPROCESSINGMIXDEPRECATED.oneofs_by_name['type']
 _POSTPROCESSINGSDEPRECATED.fields_by_name['postprocessings'].message_type = _POSTPROCESSINGSDEPRECATED_POSTPROCESSINGMIXDEPRECATED
 DESCRIPTOR.message_types_by_name['RawTensorsOutput'] = _RAWTENSORSOUTPUT
 DESCRIPTOR.message_types_by_name['StandardOutput'] = _STANDARDOUTPUT
+DESCRIPTOR.message_types_by_name['InstanceSegmentationOutput'] = _INSTANCESEGMENTATIONOUTPUT
 DESCRIPTOR.message_types_by_name['AnchoredOutput'] = _ANCHOREDOUTPUT
 DESCRIPTOR.message_types_by_name['DirectOutput'] = _DIRECTOUTPUT
 DESCRIPTOR.message_types_by_name['YoloOutput'] = _YOLOOUTPUT
 DESCRIPTOR.message_types_by_name['YoloV3Output'] = _YOLOV3OUTPUT
 DESCRIPTOR.message_types_by_name['PostProcessing'] = _POSTPROCESSING
 DESCRIPTOR.message_types_by_name['PostProcessings'] = _POSTPROCESSINGS
 DESCRIPTOR.message_types_by_name['LabelsOutput'] = _LABELSOUTPUT
 DESCRIPTOR.message_types_by_name['TextOutput'] = _TEXTOUTPUT
 DESCRIPTOR.message_types_by_name['Outputs'] = _OUTPUTS
 DESCRIPTOR.message_types_by_name['Classification'] = _CLASSIFICATION
 DESCRIPTOR.message_types_by_name['Detection'] = _DETECTION
 DESCRIPTOR.message_types_by_name['OCR'] = _OCR
+DESCRIPTOR.message_types_by_name['Segmentation'] = _SEGMENTATION
 DESCRIPTOR.message_types_by_name['PostprocessingsDeprecated'] = _POSTPROCESSINGSDEPRECATED
 _sym_db.RegisterFileDescriptor(DESCRIPTOR)
 
 RawTensorsOutput = _reflection.GeneratedProtocolMessageType('RawTensorsOutput', (_message.Message,), {
   'DESCRIPTOR' : _RAWTENSORSOUTPUT,
   '__module__' : 'buffers.protobuf.nn.Postprocessing_pb2'
   # @@protoc_insertion_point(class_scope:buffers.protobuf.nn.postprocessing.RawTensorsOutput)
@@ -965,14 +1124,21 @@
 StandardOutput = _reflection.GeneratedProtocolMessageType('StandardOutput', (_message.Message,), {
   'DESCRIPTOR' : _STANDARDOUTPUT,
   '__module__' : 'buffers.protobuf.nn.Postprocessing_pb2'
   # @@protoc_insertion_point(class_scope:buffers.protobuf.nn.postprocessing.StandardOutput)
   })
 _sym_db.RegisterMessage(StandardOutput)
 
+InstanceSegmentationOutput = _reflection.GeneratedProtocolMessageType('InstanceSegmentationOutput', (_message.Message,), {
+  'DESCRIPTOR' : _INSTANCESEGMENTATIONOUTPUT,
+  '__module__' : 'buffers.protobuf.nn.Postprocessing_pb2'
+  # @@protoc_insertion_point(class_scope:buffers.protobuf.nn.postprocessing.InstanceSegmentationOutput)
+  })
+_sym_db.RegisterMessage(InstanceSegmentationOutput)
+
 AnchoredOutput = _reflection.GeneratedProtocolMessageType('AnchoredOutput', (_message.Message,), {
   'DESCRIPTOR' : _ANCHOREDOUTPUT,
   '__module__' : 'buffers.protobuf.nn.Postprocessing_pb2'
   # @@protoc_insertion_point(class_scope:buffers.protobuf.nn.postprocessing.AnchoredOutput)
   })
 _sym_db.RegisterMessage(AnchoredOutput)
 
@@ -1073,14 +1239,29 @@
 OCR = _reflection.GeneratedProtocolMessageType('OCR', (_message.Message,), {
   'DESCRIPTOR' : _OCR,
   '__module__' : 'buffers.protobuf.nn.Postprocessing_pb2'
   # @@protoc_insertion_point(class_scope:buffers.protobuf.nn.postprocessing.OCR)
   })
 _sym_db.RegisterMessage(OCR)
 
+Segmentation = _reflection.GeneratedProtocolMessageType('Segmentation', (_message.Message,), {
+
+  'OutputMix' : _reflection.GeneratedProtocolMessageType('OutputMix', (_message.Message,), {
+    'DESCRIPTOR' : _SEGMENTATION_OUTPUTMIX,
+    '__module__' : 'buffers.protobuf.nn.Postprocessing_pb2'
+    # @@protoc_insertion_point(class_scope:buffers.protobuf.nn.postprocessing.Segmentation.OutputMix)
+    })
+  ,
+  'DESCRIPTOR' : _SEGMENTATION,
+  '__module__' : 'buffers.protobuf.nn.Postprocessing_pb2'
+  # @@protoc_insertion_point(class_scope:buffers.protobuf.nn.postprocessing.Segmentation)
+  })
+_sym_db.RegisterMessage(Segmentation)
+_sym_db.RegisterMessage(Segmentation.OutputMix)
+
 PostprocessingsDeprecated = _reflection.GeneratedProtocolMessageType('PostprocessingsDeprecated', (_message.Message,), {
 
   'PostprocessingMixDeprecated' : _reflection.GeneratedProtocolMessageType('PostprocessingMixDeprecated', (_message.Message,), {
     'DESCRIPTOR' : _POSTPROCESSINGSDEPRECATED_POSTPROCESSINGMIXDEPRECATED,
     '__module__' : 'buffers.protobuf.nn.Postprocessing_pb2'
     # @@protoc_insertion_point(class_scope:buffers.protobuf.nn.postprocessing.PostprocessingsDeprecated.PostprocessingMixDeprecated)
     })
```

### Comparing `deepomatic-rpc-0.8.8/deepomatic/rpc/buffers/protobuf/nn/frameworks/Caffe_pb2.py` & `deepomatic-rpc-0.8.9/deepomatic/rpc/buffers/protobuf/nn/frameworks/Caffe_pb2.py`

 * *Files identical despite different names*

### Comparing `deepomatic-rpc-0.8.8/deepomatic/rpc/buffers/protobuf/nn/Result_pb2.py` & `deepomatic-rpc-0.8.9/deepomatic/rpc/buffers/protobuf/nn/Result_pb2.py`

 * *Files identical despite different names*

### Comparing `deepomatic-rpc-0.8.8/deepomatic/rpc/buffers/protobuf/nn/Preprocessing_pb2.py` & `deepomatic-rpc-0.8.9/deepomatic/rpc/buffers/protobuf/nn/Preprocessing_pb2.py`

 * *Files identical despite different names*

### Comparing `deepomatic-rpc-0.8.8/deepomatic/rpc/buffers/protobuf/nn/Command_pb2.py` & `deepomatic-rpc-0.8.9/deepomatic/rpc/buffers/protobuf/nn/Command_pb2.py`

 * *Files identical despite different names*

### Comparing `deepomatic-rpc-0.8.8/deepomatic/rpc/buffers/protobuf/nn/v07/Results_pb2.py` & `deepomatic-rpc-0.8.9/deepomatic/rpc/buffers/protobuf/nn/v07/Results_pb2.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='buffers/protobuf/nn/v07/Results.proto',
   package='buffers.protobuf.nn.v07.results',
   syntax='proto3',
   serialized_options=None,
   create_key=_descriptor._internal_create_key,
-  serialized_pb=b'\n%buffers/protobuf/nn/v07/Results.proto\x12\x1f\x62uffers.protobuf.nn.v07.results\x1a#buffers/protobuf/common/Image.proto\"\x83\x01\n\tInference\x12\x42\n\x07tensors\x18\x01 \x03(\x0b\x32\x31.buffers.protobuf.nn.v07.results.Inference.Tensor\x1a\x32\n\x06Tensor\x12\x0c\n\x04\x64ims\x18\x01 \x03(\x05\x12\x0c\n\x04\x64\x61ta\x18\x02 \x03(\x02\x12\x0c\n\x04name\x18\x03 \x01(\t\"O\n\x03ROI\x12\x11\n\tregion_id\x18\x01 \x01(\r\x12-\n\x04\x62\x62ox\x18\x03 \x01(\x0b\x32\x1d.buffers.protobuf.common.BBoxH\x00\x42\x06\n\x04type\"\xb2\x02\n\x0cLabelsOutput\x12K\n\tpredicted\x18\x01 \x03(\x0b\x32\x38.buffers.protobuf.nn.v07.results.LabelsOutput.Prediction\x12K\n\tdiscarded\x18\x02 \x03(\x0b\x32\x38.buffers.protobuf.nn.v07.results.LabelsOutput.Prediction\x1a\x87\x01\n\nPrediction\x12\x10\n\x08label_id\x18\x01 \x01(\r\x12\x12\n\nlabel_name\x18\x02 \x01(\t\x12\r\n\x05score\x18\x03 \x01(\x02\x12\x11\n\tthreshold\x18\x04 \x01(\x02\x12\x31\n\x03roi\x18\x05 \x01(\x0b\x32$.buffers.protobuf.nn.v07.results.ROI\")\n\x0cScalarOutput\x12\x11\n\x07integer\x18\x01 \x01(\x04H\x00\x42\x06\n\x04type\"\x1a\n\nTextOutput\x12\x0c\n\x04text\x18\x01 \x01(\t\"\xd7\x01\n\x0eRecognitionMix\x12?\n\x06labels\x18\x01 \x01(\x0b\x32-.buffers.protobuf.nn.v07.results.LabelsOutputH\x00\x12?\n\x06scalar\x18\x02 \x01(\x0b\x32-.buffers.protobuf.nn.v07.results.ScalarOutputH\x00\x12;\n\x04text\x18\x03 \x01(\x0b\x32+.buffers.protobuf.nn.v07.results.TextOutputH\x00\x42\x06\n\x04type\"O\n\x0bRecognition\x12@\n\x07outputs\x18\x01 \x03(\x0b\x32/.buffers.protobuf.nn.v07.results.RecognitionMixb\x06proto3'
+  serialized_pb=b'\n%buffers/protobuf/nn/v07/Results.proto\x12\x1f\x62uffers.protobuf.nn.v07.results\x1a#buffers/protobuf/common/Image.proto\"\x83\x01\n\tInference\x12\x42\n\x07tensors\x18\x01 \x03(\x0b\x32\x31.buffers.protobuf.nn.v07.results.Inference.Tensor\x1a\x32\n\x06Tensor\x12\x0c\n\x04\x64ims\x18\x01 \x03(\x05\x12\x0c\n\x04\x64\x61ta\x18\x02 \x03(\x02\x12\x0c\n\x04name\x18\x03 \x01(\t\"g\n\x04Mask\x12+\n\x04\x62\x62ox\x18\x01 \x01(\x0b\x32\x1d.buffers.protobuf.common.BBox\x12\x32\n\x08polygons\x18\x02 \x03(\x0b\x32 .buffers.protobuf.common.Polygon\"\x86\x01\n\x03ROI\x12\x11\n\tregion_id\x18\x01 \x01(\r\x12-\n\x04\x62\x62ox\x18\x03 \x01(\x0b\x32\x1d.buffers.protobuf.common.BBoxH\x00\x12\x35\n\x04mask\x18\x04 \x01(\x0b\x32%.buffers.protobuf.nn.v07.results.MaskH\x00\x42\x06\n\x04type\"\xb2\x02\n\x0cLabelsOutput\x12K\n\tpredicted\x18\x01 \x03(\x0b\x32\x38.buffers.protobuf.nn.v07.results.LabelsOutput.Prediction\x12K\n\tdiscarded\x18\x02 \x03(\x0b\x32\x38.buffers.protobuf.nn.v07.results.LabelsOutput.Prediction\x1a\x87\x01\n\nPrediction\x12\x10\n\x08label_id\x18\x01 \x01(\r\x12\x12\n\nlabel_name\x18\x02 \x01(\t\x12\r\n\x05score\x18\x03 \x01(\x02\x12\x11\n\tthreshold\x18\x04 \x01(\x02\x12\x31\n\x03roi\x18\x05 \x01(\x0b\x32$.buffers.protobuf.nn.v07.results.ROI\")\n\x0cScalarOutput\x12\x11\n\x07integer\x18\x01 \x01(\x04H\x00\x42\x06\n\x04type\"\x1a\n\nTextOutput\x12\x0c\n\x04text\x18\x01 \x01(\t\"\xd7\x01\n\x0eRecognitionMix\x12?\n\x06labels\x18\x01 \x01(\x0b\x32-.buffers.protobuf.nn.v07.results.LabelsOutputH\x00\x12?\n\x06scalar\x18\x02 \x01(\x0b\x32-.buffers.protobuf.nn.v07.results.ScalarOutputH\x00\x12;\n\x04text\x18\x03 \x01(\x0b\x32+.buffers.protobuf.nn.v07.results.TextOutputH\x00\x42\x06\n\x04type\"O\n\x0bRecognition\x12@\n\x07outputs\x18\x01 \x03(\x0b\x32/.buffers.protobuf.nn.v07.results.RecognitionMixb\x06proto3'
   ,
   dependencies=[buffers_dot_protobuf_dot_common_dot_Image__pb2.DESCRIPTOR,])
 
 
 
 
 _INFERENCE_TENSOR = _descriptor.Descriptor(
@@ -100,14 +100,53 @@
   oneofs=[
   ],
   serialized_start=112,
   serialized_end=243,
 )
 
 
+_MASK = _descriptor.Descriptor(
+  name='Mask',
+  full_name='buffers.protobuf.nn.v07.results.Mask',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='bbox', full_name='buffers.protobuf.nn.v07.results.Mask.bbox', index=0,
+      number=1, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='polygons', full_name='buffers.protobuf.nn.v07.results.Mask.polygons', index=1,
+      number=2, type=11, cpp_type=10, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=245,
+  serialized_end=348,
+)
+
+
 _ROI = _descriptor.Descriptor(
   name='ROI',
   full_name='buffers.protobuf.nn.v07.results.ROI',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
@@ -122,14 +161,21 @@
     _descriptor.FieldDescriptor(
       name='bbox', full_name='buffers.protobuf.nn.v07.results.ROI.bbox', index=1,
       number=3, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='mask', full_name='buffers.protobuf.nn.v07.results.ROI.mask', index=2,
+      number=4, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
   ],
   serialized_options=None,
@@ -139,16 +185,16 @@
   oneofs=[
     _descriptor.OneofDescriptor(
       name='type', full_name='buffers.protobuf.nn.v07.results.ROI.type',
       index=0, containing_type=None,
       create_key=_descriptor._internal_create_key,
     fields=[]),
   ],
-  serialized_start=245,
-  serialized_end=324,
+  serialized_start=351,
+  serialized_end=485,
 )
 
 
 _LABELSOUTPUT_PREDICTION = _descriptor.Descriptor(
   name='Prediction',
   full_name='buffers.protobuf.nn.v07.results.LabelsOutput.Prediction',
   filename=None,
@@ -199,16 +245,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=498,
-  serialized_end=633,
+  serialized_start=659,
+  serialized_end=794,
 )
 
 _LABELSOUTPUT = _descriptor.Descriptor(
   name='LabelsOutput',
   full_name='buffers.protobuf.nn.v07.results.LabelsOutput',
   filename=None,
   file=DESCRIPTOR,
@@ -237,16 +283,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=327,
-  serialized_end=633,
+  serialized_start=488,
+  serialized_end=794,
 )
 
 
 _SCALAROUTPUT = _descriptor.Descriptor(
   name='ScalarOutput',
   full_name='buffers.protobuf.nn.v07.results.ScalarOutput',
   filename=None,
@@ -274,16 +320,16 @@
   oneofs=[
     _descriptor.OneofDescriptor(
       name='type', full_name='buffers.protobuf.nn.v07.results.ScalarOutput.type',
       index=0, containing_type=None,
       create_key=_descriptor._internal_create_key,
     fields=[]),
   ],
-  serialized_start=635,
-  serialized_end=676,
+  serialized_start=796,
+  serialized_end=837,
 )
 
 
 _TEXTOUTPUT = _descriptor.Descriptor(
   name='TextOutput',
   full_name='buffers.protobuf.nn.v07.results.TextOutput',
   filename=None,
@@ -306,16 +352,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=678,
-  serialized_end=704,
+  serialized_start=839,
+  serialized_end=865,
 )
 
 
 _RECOGNITIONMIX = _descriptor.Descriptor(
   name='RecognitionMix',
   full_name='buffers.protobuf.nn.v07.results.RecognitionMix',
   filename=None,
@@ -357,16 +403,16 @@
   oneofs=[
     _descriptor.OneofDescriptor(
       name='type', full_name='buffers.protobuf.nn.v07.results.RecognitionMix.type',
       index=0, containing_type=None,
       create_key=_descriptor._internal_create_key,
     fields=[]),
   ],
-  serialized_start=707,
-  serialized_end=922,
+  serialized_start=868,
+  serialized_end=1083,
 )
 
 
 _RECOGNITION = _descriptor.Descriptor(
   name='Recognition',
   full_name='buffers.protobuf.nn.v07.results.Recognition',
   filename=None,
@@ -389,24 +435,30 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=924,
-  serialized_end=1003,
+  serialized_start=1085,
+  serialized_end=1164,
 )
 
 _INFERENCE_TENSOR.containing_type = _INFERENCE
 _INFERENCE.fields_by_name['tensors'].message_type = _INFERENCE_TENSOR
+_MASK.fields_by_name['bbox'].message_type = buffers_dot_protobuf_dot_common_dot_Image__pb2._BBOX
+_MASK.fields_by_name['polygons'].message_type = buffers_dot_protobuf_dot_common_dot_Image__pb2._POLYGON
 _ROI.fields_by_name['bbox'].message_type = buffers_dot_protobuf_dot_common_dot_Image__pb2._BBOX
+_ROI.fields_by_name['mask'].message_type = _MASK
 _ROI.oneofs_by_name['type'].fields.append(
   _ROI.fields_by_name['bbox'])
 _ROI.fields_by_name['bbox'].containing_oneof = _ROI.oneofs_by_name['type']
+_ROI.oneofs_by_name['type'].fields.append(
+  _ROI.fields_by_name['mask'])
+_ROI.fields_by_name['mask'].containing_oneof = _ROI.oneofs_by_name['type']
 _LABELSOUTPUT_PREDICTION.fields_by_name['roi'].message_type = _ROI
 _LABELSOUTPUT_PREDICTION.containing_type = _LABELSOUTPUT
 _LABELSOUTPUT.fields_by_name['predicted'].message_type = _LABELSOUTPUT_PREDICTION
 _LABELSOUTPUT.fields_by_name['discarded'].message_type = _LABELSOUTPUT_PREDICTION
 _SCALAROUTPUT.oneofs_by_name['type'].fields.append(
   _SCALAROUTPUT.fields_by_name['integer'])
 _SCALAROUTPUT.fields_by_name['integer'].containing_oneof = _SCALAROUTPUT.oneofs_by_name['type']
@@ -420,14 +472,15 @@
   _RECOGNITIONMIX.fields_by_name['scalar'])
 _RECOGNITIONMIX.fields_by_name['scalar'].containing_oneof = _RECOGNITIONMIX.oneofs_by_name['type']
 _RECOGNITIONMIX.oneofs_by_name['type'].fields.append(
   _RECOGNITIONMIX.fields_by_name['text'])
 _RECOGNITIONMIX.fields_by_name['text'].containing_oneof = _RECOGNITIONMIX.oneofs_by_name['type']
 _RECOGNITION.fields_by_name['outputs'].message_type = _RECOGNITIONMIX
 DESCRIPTOR.message_types_by_name['Inference'] = _INFERENCE
+DESCRIPTOR.message_types_by_name['Mask'] = _MASK
 DESCRIPTOR.message_types_by_name['ROI'] = _ROI
 DESCRIPTOR.message_types_by_name['LabelsOutput'] = _LABELSOUTPUT
 DESCRIPTOR.message_types_by_name['ScalarOutput'] = _SCALAROUTPUT
 DESCRIPTOR.message_types_by_name['TextOutput'] = _TEXTOUTPUT
 DESCRIPTOR.message_types_by_name['RecognitionMix'] = _RECOGNITIONMIX
 DESCRIPTOR.message_types_by_name['Recognition'] = _RECOGNITION
 _sym_db.RegisterFileDescriptor(DESCRIPTOR)
@@ -443,14 +496,21 @@
   'DESCRIPTOR' : _INFERENCE,
   '__module__' : 'buffers.protobuf.nn.v07.Results_pb2'
   # @@protoc_insertion_point(class_scope:buffers.protobuf.nn.v07.results.Inference)
   })
 _sym_db.RegisterMessage(Inference)
 _sym_db.RegisterMessage(Inference.Tensor)
 
+Mask = _reflection.GeneratedProtocolMessageType('Mask', (_message.Message,), {
+  'DESCRIPTOR' : _MASK,
+  '__module__' : 'buffers.protobuf.nn.v07.Results_pb2'
+  # @@protoc_insertion_point(class_scope:buffers.protobuf.nn.v07.results.Mask)
+  })
+_sym_db.RegisterMessage(Mask)
+
 ROI = _reflection.GeneratedProtocolMessageType('ROI', (_message.Message,), {
   'DESCRIPTOR' : _ROI,
   '__module__' : 'buffers.protobuf.nn.v07.Results_pb2'
   # @@protoc_insertion_point(class_scope:buffers.protobuf.nn.v07.results.ROI)
   })
 _sym_db.RegisterMessage(ROI)
```

### Comparing `deepomatic-rpc-0.8.8/deepomatic/rpc/buffers/protobuf/nn/v07/Commands_pb2.py` & `deepomatic-rpc-0.8.9/deepomatic/rpc/buffers/protobuf/nn/v07/Commands_pb2.py`

 * *Files identical despite different names*

### Comparing `deepomatic-rpc-0.8.8/deepomatic/rpc/buffers/protobuf/nn/v07/Inputs_pb2.py` & `deepomatic-rpc-0.8.9/deepomatic/rpc/buffers/protobuf/nn/v07/Inputs_pb2.py`

 * *Files identical despite different names*

### Comparing `deepomatic-rpc-0.8.8/deepomatic/rpc/buffers/protobuf/nn/v07/Workflows_pb2.py` & `deepomatic-rpc-0.8.9/deepomatic/rpc/buffers/protobuf/nn/v07/Workflows_pb2.py`

 * *Files identical despite different names*

### Comparing `deepomatic-rpc-0.8.8/deepomatic/rpc/buffers/protobuf/nn/Message_pb2.py` & `deepomatic-rpc-0.8.9/deepomatic/rpc/buffers/protobuf/nn/Message_pb2.py`

 * *Files identical despite different names*

### Comparing `deepomatic-rpc-0.8.8/deepomatic/rpc/amqp/client.py` & `deepomatic-rpc-0.8.9/deepomatic/rpc/amqp/client.py`

 * *Files identical despite different names*

### Comparing `deepomatic-rpc-0.8.8/deepomatic/rpc/amqp/entities.py` & `deepomatic-rpc-0.8.9/deepomatic/rpc/amqp/entities.py`

 * *Files identical despite different names*

### Comparing `deepomatic-rpc-0.8.8/deepomatic/rpc/response.py` & `deepomatic-rpc-0.8.9/deepomatic/rpc/response.py`

 * *Files identical despite different names*

### Comparing `deepomatic-rpc-0.8.8/deepomatic/rpc/helpers/v07_proto.py` & `deepomatic-rpc-0.8.9/deepomatic/rpc/helpers/v07_proto.py`

 * *Files identical despite different names*

### Comparing `deepomatic-rpc-0.8.8/deepomatic/rpc/helpers/proto.py` & `deepomatic-rpc-0.8.9/deepomatic/rpc/helpers/proto.py`

 * *Files identical despite different names*

### Comparing `deepomatic-rpc-0.8.8/deepomatic_rpc.egg-info/PKG-INFO` & `deepomatic-rpc-0.8.9/deepomatic_rpc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepomatic-rpc
-Version: 0.8.8
+Version: 0.8.9
 Summary: Deepomatic RPC python client
 Home-page: https://www.deepomatic.com
 Author: deepomatic
 Author-email: support@deepomatic.com
 License: UNLICENSED
 Project-URL: Product, https://www.deepomatic.com
 Description: # Table of contents
```

### Comparing `deepomatic-rpc-0.8.8/deepomatic_rpc.egg-info/SOURCES.txt` & `deepomatic-rpc-0.8.9/deepomatic_rpc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deepomatic-rpc-0.8.8/README.md` & `deepomatic-rpc-0.8.9/README.md`

 * *Files identical despite different names*

### Comparing `deepomatic-rpc-0.8.8/setup.py` & `deepomatic-rpc-0.8.9/setup.py`

 * *Files identical despite different names*

