# Comparing `tmp/flwr_nightly-1.5.0.dev20230608.tar.gz` & `tmp/flwr_nightly-1.5.0.dev20230614.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flwr_nightly-1.5.0.dev20230608.tar", max compression
+gzip compressed data, was "flwr_nightly-1.5.0.dev20230614.tar", max compression
```

## Comparing `flwr_nightly-1.5.0.dev20230608.tar` & `flwr_nightly-1.5.0.dev20230614.tar`

### file list

```diff
@@ -1,113 +1,113 @@
--rw-r--r--   0        0        0    11358 2023-06-08 23:02:45.679186 flwr_nightly-1.5.0.dev20230608/LICENSE
--rw-r--r--   0        0        0    10363 2023-06-08 23:02:45.679186 flwr_nightly-1.5.0.dev20230608/README.md
--rw-r--r--   0        0        0     4333 2023-06-08 23:03:20.659572 flwr_nightly-1.5.0.dev20230608/pyproject.toml
--rw-r--r--   0        0        0      952 2023-06-08 23:02:46.011190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/__init__.py
--rw-r--r--   0        0        0     1164 2023-06-08 23:02:46.011190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/client/__init__.py
--rw-r--r--   0        0        0    13838 2023-06-08 23:02:46.011190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/client/app.py
--rw-r--r--   0        0        0     7681 2023-06-08 23:02:46.011190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/client/client.py
--rw-r--r--   0        0        0     3351 2023-06-08 23:02:46.011190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/client/dpfedavg_numpy_client.py
--rw-r--r--   0        0        0      728 2023-06-08 23:02:46.011190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/client/grpc_client/__init__.py
--rw-r--r--   0        0        0     4293 2023-06-08 23:02:46.011190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/client/grpc_client/connection.py
--rw-r--r--   0        0        0      745 2023-06-08 23:02:46.011190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/client/grpc_rere_client/__init__.py
--rw-r--r--   0        0        0     5476 2023-06-08 23:02:46.011190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/client/grpc_rere_client/connection.py
--rw-r--r--   0        0        0      712 2023-06-08 23:02:46.011190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/client/message_handler/__init__.py
--rw-r--r--   0        0        0     5077 2023-06-08 23:02:46.011190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/client/message_handler/message_handler.py
--rw-r--r--   0        0        0     1686 2023-06-08 23:02:46.011190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/client/message_handler/task_handler.py
--rw-r--r--   0        0        0     5319 2023-06-08 23:02:46.011190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/client/numpy_client.py
--rw-r--r--   0        0        0      728 2023-06-08 23:02:46.011190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/client/rest_client/__init__.py
--rw-r--r--   0        0        0     8336 2023-06-08 23:02:46.011190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/client/rest_client/connection.py
--rw-r--r--   0        0        0     2877 2023-06-08 23:02:46.011190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/common/__init__.py
--rw-r--r--   0        0        0     1876 2023-06-08 23:02:46.011190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/common/address.py
--rw-r--r--   0        0        0     1113 2023-06-08 23:02:46.011190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/common/constant.py
--rw-r--r--   0        0        0      884 2023-06-08 23:02:46.011190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/common/date.py
--rw-r--r--   0        0        0     1828 2023-06-08 23:02:46.011190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/common/dp.py
--rw-r--r--   0        0        0     1890 2023-06-08 23:02:46.011190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/common/grpc.py
--rw-r--r--   0        0        0     3483 2023-06-08 23:02:46.011190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/common/logger.py
--rw-r--r--   0        0        0     2120 2023-06-08 23:02:46.011190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/common/parameter.py
--rw-r--r--   0        0        0    16316 2023-06-08 23:02:46.011190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/common/serde.py
--rw-r--r--   0        0        0     7805 2023-06-08 23:02:46.011190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/common/telemetry.py
--rw-r--r--   0        0        0     3714 2023-06-08 23:02:46.015190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/common/typing.py
--rw-r--r--   0        0        0      848 2023-06-08 23:02:46.015190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/common/version.py
--rw-r--r--   0        0        0      809 2023-06-08 23:02:46.015190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/driver/__init__.py
--rw-r--r--   0        0        0     4826 2023-06-08 23:02:46.015190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/driver/app.py
--rw-r--r--   0        0        0     3909 2023-06-08 23:02:46.015190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/driver/driver.py
--rw-r--r--   0        0        0     4414 2023-06-08 23:02:46.015190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/driver/driver_client_manager.py
--rw-r--r--   0        0        0     5654 2023-06-08 23:02:46.015190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/driver/driver_client_proxy.py
--rw-r--r--   0        0        0      676 2023-06-08 23:02:46.015190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/proto/__init__.py
--rw-r--r--   0        0        0     4663 2023-06-08 23:02:46.015190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/proto/driver_pb2.py
--rw-r--r--   0        0        0     3815 2023-06-08 23:02:46.015190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/proto/driver_pb2.pyi
--rw-r--r--   0        0        0     5727 2023-06-08 23:02:46.015190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/proto/driver_pb2_grpc.py
--rw-r--r--   0        0        0     1617 2023-06-08 23:02:46.015190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/proto/driver_pb2_grpc.pyi
--rw-r--r--   0        0        0     4982 2023-06-08 23:02:46.015190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/proto/fleet_pb2.py
--rw-r--r--   0        0        0     4554 2023-06-08 23:02:46.015190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/proto/fleet_pb2.pyi
--rw-r--r--   0        0        0     4275 2023-06-08 23:02:46.015190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/proto/fleet_pb2_grpc.py
--rw-r--r--   0        0        0     1495 2023-06-08 23:02:46.015190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/proto/fleet_pb2_grpc.pyi
--rw-r--r--   0        0        0     1188 2023-06-08 23:02:46.015190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/proto/node_pb2.py
--rw-r--r--   0        0        0      751 2023-06-08 23:02:46.015190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/proto/node_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-08 23:02:46.015190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/proto/node_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-08 23:02:46.015190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/proto/node_pb2_grpc.pyi
--rw-r--r--   0        0        0     3217 2023-06-08 23:02:46.015190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/proto/task_pb2.py
--rw-r--r--   0        0        0     4286 2023-06-08 23:02:46.015190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/proto/task_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-08 23:02:46.015190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/proto/task_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-08 23:02:46.015190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/proto/task_pb2_grpc.pyi
--rw-r--r--   0        0        0    18721 2023-06-08 23:02:46.015190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/proto/transport_pb2.py
--rw-r--r--   0        0        0    21497 2023-06-08 23:02:46.015190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/proto/transport_pb2.pyi
--rw-r--r--   0        0        0     2598 2023-06-08 23:02:46.015190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/proto/transport_pb2_grpc.py
--rw-r--r--   0        0        0      766 2023-06-08 23:02:46.015190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/proto/transport_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-06-08 23:02:46.015190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/py.typed
--rw-r--r--   0        0        0     1370 2023-06-08 23:02:46.015190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/__init__.py
--rw-r--r--   0        0        0    26342 2023-06-08 23:02:46.015190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/app.py
--rw-r--r--   0        0        0     5941 2023-06-08 23:02:46.015190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/client_manager.py
--rw-r--r--   0        0        0     2228 2023-06-08 23:02:46.015190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/client_proxy.py
--rw-r--r--   0        0        0     1058 2023-06-08 23:02:46.015190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/criterion.py
--rw-r--r--   0        0        0      705 2023-06-08 23:02:46.015190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/driver/__init__.py
--rw-r--r--   0        0        0     3919 2023-06-08 23:02:46.015190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/driver/driver_servicer.py
--rw-r--r--   0        0        0      704 2023-06-08 23:02:46.015190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/fleet/__init__.py
--rw-r--r--   0        0        0      728 2023-06-08 23:02:46.015190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/fleet/grpc_bidi/__init__.py
--rw-r--r--   0        0        0     4467 2023-06-08 23:02:46.015190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/fleet/grpc_bidi/driver_client_manager.py
--rw-r--r--   0        0        0     5602 2023-06-08 23:02:46.015190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/fleet/grpc_bidi/flower_service_servicer.py
--rw-r--r--   0        0        0     6416 2023-06-08 23:02:46.015190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/fleet/grpc_bidi/grpc_bridge.py
--rw-r--r--   0        0        0     4651 2023-06-08 23:02:46.015190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/fleet/grpc_bidi/grpc_client_proxy.py
--rw-r--r--   0        0        0    11523 2023-06-08 23:02:46.015190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/fleet/grpc_bidi/grpc_server.py
--rw-r--r--   0        0        0     6314 2023-06-08 23:02:46.015190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/fleet/grpc_bidi/ins_scheduler.py
--rw-r--r--   0        0        0      751 2023-06-08 23:02:46.015190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/fleet/grpc_rere/__init__.py
--rw-r--r--   0        0        0     1858 2023-06-08 23:02:46.015190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/fleet/grpc_rere/fleet_servicer.py
--rw-r--r--   0        0        0      724 2023-06-08 23:02:46.015190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/fleet/message_handler/__init__.py
--rw-r--r--   0        0        0     2026 2023-06-08 23:02:46.015190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/fleet/message_handler/message_handler.py
--rw-r--r--   0        0        0      728 2023-06-08 23:02:46.015190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/fleet/rest_rere/__init__.py
--rw-r--r--   0        0        0     3718 2023-06-08 23:02:46.015190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/fleet/rest_rere/rest_api.py
--rw-r--r--   0        0        0     4457 2023-06-08 23:02:46.015190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/history.py
--rw-r--r--   0        0        0    15963 2023-06-08 23:02:46.019190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/server.py
--rw-r--r--   0        0        0      996 2023-06-08 23:02:46.019190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/state/__init__.py
--rw-r--r--   0        0        0     6521 2023-06-08 23:02:46.019190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/state/in_memory_state.py
--rw-r--r--   0        0        0    19280 2023-06-08 23:02:46.019190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/state/sqlite_state.py
--rw-r--r--   0        0        0     4805 2023-06-08 23:02:46.019190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/state/state.py
--rw-r--r--   0        0        0     1648 2023-06-08 23:02:46.019190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/state/state_factory.py
--rw-r--r--   0        0        0     1667 2023-06-08 23:02:46.019190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/strategy/__init__.py
--rw-r--r--   0        0        0     6099 2023-06-08 23:02:46.019190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/strategy/aggregate.py
--rw-r--r--   0        0        0     4508 2023-06-08 23:02:46.019190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/strategy/dpfedavg_adaptive.py
--rw-r--r--   0        0        0     4867 2023-06-08 23:02:46.019190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/strategy/dpfedavg_fixed.py
--rw-r--r--   0        0        0     5830 2023-06-08 23:02:46.019190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/strategy/fault_tolerant_fedavg.py
--rw-r--r--   0        0        0     6722 2023-06-08 23:02:46.019190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/strategy/fedadagrad.py
--rw-r--r--   0        0        0     7004 2023-06-08 23:02:46.019190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/strategy/fedadam.py
--rw-r--r--   0        0        0    11487 2023-06-08 23:02:46.019190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/strategy/fedavg.py
--rw-r--r--   0        0        0     9977 2023-06-08 23:02:46.019190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/strategy/fedavg_android.py
--rw-r--r--   0        0        0     8244 2023-06-08 23:02:46.019190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/strategy/fedavgm.py
--rw-r--r--   0        0        0     2666 2023-06-08 23:02:46.019190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/strategy/fedmedian.py
--rw-r--r--   0        0        0     5385 2023-06-08 23:02:46.019190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/strategy/fedopt.py
--rw-r--r--   0        0        0     7057 2023-06-08 23:02:46.019190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/strategy/fedprox.py
--rw-r--r--   0        0        0     5916 2023-06-08 23:02:46.019190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/strategy/fedtrimmedavg.py
--rw-r--r--   0        0        0     3368 2023-06-08 23:02:46.019190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/strategy/fedxgb_nn_avg.py
--rw-r--r--   0        0        0     7036 2023-06-08 23:02:46.019190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/strategy/fedyogi.py
--rw-r--r--   0        0        0     6302 2023-06-08 23:02:46.019190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/strategy/krum.py
--rw-r--r--   0        0        0    10139 2023-06-08 23:02:46.019190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/strategy/qfedavg.py
--rw-r--r--   0        0        0     7484 2023-06-08 23:02:46.019190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/strategy/strategy.py
--rw-r--r--   0        0        0      901 2023-06-08 23:02:46.019190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/utils/__init__.py
--rw-r--r--   0        0        0     5098 2023-06-08 23:02:46.019190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/utils/tensorboard.py
--rw-r--r--   0        0        0     4941 2023-06-08 23:02:46.019190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/utils/validator.py
--rw-r--r--   0        0        0     1271 2023-06-08 23:02:46.019190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/simulation/__init__.py
--rw-r--r--   0        0        0     7763 2023-06-08 23:02:46.019190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/simulation/app.py
--rw-r--r--   0        0        0      727 2023-06-08 23:02:46.019190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/simulation/ray_transport/__init__.py
--rw-r--r--   0        0        0     5472 2023-06-08 23:02:46.019190 flwr_nightly-1.5.0.dev20230608/src/py/flwr/simulation/ray_transport/ray_client_proxy.py
--rw-r--r--   0        0        0    12494 1970-01-01 00:00:00.000000 flwr_nightly-1.5.0.dev20230608/setup.py
--rw-r--r--   0        0        0    12838 1970-01-01 00:00:00.000000 flwr_nightly-1.5.0.dev20230608/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-06-14 23:02:38.036888 flwr_nightly-1.5.0.dev20230614/LICENSE
+-rw-r--r--   0        0        0    10363 2023-06-14 23:02:38.036888 flwr_nightly-1.5.0.dev20230614/README.md
+-rw-r--r--   0        0        0     4397 2023-06-14 23:03:04.436708 flwr_nightly-1.5.0.dev20230614/pyproject.toml
+-rw-r--r--   0        0        0      952 2023-06-14 23:02:38.324891 flwr_nightly-1.5.0.dev20230614/src/py/flwr/__init__.py
+-rw-r--r--   0        0        0     1164 2023-06-14 23:02:38.324891 flwr_nightly-1.5.0.dev20230614/src/py/flwr/client/__init__.py
+-rw-r--r--   0        0        0    13835 2023-06-14 23:02:38.324891 flwr_nightly-1.5.0.dev20230614/src/py/flwr/client/app.py
+-rw-r--r--   0        0        0     7677 2023-06-14 23:02:38.324891 flwr_nightly-1.5.0.dev20230614/src/py/flwr/client/client.py
+-rw-r--r--   0        0        0     3351 2023-06-14 23:02:38.324891 flwr_nightly-1.5.0.dev20230614/src/py/flwr/client/dpfedavg_numpy_client.py
+-rw-r--r--   0        0        0      728 2023-06-14 23:02:38.324891 flwr_nightly-1.5.0.dev20230614/src/py/flwr/client/grpc_client/__init__.py
+-rw-r--r--   0        0        0     4293 2023-06-14 23:02:38.324891 flwr_nightly-1.5.0.dev20230614/src/py/flwr/client/grpc_client/connection.py
+-rw-r--r--   0        0        0      745 2023-06-14 23:02:38.324891 flwr_nightly-1.5.0.dev20230614/src/py/flwr/client/grpc_rere_client/__init__.py
+-rw-r--r--   0        0        0     5474 2023-06-14 23:02:38.324891 flwr_nightly-1.5.0.dev20230614/src/py/flwr/client/grpc_rere_client/connection.py
+-rw-r--r--   0        0        0      712 2023-06-14 23:02:38.324891 flwr_nightly-1.5.0.dev20230614/src/py/flwr/client/message_handler/__init__.py
+-rw-r--r--   0        0        0     5077 2023-06-14 23:02:38.324891 flwr_nightly-1.5.0.dev20230614/src/py/flwr/client/message_handler/message_handler.py
+-rw-r--r--   0        0        0     1685 2023-06-14 23:02:38.324891 flwr_nightly-1.5.0.dev20230614/src/py/flwr/client/message_handler/task_handler.py
+-rw-r--r--   0        0        0     5318 2023-06-14 23:02:38.324891 flwr_nightly-1.5.0.dev20230614/src/py/flwr/client/numpy_client.py
+-rw-r--r--   0        0        0      728 2023-06-14 23:02:38.324891 flwr_nightly-1.5.0.dev20230614/src/py/flwr/client/rest_client/__init__.py
+-rw-r--r--   0        0        0     8333 2023-06-14 23:02:38.324891 flwr_nightly-1.5.0.dev20230614/src/py/flwr/client/rest_client/connection.py
+-rw-r--r--   0        0        0     2877 2023-06-14 23:02:38.324891 flwr_nightly-1.5.0.dev20230614/src/py/flwr/common/__init__.py
+-rw-r--r--   0        0        0     1875 2023-06-14 23:02:38.324891 flwr_nightly-1.5.0.dev20230614/src/py/flwr/common/address.py
+-rw-r--r--   0        0        0     1113 2023-06-14 23:02:38.324891 flwr_nightly-1.5.0.dev20230614/src/py/flwr/common/constant.py
+-rw-r--r--   0        0        0      884 2023-06-14 23:02:38.324891 flwr_nightly-1.5.0.dev20230614/src/py/flwr/common/date.py
+-rw-r--r--   0        0        0     1791 2023-06-14 23:02:38.324891 flwr_nightly-1.5.0.dev20230614/src/py/flwr/common/dp.py
+-rw-r--r--   0        0        0     1889 2023-06-14 23:02:38.324891 flwr_nightly-1.5.0.dev20230614/src/py/flwr/common/grpc.py
+-rw-r--r--   0        0        0     3482 2023-06-14 23:02:38.324891 flwr_nightly-1.5.0.dev20230614/src/py/flwr/common/logger.py
+-rw-r--r--   0        0        0     2120 2023-06-14 23:02:38.324891 flwr_nightly-1.5.0.dev20230614/src/py/flwr/common/parameter.py
+-rw-r--r--   0        0        0    16315 2023-06-14 23:02:38.324891 flwr_nightly-1.5.0.dev20230614/src/py/flwr/common/serde.py
+-rw-r--r--   0        0        0     7805 2023-06-14 23:02:38.324891 flwr_nightly-1.5.0.dev20230614/src/py/flwr/common/telemetry.py
+-rw-r--r--   0        0        0     3714 2023-06-14 23:02:38.324891 flwr_nightly-1.5.0.dev20230614/src/py/flwr/common/typing.py
+-rw-r--r--   0        0        0      848 2023-06-14 23:02:38.324891 flwr_nightly-1.5.0.dev20230614/src/py/flwr/common/version.py
+-rw-r--r--   0        0        0      809 2023-06-14 23:02:38.324891 flwr_nightly-1.5.0.dev20230614/src/py/flwr/driver/__init__.py
+-rw-r--r--   0        0        0     4826 2023-06-14 23:02:38.324891 flwr_nightly-1.5.0.dev20230614/src/py/flwr/driver/app.py
+-rw-r--r--   0        0        0     3906 2023-06-14 23:02:38.324891 flwr_nightly-1.5.0.dev20230614/src/py/flwr/driver/driver.py
+-rw-r--r--   0        0        0     4414 2023-06-14 23:02:38.324891 flwr_nightly-1.5.0.dev20230614/src/py/flwr/driver/driver_client_manager.py
+-rw-r--r--   0        0        0     5653 2023-06-14 23:02:38.324891 flwr_nightly-1.5.0.dev20230614/src/py/flwr/driver/driver_client_proxy.py
+-rw-r--r--   0        0        0      676 2023-06-14 23:02:38.324891 flwr_nightly-1.5.0.dev20230614/src/py/flwr/proto/__init__.py
+-rw-r--r--   0        0        0     4663 2023-06-14 23:02:38.324891 flwr_nightly-1.5.0.dev20230614/src/py/flwr/proto/driver_pb2.py
+-rw-r--r--   0        0        0     3815 2023-06-14 23:02:38.324891 flwr_nightly-1.5.0.dev20230614/src/py/flwr/proto/driver_pb2.pyi
+-rw-r--r--   0        0        0     5727 2023-06-14 23:02:38.324891 flwr_nightly-1.5.0.dev20230614/src/py/flwr/proto/driver_pb2_grpc.py
+-rw-r--r--   0        0        0     1617 2023-06-14 23:02:38.324891 flwr_nightly-1.5.0.dev20230614/src/py/flwr/proto/driver_pb2_grpc.pyi
+-rw-r--r--   0        0        0     4982 2023-06-14 23:02:38.324891 flwr_nightly-1.5.0.dev20230614/src/py/flwr/proto/fleet_pb2.py
+-rw-r--r--   0        0        0     4554 2023-06-14 23:02:38.324891 flwr_nightly-1.5.0.dev20230614/src/py/flwr/proto/fleet_pb2.pyi
+-rw-r--r--   0        0        0     4275 2023-06-14 23:02:38.324891 flwr_nightly-1.5.0.dev20230614/src/py/flwr/proto/fleet_pb2_grpc.py
+-rw-r--r--   0        0        0     1495 2023-06-14 23:02:38.324891 flwr_nightly-1.5.0.dev20230614/src/py/flwr/proto/fleet_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1188 2023-06-14 23:02:38.324891 flwr_nightly-1.5.0.dev20230614/src/py/flwr/proto/node_pb2.py
+-rw-r--r--   0        0        0      751 2023-06-14 23:02:38.324891 flwr_nightly-1.5.0.dev20230614/src/py/flwr/proto/node_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-14 23:02:38.324891 flwr_nightly-1.5.0.dev20230614/src/py/flwr/proto/node_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-14 23:02:38.324891 flwr_nightly-1.5.0.dev20230614/src/py/flwr/proto/node_pb2_grpc.pyi
+-rw-r--r--   0        0        0     8232 2023-06-14 23:02:38.324891 flwr_nightly-1.5.0.dev20230614/src/py/flwr/proto/task_pb2.py
+-rw-r--r--   0        0        0    10889 2023-06-14 23:02:38.324891 flwr_nightly-1.5.0.dev20230614/src/py/flwr/proto/task_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-14 23:02:38.324891 flwr_nightly-1.5.0.dev20230614/src/py/flwr/proto/task_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-14 23:02:38.324891 flwr_nightly-1.5.0.dev20230614/src/py/flwr/proto/task_pb2_grpc.pyi
+-rw-r--r--   0        0        0    18721 2023-06-14 23:02:38.324891 flwr_nightly-1.5.0.dev20230614/src/py/flwr/proto/transport_pb2.py
+-rw-r--r--   0        0        0    21497 2023-06-14 23:02:38.324891 flwr_nightly-1.5.0.dev20230614/src/py/flwr/proto/transport_pb2.pyi
+-rw-r--r--   0        0        0     2598 2023-06-14 23:02:38.324891 flwr_nightly-1.5.0.dev20230614/src/py/flwr/proto/transport_pb2_grpc.py
+-rw-r--r--   0        0        0      766 2023-06-14 23:02:38.324891 flwr_nightly-1.5.0.dev20230614/src/py/flwr/proto/transport_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-06-14 23:02:38.324891 flwr_nightly-1.5.0.dev20230614/src/py/flwr/py.typed
+-rw-r--r--   0        0        0     1370 2023-06-14 23:02:38.324891 flwr_nightly-1.5.0.dev20230614/src/py/flwr/server/__init__.py
+-rw-r--r--   0        0        0    26335 2023-06-14 23:02:38.324891 flwr_nightly-1.5.0.dev20230614/src/py/flwr/server/app.py
+-rw-r--r--   0        0        0     6120 2023-06-14 23:02:38.324891 flwr_nightly-1.5.0.dev20230614/src/py/flwr/server/client_manager.py
+-rw-r--r--   0        0        0     2227 2023-06-14 23:02:38.324891 flwr_nightly-1.5.0.dev20230614/src/py/flwr/server/client_proxy.py
+-rw-r--r--   0        0        0     1054 2023-06-14 23:02:38.324891 flwr_nightly-1.5.0.dev20230614/src/py/flwr/server/criterion.py
+-rw-r--r--   0        0        0      705 2023-06-14 23:02:38.324891 flwr_nightly-1.5.0.dev20230614/src/py/flwr/server/driver/__init__.py
+-rw-r--r--   0        0        0     3919 2023-06-14 23:02:38.324891 flwr_nightly-1.5.0.dev20230614/src/py/flwr/server/driver/driver_servicer.py
+-rw-r--r--   0        0        0      704 2023-06-14 23:02:38.328891 flwr_nightly-1.5.0.dev20230614/src/py/flwr/server/fleet/__init__.py
+-rw-r--r--   0        0        0      728 2023-06-14 23:02:38.328891 flwr_nightly-1.5.0.dev20230614/src/py/flwr/server/fleet/grpc_bidi/__init__.py
+-rw-r--r--   0        0        0     4467 2023-06-14 23:02:38.328891 flwr_nightly-1.5.0.dev20230614/src/py/flwr/server/fleet/grpc_bidi/driver_client_manager.py
+-rw-r--r--   0        0        0     5686 2023-06-14 23:02:38.328891 flwr_nightly-1.5.0.dev20230614/src/py/flwr/server/fleet/grpc_bidi/flower_service_servicer.py
+-rw-r--r--   0        0        0     6408 2023-06-14 23:02:38.328891 flwr_nightly-1.5.0.dev20230614/src/py/flwr/server/fleet/grpc_bidi/grpc_bridge.py
+-rw-r--r--   0        0        0     4650 2023-06-14 23:02:38.328891 flwr_nightly-1.5.0.dev20230614/src/py/flwr/server/fleet/grpc_bidi/grpc_client_proxy.py
+-rw-r--r--   0        0        0    11501 2023-06-14 23:02:38.328891 flwr_nightly-1.5.0.dev20230614/src/py/flwr/server/fleet/grpc_bidi/grpc_server.py
+-rw-r--r--   0        0        0     6313 2023-06-14 23:02:38.328891 flwr_nightly-1.5.0.dev20230614/src/py/flwr/server/fleet/grpc_bidi/ins_scheduler.py
+-rw-r--r--   0        0        0      751 2023-06-14 23:02:38.328891 flwr_nightly-1.5.0.dev20230614/src/py/flwr/server/fleet/grpc_rere/__init__.py
+-rw-r--r--   0        0        0     1858 2023-06-14 23:02:38.328891 flwr_nightly-1.5.0.dev20230614/src/py/flwr/server/fleet/grpc_rere/fleet_servicer.py
+-rw-r--r--   0        0        0      724 2023-06-14 23:02:38.328891 flwr_nightly-1.5.0.dev20230614/src/py/flwr/server/fleet/message_handler/__init__.py
+-rw-r--r--   0        0        0     2024 2023-06-14 23:02:38.328891 flwr_nightly-1.5.0.dev20230614/src/py/flwr/server/fleet/message_handler/message_handler.py
+-rw-r--r--   0        0        0      728 2023-06-14 23:02:38.328891 flwr_nightly-1.5.0.dev20230614/src/py/flwr/server/fleet/rest_rere/__init__.py
+-rw-r--r--   0        0        0     3718 2023-06-14 23:02:38.328891 flwr_nightly-1.5.0.dev20230614/src/py/flwr/server/fleet/rest_rere/rest_api.py
+-rw-r--r--   0        0        0     4897 2023-06-14 23:02:38.328891 flwr_nightly-1.5.0.dev20230614/src/py/flwr/server/history.py
+-rw-r--r--   0        0        0    15958 2023-06-14 23:02:38.328891 flwr_nightly-1.5.0.dev20230614/src/py/flwr/server/server.py
+-rw-r--r--   0        0        0      996 2023-06-14 23:02:38.328891 flwr_nightly-1.5.0.dev20230614/src/py/flwr/server/state/__init__.py
+-rw-r--r--   0        0        0     6516 2023-06-14 23:02:38.328891 flwr_nightly-1.5.0.dev20230614/src/py/flwr/server/state/in_memory_state.py
+-rw-r--r--   0        0        0    19296 2023-06-14 23:02:38.328891 flwr_nightly-1.5.0.dev20230614/src/py/flwr/server/state/sqlite_state.py
+-rw-r--r--   0        0        0     4833 2023-06-14 23:02:38.328891 flwr_nightly-1.5.0.dev20230614/src/py/flwr/server/state/state.py
+-rw-r--r--   0        0        0     1647 2023-06-14 23:02:38.328891 flwr_nightly-1.5.0.dev20230614/src/py/flwr/server/state/state_factory.py
+-rw-r--r--   0        0        0     1667 2023-06-14 23:02:38.328891 flwr_nightly-1.5.0.dev20230614/src/py/flwr/server/strategy/__init__.py
+-rw-r--r--   0        0        0     6099 2023-06-14 23:02:38.328891 flwr_nightly-1.5.0.dev20230614/src/py/flwr/server/strategy/aggregate.py
+-rw-r--r--   0        0        0     4507 2023-06-14 23:02:38.328891 flwr_nightly-1.5.0.dev20230614/src/py/flwr/server/strategy/dpfedavg_adaptive.py
+-rw-r--r--   0        0        0     4866 2023-06-14 23:02:38.328891 flwr_nightly-1.5.0.dev20230614/src/py/flwr/server/strategy/dpfedavg_fixed.py
+-rw-r--r--   0        0        0     5830 2023-06-14 23:02:38.328891 flwr_nightly-1.5.0.dev20230614/src/py/flwr/server/strategy/fault_tolerant_fedavg.py
+-rw-r--r--   0        0        0     6722 2023-06-14 23:02:38.328891 flwr_nightly-1.5.0.dev20230614/src/py/flwr/server/strategy/fedadagrad.py
+-rw-r--r--   0        0        0     7004 2023-06-14 23:02:38.328891 flwr_nightly-1.5.0.dev20230614/src/py/flwr/server/strategy/fedadam.py
+-rw-r--r--   0        0        0    11479 2023-06-14 23:02:38.328891 flwr_nightly-1.5.0.dev20230614/src/py/flwr/server/strategy/fedavg.py
+-rw-r--r--   0        0        0     9969 2023-06-14 23:02:38.328891 flwr_nightly-1.5.0.dev20230614/src/py/flwr/server/strategy/fedavg_android.py
+-rw-r--r--   0        0        0     8244 2023-06-14 23:02:38.328891 flwr_nightly-1.5.0.dev20230614/src/py/flwr/server/strategy/fedavgm.py
+-rw-r--r--   0        0        0     2666 2023-06-14 23:02:38.328891 flwr_nightly-1.5.0.dev20230614/src/py/flwr/server/strategy/fedmedian.py
+-rw-r--r--   0        0        0     5385 2023-06-14 23:02:38.328891 flwr_nightly-1.5.0.dev20230614/src/py/flwr/server/strategy/fedopt.py
+-rw-r--r--   0        0        0     7057 2023-06-14 23:02:38.328891 flwr_nightly-1.5.0.dev20230614/src/py/flwr/server/strategy/fedprox.py
+-rw-r--r--   0        0        0     5916 2023-06-14 23:02:38.328891 flwr_nightly-1.5.0.dev20230614/src/py/flwr/server/strategy/fedtrimmedavg.py
+-rw-r--r--   0        0        0     3368 2023-06-14 23:02:38.328891 flwr_nightly-1.5.0.dev20230614/src/py/flwr/server/strategy/fedxgb_nn_avg.py
+-rw-r--r--   0        0        0     7036 2023-06-14 23:02:38.328891 flwr_nightly-1.5.0.dev20230614/src/py/flwr/server/strategy/fedyogi.py
+-rw-r--r--   0        0        0     6302 2023-06-14 23:02:38.328891 flwr_nightly-1.5.0.dev20230614/src/py/flwr/server/strategy/krum.py
+-rw-r--r--   0        0        0    10131 2023-06-14 23:02:38.328891 flwr_nightly-1.5.0.dev20230614/src/py/flwr/server/strategy/qfedavg.py
+-rw-r--r--   0        0        0     7484 2023-06-14 23:02:38.328891 flwr_nightly-1.5.0.dev20230614/src/py/flwr/server/strategy/strategy.py
+-rw-r--r--   0        0        0      901 2023-06-14 23:02:38.328891 flwr_nightly-1.5.0.dev20230614/src/py/flwr/server/utils/__init__.py
+-rw-r--r--   0        0        0     5082 2023-06-14 23:02:38.328891 flwr_nightly-1.5.0.dev20230614/src/py/flwr/server/utils/tensorboard.py
+-rw-r--r--   0        0        0     4940 2023-06-14 23:02:38.328891 flwr_nightly-1.5.0.dev20230614/src/py/flwr/server/utils/validator.py
+-rw-r--r--   0        0        0     1271 2023-06-14 23:02:38.328891 flwr_nightly-1.5.0.dev20230614/src/py/flwr/simulation/__init__.py
+-rw-r--r--   0        0        0     7826 2023-06-14 23:02:38.328891 flwr_nightly-1.5.0.dev20230614/src/py/flwr/simulation/app.py
+-rw-r--r--   0        0        0      727 2023-06-14 23:02:38.328891 flwr_nightly-1.5.0.dev20230614/src/py/flwr/simulation/ray_transport/__init__.py
+-rw-r--r--   0        0        0     5535 2023-06-14 23:02:38.328891 flwr_nightly-1.5.0.dev20230614/src/py/flwr/simulation/ray_transport/ray_client_proxy.py
+-rw-r--r--   0        0        0    12494 1970-01-01 00:00:00.000000 flwr_nightly-1.5.0.dev20230614/setup.py
+-rw-r--r--   0        0        0    12838 1970-01-01 00:00:00.000000 flwr_nightly-1.5.0.dev20230614/PKG-INFO
```

### Comparing `flwr_nightly-1.5.0.dev20230608/LICENSE` & `flwr_nightly-1.5.0.dev20230614/LICENSE`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230608/README.md` & `flwr_nightly-1.5.0.dev20230614/README.md`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230608/pyproject.toml` & `flwr_nightly-1.5.0.dev20230614/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.4.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "flwr-nightly"
-version = "1.5.0-dev20230608"
+version = "1.5.0-dev20230614"
 description = "Flower: A Friendly Federated Learning Framework"
 license = "Apache-2.0"
 authors = ["The Flower Authors <hello@flower.dev>"]
 readme = "README.md"
 homepage = "https://flower.dev"
 repository = "https://github.com/adap/flower"
 documentation = "https://flower.dev"
@@ -148,7 +148,11 @@
 follow_imports_for_stubs = true
 disallow_untyped_calls = false
 
 [[tool.mypy.overrides]]
 module = "torch.*"
 follow_imports = "skip"
 follow_imports_for_stubs = true
+
+[tool.docformatter]
+wrap-summaries = 88
+wrap-descriptions = 88
```

### Comparing `flwr_nightly-1.5.0.dev20230608/src/py/flwr/__init__.py` & `flwr_nightly-1.5.0.dev20230614/src/py/flwr/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230608/src/py/flwr/client/__init__.py` & `flwr_nightly-1.5.0.dev20230614/src/py/flwr/client/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230608/src/py/flwr/client/app.py` & `flwr_nightly-1.5.0.dev20230614/src/py/flwr/client/app.py`

 * *Files 0% similar despite different names*

```diff
@@ -146,15 +146,14 @@
     >>> from pathlib import Path
     >>> start_client(
     >>>     server_address=localhost:8080,
     >>>     client=FlowerClient(),
     >>>     root_certificates=Path("/crts/root.pem").read_bytes(),
     >>> )
     """
-
     event(EventType.START_CLIENT_ENTER)
 
     # Parse IP address
     parsed_address = parse_address(server_address)
     if not parsed_address:
         sys.exit(f"Server address ({server_address}) cannot be parsed.")
     host, port, is_v6 = parsed_address
@@ -274,15 +273,14 @@
     >>> from pathlib import Path
     >>> start_client(
     >>>     server_address=localhost:8080,
     >>>     client=FlowerClient(),
     >>>     root_certificates=Path("/crts/root.pem").read_bytes(),
     >>> )
     """
-
     # Start
     start_client(
         server_address=server_address,
         client=_wrap_numpy_client(client=client),
         grpc_max_message_length=grpc_max_message_length,
         root_certificates=root_certificates,
         rest=rest,
@@ -317,15 +315,14 @@
     return GetParametersRes(
         status=Status(code=Code.OK, message="Success"), parameters=parameters_proto
     )
 
 
 def _fit(self: Client, ins: FitIns) -> FitRes:
     """Refine the provided parameters using the locally held dataset."""
-
     # Deconstruct FitIns
     parameters: NDArrays = parameters_to_ndarrays(ins.parameters)
 
     # Train
     results = self.numpy_client.fit(parameters, ins.config)  # type: ignore
     if not (
         len(results) == 3
```

### Comparing `flwr_nightly-1.5.0.dev20230608/src/py/flwr/client/client.py` & `flwr_nightly-1.5.0.dev20230614/src/py/flwr/client/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -157,15 +157,14 @@
     return type(client).evaluate != Client.evaluate
 
 
 def maybe_call_get_properties(
     client: Client, get_properties_ins: GetPropertiesIns
 ) -> GetPropertiesRes:
     """Call `get_properties` if the client overrides it."""
-
     # Check if client overrides `get_properties`
     if not has_get_properties(client=client):
         # If client does not override `get_properties`, don't call it
         status = Status(
             code=Code.GET_PROPERTIES_NOT_IMPLEMENTED,
             message="Client does not implement `get_properties`",
         )
@@ -178,15 +177,14 @@
     return client.get_properties(get_properties_ins)
 
 
 def maybe_call_get_parameters(
     client: Client, get_parameters_ins: GetParametersIns
 ) -> GetParametersRes:
     """Call `get_parameters` if the client overrides it."""
-
     # Check if client overrides `get_parameters`
     if not has_get_parameters(client=client):
         # If client does not override `get_parameters`, don't call it
         status = Status(
             code=Code.GET_PARAMETERS_NOT_IMPLEMENTED,
             message="Client does not implement `get_parameters`",
         )
@@ -197,15 +195,14 @@
 
     # If the client implements `get_parameters`, call it
     return client.get_parameters(get_parameters_ins)
 
 
 def maybe_call_fit(client: Client, fit_ins: FitIns) -> FitRes:
     """Call `fit` if the client overrides it."""
-
     # Check if client overrides `fit`
     if not has_fit(client=client):
         # If client does not override `fit`, don't call it
         status = Status(
             code=Code.FIT_NOT_IMPLEMENTED,
             message="Client does not implement `fit`",
         )
@@ -218,15 +215,14 @@
 
     # If the client implements `fit`, call it
     return client.fit(fit_ins)
 
 
 def maybe_call_evaluate(client: Client, evaluate_ins: EvaluateIns) -> EvaluateRes:
     """Call `evaluate` if the client overrides it."""
-
     # Check if client overrides `evaluate`
     if not has_evaluate(client=client):
         # If client does not override `evaluate`, don't call it
         status = Status(
             code=Code.EVALUATE_NOT_IMPLEMENTED,
             message="Client does not implement `evaluate`",
         )
```

### Comparing `flwr_nightly-1.5.0.dev20230608/src/py/flwr/client/dpfedavg_numpy_client.py` & `flwr_nightly-1.5.0.dev20230614/src/py/flwr/client/dpfedavg_numpy_client.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230608/src/py/flwr/client/grpc_client/__init__.py` & `flwr_nightly-1.5.0.dev20230614/src/py/flwr/client/grpc_client/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230608/src/py/flwr/client/grpc_client/connection.py` & `flwr_nightly-1.5.0.dev20230614/src/py/flwr/client/grpc_client/connection.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230608/src/py/flwr/client/grpc_rere_client/__init__.py` & `flwr_nightly-1.5.0.dev20230614/src/py/flwr/client/grpc_rere_client/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230608/src/py/flwr/client/grpc_rere_client/connection.py` & `flwr_nightly-1.5.0.dev20230614/src/py/flwr/client/grpc_rere_client/connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,15 +94,14 @@
 
     ###########################################################################
     # receive/send functions
     ###########################################################################
 
     def receive() -> Optional[ServerMessage]:
         """Receive next task from server."""
-
         # Request instructions (task) from server
         request = PullTaskInsRequest(
             node=Node(node_id=0, anonymous=True),
         )
         response = stub.PullTaskIns(request=request)
 
         # Remember the current TaskIns
@@ -117,15 +116,14 @@
         state[KEY_TASK_INS] = task_ins
 
         # Return the ServerMessage
         return server_message
 
     def send(client_message_proto: ClientMessage) -> None:
         """Send task result back to server."""
-
         if state[KEY_TASK_INS] is None:
             log(ERROR, "No current TaskIns")
             return
 
         task_ins: TaskIns = cast(TaskIns, state[KEY_TASK_INS])
 
         # Wrap ClientMessage in TaskRes
```

### Comparing `flwr_nightly-1.5.0.dev20230608/src/py/flwr/client/message_handler/__init__.py` & `flwr_nightly-1.5.0.dev20230614/src/py/flwr/client/message_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230608/src/py/flwr/client/message_handler/message_handler.py` & `flwr_nightly-1.5.0.dev20230614/src/py/flwr/client/message_handler/message_handler.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230608/src/py/flwr/client/message_handler/task_handler.py` & `flwr_nightly-1.5.0.dev20230614/src/py/flwr/client/message_handler/task_handler.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 from flwr.proto.transport_pb2 import ServerMessage
 
 
 def get_server_message(
     pull_task_ins_response: PullTaskInsResponse,
 ) -> Optional[Tuple[TaskIns, ServerMessage]]:
     """Get the first ServerMessage, if available."""
-
     # Extract a single ServerMessage from the response, if possible
     if len(pull_task_ins_response.task_ins_list) == 0:
         return None
 
     # Only evaluate the first message
     task_ins: TaskIns = pull_task_ins_response.task_ins_list[0]
```

### Comparing `flwr_nightly-1.5.0.dev20230608/src/py/flwr/client/numpy_client.py` & `flwr_nightly-1.5.0.dev20230614/src/py/flwr/client/numpy_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from flwr.common import Config, NDArrays, Scalar
 
 
 class NumPyClient(ABC):
     """Abstract base class for Flower clients using NumPy."""
 
     def get_properties(self, config: Config) -> Dict[str, Scalar]:
-        """Returns a client's set of properties.
+        """Return a client's set of properties.
 
         Parameters
         ----------
         config : Config
             Configuration parameters requested by the server.
             This can be used to tell the client which properties
             are needed along with some Scalar attributes.
```

### Comparing `flwr_nightly-1.5.0.dev20230608/src/py/flwr/client/rest_client/__init__.py` & `flwr_nightly-1.5.0.dev20230614/src/py/flwr/client/rest_client/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230608/src/py/flwr/client/rest_client/connection.py` & `flwr_nightly-1.5.0.dev20230614/src/py/flwr/client/rest_client/connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,14 @@
         connection using the certificates will be established to an SSL-enabled
         Flower server. Bytes won't work for the REST API.
 
     Returns
     -------
     receive, send : Callable, Callable
     """
-
     log(
         WARN,
         """
         EXPERIMENTAL: `rest` is an experimental feature, it might change
         considerably in future versions of Flower
         """,
     )
@@ -109,15 +108,14 @@
 
     ###########################################################################
     # receive/send functions
     ###########################################################################
 
     def receive() -> Optional[ServerMessage]:
         """Receive next task from server."""
-
         # Serialize ProtoBuf to bytes
         pull_task_ins_req_proto = PullTaskInsRequest(
             node=Node(node_id=0, anonymous=True),
         )
         pull_task_ins_req_bytes: bytes = pull_task_ins_req_proto.SerializeToString()
 
         # Request instructions (task) from server
@@ -166,15 +164,14 @@
 
         # Return the ServerMessage
         log(INFO, "[Node] POST /%s: success", PATH_PULL_TASK_INS)
         return server_message
 
     def send(client_message_proto: ClientMessage) -> None:
         """Send task result back to server."""
-
         if state[KEY_TASK_INS] is None:
             log(ERROR, "No current TaskIns")
             return
 
         task_ins: TaskIns = cast(TaskIns, state[KEY_TASK_INS])
 
         # Wrap ClientMessage in TaskRes
```

### Comparing `flwr_nightly-1.5.0.dev20230608/src/py/flwr/common/__init__.py` & `flwr_nightly-1.5.0.dev20230614/src/py/flwr/common/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230608/src/py/flwr/common/address.py` & `flwr_nightly-1.5.0.dev20230614/src/py/flwr/common/address.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from ipaddress import ip_address
 from typing import Optional, Tuple
 
 IPV6: int = 6
 
 
 def parse_address(address: str) -> Optional[Tuple[str, int, Optional[bool]]]:
-    """Parses an IP address into host, port, and version.
+    """Parse an IP address into host, port, and version.
 
     Parameters
     ----------
     address : str
         The string representation of a domain, an IPv4, or an IPV6 address
         with the port number.
```

### Comparing `flwr_nightly-1.5.0.dev20230608/src/py/flwr/common/constant.py` & `flwr_nightly-1.5.0.dev20230614/src/py/flwr/common/constant.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230608/src/py/flwr/common/date.py` & `flwr_nightly-1.5.0.dev20230614/src/py/flwr/common/date.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230608/src/py/flwr/common/dp.py` & `flwr_nightly-1.5.0.dev20230614/src/py/flwr/common/dp.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,16 +27,15 @@
     flattened_update = update[0]
     for i in range(1, len(update)):
         flattened_update = np.append(flattened_update, update[i])  # type: ignore
     return float(np.sqrt(np.sum(np.square(flattened_update))))
 
 
 def add_gaussian_noise(update: NDArrays, std_dev: float) -> NDArrays:
-    """Adds iid Gaussian noise of the given standard deviation to each floating
-    point value in the update."""
+    """Add iid Gaussian noise to each floating point value in the update."""
     update_noised = [
         layer + np.random.normal(0, std_dev, layer.shape) for layer in update
     ]
     return update_noised
 
 
 def clip_by_l2(update: NDArrays, threshold: float) -> Tuple[NDArrays, bool]:
```

### Comparing `flwr_nightly-1.5.0.dev20230608/src/py/flwr/common/grpc.py` & `flwr_nightly-1.5.0.dev20230614/src/py/flwr/common/grpc.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,14 @@
 
 def create_channel(
     server_address: str,
     root_certificates: Optional[bytes] = None,
     max_message_length: int = GRPC_MAX_MESSAGE_LENGTH,
 ) -> grpc.Channel:
     """Create a gRPC channel, either secure or insecure."""
-
     # Possible options:
     # https://github.com/grpc/grpc/blob/v1.43.x/include/grpc/impl/codegen/grpc_types.h
     channel_options = [
         ("grpc.max_send_message_length", max_message_length),
         ("grpc.max_receive_message_length", max_message_length),
     ]
```

### Comparing `flwr_nightly-1.5.0.dev20230608/src/py/flwr/common/logger.py` & `flwr_nightly-1.5.0.dev20230614/src/py/flwr/common/logger.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,14 @@
         }
 
 
 def configure(
     identifier: str, filename: Optional[str] = None, host: Optional[str] = None
 ) -> None:
     """Configure logging to file and/or remote log server."""
-
     # Create formatter
     string_to_input = f"{identifier} | %(levelname)s %(name)s %(asctime)s "
     string_to_input += "| %(filename)s:%(lineno)d | %(message)s"
     formatter = logging.Formatter(string_to_input)
 
     if filename:
         # Create file handler and log to disk
```

### Comparing `flwr_nightly-1.5.0.dev20230608/src/py/flwr/common/parameter.py` & `flwr_nightly-1.5.0.dev20230614/src/py/flwr/common/parameter.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230608/src/py/flwr/common/serde.py` & `flwr_nightly-1.5.0.dev20230614/src/py/flwr/common/serde.py`

 * *Files 0% similar despite different names*

```diff
@@ -454,15 +454,14 @@
 
 
 # === Scalar messages ===
 
 
 def scalar_to_proto(scalar: typing.Scalar) -> Scalar:
     """Serialize `Scalar` to ProtoBuf."""
-
     if isinstance(scalar, bool):
         return Scalar(bool=scalar)
 
     if isinstance(scalar, bytes):
         return Scalar(bytes=scalar)
 
     if isinstance(scalar, float):
```

### Comparing `flwr_nightly-1.5.0.dev20230608/src/py/flwr/common/telemetry.py` & `flwr_nightly-1.5.0.dev20230614/src/py/flwr/common/telemetry.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230608/src/py/flwr/common/typing.py` & `flwr_nightly-1.5.0.dev20230614/src/py/flwr/common/typing.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230608/src/py/flwr/common/version.py` & `flwr_nightly-1.5.0.dev20230614/src/py/flwr/common/version.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230608/src/py/flwr/driver/__init__.py` & `flwr_nightly-1.5.0.dev20230614/src/py/flwr/driver/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230608/src/py/flwr/driver/app.py` & `flwr_nightly-1.5.0.dev20230614/src/py/flwr/driver/app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230608/src/py/flwr/driver/driver.py` & `flwr_nightly-1.5.0.dev20230614/src/py/flwr/driver/driver.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,43 +71,40 @@
         self.channel = None
         self.stub = None
         channel.close()
         log(INFO, "[Driver] Disconnected")
 
     def get_nodes(self, req: driver_pb2.GetNodesRequest) -> driver_pb2.GetNodesResponse:
         """Get client IDs."""
-
         # Check if channel is open
         if self.stub is None:
             log(ERROR, ERROR_MESSAGE_DRIVER_NOT_CONNECTED)
             raise Exception("`Driver` instance not connected")
 
         # Call Driver API
         res: driver_pb2.GetNodesResponse = self.stub.GetNodes(request=req)
         return res
 
     def push_task_ins(
         self, req: driver_pb2.PushTaskInsRequest
     ) -> driver_pb2.PushTaskInsResponse:
         """Schedule tasks."""
-
         # Check if channel is open
         if self.stub is None:
             log(ERROR, ERROR_MESSAGE_DRIVER_NOT_CONNECTED)
             raise Exception("`Driver` instance not connected")
 
         # Call Driver API
         res: driver_pb2.PushTaskInsResponse = self.stub.PushTaskIns(request=req)
         return res
 
     def pull_task_res(
         self, req: driver_pb2.PullTaskResRequest
     ) -> driver_pb2.PullTaskResResponse:
         """Get task results."""
-
         # Check if channel is open
         if self.stub is None:
             log(ERROR, ERROR_MESSAGE_DRIVER_NOT_CONNECTED)
             raise Exception("`Driver` instance not connected")
 
         # Call Driver API
         res: driver_pb2.PullTaskResResponse = self.stub.PullTaskRes(request=req)
```

### Comparing `flwr_nightly-1.5.0.dev20230608/src/py/flwr/driver/driver_client_manager.py` & `flwr_nightly-1.5.0.dev20230614/src/py/flwr/driver/driver_client_manager.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230608/src/py/flwr/driver/driver_client_proxy.py` & `flwr_nightly-1.5.0.dev20230614/src/py/flwr/driver/driver_client_proxy.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         self.node_id = node_id
         self.driver = driver
         self.anonymous = anonymous
 
     def get_properties(
         self, ins: common.GetPropertiesIns, timeout: Optional[float]
     ) -> common.GetPropertiesRes:
-        """Returns client's properties."""
+        """Return client's properties."""
         server_message_proto: transport_pb2.ServerMessage = (
             serde.server_message_to_proto(
                 server_message=common.ServerMessage(get_properties_ins=ins)
             )
         )
         return cast(
             common.GetPropertiesRes,
```

### Comparing `flwr_nightly-1.5.0.dev20230608/src/py/flwr/proto/__init__.py` & `flwr_nightly-1.5.0.dev20230614/src/py/flwr/proto/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230608/src/py/flwr/proto/driver_pb2.py` & `flwr_nightly-1.5.0.dev20230614/src/py/flwr/proto/driver_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230608/src/py/flwr/proto/driver_pb2.pyi` & `flwr_nightly-1.5.0.dev20230614/src/py/flwr/proto/driver_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230608/src/py/flwr/proto/driver_pb2_grpc.py` & `flwr_nightly-1.5.0.dev20230614/src/py/flwr/proto/driver_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230608/src/py/flwr/proto/driver_pb2_grpc.pyi` & `flwr_nightly-1.5.0.dev20230614/src/py/flwr/proto/driver_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230608/src/py/flwr/proto/fleet_pb2.py` & `flwr_nightly-1.5.0.dev20230614/src/py/flwr/proto/fleet_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230608/src/py/flwr/proto/fleet_pb2.pyi` & `flwr_nightly-1.5.0.dev20230614/src/py/flwr/proto/fleet_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230608/src/py/flwr/proto/fleet_pb2_grpc.py` & `flwr_nightly-1.5.0.dev20230614/src/py/flwr/proto/fleet_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230608/src/py/flwr/proto/fleet_pb2_grpc.pyi` & `flwr_nightly-1.5.0.dev20230614/src/py/flwr/proto/fleet_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230608/src/py/flwr/proto/node_pb2.py` & `flwr_nightly-1.5.0.dev20230614/src/py/flwr/proto/node_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230608/src/py/flwr/proto/node_pb2.pyi` & `flwr_nightly-1.5.0.dev20230614/src/py/flwr/proto/node_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230608/src/py/flwr/proto/transport_pb2.py` & `flwr_nightly-1.5.0.dev20230614/src/py/flwr/proto/transport_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230608/src/py/flwr/proto/transport_pb2.pyi` & `flwr_nightly-1.5.0.dev20230614/src/py/flwr/proto/transport_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230608/src/py/flwr/proto/transport_pb2_grpc.py` & `flwr_nightly-1.5.0.dev20230614/src/py/flwr/proto/transport_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230608/src/py/flwr/proto/transport_pb2_grpc.pyi` & `flwr_nightly-1.5.0.dev20230614/src/py/flwr/proto/transport_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/__init__.py` & `flwr_nightly-1.5.0.dev20230614/src/py/flwr/server/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/app.py` & `flwr_nightly-1.5.0.dev20230614/src/py/flwr/server/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,16 +62,16 @@
 DATABASE = ":flwr-in-memory-state:"
 
 
 @dataclass
 class ServerConfig:
     """Flower server config.
 
-    All attributes have default values which allows users to configure
-    just the ones they care about.
+    All attributes have default values which allows users to configure just the ones
+    they care about.
     """
 
     num_rounds: int = 1
     round_timeout: Optional[float] = None
 
 
 def start_server(  # pylint: disable=too-many-arguments,too-many-locals
@@ -232,15 +232,14 @@
     server.disconnect_all_clients(timeout=config.round_timeout)
 
     return hist
 
 
 def run_driver_api() -> None:
     """Run Flower server (Driver API)."""
-
     log(INFO, "Starting Flower server (Driver API)")
     event(EventType.RUN_DRIVER_API_ENTER)
     args = _parse_args_driver().parse_args()
 
     # Parse IP address
     parsed_address = parse_address(args.driver_api_address)
     if not parsed_address:
@@ -266,15 +265,14 @@
 
     # Block
     grpc_server.wait_for_termination()
 
 
 def run_fleet_api() -> None:
     """Run Flower server (Fleet API)."""
-
     log(INFO, "Starting Flower server (Fleet API)")
     event(EventType.RUN_FLEET_API_ENTER)
     args = _parse_args_fleet().parse_args()
 
     # Initialize StateFactory
     state_factory = StateFactory(args.database)
 
@@ -348,15 +346,14 @@
     elif len(bckg_threads) > 0:
         bckg_threads[0].join()
 
 
 # pylint: disable=too-many-branches
 def run_server() -> None:
     """Run Flower server (Driver API and Fleet API)."""
-
     log(INFO, "Starting Flower server")
     event(EventType.RUN_SERVER_ENTER)
     args = _parse_args_server().parse_args()
 
     # Parse IP address
     parsed_address = parse_address(args.driver_api_address)
     if not parsed_address:
@@ -458,18 +455,17 @@
 
     def graceful_exit_handler(  # type: ignore
         signalnum,
         frame: FrameType,  # pylint: disable=unused-argument
     ) -> None:
         """Exit handler to be registered with signal.signal.
 
-        When called will reset signal handler to original signal handler
-        from default_handlers.
+        When called will reset signal handler to original signal handler from
+        default_handlers.
         """
-
         # Reset to default handler
         signal(signalnum, default_handlers[signalnum])
 
         event_res = event(event_type=event_type)
 
         for grpc_server in grpc_servers:
             grpc_server.stop(grace=1)
@@ -494,15 +490,14 @@
 
 
 def _run_driver_api_grpc(
     address: str,
     state_factory: StateFactory,
 ) -> grpc.Server:
     """Run Driver API (gRPC, request-response)."""
-
     # Create Driver API gRPC server
     driver_servicer: grpc.Server = DriverServicer(
         state_factory=state_factory,
     )
     driver_add_servicer_to_server_fn = add_DriverServicer_to_server
     driver_grpc_server = generic_create_grpc_server(
         servicer_and_add_fn=(driver_servicer, driver_add_servicer_to_server_fn),
@@ -518,15 +513,14 @@
 
 
 def _run_fleet_api_grpc_bidi(
     address: str,
     state_factory: StateFactory,
 ) -> grpc.Server:
     """Run Fleet API (gRPC, bidirectional streaming)."""
-
     # DriverClientManager
     driver_client_manager = DriverClientManager(
         state_factory=state_factory,
     )
 
     # Create (legacy) Fleet API gRPC server
     fleet_servicer = FlowerServiceServicer(
@@ -547,15 +541,14 @@
 
 
 def _run_fleet_api_grpc_rere(
     address: str,
     state_factory: StateFactory,
 ) -> grpc.Server:
     """Run Fleet API (gRPC, request-response)."""
-
     # Create Fleet API gRPC server
     fleet_servicer = FleetServicer(
         state=state_factory.state(),
     )
     fleet_add_servicer_to_server_fn = add_FleetServicer_to_server
     fleet_grpc_server = generic_create_grpc_server(
         servicer_and_add_fn=(fleet_servicer, fleet_add_servicer_to_server_fn),
```

### Comparing `flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/client_manager.py` & `flwr_nightly-1.5.0.dev20230614/src/py/flwr/server/client_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,14 +88,21 @@
     """Provides a pool of available clients."""
 
     def __init__(self) -> None:
         self.clients: Dict[str, ClientProxy] = {}
         self._cv = threading.Condition()
 
     def __len__(self) -> int:
+        """Return the number of available clients.
+
+        Returns
+        -------
+        num_available : int
+            The number of currently available clients.
+        """
         return len(self.clients)
 
     def num_available(self) -> int:
         """Return the number of available clients.
 
         Returns
         -------
```

### Comparing `flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/client_proxy.py` & `flwr_nightly-1.5.0.dev20230614/src/py/flwr/server/client_proxy.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 
     @abstractmethod
     def get_properties(
         self,
         ins: GetPropertiesIns,
         timeout: Optional[float],
     ) -> GetPropertiesRes:
-        """Returns the client's properties."""
+        """Return the client's properties."""
 
     @abstractmethod
     def get_parameters(
         self,
         ins: GetParametersIns,
         timeout: Optional[float],
     ) -> GetParametersRes:
```

### Comparing `flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/criterion.py` & `flwr_nightly-1.5.0.dev20230614/src/py/flwr/server/criterion.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,13 +17,12 @@
 
 from abc import ABC, abstractmethod
 
 from .client_proxy import ClientProxy
 
 
 class Criterion(ABC):
-    """Abstract class which allows subclasses to implement criterion
-    sampling."""
+    """Abstract class which allows subclasses to implement criterion sampling."""
 
     @abstractmethod
     def select(self, client: ClientProxy) -> bool:
         """Decide whether a client should be eligible for sampling or not."""
```

### Comparing `flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/driver/__init__.py` & `flwr_nightly-1.5.0.dev20230614/src/py/flwr/server/driver/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/driver/driver_servicer.py` & `flwr_nightly-1.5.0.dev20230614/src/py/flwr/server/driver/driver_servicer.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/fleet/__init__.py` & `flwr_nightly-1.5.0.dev20230614/src/py/flwr/server/fleet/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/fleet/grpc_bidi/__init__.py` & `flwr_nightly-1.5.0.dev20230614/src/py/flwr/server/fleet/grpc_bidi/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/fleet/grpc_bidi/driver_client_manager.py` & `flwr_nightly-1.5.0.dev20230614/src/py/flwr/server/fleet/grpc_bidi/driver_client_manager.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/fleet/grpc_bidi/flower_service_servicer.py` & `flwr_nightly-1.5.0.dev20230614/src/py/flwr/server/fleet/grpc_bidi/flower_service_servicer.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,15 +74,17 @@
         self.client_proxy_factory = grpc_client_proxy_factory
 
     def Join(  # pylint: disable=invalid-name
         self,
         request_iterator: Iterator[ClientMessage],
         context: grpc.ServicerContext,
     ) -> Iterator[ServerMessage]:
-        """Invoked by each gRPC client which participates in the network.
+        """Facilitate bi-directional streaming of messages between server and client.
+
+        Invoked by each gRPC client which participates in the network.
 
         Protocol:
         - The first message is sent from the server to the client
         - Both `ServerMessage` and `ClientMessage` are message "wrappers"
           wrapping the actual message
         - The `Join` method is (pretty much) unaware of the protocol
         """
```

### Comparing `flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/fleet/grpc_bidi/grpc_bridge.py` & `flwr_nightly-1.5.0.dev20230614/src/py/flwr/server/fleet/grpc_bidi/grpc_bridge.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,16 +76,15 @@
     def _raise_if_closed(self) -> None:
         if self._status == Status.CLOSED:
             raise GrpcBridgeClosed()
 
     def _transition(self, next_status: Status) -> None:
         """Validate status transition and set next status.
 
-        The caller of the transition method will have to aquire
-        conditional variable.
+        The caller of the transition method will have to aquire conditional variable.
         """
         if next_status == Status.CLOSED:
             self._status = next_status
         elif (
             self._status == Status.AWAITING_INS_WRAPPER
             and next_status == Status.INS_WRAPPER_AVAILABLE
             and self._ins_wrapper is not None
```

### Comparing `flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/fleet/grpc_bidi/grpc_client_proxy.py` & `flwr_nightly-1.5.0.dev20230614/src/py/flwr/server/fleet/grpc_bidi/grpc_client_proxy.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         self.bridge = bridge
 
     def get_properties(
         self,
         ins: common.GetPropertiesIns,
         timeout: Optional[float],
     ) -> common.GetPropertiesRes:
-        """Requests client's set of internal properties."""
+        """Request client's set of internal properties."""
         get_properties_msg = serde.get_properties_ins_to_proto(ins)
         res_wrapper: ResWrapper = self.bridge.request(
             ins_wrapper=InsWrapper(
                 server_message=ServerMessage(get_properties_ins=get_properties_msg),
                 timeout=timeout,
             )
         )
```

### Comparing `flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/fleet/grpc_bidi/grpc_server.py` & `flwr_nightly-1.5.0.dev20230614/src/py/flwr/server/fleet/grpc_bidi/grpc_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,15 +126,14 @@
     >>>     certificates=(
     >>>         Path("/crts/root.pem").read_bytes(),
     >>>         Path("/crts/localhost.crt").read_bytes(),
     >>>         Path("/crts/localhost.key").read_bytes(),
     >>>     ),
     >>> )
     """
-
     servicer = FlowerServiceServicer(client_manager)
     add_servicer_to_server_fn = add_FlowerServiceServicer_to_server
 
     server = generic_create_grpc_server(
         servicer_and_add_fn=(servicer, add_servicer_to_server_fn),
         server_address=server_address,
         max_concurrent_workers=max_concurrent_workers,
@@ -156,15 +155,15 @@
     ],
     server_address: str,
     max_concurrent_workers: int = 1000,
     max_message_length: int = GRPC_MAX_MESSAGE_LENGTH,
     keepalive_time_ms: int = 210000,
     certificates: Optional[Tuple[bytes, bytes, bytes]] = None,
 ) -> grpc.Server:
-    """Generic function to create a gRPC server with a single servicer.
+    """Create a gRPC server with a single servicer.
 
     Parameters
     ----------
     servicer_and_add_fn : Tuple
         A tuple holding a servicer implementation and a matching
         add_Servicer_to_server function.
     server_address : str
@@ -206,15 +205,14 @@
             * server private key.
 
     Returns
     -------
     server : grpc.Server
         A non-running instance of a gRPC server.
     """
-
     # Deconstruct tuple into servicer and function
     servicer, add_servicer_to_server_fn = servicer_and_add_fn
 
     # Possible options:
     # https://github.com/grpc/grpc/blob/v1.43.x/include/grpc/impl/codegen/grpc_types.h
     options = [
         # Maximum number of concurrent incoming streams to allow on a http2
```

### Comparing `flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/fleet/grpc_bidi/ins_scheduler.py` & `flwr_nightly-1.5.0.dev20230614/src/py/flwr/server/fleet/grpc_bidi/ins_scheduler.py`

 * *Files 0% similar despite different names*

```diff
@@ -119,15 +119,14 @@
     log(DEBUG, "Worker for node %i stopped", client_proxy.node_id)
 
 
 def _call_client_proxy(
     client_proxy: ClientProxy, server_message: ServerMessage, timeout: Optional[float]
 ) -> ClientMessage:
     """."""
-
     # pylint: disable=too-many-locals
 
     field = server_message.WhichOneof("msg")
 
     if field == "get_properties_ins":
         get_properties_ins = serde.get_properties_ins_from_proto(
             msg=server_message.get_properties_ins
```

### Comparing `flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/fleet/grpc_rere/__init__.py` & `flwr_nightly-1.5.0.dev20230614/src/py/flwr/server/fleet/grpc_rere/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/fleet/grpc_rere/fleet_servicer.py` & `flwr_nightly-1.5.0.dev20230614/src/py/flwr/server/fleet/grpc_rere/fleet_servicer.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/fleet/message_handler/__init__.py` & `flwr_nightly-1.5.0.dev20230614/src/py/flwr/server/fleet/message_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/fleet/message_handler/message_handler.py` & `flwr_nightly-1.5.0.dev20230614/src/py/flwr/server/fleet/message_handler/message_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,14 @@
 )
 from flwr.proto.task_pb2 import TaskIns, TaskRes
 from flwr.server.state import State
 
 
 def pull_task_ins(request: PullTaskInsRequest, state: State) -> PullTaskInsResponse:
     """Pull TaskIns handler."""
-
     # Get node_id if client node is not anonymous
     node = request.node  # pylint: disable=no-member
     node_id: Optional[int] = None if node.anonymous else node.node_id
 
     # Retrieve TaskIns from State
     task_ins_list: List[TaskIns] = state.get_task_ins(node_id=node_id, limit=1)
 
@@ -44,15 +43,14 @@
         task_ins_list=task_ins_list,
     )
     return response
 
 
 def push_task_res(request: PushTaskResRequest, state: State) -> PushTaskResResponse:
     """Push TaskRes handler."""
-
     # pylint: disable=no-member
     task_res: TaskRes = request.task_res_list[0]
     # pylint: enable=no-member
 
     # Store TaskRes in State
     task_id: Optional[UUID] = state.store_task_res(task_res=task_res)
```

### Comparing `flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/fleet/rest_rere/__init__.py` & `flwr_nightly-1.5.0.dev20230614/src/py/flwr/server/fleet/rest_rere/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/fleet/rest_rere/rest_api.py` & `flwr_nightly-1.5.0.dev20230614/src/py/flwr/server/fleet/rest_rere/rest_api.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/history.py` & `flwr_nightly-1.5.0.dev20230614/src/py/flwr/server/history.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,14 +69,29 @@
             # if not (isinstance(metrics[key], float) or isinstance(metrics[key], int)):
             #     continue  # ignore non-numeric key/value pairs
             if key not in self.metrics_centralized:
                 self.metrics_centralized[key] = []
             self.metrics_centralized[key].append((server_round, metrics[key]))
 
     def __repr__(self) -> str:
+        """Create a representation of History.
+
+        The representation consists of the following data (for each round) if present:
+
+        * distributed loss.
+        * centralized loss.
+        * distributed training metrics.
+        * distributed evaluation metrics.
+        * centralized metrics.
+
+        Returns
+        -------
+        representation : str
+            The string representation of the history object.
+        """
         rep = ""
         if self.losses_distributed:
             rep += "History (loss, distributed):\n" + reduce(
                 lambda a, b: a + b,
                 [
                     f"\tround {server_round}: {loss}\n"
                     for server_round, loss in self.losses_distributed
```

### Comparing `flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/server.py` & `flwr_nightly-1.5.0.dev20230614/src/py/flwr/server/server.py`

 * *Files 0% similar despite different names*

```diff
@@ -157,15 +157,14 @@
         self,
         server_round: int,
         timeout: Optional[float],
     ) -> Optional[
         Tuple[Optional[float], Dict[str, Scalar], EvaluateResultsAndFailures]
     ]:
         """Validate current global model on a number of clients."""
-
         # Get clients and their respective instructions from strategy
         client_instructions = self.strategy.configure_evaluate(
             server_round=server_round,
             parameters=self.parameters,
             client_manager=self._client_manager,
         )
         if not client_instructions:
@@ -206,15 +205,14 @@
         self,
         server_round: int,
         timeout: Optional[float],
     ) -> Optional[
         Tuple[Optional[Parameters], Dict[str, Scalar], FitResultsAndFailures]
     ]:
         """Perform a single round of federated averaging."""
-
         # Get clients and their respective instructions from strategy
         client_instructions = self.strategy.configure_fit(
             server_round=server_round,
             parameters=self.parameters,
             client_manager=self._client_manager,
         )
 
@@ -262,15 +260,14 @@
             client_instructions=client_instructions,
             max_workers=self.max_workers,
             timeout=timeout,
         )
 
     def _get_initial_parameters(self, timeout: Optional[float]) -> Parameters:
         """Get initial parameters from one of the available clients."""
-
         # Server-side parameter initialization
         parameters: Optional[Parameters] = self.strategy.initialize_parameters(
             client_manager=self._client_manager
         )
         if parameters is not None:
             log(INFO, "Using initial parameters provided by strategy")
             return parameters
@@ -362,15 +359,14 @@
 
 def _handle_finished_future_after_fit(
     future: concurrent.futures.Future,  # type: ignore
     results: List[Tuple[ClientProxy, FitRes]],
     failures: List[Union[Tuple[ClientProxy, FitRes], BaseException]],
 ) -> None:
     """Convert finished future into either a result or a failure."""
-
     # Check if there was an exception
     failure = future.exception()
     if failure is not None:
         failures.append(failure)
         return
 
     # Successfully received a result from a client
@@ -424,15 +420,14 @@
 
 def _handle_finished_future_after_evaluate(
     future: concurrent.futures.Future,  # type: ignore
     results: List[Tuple[ClientProxy, EvaluateRes]],
     failures: List[Union[Tuple[ClientProxy, EvaluateRes], BaseException]],
 ) -> None:
     """Convert finished future into either a result or a failure."""
-
     # Check if there was an exception
     failure = future.exception()
     if failure is not None:
         failures.append(failure)
         return
 
     # Successfully received a result from a client
```

### Comparing `flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/state/__init__.py` & `flwr_nightly-1.5.0.dev20230614/src/py/flwr/server/state/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/state/in_memory_state.py` & `flwr_nightly-1.5.0.dev20230614/src/py/flwr/server/state/in_memory_state.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,14 @@
     def __init__(self) -> None:
         self.node_ids: Set[int] = set()
         self.task_ins_store: Dict[UUID, TaskIns] = {}
         self.task_res_store: Dict[UUID, TaskRes] = {}
 
     def store_task_ins(self, task_ins: TaskIns) -> Optional[UUID]:
         """Store one TaskIns."""
-
         # Validate task
         errors = validate_task_ins_or_res(task_ins)
         if any(errors):
             log(ERROR, errors)
             return None
 
         # Create task_id, created_at and ttl
@@ -57,15 +56,14 @@
         # Return the new task_id
         return task_id
 
     def get_task_ins(
         self, node_id: Optional[int], limit: Optional[int]
     ) -> List[TaskIns]:
         """Get all TaskIns that have not been delivered yet."""
-
         if limit is not None and limit < 1:
             raise AssertionError("`limit` must be >= 1")
 
         # Find TaskIns for node_id that were not delivered yet
         task_ins_list: List[TaskIns] = []
         for _, task_ins in self.task_ins_store.items():
             # pylint: disable=too-many-boolean-expressions
@@ -90,15 +88,14 @@
             task_ins.task.delivered_at = delivered_at
 
         # Return TaskIns
         return task_ins_list
 
     def store_task_res(self, task_res: TaskRes) -> Optional[UUID]:
         """Store one TaskRes."""
-
         # Validate task
         errors = validate_task_ins_or_res(task_res)
         if any(errors):
             log(ERROR, errors)
             return None
 
         # Create task_id, created_at and ttl
@@ -113,15 +110,14 @@
         self.task_res_store[task_id] = task_res
 
         # Return the new task_id
         return task_id
 
     def get_task_res(self, task_ids: Set[UUID], limit: Optional[int]) -> List[TaskRes]:
         """Get all TaskRes that have not been delivered yet."""
-
         if limit is not None and limit < 1:
             raise AssertionError("`limit` must be >= 1")
 
         # Find TaskRes that were not delivered yet
         task_res_list: List[TaskRes] = []
         for _, task_res in self.task_res_store.items():
             if (
@@ -138,15 +134,14 @@
             task_res.task.delivered_at = delivered_at
 
         # Return TaskRes
         return task_res_list
 
     def delete_tasks(self, task_ids: Set[UUID]) -> None:
         """Delete all delivered TaskIns/TaskRes pairs."""
-
         task_ins_to_be_deleted: Set[UUID] = set()
         task_res_to_be_deleted: Set[UUID] = set()
 
         for task_ins_id in task_ids:
             # Find the task_id of the matching task_res
             for task_res_id, task_res in self.task_res_store.items():
                 if UUID(task_res.task.ancestry[0]) != task_ins_id:
```

### Comparing `flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/state/sqlite_state.py` & `flwr_nightly-1.5.0.dev20230614/src/py/flwr/server/state/sqlite_state.py`

 * *Files 1% similar despite different names*

```diff
@@ -386,26 +386,26 @@
             # Run query
             rows = self.query(query, data)
 
         result = [dict_to_task_res(row) for row in rows]
         return result
 
     def num_task_ins(self) -> int:
-        """Number of task_ins in store.
+        """Calculate the number of task_ins in store.
 
         This includes delivered but not yet deleted task_ins.
         """
         query = "SELECT count(*) AS num FROM task_ins;"
         rows = self.query(query)
         result = rows[0]
         num = cast(int, result["num"])
         return num
 
     def num_task_res(self) -> int:
-        """Number of task_res in store.
+        """Calculate the number of task_res in store.
 
         This includes delivered but not yet deleted task_res.
         """
         query = "SELECT count(*) AS num FROM task_res;"
         rows = self.query(query)
         result: Dict[str, int] = rows[0]
         return result["num"]
@@ -465,18 +465,17 @@
         return result
 
 
 def dict_factory(
     cursor: sqlite3.Cursor,
     row: sqlite3.Row,
 ) -> Dict[str, Any]:
-    """Used to turn SQLite results into dicts.
+    """Turn SQLite results into dicts.
 
-    Less efficent for retrival of large amounts of data but easier to
-    use.
+    Less efficent for retrival of large amounts of data but easier to use.
     """
     fields = [column[0] for column in cursor.description]
     return dict(zip(fields, row))
 
 
 def task_ins_to_dict(task_msg: TaskIns) -> Dict[str, Any]:
     """Transform TaskIns to dict."""
```

### Comparing `flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/state/state.py` & `flwr_nightly-1.5.0.dev20230614/src/py/flwr/server/state/state.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,22 +105,22 @@
         If `limit` is not `None`, return, at most, `limit` number of TaskRes. The limit
         will only take effect if enough task_ids are in the set AND are currently
         available. If `limit` is set, it has to be greater zero.
         """
 
     @abc.abstractmethod
     def num_task_ins(self) -> int:
-        """Number of task_ins in store.
+        """Calculate the number of task_ins in store.
 
         This includes delivered but not yet deleted task_ins.
         """
 
     @abc.abstractmethod
     def num_task_res(self) -> int:
-        """Number of task_res in store.
+        """Calculate the number of task_res in store.
 
         This includes delivered but not yet deleted task_res.
         """
 
     @abc.abstractmethod
     def delete_tasks(self, task_ids: Set[UUID]) -> None:
         """Delete all delivered TaskIns/TaskRes pairs."""
```

### Comparing `flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/state/state_factory.py` & `flwr_nightly-1.5.0.dev20230614/src/py/flwr/server/state/state_factory.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,14 @@
 
     def __init__(self, database: str) -> None:
         self.database = database
         self.state_instance: Optional[State] = None
 
     def state(self) -> State:
         """Return a State instance and create it, if necessary."""
-
         # InMemoryState
         if self.database == ":flwr-in-memory-state:":
             if self.state_instance is None:
                 self.state_instance = InMemoryState()
             log(DEBUG, "Using InMemoryState")
             return self.state_instance
```

### Comparing `flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/strategy/__init__.py` & `flwr_nightly-1.5.0.dev20230614/src/py/flwr/server/strategy/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/strategy/aggregate.py` & `flwr_nightly-1.5.0.dev20230614/src/py/flwr/server/strategy/aggregate.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/strategy/dpfedavg_adaptive.py` & `flwr_nightly-1.5.0.dev20230614/src/py/flwr/server/strategy/dpfedavg_adaptive.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,14 @@
         rep = "Strategy with DP with Adaptive Clipping enabled."
         return rep
 
     def configure_fit(
         self, server_round: int, parameters: Parameters, client_manager: ClientManager
     ) -> List[Tuple[ClientProxy, FitIns]]:
         """Configure the next round of training."""
-
         additional_config = {"dpfedavg_adaptive_clip_enabled": True}
 
         client_instructions = super().configure_fit(
             server_round, parameters, client_manager
         )
 
         for _, fit_ins in client_instructions:
```

### Comparing `flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/strategy/dpfedavg_fixed.py` & `flwr_nightly-1.5.0.dev20230614/src/py/flwr/server/strategy/dpfedavg_fixed.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,14 @@
     ) -> Optional[Parameters]:
         return self.strategy.initialize_parameters(client_manager)
 
     def configure_fit(
         self, server_round: int, parameters: Parameters, client_manager: ClientManager
     ) -> List[Tuple[ClientProxy, FitIns]]:
         """Configure the next round of training."""
-
         additional_config = {"dpfedavg_clip_norm": self.clip_norm}
         if not self.server_side_noising:
             additional_config[
                 "dpfedavg_noise_stddev"
             ] = self._calc_client_noise_stddev()
 
         client_instructions = self.strategy.configure_fit(
```

### Comparing `flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/strategy/fault_tolerant_fedavg.py` & `flwr_nightly-1.5.0.dev20230614/src/py/flwr/server/strategy/fault_tolerant_fedavg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/strategy/fedadagrad.py` & `flwr_nightly-1.5.0.dev20230614/src/py/flwr/server/strategy/fedadagrad.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-"""Adaptive Federated Optimization using Adagrad (FedAdagrad) [Reddi et al.,
-2020] strategy.
+"""Adaptive Federated Optimization using Adagrad (FedAdagrad) [Reddi et al., 2020]
+strategy.
 
 Paper: arxiv.org/abs/2003.00295
 """
 
 
 from typing import Callable, Dict, List, Optional, Tuple, Union
 
@@ -35,16 +35,16 @@
 from flwr.server.client_proxy import ClientProxy
 
 from .fedopt import FedOpt
 
 
 # flake8: noqa: E501
 class FedAdagrad(FedOpt):
-    """Adaptive Federated Optimization using Adagrad (FedAdagrad) [Reddi et
-    al., 2020] strategy.
+    """Adaptive Federated Optimization using Adagrad (FedAdagrad) [Reddi et al., 2020]
+    strategy.
 
     Paper: https://arxiv.org/abs/2003.00295
     """
 
     # pylint: disable=too-many-arguments,too-many-locals,too-many-instance-attributes,line-too-long
     def __init__(
         self,
```

### Comparing `flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/strategy/fedadam.py` & `flwr_nightly-1.5.0.dev20230614/src/py/flwr/server/strategy/fedadam.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,16 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-"""Adaptive Federated Optimization using Adam (FedAdam) [Reddi et al., 2020]
-strategy.
+"""Adaptive Federated Optimization using Adam (FedAdam) [Reddi et al., 2020] strategy.
 
 Paper: arxiv.org/abs/2003.00295
 """
 
 
 from typing import Callable, Dict, List, Optional, Tuple, Union
 
@@ -35,16 +34,16 @@
 from flwr.server.client_proxy import ClientProxy
 
 from .fedopt import FedOpt
 
 
 # flake8: noqa: E501
 class FedAdam(FedOpt):
-    """Adaptive Federated Optimization using Adam (FedAdam) [Reddi et al.,
-    2020] strategy.
+    """Adaptive Federated Optimization using Adam (FedAdam) [Reddi et al., 2020]
+    strategy.
 
     Paper: https://arxiv.org/abs/2003.00295
     """
 
     # pylint: disable=too-many-arguments,too-many-instance-attributes,too-many-locals,line-too-long
     def __init__(
         self,
```

### Comparing `flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/strategy/fedavg.py` & `flwr_nightly-1.5.0.dev20230614/src/py/flwr/server/strategy/fedavg.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,16 +131,15 @@
         self.evaluate_metrics_aggregation_fn = evaluate_metrics_aggregation_fn
 
     def __repr__(self) -> str:
         rep = f"FedAvg(accept_failures={self.accept_failures})"
         return rep
 
     def num_fit_clients(self, num_available_clients: int) -> Tuple[int, int]:
-        """Return the sample size and the required number of available
-        clients."""
+        """Return the sample size and the required number of available clients."""
         num_clients = int(num_available_clients * self.fraction_fit)
         return max(num_clients, self.min_fit_clients), self.min_available_clients
 
     def num_evaluation_clients(self, num_available_clients: int) -> Tuple[int, int]:
         """Use a fraction of available clients for evaluation."""
         num_clients = int(num_available_clients * self.fraction_evaluate)
         return max(num_clients, self.min_evaluate_clients), self.min_available_clients
```

### Comparing `flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/strategy/fedavg_android.py` & `flwr_nightly-1.5.0.dev20230614/src/py/flwr/server/strategy/fedavg_android.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,16 +105,15 @@
         self.initial_parameters = initial_parameters
 
     def __repr__(self) -> str:
         rep = f"FedAvg(accept_failures={self.accept_failures})"
         return rep
 
     def num_fit_clients(self, num_available_clients: int) -> Tuple[int, int]:
-        """Return the sample size and the required number of available
-        clients."""
+        """Return the sample size and the required number of available clients."""
         num_clients = int(num_available_clients * self.fraction_fit)
         return max(num_clients, self.min_fit_clients), self.min_available_clients
 
     def num_evaluation_clients(self, num_available_clients: int) -> Tuple[int, int]:
         """Use a fraction of available clients for evaluation."""
         num_clients = int(num_available_clients * self.fraction_evaluate)
         return max(num_clients, self.min_evaluate_clients), self.min_available_clients
```

### Comparing `flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/strategy/fedavgm.py` & `flwr_nightly-1.5.0.dev20230614/src/py/flwr/server/strategy/fedavgm.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/strategy/fedmedian.py` & `flwr_nightly-1.5.0.dev20230614/src/py/flwr/server/strategy/fedmedian.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/strategy/fedopt.py` & `flwr_nightly-1.5.0.dev20230614/src/py/flwr/server/strategy/fedopt.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,16 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-"""Adaptive Federated Optimization (FedOpt) [Reddi et al., 2020] abstract
-strategy.
+"""Adaptive Federated Optimization (FedOpt) [Reddi et al., 2020] abstract strategy.
 
 Paper: arxiv.org/abs/2003.00295
 """
 
 
 from typing import Callable, Dict, Optional, Tuple
```

### Comparing `flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/strategy/fedprox.py` & `flwr_nightly-1.5.0.dev20230614/src/py/flwr/server/strategy/fedprox.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/strategy/fedtrimmedavg.py` & `flwr_nightly-1.5.0.dev20230614/src/py/flwr/server/strategy/fedtrimmedavg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/strategy/fedxgb_nn_avg.py` & `flwr_nightly-1.5.0.dev20230614/src/py/flwr/server/strategy/fedxgb_nn_avg.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-"""Federated XGBoost in the horizontal setting based on building Neural Network
-and averaging on prediction outcomes [Ma et al., 2023].
+"""Federated XGBoost in the horizontal setting based on building Neural Network and
+averaging on prediction outcomes [Ma et al., 2023].
 
 Paper: Coming
 """
 
 
 from logging import WARNING
 from typing import Any, Dict, List, Optional, Tuple, Union
```

### Comparing `flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/strategy/fedyogi.py` & `flwr_nightly-1.5.0.dev20230614/src/py/flwr/server/strategy/fedyogi.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-"""Adaptive Federated Optimization using Yogi (FedYogi) [Reddi et al., 2020]
-strategy.
+"""Adaptive Federated Optimization using Yogi (FedYogi) [Reddi et al., 2020] strategy.
 
 Paper: arxiv.org/abs/2003.00295
 """
 
 
 from typing import Callable, Dict, List, Optional, Tuple, Union
 
@@ -35,16 +34,16 @@
 from flwr.server.client_proxy import ClientProxy
 
 from .fedopt import FedOpt
 
 
 # flake8: noqa: E501
 class FedYogi(FedOpt):
-    """Adaptive Federated Optimization using Yogi (FedYogi) [Reddi et al.,
-    2020] strategy.
+    """Adaptive Federated Optimization using Yogi (FedYogi) [Reddi et al., 2020]
+    strategy.
 
     Paper: https://arxiv.org/abs/2003.00295
     """
 
     # pylint: disable=too-many-arguments,too-many-instance-attributes,too-many-locals,line-too-long
     def __init__(
         self,
```

### Comparing `flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/strategy/krum.py` & `flwr_nightly-1.5.0.dev20230614/src/py/flwr/server/strategy/krum.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/strategy/qfedavg.py` & `flwr_nightly-1.5.0.dev20230614/src/py/flwr/server/strategy/qfedavg.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,16 +92,15 @@
     def __repr__(self) -> str:
         # pylint: disable=line-too-long
         rep = f"QffedAvg(learning_rate={self.learning_rate}, "
         rep += f"q_param={self.q_param}, pre_weights={self.pre_weights})"
         return rep
 
     def num_fit_clients(self, num_available_clients: int) -> Tuple[int, int]:
-        """Return the sample size and the required number of available
-        clients."""
+        """Return the sample size and the required number of available clients."""
         num_clients = int(num_available_clients * self.fraction_fit)
         return max(num_clients, self.min_fit_clients), self.min_available_clients
 
     def num_evaluation_clients(self, num_available_clients: int) -> Tuple[int, int]:
         """Use a fraction of available clients for evaluation."""
         num_clients = int(num_available_clients * self.fraction_evaluate)
         return max(num_clients, self.min_evaluate_clients), self.min_available_clients
```

### Comparing `flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/strategy/strategy.py` & `flwr_nightly-1.5.0.dev20230614/src/py/flwr/server/strategy/strategy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/utils/__init__.py` & `flwr_nightly-1.5.0.dev20230614/src/py/flwr/server/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/utils/tensorboard.py` & `flwr_nightly-1.5.0.dev20230614/src/py/flwr/server/utils/tensorboard.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,16 +78,15 @@
 
             def aggregate_evaluate(
                 self,
                 server_round: int,
                 results: List[Tuple[ClientProxy, EvaluateRes]],
                 failures: List[Union[Tuple[ClientProxy, EvaluateRes], BaseException]],
             ) -> Tuple[Optional[float], Dict[str, Scalar]]:
-                """Hooks into aggregate_evaluate for TensorBoard logging
-                purpose."""
+                """Hooks into aggregate_evaluate for TensorBoard logging purpose."""
                 # Execute decorated function and extract results for logging
                 # They will be returned at the end of this function but also
                 # used for logging
                 loss_aggregated, config = super().aggregate_evaluate(
                     server_round,
                     results,
                     failures,
```

### Comparing `flwr_nightly-1.5.0.dev20230608/src/py/flwr/server/utils/validator.py` & `flwr_nightly-1.5.0.dev20230614/src/py/flwr/server/utils/validator.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 
 from flwr.proto.task_pb2 import TaskIns, TaskRes
 
 
 # pylint: disable-next=too-many-branches
 def validate_task_ins_or_res(tasks_ins_res: Union[TaskIns, TaskRes]) -> List[str]:
     """Validate a TaskIns or TaskRes."""
-
     validation_errors = []
 
     if tasks_ins_res.task_id != "":
         validation_errors.append("non-empty `task_id`")
 
     if not tasks_ins_res.HasField("task"):
         validation_errors.append("`task` does not set field `task`")
```

### Comparing `flwr_nightly-1.5.0.dev20230608/src/py/flwr/simulation/__init__.py` & `flwr_nightly-1.5.0.dev20230614/src/py/flwr/simulation/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230608/src/py/flwr/simulation/app.py` & `flwr_nightly-1.5.0.dev20230614/src/py/flwr/simulation/app.py`

 * *Files 3% similar despite different names*

```diff
@@ -125,15 +125,14 @@
         Set to True to prevent `ray.shutdown()` in case `ray.is_initialized()=True`.
 
     Returns
     -------
     hist : flwr.server.history.History
         Object containing metrics from training.
     """
-
     # pylint: disable-msg=too-many-locals
     event(
         EventType.START_SIMULATION_ENTER,
         {"num_clients": len(clients_ids) if clients_ids is not None else num_clients},
     )
 
     # Initialize server and server config
@@ -168,23 +167,23 @@
     if not ray_init_args:
         ray_init_args = {
             "ignore_reinit_error": True,
             "include_dashboard": False,
         }
 
     # Shut down Ray if it has already been initialized (unless asked not to)
-    if ray.is_initialized() and not keep_initialised:
-        ray.shutdown()
+    if ray.is_initialized() and not keep_initialised:  # type: ignore
+        ray.shutdown()  # type: ignore
 
     # Initialize Ray
-    ray.init(**ray_init_args)
+    ray.init(**ray_init_args)  # type: ignore
     log(
         INFO,
         "Flower VCE: Ray initialized with resources: %s",
-        ray.cluster_resources(),
+        ray.cluster_resources(),  # type: ignore
     )
 
     # Register one RayClientProxy object for each client with the ClientManager
     resources = client_resources if client_resources is not None else {}
     for cid in cids:
         client_proxy = RayClientProxy(
             client_fn=client_fn,
```

### Comparing `flwr_nightly-1.5.0.dev20230608/src/py/flwr/simulation/ray_transport/__init__.py` & `flwr_nightly-1.5.0.dev20230614/src/py/flwr/simulation/ray_transport/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230608/src/py/flwr/simulation/ray_transport/ray_client_proxy.py` & `flwr_nightly-1.5.0.dev20230614/src/py/flwr/simulation/ray_transport/ray_client_proxy.py`

 * *Files 12% similar despite different names*

```diff
@@ -41,69 +41,69 @@
         super().__init__(cid)
         self.client_fn = client_fn
         self.resources = resources
 
     def get_properties(
         self, ins: common.GetPropertiesIns, timeout: Optional[float]
     ) -> common.GetPropertiesRes:
-        """Returns client's properties."""
-        future_get_properties_res = launch_and_get_properties.options(  # type: ignore
+        """Return client's properties."""
+        future_get_properties_res = launch_and_get_properties.options(
             **self.resources,
         ).remote(self.client_fn, self.cid, ins)
         try:
-            res = ray.get(future_get_properties_res, timeout=timeout)
+            res = ray.get(future_get_properties_res, timeout=timeout)  # type: ignore
         except Exception as ex:
             log(ERROR, ex)
             raise ex
         return cast(
             common.GetPropertiesRes,
             res,
         )
 
     def get_parameters(
         self, ins: common.GetParametersIns, timeout: Optional[float]
     ) -> common.GetParametersRes:
         """Return the current local model parameters."""
-        future_paramseters_res = launch_and_get_parameters.options(  # type: ignore
+        future_paramseters_res = launch_and_get_parameters.options(
             **self.resources,
         ).remote(self.client_fn, self.cid, ins)
         try:
-            res = ray.get(future_paramseters_res, timeout=timeout)
+            res = ray.get(future_paramseters_res, timeout=timeout)  # type: ignore
         except Exception as ex:
             log(ERROR, ex)
             raise ex
         return cast(
             common.GetParametersRes,
             res,
         )
 
     def fit(self, ins: common.FitIns, timeout: Optional[float]) -> common.FitRes:
         """Train model parameters on the locally held dataset."""
-        future_fit_res = launch_and_fit.options(  # type: ignore
+        future_fit_res = launch_and_fit.options(
             **self.resources,
         ).remote(self.client_fn, self.cid, ins)
         try:
-            res = ray.get(future_fit_res, timeout=timeout)
+            res = ray.get(future_fit_res, timeout=timeout)  # type: ignore
         except Exception as ex:
             log(ERROR, ex)
             raise ex
         return cast(
             common.FitRes,
             res,
         )
 
     def evaluate(
         self, ins: common.EvaluateIns, timeout: Optional[float]
     ) -> common.EvaluateRes:
         """Evaluate model parameters on the locally held dataset."""
-        future_evaluate_res = launch_and_evaluate.options(  # type: ignore
+        future_evaluate_res = launch_and_evaluate.options(
             **self.resources,
         ).remote(self.client_fn, self.cid, ins)
         try:
-            res = ray.get(future_evaluate_res, timeout=timeout)
+            res = ray.get(future_evaluate_res, timeout=timeout)  # type: ignore
         except Exception as ex:
             log(ERROR, ex)
             raise ex
         return cast(
             common.EvaluateRes,
             res,
         )
@@ -111,51 +111,51 @@
     def reconnect(
         self, ins: common.ReconnectIns, timeout: Optional[float]
     ) -> common.DisconnectRes:
         """Disconnect and (optionally) reconnect later."""
         return common.DisconnectRes(reason="")  # Nothing to do here (yet)
 
 
-@ray.remote
+@ray.remote  # type: ignore
 def launch_and_get_properties(
     client_fn: ClientFn, cid: str, get_properties_ins: common.GetPropertiesIns
 ) -> common.GetPropertiesRes:
     """Exectue get_properties remotely."""
     client: Client = _create_client(client_fn, cid)
     return maybe_call_get_properties(
         client=client,
         get_properties_ins=get_properties_ins,
     )
 
 
-@ray.remote
+@ray.remote  # type: ignore
 def launch_and_get_parameters(
     client_fn: ClientFn, cid: str, get_parameters_ins: common.GetParametersIns
 ) -> common.GetParametersRes:
     """Exectue get_parameters remotely."""
     client: Client = _create_client(client_fn, cid)
     return maybe_call_get_parameters(
         client=client,
         get_parameters_ins=get_parameters_ins,
     )
 
 
-@ray.remote
+@ray.remote  # type: ignore
 def launch_and_fit(
     client_fn: ClientFn, cid: str, fit_ins: common.FitIns
 ) -> common.FitRes:
     """Exectue fit remotely."""
     client: Client = _create_client(client_fn, cid)
     return maybe_call_fit(
         client=client,
         fit_ins=fit_ins,
     )
 
 
-@ray.remote
+@ray.remote  # type: ignore
 def launch_and_evaluate(
     client_fn: ClientFn, cid: str, evaluate_ins: common.EvaluateIns
 ) -> common.EvaluateRes:
     """Exectue evaluate remotely."""
     client: Client = _create_client(client_fn, cid)
     return maybe_call_evaluate(
         client=client,
```

### Comparing `flwr_nightly-1.5.0.dev20230608/setup.py` & `flwr_nightly-1.5.0.dev20230614/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 {'console_scripts': ['flower-client = flwr.client:run_client',
                      'flower-driver-api = flwr.server:run_driver_api',
                      'flower-fleet-api = flwr.server:run_fleet_api',
                      'flower-server = flwr.server:run_server']}
 
 setup_kwargs = {
     'name': 'flwr-nightly',
-    'version': '1.5.0.dev20230608',
+    'version': '1.5.0.dev20230614',
     'description': 'Flower: A Friendly Federated Learning Framework',
     'long_description': '# Flower: A Friendly Federated Learning Framework\n\n<p align="center">\n  <a href="https://flower.dev/">\n    <img src="https://flower.dev/_next/image/?url=%2F_next%2Fstatic%2Fmedia%2Fflower_white_border.c2012e70.png&w=640&q=75" width="140px" alt="Flower Website" />\n  </a>\n</p>\n<p align="center">\n    <a href="https://flower.dev/">Website</a> |\n    <a href="https://flower.dev/blog">Blog</a> |\n    <a href="https://flower.dev/docs/">Docs</a> |\n    <a href="https://flower.dev/conf/flower-summit-2022">Conference</a> |\n    <a href="https://flower.dev/join-slack">Slack</a>\n    <br /><br />\n</p>\n\n[![GitHub license](https://img.shields.io/github/license/adap/flower)](https://github.com/adap/flower/blob/main/LICENSE)\n[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://github.com/adap/flower/blob/main/CONTRIBUTING.md)\n![Build](https://github.com/adap/flower/actions/workflows/flower.yml/badge.svg)\n![Downloads](https://pepy.tech/badge/flwr)\n[![Slack](https://img.shields.io/badge/Chat-Slack-red)](https://flower.dev/join-slack)\n\nFlower (`flwr`) is a framework for building federated learning systems. The\ndesign of Flower is based on a few guiding principles:\n\n* **Customizable**: Federated learning systems vary wildly from one use case to\n  another. Flower allows for a wide range of different configurations depending\n  on the needs of each individual use case.\n\n* **Extendable**: Flower originated from a research project at the University of\n  Oxford, so it was built with AI research in mind. Many components can be\n  extended and overridden to build new state-of-the-art systems.\n\n* **Framework-agnostic**: Different machine learning frameworks have different\n  strengths. Flower can be used with any machine learning framework, for\n  example, [PyTorch](https://pytorch.org),\n  [TensorFlow](https://tensorflow.org), [Hugging Face Transformers](https://huggingface.co/), [PyTorch Lightning](https://pytorchlightning.ai/), [MXNet](https://mxnet.apache.org/), [scikit-learn](https://scikit-learn.org/), [JAX](https://jax.readthedocs.io/), [TFLite](https://tensorflow.org/lite/), [fastai](https://www.fast.ai/), [Pandas](https://pandas.pydata.org/\n) for federated analytics, or even raw [NumPy](https://numpy.org/)\n  for users who enjoy computing gradients by hand.\n\n* **Understandable**: Flower is written with maintainability in mind. The\n  community is encouraged to both read and contribute to the codebase.\n\nMeet the Flower community on [flower.dev](https://flower.dev)!\n\n## Federated Learning Tutorial\n\nFlower\'s goal is to make federated learning accessible to everyone. This series of tutorials introduces the fundamentals of federated learning and how to implement them in Flower.\n\n0. **What is Federated Learning?**\n\n   [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adap/flower/blob/main/doc/source/tutorial/Flower-0-What-is-FL.ipynb) (or open the [Jupyter Notebook](https://github.com/adap/flower/blob/main/doc/source/tutorial/Flower-0-What-is-FL.ipynb))\n\n1. **An Introduction to Federated Learning**\n\n   [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adap/flower/blob/main/doc/source/tutorial/Flower-1-Intro-to-FL-PyTorch.ipynb) (or open the [Jupyter Notebook](https://github.com/adap/flower/blob/main/doc/source/tutorial/Flower-1-Intro-to-FL-PyTorch.ipynb))\n\n2. **Using Strategies in Federated Learning**\n\n   [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adap/flower/blob/main/doc/source/tutorial/Flower-2-Strategies-in-FL-PyTorch.ipynb) (or open the [Jupyter Notebook](https://github.com/adap/flower/blob/main/doc/source/tutorial/Flower-2-Strategies-in-FL-PyTorch.ipynb))\n   \n3. **Building Strategies for Federated Learning**\n\n   [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adap/flower/blob/main/doc/source/tutorial/Flower-3-Building-a-Strategy-PyTorch.ipynb) (or open the [Jupyter Notebook](https://github.com/adap/flower/blob/main/doc/source/tutorial/Flower-3-Building-a-Strategy-PyTorch.ipynb))\n   \n4. **Custom Clients for Federated Learning**\n\n   [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adap/flower/blob/main/doc/source/tutorial/Flower-4-Client-and-NumPyClient-PyTorch.ipynb) (or open the [Jupyter Notebook](https://github.com/adap/flower/blob/main/doc/source/tutorial/Flower-4-Client-and-NumPyClient-PyTorch.ipynb))\n\nStay tuned, more tutorials are coming soon. Topics include **Privacy and Security in Federated Learning**, and **Scaling Federated Learning**.\n\n## Documentation\n\n[Flower Docs](https://flower.dev/docs):\n* [Installation](https://flower.dev/docs/installation.html)\n* [Quickstart (TensorFlow)](https://flower.dev/docs/quickstart-tensorflow.html)\n* [Quickstart (PyTorch)](https://flower.dev/docs/quickstart-pytorch.html)\n* [Quickstart (Hugging Face [code example])](https://flower.dev/docs/quickstart-huggingface.html)\n* [Quickstart (PyTorch Lightning [code example])](https://flower.dev/docs/quickstart-pytorch-lightning.html)\n* [Quickstart (MXNet)](https://flower.dev/docs/example-mxnet-walk-through.html)\n* [Quickstart (Pandas)](https://flower.dev/docs/quickstart-pandas.html)\n* [Quickstart (fastai)](https://flower.dev/docs/quickstart-fastai.html)\n* [Quickstart (JAX)](https://github.com/adap/flower/tree/main/examples/quickstart_jax)\n* [Quickstart (scikit-learn)](https://github.com/adap/flower/tree/main/examples/sklearn-logreg-mnist)\n* [Quickstart (TFLite on Android [code example])](https://github.com/adap/flower/tree/main/examples/android)\n* [Quickstart (iOS)](https://flower.dev/docs/quickstart-ios.html)\n\n## Flower Baselines\n\nFlower Baselines is a collection of community-contributed experiments that reproduce the experiments performed in popular federated learning publications. Researchers can build on Flower Baselines to quickly evaluate new ideas:\n\n* [FedAvg](https://arxiv.org/abs/1602.05629):\n  * [MNIST](https://github.com/adap/flower/tree/main/baselines/flwr_baselines/publications/fedavg_mnist)\n* [FedProx](https://arxiv.org/abs/1812.06127):\n  * [MNIST](https://github.com/adap/flower/tree/main/baselines/flwr_baselines/publications/fedprox_mnist)\n* [FedBN: Federated Learning on non-IID Features via Local Batch Normalization](https://arxiv.org/abs/2102.07623):\n  * [Convergence Rate](https://github.com/adap/flower/tree/main/baselines/flwr_baselines/publications/fedbn/convergence_rate)\n* [Adaptive Federated Optimization](https://arxiv.org/abs/2003.00295):\n  * [CIFAR-10/100](https://github.com/adap/flower/tree/main/baselines/flwr_baselines/publications/adaptive_federated_optimization)\n\nCheck the Flower documentation to learn more: [Using Baselines](https://flower.dev/docs/using-baselines.html)\n\nThe Flower community loves contributions! Make your work more visible and enable others to build on it by contributing it as a baseline: [Contributing Baselines](https://flower.dev/docs/contributing-baselines.html)\n\n## Flower Usage Examples\n\nSeveral code examples show different usage scenarios of Flower (in combination with popular machine learning frameworks such as PyTorch or TensorFlow).\n\nQuickstart examples:\n\n* [Quickstart (TensorFlow)](https://github.com/adap/flower/tree/main/examples/quickstart_tensorflow)\n* [Quickstart (PyTorch)](https://github.com/adap/flower/tree/main/examples/quickstart_pytorch)\n* [Quickstart (Hugging Face)](https://github.com/adap/flower/tree/main/examples/quickstart_huggingface)\n* [Quickstart (PyTorch Lightning)](https://github.com/adap/flower/tree/main/examples/quickstart_pytorch_lightning)\n* [Quickstart (fastai)](https://github.com/adap/flower/tree/main/examples/quickstart_fastai)\n* [Quickstart (Pandas)](https://github.com/adap/flower/tree/main/examples/quickstart_pandas)\n* [Quickstart (MXNet)](https://github.com/adap/flower/tree/main/examples/quickstart_mxnet)\n* [Quickstart (JAX)](https://github.com/adap/flower/tree/main/examples/quickstart_jax)\n* [Quickstart (scikit-learn)](https://github.com/adap/flower/tree/main/examples/sklearn-logreg-mnist)\n* [Quickstart (TFLite on Android)](https://github.com/adap/flower/tree/main/examples/android)\n\nOther [examples](https://github.com/adap/flower/tree/main/examples):\n\n* [Raspberry Pi & Nvidia Jetson Tutorial](https://github.com/adap/flower/tree/main/examples/embedded_devices)\n* [Android & TFLite](https://github.com/adap/flower/tree/main/examples/android)\n* [PyTorch: From Centralized to Federated](https://github.com/adap/flower/tree/main/examples/pytorch_from_centralized_to_federated)\n* [MXNet: From Centralized to Federated](https://github.com/adap/flower/tree/main/examples/mxnet_from_centralized_to_federated)\n* [Advanced Flower with TensorFlow/Keras](https://github.com/adap/flower/tree/main/examples/advanced_tensorflow)\n* [Advanced Flower with PyTorch](https://github.com/adap/flower/tree/main/examples/advanced_pytorch)\n* Single-Machine Simulation of Federated Learning Systems ([PyTorch](https://github.com/adap/flower/tree/main/examples/simulation_pytorch)) ([Tensorflow](https://github.com/adap/flower/tree/main/examples/simulation_tensorflow))\n\n## Community\n\nFlower is built by a wonderful community of researchers and engineers. [Join Slack](https://flower.dev/join-slack) to meet them, [contributions](#contributing-to-flower) are welcome.\n\n<a href="https://github.com/adap/flower/graphs/contributors">\n  <img src="https://contrib.rocks/image?repo=adap/flower" />\n</a>\n\n## Citation\n\nIf you publish work that uses Flower, please cite Flower as follows: \n\n```bibtex\n@article{beutel2020flower,\n  title={Flower: A Friendly Federated Learning Research Framework},\n  author={Beutel, Daniel J and Topal, Taner and Mathur, Akhil and Qiu, Xinchi and Fernandez-Marques, Javier and Gao, Yan and Sani, Lorenzo and Kwing, Hei Li and Parcollet, Titouan and Gusmão, Pedro PB de and Lane, Nicholas D}, \n  journal={arXiv preprint arXiv:2007.14390},\n  year={2020}\n}\n```\n\nPlease also consider adding your publication to the list of Flower-based publications in the docs, just open a Pull Request.\n\n## Contributing to Flower\n\nWe welcome contributions. Please see [CONTRIBUTING.md](CONTRIBUTING.md) to get started!\n',
     'author': 'The Flower Authors',
     'author_email': 'hello@flower.dev',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://flower.dev',
```

#### html2text {}

```diff
@@ -12,15 +12,15 @@
 extras_require = \ {':python_version < "3.8"': ['importlib-
 metadata>=4.0.0,<5.0.0'], 'rest': ['requests>=2.28.2,<3.0.0',
 'fastapi>=0.95.0,<0.96.0', 'starlette>=0.26.1,<0.27.0', 'uvicorn
 [standard]>=0.21.1,<0.22.0'], 'simulation': ['ray[default]>=2.4.0,<3.0.0']}
 entry_points = \ {'console_scripts': ['flower-client = flwr.client:run_client',
 'flower-driver-api = flwr.server:run_driver_api', 'flower-fleet-api =
 flwr.server:run_fleet_api', 'flower-server = flwr.server:run_server']}
-setup_kwargs = { 'name': 'flwr-nightly', 'version': '1.5.0.dev20230608',
+setup_kwargs = { 'name': 'flwr-nightly', 'version': '1.5.0.dev20230614',
 'description': 'Flower: A Friendly Federated Learning Framework',
 'long_description': '# Flower: A Friendly Federated Learning Framework\n\n
                           \n \n_[Flower_Website]\n\n
 \n
            \n Website |\n Blog |\n Docs |\n Conference |\n Slack\n
 
                                       \n
```

### Comparing `flwr_nightly-1.5.0.dev20230608/PKG-INFO` & `flwr_nightly-1.5.0.dev20230614/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flwr-nightly
-Version: 1.5.0.dev20230608
+Version: 1.5.0.dev20230614
 Summary: Flower: A Friendly Federated Learning Framework
 Home-page: https://flower.dev
 License: Apache-2.0
 Author: The Flower Authors
 Author-email: hello@flower.dev
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: flwr-nightly Version: 1.5.0.dev20230608 Summary:
+Metadata-Version: 2.1 Name: flwr-nightly Version: 1.5.0.dev20230614 Summary:
 Flower: A Friendly Federated Learning Framework Home-page: https://flower.dev
 License: Apache-2.0 Author: The Flower Authors Author-email: hello@flower.dev
 Requires-Python: >=3.7,<4.0 Classifier: Development Status :: 5 - Production/
 Stable Classifier: Intended Audience :: Developers Classifier: Intended
 Audience :: Science/Research Classifier: License :: OSI Approved :: Apache
 Software License Classifier: Operating System :: MacOS :: MacOS X Classifier:
 Operating System :: POSIX :: Linux Classifier: Programming Language :: Python
```

