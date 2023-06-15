# Comparing `tmp/neptune-1.2.0.tar.gz` & `tmp/neptune-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neptune-1.2.0.tar", max compression
+gzip compressed data, was "neptune-1.3.0.tar", max compression
```

## Comparing `neptune-1.2.0.tar` & `neptune-1.3.0.tar`

### file list

```diff
@@ -1,323 +1,324 @@
--rw-r--r--   0        0        0    25159 2023-05-10 07:50:35.696217 neptune-1.2.0/CHANGELOG.md
--rw-r--r--   0        0        0    11357 2023-05-10 07:50:35.696217 neptune-1.2.0/LICENSE
--rw-r--r--   0        0        0    14357 2023-05-10 07:50:35.696217 neptune-1.2.0/README.md
--rw-r--r--   0        0        0     5315 2023-05-10 07:50:51.312430 neptune-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     3532 2023-05-10 07:50:35.696217 neptune-1.2.0/src/neptune/__init__.py
--rw-r--r--   0        0        0     1218 2023-05-10 07:50:35.696217 neptune-1.2.0/src/neptune/attributes/__init__.py
--rw-r--r--   0        0        0     1011 2023-05-10 07:50:35.696217 neptune-1.2.0/src/neptune/attributes/atoms/__init__.py
--rw-r--r--   0        0        0     3048 2023-05-10 07:50:35.696217 neptune-1.2.0/src/neptune/attributes/atoms/artifact.py
--rw-r--r--   0        0        0      701 2023-05-10 07:50:35.696217 neptune-1.2.0/src/neptune/attributes/atoms/atom.py
--rw-r--r--   0        0        0     1709 2023-05-10 07:50:35.696217 neptune-1.2.0/src/neptune/attributes/atoms/boolean.py
--rw-r--r--   0        0        0     2121 2023-05-10 07:50:35.696217 neptune-1.2.0/src/neptune/attributes/atoms/copiable_atom.py
--rw-r--r--   0        0        0     2075 2023-05-10 07:50:35.696217 neptune-1.2.0/src/neptune/attributes/atoms/datetime.py
--rw-r--r--   0        0        0     1788 2023-05-10 07:50:35.696217 neptune-1.2.0/src/neptune/attributes/atoms/file.py
--rw-r--r--   0        0        0     1704 2023-05-10 07:50:35.696217 neptune-1.2.0/src/neptune/attributes/atoms/float.py
--rw-r--r--   0        0        0      696 2023-05-10 07:50:35.696217 neptune-1.2.0/src/neptune/attributes/atoms/git_ref.py
--rw-r--r--   0        0        0     2395 2023-05-10 07:50:35.696217 neptune-1.2.0/src/neptune/attributes/atoms/integer.py
--rw-r--r--   0        0        0      707 2023-05-10 07:50:35.696217 neptune-1.2.0/src/neptune/attributes/atoms/notebook_ref.py
--rw-r--r--   0        0        0      700 2023-05-10 07:50:35.700217 neptune-1.2.0/src/neptune/attributes/atoms/run_state.py
--rw-r--r--   0        0        0     2658 2023-05-10 07:50:35.700217 neptune-1.2.0/src/neptune/attributes/atoms/string.py
--rw-r--r--   0        0        0     2159 2023-05-10 07:50:35.700217 neptune-1.2.0/src/neptune/attributes/attribute.py
--rw-r--r--   0        0        0     2538 2023-05-10 07:50:35.700217 neptune-1.2.0/src/neptune/attributes/constants.py
--rw-r--r--   0        0        0     2642 2023-05-10 07:50:35.700217 neptune-1.2.0/src/neptune/attributes/file_set.py
--rw-r--r--   0        0        0     4266 2023-05-10 07:50:35.700217 neptune-1.2.0/src/neptune/attributes/namespace.py
--rw-r--r--   0        0        0      782 2023-05-10 07:50:35.700217 neptune-1.2.0/src/neptune/attributes/series/__init__.py
--rw-r--r--   0        0        0     1949 2023-05-10 07:50:35.700217 neptune-1.2.0/src/neptune/attributes/series/fetchable_series.py
--rw-r--r--   0        0        0     4292 2023-05-10 07:50:35.700217 neptune-1.2.0/src/neptune/attributes/series/file_series.py
--rw-r--r--   0        0        0     2656 2023-05-10 07:50:35.700217 neptune-1.2.0/src/neptune/attributes/series/float_series.py
--rw-r--r--   0        0        0     6003 2023-05-10 07:50:35.700217 neptune-1.2.0/src/neptune/attributes/series/series.py
--rw-r--r--   0        0        0     3498 2023-05-10 07:50:35.700217 neptune-1.2.0/src/neptune/attributes/series/string_series.py
--rw-r--r--   0        0        0      662 2023-05-10 07:50:35.700217 neptune-1.2.0/src/neptune/attributes/sets/__init__.py
--rw-r--r--   0        0        0      699 2023-05-10 07:50:35.700217 neptune-1.2.0/src/neptune/attributes/sets/set.py
--rw-r--r--   0        0        0     2627 2023-05-10 07:50:35.700217 neptune-1.2.0/src/neptune/attributes/sets/string_set.py
--rw-r--r--   0        0        0     2157 2023-05-10 07:50:35.700217 neptune-1.2.0/src/neptune/attributes/utils.py
--rw-r--r--   0        0        0      686 2023-05-10 07:50:35.700217 neptune-1.2.0/src/neptune/cli/__init__.py
--rw-r--r--   0        0        0     1017 2023-05-10 07:50:35.700217 neptune-1.2.0/src/neptune/cli/__main__.py
--rw-r--r--   0        0        0      866 2023-05-10 07:50:35.700217 neptune-1.2.0/src/neptune/cli/abstract_backend_runner.py
--rw-r--r--   0        0        0     3436 2023-05-10 07:50:35.700217 neptune-1.2.0/src/neptune/cli/clear.py
--rw-r--r--   0        0        0     5574 2023-05-10 07:50:35.700217 neptune-1.2.0/src/neptune/cli/commands.py
--rw-r--r--   0        0        0     2814 2023-05-10 07:50:35.700217 neptune-1.2.0/src/neptune/cli/container_manager.py
--rw-r--r--   0        0        0     1947 2023-05-10 07:50:35.700217 neptune-1.2.0/src/neptune/cli/path_option.py
--rw-r--r--   0        0        0     3899 2023-05-10 07:50:35.700217 neptune-1.2.0/src/neptune/cli/status.py
--rw-r--r--   0        0        0     9995 2023-05-10 07:50:35.700217 neptune-1.2.0/src/neptune/cli/sync.py
--rw-r--r--   0        0        0     5028 2023-05-10 07:50:35.700217 neptune-1.2.0/src/neptune/cli/utils.py
--rw-r--r--   0        0        0      596 2023-05-10 07:50:35.700217 neptune-1.2.0/src/neptune/common/__init__.py
--rw-r--r--   0        0        0      596 2023-05-10 07:50:35.700217 neptune-1.2.0/src/neptune/common/backends/__init__.py
--rw-r--r--   0        0        0     1038 2023-05-10 07:50:35.700217 neptune-1.2.0/src/neptune/common/backends/api_model.py
--rw-r--r--   0        0        0     4230 2023-05-10 07:50:35.700217 neptune-1.2.0/src/neptune/common/backends/utils.py
--rw-r--r--   0        0        0      859 2023-05-10 07:50:35.700217 neptune-1.2.0/src/neptune/common/envs.py
--rw-r--r--   0        0        0    14106 2023-05-10 07:50:35.700217 neptune-1.2.0/src/neptune/common/exceptions.py
--rw-r--r--   0        0        0      629 2023-05-10 07:50:35.700217 neptune-1.2.0/src/neptune/common/experiments.py
--rw-r--r--   0        0        0     2490 2023-05-10 07:50:35.700217 neptune-1.2.0/src/neptune/common/git_info.py
--rw-r--r--   0        0        0      596 2023-05-10 07:50:35.700217 neptune-1.2.0/src/neptune/common/hardware/__init__.py
--rw-r--r--   0        0        0      596 2023-05-10 07:50:35.700217 neptune-1.2.0/src/neptune/common/hardware/cgroup/__init__.py
--rw-r--r--   0        0        0     2638 2023-05-10 07:50:35.700217 neptune-1.2.0/src/neptune/common/hardware/cgroup/cgroup_filesystem_reader.py
--rw-r--r--   0        0        0     3212 2023-05-10 07:50:35.700217 neptune-1.2.0/src/neptune/common/hardware/cgroup/cgroup_monitor.py
--rw-r--r--   0        0        0      694 2023-05-10 07:50:35.700217 neptune-1.2.0/src/neptune/common/hardware/constants.py
--rw-r--r--   0        0        0      596 2023-05-10 07:50:35.700217 neptune-1.2.0/src/neptune/common/hardware/gauges/__init__.py
--rw-r--r--   0        0        0     1554 2023-05-10 07:50:35.700217 neptune-1.2.0/src/neptune/common/hardware/gauges/cpu.py
--rw-r--r--   0        0        0      979 2023-05-10 07:50:35.700217 neptune-1.2.0/src/neptune/common/hardware/gauges/gauge.py
--rw-r--r--   0        0        0     2023 2023-05-10 07:50:35.700217 neptune-1.2.0/src/neptune/common/hardware/gauges/gauge_factory.py
--rw-r--r--   0        0        0      667 2023-05-10 07:50:35.700217 neptune-1.2.0/src/neptune/common/hardware/gauges/gauge_mode.py
--rw-r--r--   0        0        0     1766 2023-05-10 07:50:35.700217 neptune-1.2.0/src/neptune/common/hardware/gauges/gpu.py
--rw-r--r--   0        0        0     1748 2023-05-10 07:50:35.700217 neptune-1.2.0/src/neptune/common/hardware/gauges/memory.py
--rw-r--r--   0        0        0      596 2023-05-10 07:50:35.700217 neptune-1.2.0/src/neptune/common/hardware/gpu/__init__.py
--rw-r--r--   0        0        0     2568 2023-05-10 07:50:35.700217 neptune-1.2.0/src/neptune/common/hardware/gpu/gpu_monitor.py
--rw-r--r--   0        0        0      596 2023-05-10 07:50:35.700217 neptune-1.2.0/src/neptune/common/hardware/metrics/__init__.py
--rw-r--r--   0        0        0     2432 2023-05-10 07:50:35.700217 neptune-1.2.0/src/neptune/common/hardware/metrics/metric.py
--rw-r--r--   0        0        0     1216 2023-05-10 07:50:35.700217 neptune-1.2.0/src/neptune/common/hardware/metrics/metrics_container.py
--rw-r--r--   0        0        0     3490 2023-05-10 07:50:35.700217 neptune-1.2.0/src/neptune/common/hardware/metrics/metrics_factory.py
--rw-r--r--   0        0        0      596 2023-05-10 07:50:35.700217 neptune-1.2.0/src/neptune/common/hardware/metrics/reports/__init__.py
--rw-r--r--   0        0        0      792 2023-05-10 07:50:35.700217 neptune-1.2.0/src/neptune/common/hardware/metrics/reports/metric_report.py
--rw-r--r--   0        0        0     1679 2023-05-10 07:50:35.700217 neptune-1.2.0/src/neptune/common/hardware/metrics/reports/metric_reporter.py
--rw-r--r--   0        0        0      947 2023-05-10 07:50:35.700217 neptune-1.2.0/src/neptune/common/hardware/metrics/reports/metric_reporter_factory.py
--rw-r--r--   0        0        0      596 2023-05-10 07:50:35.700217 neptune-1.2.0/src/neptune/common/hardware/metrics/service/__init__.py
--rw-r--r--   0        0        0     1106 2023-05-10 07:50:35.700217 neptune-1.2.0/src/neptune/common/hardware/metrics/service/metric_service.py
--rw-r--r--   0        0        0     2309 2023-05-10 07:50:35.700217 neptune-1.2.0/src/neptune/common/hardware/metrics/service/metric_service_factory.py
--rw-r--r--   0        0        0      596 2023-05-10 07:50:35.700217 neptune-1.2.0/src/neptune/common/hardware/resources/__init__.py
--rw-r--r--   0        0        0     1821 2023-05-10 07:50:35.704218 neptune-1.2.0/src/neptune/common/hardware/resources/gpu_card_indices_provider.py
--rw-r--r--   0        0        0     1574 2023-05-10 07:50:35.704218 neptune-1.2.0/src/neptune/common/hardware/resources/system_resource_info.py
--rw-r--r--   0        0        0     2504 2023-05-10 07:50:35.704218 neptune-1.2.0/src/neptune/common/hardware/resources/system_resource_info_factory.py
--rw-r--r--   0        0        0      596 2023-05-10 07:50:35.704218 neptune-1.2.0/src/neptune/common/hardware/system/__init__.py
--rw-r--r--   0        0        0      964 2023-05-10 07:50:35.704218 neptune-1.2.0/src/neptune/common/hardware/system/system_monitor.py
--rw-r--r--   0        0        0     4772 2023-05-10 07:50:35.704218 neptune-1.2.0/src/neptune/common/oauth.py
--rw-r--r--   0        0        0      884 2023-05-10 07:50:35.704218 neptune-1.2.0/src/neptune/common/patches/__init__.py
--rw-r--r--   0        0        0     2731 2023-05-10 07:50:35.704218 neptune-1.2.0/src/neptune/common/patches/bravado.py
--rw-r--r--   0        0        0      726 2023-05-10 07:50:35.704218 neptune-1.2.0/src/neptune/common/patterns.py
--rw-r--r--   0        0        0      596 2023-05-10 07:50:35.704218 neptune-1.2.0/src/neptune/common/storage/__init__.py
--rw-r--r--   0        0        0     3223 2023-05-10 07:50:35.704218 neptune-1.2.0/src/neptune/common/storage/datastream.py
--rw-r--r--   0        0        0     7335 2023-05-10 07:50:35.704218 neptune-1.2.0/src/neptune/common/storage/storage_utils.py
--rw-r--r--   0        0        0     7075 2023-05-10 07:50:35.704218 neptune-1.2.0/src/neptune/common/utils.py
--rw-r--r--   0        0        0     2206 2023-05-10 07:50:35.704218 neptune-1.2.0/src/neptune/common/warnings.py
--rw-r--r--   0        0        0      596 2023-05-10 07:50:35.704218 neptune-1.2.0/src/neptune/common/websockets/__init__.py
--rw-r--r--   0        0        0     3589 2023-05-10 07:50:35.704218 neptune-1.2.0/src/neptune/common/websockets/reconnecting_websocket.py
--rw-r--r--   0        0        0     2693 2023-05-10 07:50:35.704218 neptune-1.2.0/src/neptune/common/websockets/websocket_client_adapter.py
--rw-r--r--   0        0        0      985 2023-05-10 07:50:35.704218 neptune-1.2.0/src/neptune/constants.py
--rw-r--r--   0        0        0     1863 2023-05-10 07:50:35.704218 neptune-1.2.0/src/neptune/envs.py
--rw-r--r--   0        0        0    41966 2023-05-10 07:50:35.704218 neptune-1.2.0/src/neptune/exceptions.py
--rw-r--r--   0        0        0    29698 2023-05-10 07:50:35.704218 neptune-1.2.0/src/neptune/handler.py
--rw-r--r--   0        0        0      596 2023-05-10 07:50:35.704218 neptune-1.2.0/src/neptune/integrations/__init__.py
--rw-r--r--   0        0        0      973 2023-05-10 07:50:35.704218 neptune-1.2.0/src/neptune/integrations/aws/__init__.py
--rw-r--r--   0        0        0     1014 2023-05-10 07:50:35.704218 neptune-1.2.0/src/neptune/integrations/detectron2/__init__.py
--rw-r--r--   0        0        0      985 2023-05-10 07:50:35.704218 neptune-1.2.0/src/neptune/integrations/fastai/__init__.py
--rw-r--r--   0        0        0      976 2023-05-10 07:50:35.704218 neptune-1.2.0/src/neptune/integrations/kedro/__init__.py
--rw-r--r--   0        0        0      993 2023-05-10 07:50:35.704218 neptune-1.2.0/src/neptune/integrations/lightgbm/__init__.py
--rw-r--r--   0        0        0      985 2023-05-10 07:50:35.704218 neptune-1.2.0/src/neptune/integrations/optuna/__init__.py
--rw-r--r--   0        0        0      989 2023-05-10 07:50:35.704218 neptune-1.2.0/src/neptune/integrations/prophet/__init__.py
--rw-r--r--   0        0        0     3084 2023-05-10 07:50:35.704218 neptune-1.2.0/src/neptune/integrations/python_logger.py
--rw-r--r--   0        0        0     1006 2023-05-10 07:50:35.704218 neptune-1.2.0/src/neptune/integrations/pytorch/__init__.py
--rw-r--r--   0        0        0     1042 2023-05-10 07:50:35.704218 neptune-1.2.0/src/neptune/integrations/pytorch_lightning/__init__.py
--rw-r--r--   0        0        0      985 2023-05-10 07:50:35.704218 neptune-1.2.0/src/neptune/integrations/sacred/__init__.py
--rw-r--r--   0        0        0      989 2023-05-10 07:50:35.704218 neptune-1.2.0/src/neptune/integrations/sklearn/__init__.py
--rw-r--r--   0        0        0     1038 2023-05-10 07:50:35.704218 neptune-1.2.0/src/neptune/integrations/tensorflow_keras/__init__.py
--rw-r--r--   0        0        0     1032 2023-05-10 07:50:35.704218 neptune-1.2.0/src/neptune/integrations/transformers/__init__.py
--rw-r--r--   0        0        0     1164 2023-05-10 07:50:35.704218 neptune-1.2.0/src/neptune/integrations/utils.py
--rw-r--r--   0        0        0      989 2023-05-10 07:50:35.704218 neptune-1.2.0/src/neptune/integrations/xgboost/__init__.py
--rw-r--r--   0        0        0      596 2023-05-10 07:50:35.704218 neptune-1.2.0/src/neptune/internal/__init__.py
--rw-r--r--   0        0        0      760 2023-05-10 07:50:35.704218 neptune-1.2.0/src/neptune/internal/artifacts/__init__.py
--rw-r--r--   0        0        0      791 2023-05-10 07:50:35.704218 neptune-1.2.0/src/neptune/internal/artifacts/drivers/__init__.py
--rw-r--r--   0        0        0     4240 2023-05-10 07:50:35.704218 neptune-1.2.0/src/neptune/internal/artifacts/drivers/local.py
--rw-r--r--   0        0        0     4810 2023-05-10 07:50:35.704218 neptune-1.2.0/src/neptune/internal/artifacts/drivers/s3.py
--rw-r--r--   0        0        0     4017 2023-05-10 07:50:35.704218 neptune-1.2.0/src/neptune/internal/artifacts/file_hasher.py
--rw-r--r--   0        0        0     2318 2023-05-10 07:50:35.704218 neptune-1.2.0/src/neptune/internal/artifacts/local_file_hash_storage.py
--rw-r--r--   0        0        0     3578 2023-05-10 07:50:35.704218 neptune-1.2.0/src/neptune/internal/artifacts/types.py
--rw-r--r--   0        0        0      999 2023-05-10 07:50:35.704218 neptune-1.2.0/src/neptune/internal/artifacts/utils.py
--rw-r--r--   0        0        0      596 2023-05-10 07:50:35.704218 neptune-1.2.0/src/neptune/internal/backends/__init__.py
--rw-r--r--   0        0        0     7169 2023-05-10 07:50:35.704218 neptune-1.2.0/src/neptune/internal/backends/api_model.py
--rw-r--r--   0        0        0     1703 2023-05-10 07:50:35.704218 neptune-1.2.0/src/neptune/internal/backends/factory.py
--rw-r--r--   0        0        0     6700 2023-05-10 07:50:35.704218 neptune-1.2.0/src/neptune/internal/backends/hosted_artifact_operations.py
--rw-r--r--   0        0        0     5942 2023-05-10 07:50:35.704218 neptune-1.2.0/src/neptune/internal/backends/hosted_client.py
--rw-r--r--   0        0        0    17136 2023-05-10 07:50:35.704218 neptune-1.2.0/src/neptune/internal/backends/hosted_file_operations.py
--rw-r--r--   0        0        0    40705 2023-05-10 07:50:35.704218 neptune-1.2.0/src/neptune/internal/backends/hosted_neptune_backend.py
--rw-r--r--   0        0        0     8506 2023-05-10 07:50:35.704218 neptune-1.2.0/src/neptune/internal/backends/neptune_backend.py
--rw-r--r--   0        0        0    31714 2023-05-10 07:50:35.704218 neptune-1.2.0/src/neptune/internal/backends/neptune_backend_mock.py
--rw-r--r--   0        0        0     1942 2023-05-10 07:50:35.704218 neptune-1.2.0/src/neptune/internal/backends/nql.py
--rw-r--r--   0        0        0     4471 2023-05-10 07:50:35.704218 neptune-1.2.0/src/neptune/internal/backends/offline_neptune_backend.py
--rw-r--r--   0        0        0     3946 2023-05-10 07:50:35.704218 neptune-1.2.0/src/neptune/internal/backends/operation_api_name_visitor.py
--rw-r--r--   0        0        0     5003 2023-05-10 07:50:35.704218 neptune-1.2.0/src/neptune/internal/backends/operation_api_object_converter.py
--rw-r--r--   0        0        0    13841 2023-05-10 07:50:35.708217 neptune-1.2.0/src/neptune/internal/backends/operations_preprocessor.py
--rw-r--r--   0        0        0     1619 2023-05-10 07:50:35.708217 neptune-1.2.0/src/neptune/internal/backends/project_name_lookup.py
--rw-r--r--   0        0        0     5282 2023-05-10 07:50:35.708217 neptune-1.2.0/src/neptune/internal/backends/swagger_client_wrapper.py
--rw-r--r--   0        0        0     8765 2023-05-10 07:50:35.708217 neptune-1.2.0/src/neptune/internal/backends/utils.py
--rw-r--r--   0        0        0     1381 2023-05-10 07:50:35.708217 neptune-1.2.0/src/neptune/internal/backgroud_job_list.py
--rw-r--r--   0        0        0     1035 2023-05-10 07:50:35.708217 neptune-1.2.0/src/neptune/internal/background_job.py
--rw-r--r--   0        0        0      350 2023-05-10 07:50:35.708217 neptune-1.2.0/src/neptune/internal/constants.py
--rw-r--r--   0        0        0     4486 2023-05-10 07:50:35.708217 neptune-1.2.0/src/neptune/internal/container_structure.py
--rw-r--r--   0        0        0     1302 2023-05-10 07:50:35.708217 neptune-1.2.0/src/neptune/internal/container_type.py
--rw-r--r--   0        0        0     2345 2023-05-10 07:50:35.708217 neptune-1.2.0/src/neptune/internal/credentials.py
--rw-r--r--   0        0        0     8468 2023-05-10 07:50:35.708217 neptune-1.2.0/src/neptune/internal/disk_queue.py
--rw-r--r--   0        0        0      689 2023-05-10 07:50:35.708217 neptune-1.2.0/src/neptune/internal/exceptions.py
--rw-r--r--   0        0        0      596 2023-05-10 07:50:35.708217 neptune-1.2.0/src/neptune/internal/hardware/__init__.py
--rw-r--r--   0        0        0      596 2023-05-10 07:50:35.708217 neptune-1.2.0/src/neptune/internal/hardware/gpu/__init__.py
--rw-r--r--   0        0        0     2466 2023-05-10 07:50:35.708217 neptune-1.2.0/src/neptune/internal/hardware/gpu/gpu_monitor.py
--rw-r--r--   0        0        0     4997 2023-05-10 07:50:35.708217 neptune-1.2.0/src/neptune/internal/hardware/hardware_metric_reporting_job.py
--rw-r--r--   0        0        0      933 2023-05-10 07:50:35.708217 neptune-1.2.0/src/neptune/internal/id_formats.py
--rw-r--r--   0        0        0      596 2023-05-10 07:50:35.708217 neptune-1.2.0/src/neptune/internal/init/__init__.py
--rw-r--r--   0        0        0      796 2023-05-10 07:50:35.708217 neptune-1.2.0/src/neptune/internal/init/parameters.py
--rw-r--r--   0        0        0      596 2023-05-10 07:50:35.708217 neptune-1.2.0/src/neptune/internal/notebooks/__init__.py
--rw-r--r--   0        0        0     1572 2023-05-10 07:50:35.708217 neptune-1.2.0/src/neptune/internal/notebooks/comm.py
--rw-r--r--   0        0        0     1831 2023-05-10 07:50:35.708217 neptune-1.2.0/src/neptune/internal/notebooks/notebooks.py
--rw-r--r--   0        0        0    17310 2023-05-10 07:50:35.708217 neptune-1.2.0/src/neptune/internal/operation.py
--rw-r--r--   0        0        0      596 2023-05-10 07:50:35.708217 neptune-1.2.0/src/neptune/internal/operation_processors/__init__.py
--rw-r--r--   0        0        0    10851 2023-05-10 07:50:35.708217 neptune-1.2.0/src/neptune/internal/operation_processors/async_operation_processor.py
--rw-r--r--   0        0        0     2177 2023-05-10 07:50:35.708217 neptune-1.2.0/src/neptune/internal/operation_processors/factory.py
--rw-r--r--   0        0        0     2136 2023-05-10 07:50:35.708217 neptune-1.2.0/src/neptune/internal/operation_processors/offline_operation_processor.py
--rw-r--r--   0        0        0     1140 2023-05-10 07:50:35.708217 neptune-1.2.0/src/neptune/internal/operation_processors/operation_processor.py
--rw-r--r--   0        0        0     1998 2023-05-10 07:50:35.708217 neptune-1.2.0/src/neptune/internal/operation_processors/operation_storage.py
--rw-r--r--   0        0        0     1577 2023-05-10 07:50:35.708217 neptune-1.2.0/src/neptune/internal/operation_processors/read_only_operation_processor.py
--rw-r--r--   0        0        0     2483 2023-05-10 07:50:35.708217 neptune-1.2.0/src/neptune/internal/operation_processors/sync_operation_processor.py
--rw-r--r--   0        0        0     3724 2023-05-10 07:50:35.708217 neptune-1.2.0/src/neptune/internal/operation_visitor.py
--rw-r--r--   0        0        0      776 2023-05-10 07:50:35.708217 neptune-1.2.0/src/neptune/internal/state.py
--rw-r--r--   0        0        0      596 2023-05-10 07:50:35.708217 neptune-1.2.0/src/neptune/internal/streams/__init__.py
--rw-r--r--   0        0        0     1815 2023-05-10 07:50:35.708217 neptune-1.2.0/src/neptune/internal/streams/std_capture_background_job.py
--rw-r--r--   0        0        0     2418 2023-05-10 07:50:35.708217 neptune-1.2.0/src/neptune/internal/streams/std_stream_capture_logger.py
--rw-r--r--   0        0        0      596 2023-05-10 07:50:35.708217 neptune-1.2.0/src/neptune/internal/threading/__init__.py
--rw-r--r--   0        0        0     3567 2023-05-10 07:50:35.708217 neptune-1.2.0/src/neptune/internal/threading/daemon.py
--rw-r--r--   0        0        0      596 2023-05-10 07:50:35.708217 neptune-1.2.0/src/neptune/internal/types/__init__.py
--rw-r--r--   0        0        0     4584 2023-05-10 07:50:35.708217 neptune-1.2.0/src/neptune/internal/types/file_types.py
--rw-r--r--   0        0        0     1665 2023-05-10 07:50:35.708217 neptune-1.2.0/src/neptune/internal/types/stringify_value.py
--rw-r--r--   0        0        0     4856 2023-05-10 07:50:35.708217 neptune-1.2.0/src/neptune/internal/utils/__init__.py
--rw-r--r--   0        0        0     2114 2023-05-10 07:50:35.708217 neptune-1.2.0/src/neptune/internal/utils/deprecation.py
--rw-r--r--   0        0        0     2374 2023-05-10 07:50:35.708217 neptune-1.2.0/src/neptune/internal/utils/generic_attribute_mapper.py
--rw-r--r--   0        0        0     2568 2023-05-10 07:50:35.708217 neptune-1.2.0/src/neptune/internal/utils/git.py
--rw-r--r--   0        0        0      849 2023-05-10 07:50:35.708217 neptune-1.2.0/src/neptune/internal/utils/hashing.py
--rw-r--r--   0        0        0     9732 2023-05-10 07:50:35.708217 neptune-1.2.0/src/neptune/internal/utils/images.py
--rw-r--r--   0        0        0     1288 2023-05-10 07:50:35.708217 neptune-1.2.0/src/neptune/internal/utils/iteration.py
--rw-r--r--   0        0        0     3053 2023-05-10 07:50:35.708217 neptune-1.2.0/src/neptune/internal/utils/json_file_splitter.py
--rw-r--r--   0        0        0     1633 2023-05-10 07:50:35.708217 neptune-1.2.0/src/neptune/internal/utils/limits.py
--rw-r--r--   0        0        0     1488 2023-05-10 07:50:35.708217 neptune-1.2.0/src/neptune/internal/utils/logger.py
--rw-r--r--   0        0        0     1042 2023-05-10 07:50:35.708217 neptune-1.2.0/src/neptune/internal/utils/paths.py
--rw-r--r--   0        0        0     2049 2023-05-10 07:50:35.708217 neptune-1.2.0/src/neptune/internal/utils/ping_background_job.py
--rw-r--r--   0        0        0     1809 2023-05-10 07:50:35.708217 neptune-1.2.0/src/neptune/internal/utils/process_killer.py
--rw-r--r--   0        0        0     1564 2023-05-10 07:50:35.708217 neptune-1.2.0/src/neptune/internal/utils/run_state.py
--rw-r--r--   0        0        0     1207 2023-05-10 07:50:35.708217 neptune-1.2.0/src/neptune/internal/utils/runningmode.py
--rw-r--r--   0        0        0     1340 2023-05-10 07:50:35.708217 neptune-1.2.0/src/neptune/internal/utils/s3.py
--rw-r--r--   0        0        0     2270 2023-05-10 07:50:35.708217 neptune-1.2.0/src/neptune/internal/utils/source_code.py
--rw-r--r--   0        0        0     1457 2023-05-10 07:50:35.708217 neptune-1.2.0/src/neptune/internal/utils/sync_offset_file.py
--rw-r--r--   0        0        0     1927 2023-05-10 07:50:35.708217 neptune-1.2.0/src/neptune/internal/utils/traceback_job.py
--rw-r--r--   0        0        0     2426 2023-05-10 07:50:35.708217 neptune-1.2.0/src/neptune/internal/utils/uncaught_exception_handler.py
--rw-r--r--   0        0        0     4462 2023-05-10 07:50:35.708217 neptune-1.2.0/src/neptune/internal/value_to_attribute_visitor.py
--rw-r--r--   0        0        0      596 2023-05-10 07:50:35.708217 neptune-1.2.0/src/neptune/internal/websockets/__init__.py
--rw-r--r--   0        0        0     5188 2023-05-10 07:50:35.708217 neptune-1.2.0/src/neptune/internal/websockets/websocket_signals_background_job.py
--rw-r--r--   0        0        0     1229 2023-05-10 07:50:35.708217 neptune-1.2.0/src/neptune/internal/websockets/websockets_factory.py
--rw-r--r--   0        0        0    13821 2023-05-10 07:50:35.708217 neptune-1.2.0/src/neptune/legacy/__init__.py
--rw-r--r--   0        0        0    11218 2023-05-10 07:50:35.708217 neptune-1.2.0/src/neptune/legacy/api_exceptions.py
--rw-r--r--   0        0        0     4710 2023-05-10 07:50:35.708217 neptune-1.2.0/src/neptune/legacy/backend.py
--rw-r--r--   0        0        0      737 2023-05-10 07:50:35.708217 neptune-1.2.0/src/neptune/legacy/checkpoint.py
--rw-r--r--   0        0        0      859 2023-05-10 07:50:35.708217 neptune-1.2.0/src/neptune/legacy/constants.py
--rw-r--r--   0        0        0      860 2023-05-10 07:50:35.708217 neptune-1.2.0/src/neptune/legacy/envs.py
--rw-r--r--   0        0        0    12780 2023-05-10 07:50:35.708217 neptune-1.2.0/src/neptune/legacy/exceptions.py
--rw-r--r--   0        0        0    42888 2023-05-10 07:50:35.712218 neptune-1.2.0/src/neptune/legacy/experiments.py
--rw-r--r--   0        0        0      663 2023-05-10 07:50:35.712218 neptune-1.2.0/src/neptune/legacy/git_info.py
--rw-r--r--   0        0        0      596 2023-05-10 07:50:35.712218 neptune-1.2.0/src/neptune/legacy/internal/__init__.py
--rw-r--r--   0        0        0     1999 2023-05-10 07:50:35.712218 neptune-1.2.0/src/neptune/legacy/internal/abort.py
--rw-r--r--   0        0        0      888 2023-05-10 07:50:35.712218 neptune-1.2.0/src/neptune/legacy/internal/api_clients/__init__.py
--rw-r--r--   0        0        0     1148 2023-05-10 07:50:35.712218 neptune-1.2.0/src/neptune/legacy/internal/api_clients/backend_factory.py
--rw-r--r--   0        0        0     1826 2023-05-10 07:50:35.712218 neptune-1.2.0/src/neptune/legacy/internal/api_clients/client_config.py
--rw-r--r--   0        0        0     3103 2023-05-10 07:50:35.712218 neptune-1.2.0/src/neptune/legacy/internal/api_clients/credentials.py
--rw-r--r--   0        0        0      596 2023-05-10 07:50:35.712218 neptune-1.2.0/src/neptune/legacy/internal/api_clients/hosted_api_clients/__init__.py
--rw-r--r--   0        0        0    46556 2023-05-10 07:50:35.712218 neptune-1.2.0/src/neptune/legacy/internal/api_clients/hosted_api_clients/hosted_alpha_leaderboard_api_client.py
--rw-r--r--   0        0        0     8710 2023-05-10 07:50:35.712218 neptune-1.2.0/src/neptune/legacy/internal/api_clients/hosted_api_clients/hosted_backend_api_client.py
--rw-r--r--   0        0        0     4456 2023-05-10 07:50:35.712218 neptune-1.2.0/src/neptune/legacy/internal/api_clients/hosted_api_clients/mixins.py
--rw-r--r--   0        0        0     3857 2023-05-10 07:50:35.712218 neptune-1.2.0/src/neptune/legacy/internal/api_clients/hosted_api_clients/utils.py
--rw-r--r--   0        0        0     4631 2023-05-10 07:50:35.712218 neptune-1.2.0/src/neptune/legacy/internal/api_clients/offline_backend.py
--rw-r--r--   0        0        0      596 2023-05-10 07:50:35.712218 neptune-1.2.0/src/neptune/legacy/internal/backends/__init__.py
--rw-r--r--   0        0        0      776 2023-05-10 07:50:35.712218 neptune-1.2.0/src/neptune/legacy/internal/backends/hosted_neptune_backend.py
--rw-r--r--   0        0        0      596 2023-05-10 07:50:35.712218 neptune-1.2.0/src/neptune/legacy/internal/channels/__init__.py
--rw-r--r--   0        0        0     3903 2023-05-10 07:50:35.712218 neptune-1.2.0/src/neptune/legacy/internal/channels/channels.py
--rw-r--r--   0        0        0     7087 2023-05-10 07:50:35.712218 neptune-1.2.0/src/neptune/legacy/internal/channels/channels_values_sender.py
--rw-r--r--   0        0        0      596 2023-05-10 07:50:35.712218 neptune-1.2.0/src/neptune/legacy/internal/execution/__init__.py
--rw-r--r--   0        0        0     6126 2023-05-10 07:50:35.712218 neptune-1.2.0/src/neptune/legacy/internal/execution/execution_context.py
--rw-r--r--   0        0        0      596 2023-05-10 07:50:35.712218 neptune-1.2.0/src/neptune/legacy/internal/experiments/__init__.py
--rw-r--r--   0        0        0      596 2023-05-10 07:50:35.712218 neptune-1.2.0/src/neptune/legacy/internal/notebooks/__init__.py
--rw-r--r--   0        0        0     1510 2023-05-10 07:50:35.712218 neptune-1.2.0/src/neptune/legacy/internal/notebooks/comm.py
--rw-r--r--   0        0        0     1711 2023-05-10 07:50:35.712218 neptune-1.2.0/src/neptune/legacy/internal/notebooks/notebooks.py
--rw-r--r--   0        0        0      596 2023-05-10 07:50:35.712218 neptune-1.2.0/src/neptune/legacy/internal/streams/__init__.py
--rw-r--r--   0        0        0     2805 2023-05-10 07:50:35.712218 neptune-1.2.0/src/neptune/legacy/internal/streams/channel_writer.py
--rw-r--r--   0        0        0     1945 2023-05-10 07:50:35.712218 neptune-1.2.0/src/neptune/legacy/internal/streams/stdstream_uploader.py
--rw-r--r--   0        0        0      596 2023-05-10 07:50:35.712218 neptune-1.2.0/src/neptune/legacy/internal/threads/__init__.py
--rw-r--r--   0        0        0     2363 2023-05-10 07:50:35.712218 neptune-1.2.0/src/neptune/legacy/internal/threads/aborting_thread.py
--rw-r--r--   0        0        0     1816 2023-05-10 07:50:35.712218 neptune-1.2.0/src/neptune/legacy/internal/threads/hardware_metric_reporting_thread.py
--rw-r--r--   0        0        0     1334 2023-05-10 07:50:35.712218 neptune-1.2.0/src/neptune/legacy/internal/threads/neptune_thread.py
--rw-r--r--   0        0        0     1556 2023-05-10 07:50:35.712218 neptune-1.2.0/src/neptune/legacy/internal/threads/ping_thread.py
--rw-r--r--   0        0        0      596 2023-05-10 07:50:35.712218 neptune-1.2.0/src/neptune/legacy/internal/utils/__init__.py
--rw-r--r--   0        0        0     8091 2023-05-10 07:50:35.712218 neptune-1.2.0/src/neptune/legacy/internal/utils/alpha_integration.py
--rw-r--r--   0        0        0      997 2023-05-10 07:50:35.712218 neptune-1.2.0/src/neptune/legacy/internal/utils/deprecation.py
--rw-r--r--   0        0        0     2597 2023-05-10 07:50:35.712218 neptune-1.2.0/src/neptune/legacy/internal/utils/http.py
--rw-r--r--   0        0        0     2597 2023-05-10 07:50:35.712218 neptune-1.2.0/src/neptune/legacy/internal/utils/http_utils.py
--rw-r--r--   0        0        0     2990 2023-05-10 07:50:35.712218 neptune-1.2.0/src/neptune/legacy/internal/utils/image.py
--rw-r--r--   0        0        0     3145 2023-05-10 07:50:35.712218 neptune-1.2.0/src/neptune/legacy/internal/utils/source_code.py
--rw-r--r--   0        0        0      596 2023-05-10 07:50:35.712218 neptune-1.2.0/src/neptune/legacy/internal/websockets/__init__.py
--rw-r--r--   0        0        0     3542 2023-05-10 07:50:35.712218 neptune-1.2.0/src/neptune/legacy/internal/websockets/message.py
--rw-r--r--   0        0        0     1097 2023-05-10 07:50:35.712218 neptune-1.2.0/src/neptune/legacy/internal/websockets/reconnecting_websocket_factory.py
--rw-r--r--   0        0        0     1228 2023-05-10 07:50:35.712218 neptune-1.2.0/src/neptune/legacy/internal/websockets/websocket_message_processor.py
--rw-r--r--   0        0        0     3938 2023-05-10 07:50:35.712218 neptune-1.2.0/src/neptune/legacy/model.py
--rw-r--r--   0        0        0     2807 2023-05-10 07:50:35.712218 neptune-1.2.0/src/neptune/legacy/notebook.py
--rw-r--r--   0        0        0      691 2023-05-10 07:50:35.712218 neptune-1.2.0/src/neptune/legacy/oauth.py
--rw-r--r--   0        0        0      678 2023-05-10 07:50:35.712218 neptune-1.2.0/src/neptune/legacy/patterns.py
--rw-r--r--   0        0        0    26377 2023-05-10 07:50:35.712218 neptune-1.2.0/src/neptune/legacy/projects.py
--rw-r--r--   0        0        0     8992 2023-05-10 07:50:35.712218 neptune-1.2.0/src/neptune/legacy/sessions.py
--rw-r--r--   0        0        0     1162 2023-05-10 07:50:35.712218 neptune-1.2.0/src/neptune/legacy/utils.py
--rw-r--r--   0        0        0      660 2023-05-10 07:50:35.712218 neptune-1.2.0/src/neptune/logging/__init__.py
--rw-r--r--   0        0        0      976 2023-05-10 07:50:35.712218 neptune-1.2.0/src/neptune/logging/logger.py
--rw-r--r--   0        0        0     4454 2023-05-10 07:50:35.716218 neptune-1.2.0/src/neptune/management/__init__.py
--rw-r--r--   0        0        0     5669 2023-05-10 07:50:35.716218 neptune-1.2.0/src/neptune/management/exceptions.py
--rw-r--r--   0        0        0      596 2023-05-10 07:50:35.716218 neptune-1.2.0/src/neptune/management/internal/__init__.py
--rw-r--r--   0        0        0    37199 2023-05-10 07:50:35.716218 neptune-1.2.0/src/neptune/management/internal/api.py
--rw-r--r--   0        0        0     2853 2023-05-10 07:50:35.716218 neptune-1.2.0/src/neptune/management/internal/dto.py
--rw-r--r--   0        0        0     1069 2023-05-10 07:50:35.716218 neptune-1.2.0/src/neptune/management/internal/types.py
--rw-r--r--   0        0        0     2013 2023-05-10 07:50:35.716218 neptune-1.2.0/src/neptune/management/internal/utils.py
--rw-r--r--   0        0        0      995 2023-05-10 07:50:35.716218 neptune-1.2.0/src/neptune/metadata_containers/__init__.py
--rw-r--r--   0        0        0     2063 2023-05-10 07:50:35.716218 neptune-1.2.0/src/neptune/metadata_containers/abstract.py
--rw-r--r--   0        0        0    20007 2023-05-10 07:50:35.716218 neptune-1.2.0/src/neptune/metadata_containers/metadata_container.py
--rw-r--r--   0        0        0     9194 2023-05-10 07:50:35.716218 neptune-1.2.0/src/neptune/metadata_containers/metadata_containers_table.py
--rw-r--r--   0        0        0    12337 2023-05-10 07:50:35.716218 neptune-1.2.0/src/neptune/metadata_containers/model.py
--rw-r--r--   0        0        0    11428 2023-05-10 07:50:35.716218 neptune-1.2.0/src/neptune/metadata_containers/model_version.py
--rw-r--r--   0        0        0    15433 2023-05-10 07:50:35.716218 neptune-1.2.0/src/neptune/metadata_containers/project.py
--rw-r--r--   0        0        0    22678 2023-05-10 07:50:35.716218 neptune-1.2.0/src/neptune/metadata_containers/run.py
--rw-r--r--   0        0        0     2606 2023-05-10 07:50:35.716218 neptune-1.2.0/src/neptune/new/__init__.py
--rw-r--r--   0        0        0     1476 2023-05-10 07:50:35.716218 neptune-1.2.0/src/neptune/new/_compatibility.py
--rw-r--r--   0        0        0      974 2023-05-10 07:50:35.716218 neptune-1.2.0/src/neptune/new/constants.py
--rw-r--r--   0        0        0     1378 2023-05-10 07:50:35.716218 neptune-1.2.0/src/neptune/new/envs.py
--rw-r--r--   0        0        0     5846 2023-05-10 07:50:35.716218 neptune-1.2.0/src/neptune/new/exceptions.py
--rw-r--r--   0        0        0      655 2023-05-10 07:50:35.716218 neptune-1.2.0/src/neptune/new/handler.py
--rw-r--r--   0        0        0      694 2023-05-10 07:50:35.716218 neptune-1.2.0/src/neptune/new/project.py
--rw-r--r--   0        0        0     1672 2023-05-10 07:50:35.716218 neptune-1.2.0/src/neptune/new/run.py
--rw-r--r--   0        0        0     1426 2023-05-10 07:50:35.716218 neptune-1.2.0/src/neptune/new/runs_table.py
--rw-r--r--   0        0        0      681 2023-05-10 07:50:35.716218 neptune-1.2.0/src/neptune/new/utils.py
--rw-r--r--   0        0        0      696 2023-05-10 07:50:35.716218 neptune-1.2.0/src/neptune/new/version.py
--rw-r--r--   0        0        0     1071 2023-05-10 07:50:35.716218 neptune-1.2.0/src/neptune/types/__init__.py
--rw-r--r--   0        0        0      914 2023-05-10 07:50:35.716218 neptune-1.2.0/src/neptune/types/atoms/__init__.py
--rw-r--r--   0        0        0     1626 2023-05-10 07:50:35.716218 neptune-1.2.0/src/neptune/types/atoms/artifact.py
--rw-r--r--   0        0        0      936 2023-05-10 07:50:35.716218 neptune-1.2.0/src/neptune/types/atoms/atom.py
--rw-r--r--   0        0        0     1302 2023-05-10 07:50:35.716218 neptune-1.2.0/src/neptune/types/atoms/boolean.py
--rw-r--r--   0        0        0     1435 2023-05-10 07:50:35.716218 neptune-1.2.0/src/neptune/types/atoms/datetime.py
--rw-r--r--   0        0        0    11695 2023-05-10 07:50:35.716218 neptune-1.2.0/src/neptune/types/atoms/file.py
--rw-r--r--   0        0        0     1297 2023-05-10 07:50:35.716218 neptune-1.2.0/src/neptune/types/atoms/float.py
--rw-r--r--   0        0        0     1902 2023-05-10 07:50:35.716218 neptune-1.2.0/src/neptune/types/atoms/git_ref.py
--rw-r--r--   0        0        0     1299 2023-05-10 07:50:35.716218 neptune-1.2.0/src/neptune/types/atoms/integer.py
--rw-r--r--   0        0        0     1473 2023-05-10 07:50:35.716218 neptune-1.2.0/src/neptune/types/atoms/string.py
--rw-r--r--   0        0        0     1485 2023-05-10 07:50:35.716218 neptune-1.2.0/src/neptune/types/file_set.py
--rw-r--r--   0        0        0      831 2023-05-10 07:50:35.716218 neptune-1.2.0/src/neptune/types/mode.py
--rw-r--r--   0        0        0      777 2023-05-10 07:50:35.716218 neptune-1.2.0/src/neptune/types/model_version_stage.py
--rw-r--r--   0        0        0     1144 2023-05-10 07:50:35.716218 neptune-1.2.0/src/neptune/types/namespace.py
--rw-r--r--   0        0        0      783 2023-05-10 07:50:35.716218 neptune-1.2.0/src/neptune/types/series/__init__.py
--rw-r--r--   0        0        0     2447 2023-05-10 07:50:35.716218 neptune-1.2.0/src/neptune/types/series/file_series.py
--rw-r--r--   0        0        0     2553 2023-05-10 07:50:35.716218 neptune-1.2.0/src/neptune/types/series/float_series.py
--rw-r--r--   0        0        0     1221 2023-05-10 07:50:35.716218 neptune-1.2.0/src/neptune/types/series/series.py
--rw-r--r--   0        0        0     1353 2023-05-10 07:50:35.716218 neptune-1.2.0/src/neptune/types/series/series_value.py
--rw-r--r--   0        0        0     2601 2023-05-10 07:50:35.716218 neptune-1.2.0/src/neptune/types/series/string_series.py
--rw-r--r--   0        0        0      655 2023-05-10 07:50:35.716218 neptune-1.2.0/src/neptune/types/sets/__init__.py
--rw-r--r--   0        0        0      934 2023-05-10 07:50:35.716218 neptune-1.2.0/src/neptune/types/sets/set.py
--rw-r--r--   0        0        0     1119 2023-05-10 07:50:35.716218 neptune-1.2.0/src/neptune/types/sets/string_set.py
--rw-r--r--   0        0        0     3551 2023-05-10 07:50:35.716218 neptune-1.2.0/src/neptune/types/type_casting.py
--rw-r--r--   0        0        0      892 2023-05-10 07:50:35.716218 neptune-1.2.0/src/neptune/types/value.py
--rw-r--r--   0        0        0     1634 2023-05-10 07:50:35.716218 neptune-1.2.0/src/neptune/types/value_copy.py
--rw-r--r--   0        0        0     2596 2023-05-10 07:50:35.716218 neptune-1.2.0/src/neptune/types/value_visitor.py
--rw-r--r--   0        0        0      698 2023-05-10 07:50:35.716218 neptune-1.2.0/src/neptune/typing.py
--rw-r--r--   0        0        0     1755 2023-05-10 07:50:35.716218 neptune-1.2.0/src/neptune/utils.py
--rw-r--r--   0        0        0        0 2023-05-10 07:50:35.716218 neptune-1.2.0/src/neptune/vendor/__init__.py
--rw-r--r--   0        0        0     6306 2023-05-10 07:50:35.716218 neptune-1.2.0/src/neptune/vendor/lib_programname.py
--rw-r--r--   0        0        0    68552 2023-05-10 07:50:35.716218 neptune-1.2.0/src/neptune/vendor/pynvml.py
--rw-r--r--   0        0        0     2228 2023-05-10 07:50:35.716218 neptune-1.2.0/src/neptune/version.py
--rw-r--r--   0        0        0    18705 1970-01-01 00:00:00.000000 neptune-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0    25669 2023-06-15 14:47:17.283504 neptune-1.3.0/CHANGELOG.md
+-rw-r--r--   0        0        0    11357 2023-06-15 14:47:17.283504 neptune-1.3.0/LICENSE
+-rw-r--r--   0        0        0    14357 2023-06-15 14:47:17.283504 neptune-1.3.0/README.md
+-rw-r--r--   0        0        0     5399 2023-06-15 14:47:35.703645 neptune-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3532 2023-06-15 14:47:17.287504 neptune-1.3.0/src/neptune/__init__.py
+-rw-r--r--   0        0        0     1218 2023-06-15 14:47:17.287504 neptune-1.3.0/src/neptune/attributes/__init__.py
+-rw-r--r--   0        0        0     1011 2023-06-15 14:47:17.287504 neptune-1.3.0/src/neptune/attributes/atoms/__init__.py
+-rw-r--r--   0        0        0     3048 2023-06-15 14:47:17.287504 neptune-1.3.0/src/neptune/attributes/atoms/artifact.py
+-rw-r--r--   0        0        0      701 2023-06-15 14:47:17.287504 neptune-1.3.0/src/neptune/attributes/atoms/atom.py
+-rw-r--r--   0        0        0     1709 2023-06-15 14:47:17.287504 neptune-1.3.0/src/neptune/attributes/atoms/boolean.py
+-rw-r--r--   0        0        0     2121 2023-06-15 14:47:17.287504 neptune-1.3.0/src/neptune/attributes/atoms/copiable_atom.py
+-rw-r--r--   0        0        0     2075 2023-06-15 14:47:17.287504 neptune-1.3.0/src/neptune/attributes/atoms/datetime.py
+-rw-r--r--   0        0        0     1788 2023-06-15 14:47:17.287504 neptune-1.3.0/src/neptune/attributes/atoms/file.py
+-rw-r--r--   0        0        0     1704 2023-06-15 14:47:17.287504 neptune-1.3.0/src/neptune/attributes/atoms/float.py
+-rw-r--r--   0        0        0      696 2023-06-15 14:47:17.287504 neptune-1.3.0/src/neptune/attributes/atoms/git_ref.py
+-rw-r--r--   0        0        0     2395 2023-06-15 14:47:17.287504 neptune-1.3.0/src/neptune/attributes/atoms/integer.py
+-rw-r--r--   0        0        0      707 2023-06-15 14:47:17.287504 neptune-1.3.0/src/neptune/attributes/atoms/notebook_ref.py
+-rw-r--r--   0        0        0      700 2023-06-15 14:47:17.287504 neptune-1.3.0/src/neptune/attributes/atoms/run_state.py
+-rw-r--r--   0        0        0     2658 2023-06-15 14:47:17.287504 neptune-1.3.0/src/neptune/attributes/atoms/string.py
+-rw-r--r--   0        0        0     2159 2023-06-15 14:47:17.287504 neptune-1.3.0/src/neptune/attributes/attribute.py
+-rw-r--r--   0        0        0     2723 2023-06-15 14:47:17.287504 neptune-1.3.0/src/neptune/attributes/constants.py
+-rw-r--r--   0        0        0     2642 2023-06-15 14:47:17.287504 neptune-1.3.0/src/neptune/attributes/file_set.py
+-rw-r--r--   0        0        0     4266 2023-06-15 14:47:17.287504 neptune-1.3.0/src/neptune/attributes/namespace.py
+-rw-r--r--   0        0        0      782 2023-06-15 14:47:17.287504 neptune-1.3.0/src/neptune/attributes/series/__init__.py
+-rw-r--r--   0        0        0     1949 2023-06-15 14:47:17.287504 neptune-1.3.0/src/neptune/attributes/series/fetchable_series.py
+-rw-r--r--   0        0        0     4292 2023-06-15 14:47:17.287504 neptune-1.3.0/src/neptune/attributes/series/file_series.py
+-rw-r--r--   0        0        0     2656 2023-06-15 14:47:17.287504 neptune-1.3.0/src/neptune/attributes/series/float_series.py
+-rw-r--r--   0        0        0     6003 2023-06-15 14:47:17.287504 neptune-1.3.0/src/neptune/attributes/series/series.py
+-rw-r--r--   0        0        0     3498 2023-06-15 14:47:17.287504 neptune-1.3.0/src/neptune/attributes/series/string_series.py
+-rw-r--r--   0        0        0      662 2023-06-15 14:47:17.287504 neptune-1.3.0/src/neptune/attributes/sets/__init__.py
+-rw-r--r--   0        0        0      699 2023-06-15 14:47:17.287504 neptune-1.3.0/src/neptune/attributes/sets/set.py
+-rw-r--r--   0        0        0     2627 2023-06-15 14:47:17.287504 neptune-1.3.0/src/neptune/attributes/sets/string_set.py
+-rw-r--r--   0        0        0     2157 2023-06-15 14:47:17.287504 neptune-1.3.0/src/neptune/attributes/utils.py
+-rw-r--r--   0        0        0      686 2023-06-15 14:47:17.287504 neptune-1.3.0/src/neptune/cli/__init__.py
+-rw-r--r--   0        0        0     1017 2023-06-15 14:47:17.287504 neptune-1.3.0/src/neptune/cli/__main__.py
+-rw-r--r--   0        0        0      866 2023-06-15 14:47:17.287504 neptune-1.3.0/src/neptune/cli/abstract_backend_runner.py
+-rw-r--r--   0        0        0     3436 2023-06-15 14:47:17.287504 neptune-1.3.0/src/neptune/cli/clear.py
+-rw-r--r--   0        0        0     5574 2023-06-15 14:47:17.287504 neptune-1.3.0/src/neptune/cli/commands.py
+-rw-r--r--   0        0        0     2814 2023-06-15 14:47:17.287504 neptune-1.3.0/src/neptune/cli/container_manager.py
+-rw-r--r--   0        0        0     1947 2023-06-15 14:47:17.287504 neptune-1.3.0/src/neptune/cli/path_option.py
+-rw-r--r--   0        0        0     3899 2023-06-15 14:47:17.287504 neptune-1.3.0/src/neptune/cli/status.py
+-rw-r--r--   0        0        0     9995 2023-06-15 14:47:17.287504 neptune-1.3.0/src/neptune/cli/sync.py
+-rw-r--r--   0        0        0     5028 2023-06-15 14:47:17.287504 neptune-1.3.0/src/neptune/cli/utils.py
+-rw-r--r--   0        0        0      596 2023-06-15 14:47:17.287504 neptune-1.3.0/src/neptune/common/__init__.py
+-rw-r--r--   0        0        0      596 2023-06-15 14:47:17.287504 neptune-1.3.0/src/neptune/common/backends/__init__.py
+-rw-r--r--   0        0        0     1038 2023-06-15 14:47:17.287504 neptune-1.3.0/src/neptune/common/backends/api_model.py
+-rw-r--r--   0        0        0     4230 2023-06-15 14:47:17.287504 neptune-1.3.0/src/neptune/common/backends/utils.py
+-rw-r--r--   0        0        0      859 2023-06-15 14:47:17.287504 neptune-1.3.0/src/neptune/common/envs.py
+-rw-r--r--   0        0        0    14106 2023-06-15 14:47:17.287504 neptune-1.3.0/src/neptune/common/exceptions.py
+-rw-r--r--   0        0        0      629 2023-06-15 14:47:17.287504 neptune-1.3.0/src/neptune/common/experiments.py
+-rw-r--r--   0        0        0     2490 2023-06-15 14:47:17.287504 neptune-1.3.0/src/neptune/common/git_info.py
+-rw-r--r--   0        0        0      596 2023-06-15 14:47:17.291504 neptune-1.3.0/src/neptune/common/hardware/__init__.py
+-rw-r--r--   0        0        0      596 2023-06-15 14:47:17.291504 neptune-1.3.0/src/neptune/common/hardware/cgroup/__init__.py
+-rw-r--r--   0        0        0     2638 2023-06-15 14:47:17.291504 neptune-1.3.0/src/neptune/common/hardware/cgroup/cgroup_filesystem_reader.py
+-rw-r--r--   0        0        0     3212 2023-06-15 14:47:17.291504 neptune-1.3.0/src/neptune/common/hardware/cgroup/cgroup_monitor.py
+-rw-r--r--   0        0        0      694 2023-06-15 14:47:17.291504 neptune-1.3.0/src/neptune/common/hardware/constants.py
+-rw-r--r--   0        0        0      596 2023-06-15 14:47:17.291504 neptune-1.3.0/src/neptune/common/hardware/gauges/__init__.py
+-rw-r--r--   0        0        0     1554 2023-06-15 14:47:17.291504 neptune-1.3.0/src/neptune/common/hardware/gauges/cpu.py
+-rw-r--r--   0        0        0      979 2023-06-15 14:47:17.291504 neptune-1.3.0/src/neptune/common/hardware/gauges/gauge.py
+-rw-r--r--   0        0        0     2023 2023-06-15 14:47:17.291504 neptune-1.3.0/src/neptune/common/hardware/gauges/gauge_factory.py
+-rw-r--r--   0        0        0      667 2023-06-15 14:47:17.291504 neptune-1.3.0/src/neptune/common/hardware/gauges/gauge_mode.py
+-rw-r--r--   0        0        0     1766 2023-06-15 14:47:17.291504 neptune-1.3.0/src/neptune/common/hardware/gauges/gpu.py
+-rw-r--r--   0        0        0     1748 2023-06-15 14:47:17.291504 neptune-1.3.0/src/neptune/common/hardware/gauges/memory.py
+-rw-r--r--   0        0        0      596 2023-06-15 14:47:17.291504 neptune-1.3.0/src/neptune/common/hardware/gpu/__init__.py
+-rw-r--r--   0        0        0     2568 2023-06-15 14:47:17.291504 neptune-1.3.0/src/neptune/common/hardware/gpu/gpu_monitor.py
+-rw-r--r--   0        0        0      596 2023-06-15 14:47:17.291504 neptune-1.3.0/src/neptune/common/hardware/metrics/__init__.py
+-rw-r--r--   0        0        0     2432 2023-06-15 14:47:17.291504 neptune-1.3.0/src/neptune/common/hardware/metrics/metric.py
+-rw-r--r--   0        0        0     1216 2023-06-15 14:47:17.291504 neptune-1.3.0/src/neptune/common/hardware/metrics/metrics_container.py
+-rw-r--r--   0        0        0     3490 2023-06-15 14:47:17.291504 neptune-1.3.0/src/neptune/common/hardware/metrics/metrics_factory.py
+-rw-r--r--   0        0        0      596 2023-06-15 14:47:17.291504 neptune-1.3.0/src/neptune/common/hardware/metrics/reports/__init__.py
+-rw-r--r--   0        0        0      792 2023-06-15 14:47:17.291504 neptune-1.3.0/src/neptune/common/hardware/metrics/reports/metric_report.py
+-rw-r--r--   0        0        0     1679 2023-06-15 14:47:17.291504 neptune-1.3.0/src/neptune/common/hardware/metrics/reports/metric_reporter.py
+-rw-r--r--   0        0        0      947 2023-06-15 14:47:17.291504 neptune-1.3.0/src/neptune/common/hardware/metrics/reports/metric_reporter_factory.py
+-rw-r--r--   0        0        0      596 2023-06-15 14:47:17.291504 neptune-1.3.0/src/neptune/common/hardware/metrics/service/__init__.py
+-rw-r--r--   0        0        0     1106 2023-06-15 14:47:17.291504 neptune-1.3.0/src/neptune/common/hardware/metrics/service/metric_service.py
+-rw-r--r--   0        0        0     2309 2023-06-15 14:47:17.291504 neptune-1.3.0/src/neptune/common/hardware/metrics/service/metric_service_factory.py
+-rw-r--r--   0        0        0      596 2023-06-15 14:47:17.291504 neptune-1.3.0/src/neptune/common/hardware/resources/__init__.py
+-rw-r--r--   0        0        0     1821 2023-06-15 14:47:17.291504 neptune-1.3.0/src/neptune/common/hardware/resources/gpu_card_indices_provider.py
+-rw-r--r--   0        0        0     1574 2023-06-15 14:47:17.291504 neptune-1.3.0/src/neptune/common/hardware/resources/system_resource_info.py
+-rw-r--r--   0        0        0     2504 2023-06-15 14:47:17.291504 neptune-1.3.0/src/neptune/common/hardware/resources/system_resource_info_factory.py
+-rw-r--r--   0        0        0      596 2023-06-15 14:47:17.291504 neptune-1.3.0/src/neptune/common/hardware/system/__init__.py
+-rw-r--r--   0        0        0      964 2023-06-15 14:47:17.291504 neptune-1.3.0/src/neptune/common/hardware/system/system_monitor.py
+-rw-r--r--   0        0        0     4772 2023-06-15 14:47:17.291504 neptune-1.3.0/src/neptune/common/oauth.py
+-rw-r--r--   0        0        0      884 2023-06-15 14:47:17.291504 neptune-1.3.0/src/neptune/common/patches/__init__.py
+-rw-r--r--   0        0        0     2731 2023-06-15 14:47:17.291504 neptune-1.3.0/src/neptune/common/patches/bravado.py
+-rw-r--r--   0        0        0      726 2023-06-15 14:47:17.291504 neptune-1.3.0/src/neptune/common/patterns.py
+-rw-r--r--   0        0        0      596 2023-06-15 14:47:17.291504 neptune-1.3.0/src/neptune/common/storage/__init__.py
+-rw-r--r--   0        0        0     3223 2023-06-15 14:47:17.291504 neptune-1.3.0/src/neptune/common/storage/datastream.py
+-rw-r--r--   0        0        0     7335 2023-06-15 14:47:17.291504 neptune-1.3.0/src/neptune/common/storage/storage_utils.py
+-rw-r--r--   0        0        0     7075 2023-06-15 14:47:17.291504 neptune-1.3.0/src/neptune/common/utils.py
+-rw-r--r--   0        0        0     2206 2023-06-15 14:47:17.291504 neptune-1.3.0/src/neptune/common/warnings.py
+-rw-r--r--   0        0        0      596 2023-06-15 14:47:17.291504 neptune-1.3.0/src/neptune/common/websockets/__init__.py
+-rw-r--r--   0        0        0     3589 2023-06-15 14:47:17.291504 neptune-1.3.0/src/neptune/common/websockets/reconnecting_websocket.py
+-rw-r--r--   0        0        0     2693 2023-06-15 14:47:17.291504 neptune-1.3.0/src/neptune/common/websockets/websocket_client_adapter.py
+-rw-r--r--   0        0        0      985 2023-06-15 14:47:17.291504 neptune-1.3.0/src/neptune/constants.py
+-rw-r--r--   0        0        0     1863 2023-06-15 14:47:17.291504 neptune-1.3.0/src/neptune/envs.py
+-rw-r--r--   0        0        0    41966 2023-06-15 14:47:17.291504 neptune-1.3.0/src/neptune/exceptions.py
+-rw-r--r--   0        0        0    29698 2023-06-15 14:47:17.291504 neptune-1.3.0/src/neptune/handler.py
+-rw-r--r--   0        0        0      596 2023-06-15 14:47:17.291504 neptune-1.3.0/src/neptune/integrations/__init__.py
+-rw-r--r--   0        0        0      973 2023-06-15 14:47:17.291504 neptune-1.3.0/src/neptune/integrations/aws/__init__.py
+-rw-r--r--   0        0        0     1014 2023-06-15 14:47:17.291504 neptune-1.3.0/src/neptune/integrations/detectron2/__init__.py
+-rw-r--r--   0        0        0      985 2023-06-15 14:47:17.291504 neptune-1.3.0/src/neptune/integrations/fastai/__init__.py
+-rw-r--r--   0        0        0      976 2023-06-15 14:47:17.291504 neptune-1.3.0/src/neptune/integrations/kedro/__init__.py
+-rw-r--r--   0        0        0      993 2023-06-15 14:47:17.291504 neptune-1.3.0/src/neptune/integrations/lightgbm/__init__.py
+-rw-r--r--   0        0        0      985 2023-06-15 14:47:17.291504 neptune-1.3.0/src/neptune/integrations/optuna/__init__.py
+-rw-r--r--   0        0        0      989 2023-06-15 14:47:17.291504 neptune-1.3.0/src/neptune/integrations/prophet/__init__.py
+-rw-r--r--   0        0        0     3084 2023-06-15 14:47:17.291504 neptune-1.3.0/src/neptune/integrations/python_logger.py
+-rw-r--r--   0        0        0     1006 2023-06-15 14:47:17.291504 neptune-1.3.0/src/neptune/integrations/pytorch/__init__.py
+-rw-r--r--   0        0        0     1042 2023-06-15 14:47:17.291504 neptune-1.3.0/src/neptune/integrations/pytorch_lightning/__init__.py
+-rw-r--r--   0        0        0      985 2023-06-15 14:47:17.291504 neptune-1.3.0/src/neptune/integrations/sacred/__init__.py
+-rw-r--r--   0        0        0      989 2023-06-15 14:47:17.291504 neptune-1.3.0/src/neptune/integrations/sklearn/__init__.py
+-rw-r--r--   0        0        0     1038 2023-06-15 14:47:17.291504 neptune-1.3.0/src/neptune/integrations/tensorflow_keras/__init__.py
+-rw-r--r--   0        0        0     1032 2023-06-15 14:47:17.291504 neptune-1.3.0/src/neptune/integrations/transformers/__init__.py
+-rw-r--r--   0        0        0     1164 2023-06-15 14:47:17.295504 neptune-1.3.0/src/neptune/integrations/utils.py
+-rw-r--r--   0        0        0      989 2023-06-15 14:47:17.295504 neptune-1.3.0/src/neptune/integrations/xgboost/__init__.py
+-rw-r--r--   0        0        0      596 2023-06-15 14:47:17.295504 neptune-1.3.0/src/neptune/internal/__init__.py
+-rw-r--r--   0        0        0      760 2023-06-15 14:47:17.295504 neptune-1.3.0/src/neptune/internal/artifacts/__init__.py
+-rw-r--r--   0        0        0      791 2023-06-15 14:47:17.295504 neptune-1.3.0/src/neptune/internal/artifacts/drivers/__init__.py
+-rw-r--r--   0        0        0     4240 2023-06-15 14:47:17.295504 neptune-1.3.0/src/neptune/internal/artifacts/drivers/local.py
+-rw-r--r--   0        0        0     4810 2023-06-15 14:47:17.295504 neptune-1.3.0/src/neptune/internal/artifacts/drivers/s3.py
+-rw-r--r--   0        0        0     4017 2023-06-15 14:47:17.295504 neptune-1.3.0/src/neptune/internal/artifacts/file_hasher.py
+-rw-r--r--   0        0        0     2318 2023-06-15 14:47:17.295504 neptune-1.3.0/src/neptune/internal/artifacts/local_file_hash_storage.py
+-rw-r--r--   0        0        0     3578 2023-06-15 14:47:17.295504 neptune-1.3.0/src/neptune/internal/artifacts/types.py
+-rw-r--r--   0        0        0      999 2023-06-15 14:47:17.295504 neptune-1.3.0/src/neptune/internal/artifacts/utils.py
+-rw-r--r--   0        0        0      596 2023-06-15 14:47:17.295504 neptune-1.3.0/src/neptune/internal/backends/__init__.py
+-rw-r--r--   0        0        0     7169 2023-06-15 14:47:17.295504 neptune-1.3.0/src/neptune/internal/backends/api_model.py
+-rw-r--r--   0        0        0     1703 2023-06-15 14:47:17.295504 neptune-1.3.0/src/neptune/internal/backends/factory.py
+-rw-r--r--   0        0        0     6700 2023-06-15 14:47:17.295504 neptune-1.3.0/src/neptune/internal/backends/hosted_artifact_operations.py
+-rw-r--r--   0        0        0     5942 2023-06-15 14:47:17.295504 neptune-1.3.0/src/neptune/internal/backends/hosted_client.py
+-rw-r--r--   0        0        0    17136 2023-06-15 14:47:17.295504 neptune-1.3.0/src/neptune/internal/backends/hosted_file_operations.py
+-rw-r--r--   0        0        0    40705 2023-06-15 14:47:17.295504 neptune-1.3.0/src/neptune/internal/backends/hosted_neptune_backend.py
+-rw-r--r--   0        0        0     8506 2023-06-15 14:47:17.295504 neptune-1.3.0/src/neptune/internal/backends/neptune_backend.py
+-rw-r--r--   0        0        0    31714 2023-06-15 14:47:17.295504 neptune-1.3.0/src/neptune/internal/backends/neptune_backend_mock.py
+-rw-r--r--   0        0        0     1942 2023-06-15 14:47:17.295504 neptune-1.3.0/src/neptune/internal/backends/nql.py
+-rw-r--r--   0        0        0     4471 2023-06-15 14:47:17.295504 neptune-1.3.0/src/neptune/internal/backends/offline_neptune_backend.py
+-rw-r--r--   0        0        0     3946 2023-06-15 14:47:17.295504 neptune-1.3.0/src/neptune/internal/backends/operation_api_name_visitor.py
+-rw-r--r--   0        0        0     5003 2023-06-15 14:47:17.295504 neptune-1.3.0/src/neptune/internal/backends/operation_api_object_converter.py
+-rw-r--r--   0        0        0    13841 2023-06-15 14:47:17.295504 neptune-1.3.0/src/neptune/internal/backends/operations_preprocessor.py
+-rw-r--r--   0        0        0     1619 2023-06-15 14:47:17.295504 neptune-1.3.0/src/neptune/internal/backends/project_name_lookup.py
+-rw-r--r--   0        0        0     5246 2023-06-15 14:47:17.295504 neptune-1.3.0/src/neptune/internal/backends/swagger_client_wrapper.py
+-rw-r--r--   0        0        0     8765 2023-06-15 14:47:17.295504 neptune-1.3.0/src/neptune/internal/backends/utils.py
+-rw-r--r--   0        0        0     1381 2023-06-15 14:47:17.295504 neptune-1.3.0/src/neptune/internal/backgroud_job_list.py
+-rw-r--r--   0        0        0     1035 2023-06-15 14:47:17.295504 neptune-1.3.0/src/neptune/internal/background_job.py
+-rw-r--r--   0        0        0      350 2023-06-15 14:47:17.295504 neptune-1.3.0/src/neptune/internal/constants.py
+-rw-r--r--   0        0        0     4486 2023-06-15 14:47:17.295504 neptune-1.3.0/src/neptune/internal/container_structure.py
+-rw-r--r--   0        0        0     1302 2023-06-15 14:47:17.295504 neptune-1.3.0/src/neptune/internal/container_type.py
+-rw-r--r--   0        0        0     2345 2023-06-15 14:47:17.295504 neptune-1.3.0/src/neptune/internal/credentials.py
+-rw-r--r--   0        0        0     8468 2023-06-15 14:47:17.295504 neptune-1.3.0/src/neptune/internal/disk_queue.py
+-rw-r--r--   0        0        0      689 2023-06-15 14:47:17.295504 neptune-1.3.0/src/neptune/internal/exceptions.py
+-rw-r--r--   0        0        0      596 2023-06-15 14:47:17.295504 neptune-1.3.0/src/neptune/internal/hardware/__init__.py
+-rw-r--r--   0        0        0      596 2023-06-15 14:47:17.295504 neptune-1.3.0/src/neptune/internal/hardware/gpu/__init__.py
+-rw-r--r--   0        0        0     2466 2023-06-15 14:47:17.295504 neptune-1.3.0/src/neptune/internal/hardware/gpu/gpu_monitor.py
+-rw-r--r--   0        0        0     4997 2023-06-15 14:47:17.295504 neptune-1.3.0/src/neptune/internal/hardware/hardware_metric_reporting_job.py
+-rw-r--r--   0        0        0      933 2023-06-15 14:47:17.295504 neptune-1.3.0/src/neptune/internal/id_formats.py
+-rw-r--r--   0        0        0      596 2023-06-15 14:47:17.295504 neptune-1.3.0/src/neptune/internal/init/__init__.py
+-rw-r--r--   0        0        0      796 2023-06-15 14:47:17.295504 neptune-1.3.0/src/neptune/internal/init/parameters.py
+-rw-r--r--   0        0        0      596 2023-06-15 14:47:17.295504 neptune-1.3.0/src/neptune/internal/notebooks/__init__.py
+-rw-r--r--   0        0        0     1572 2023-06-15 14:47:17.295504 neptune-1.3.0/src/neptune/internal/notebooks/comm.py
+-rw-r--r--   0        0        0     1831 2023-06-15 14:47:17.295504 neptune-1.3.0/src/neptune/internal/notebooks/notebooks.py
+-rw-r--r--   0        0        0    17310 2023-06-15 14:47:17.295504 neptune-1.3.0/src/neptune/internal/operation.py
+-rw-r--r--   0        0        0      596 2023-06-15 14:47:17.295504 neptune-1.3.0/src/neptune/internal/operation_processors/__init__.py
+-rw-r--r--   0        0        0    10851 2023-06-15 14:47:17.295504 neptune-1.3.0/src/neptune/internal/operation_processors/async_operation_processor.py
+-rw-r--r--   0        0        0     2177 2023-06-15 14:47:17.295504 neptune-1.3.0/src/neptune/internal/operation_processors/factory.py
+-rw-r--r--   0        0        0     2136 2023-06-15 14:47:17.295504 neptune-1.3.0/src/neptune/internal/operation_processors/offline_operation_processor.py
+-rw-r--r--   0        0        0     1140 2023-06-15 14:47:17.295504 neptune-1.3.0/src/neptune/internal/operation_processors/operation_processor.py
+-rw-r--r--   0        0        0     1998 2023-06-15 14:47:17.295504 neptune-1.3.0/src/neptune/internal/operation_processors/operation_storage.py
+-rw-r--r--   0        0        0     1577 2023-06-15 14:47:17.295504 neptune-1.3.0/src/neptune/internal/operation_processors/read_only_operation_processor.py
+-rw-r--r--   0        0        0     2483 2023-06-15 14:47:17.295504 neptune-1.3.0/src/neptune/internal/operation_processors/sync_operation_processor.py
+-rw-r--r--   0        0        0     3724 2023-06-15 14:47:17.295504 neptune-1.3.0/src/neptune/internal/operation_visitor.py
+-rw-r--r--   0        0        0      776 2023-06-15 14:47:17.295504 neptune-1.3.0/src/neptune/internal/state.py
+-rw-r--r--   0        0        0      596 2023-06-15 14:47:17.295504 neptune-1.3.0/src/neptune/internal/streams/__init__.py
+-rw-r--r--   0        0        0     1815 2023-06-15 14:47:17.295504 neptune-1.3.0/src/neptune/internal/streams/std_capture_background_job.py
+-rw-r--r--   0        0        0     2418 2023-06-15 14:47:17.295504 neptune-1.3.0/src/neptune/internal/streams/std_stream_capture_logger.py
+-rw-r--r--   0        0        0      596 2023-06-15 14:47:17.295504 neptune-1.3.0/src/neptune/internal/threading/__init__.py
+-rw-r--r--   0        0        0     3567 2023-06-15 14:47:17.295504 neptune-1.3.0/src/neptune/internal/threading/daemon.py
+-rw-r--r--   0        0        0      596 2023-06-15 14:47:17.295504 neptune-1.3.0/src/neptune/internal/types/__init__.py
+-rw-r--r--   0        0        0     4584 2023-06-15 14:47:17.299504 neptune-1.3.0/src/neptune/internal/types/file_types.py
+-rw-r--r--   0        0        0     1665 2023-06-15 14:47:17.299504 neptune-1.3.0/src/neptune/internal/types/stringify_value.py
+-rw-r--r--   0        0        0     4856 2023-06-15 14:47:17.299504 neptune-1.3.0/src/neptune/internal/utils/__init__.py
+-rw-r--r--   0        0        0     1171 2023-06-15 14:47:17.299504 neptune-1.3.0/src/neptune/internal/utils/dependency_tracking.py
+-rw-r--r--   0        0        0     2114 2023-06-15 14:47:17.299504 neptune-1.3.0/src/neptune/internal/utils/deprecation.py
+-rw-r--r--   0        0        0     2374 2023-06-15 14:47:17.299504 neptune-1.3.0/src/neptune/internal/utils/generic_attribute_mapper.py
+-rw-r--r--   0        0        0     5537 2023-06-15 14:47:17.299504 neptune-1.3.0/src/neptune/internal/utils/git.py
+-rw-r--r--   0        0        0      849 2023-06-15 14:47:17.299504 neptune-1.3.0/src/neptune/internal/utils/hashing.py
+-rw-r--r--   0        0        0     9732 2023-06-15 14:47:17.299504 neptune-1.3.0/src/neptune/internal/utils/images.py
+-rw-r--r--   0        0        0     1288 2023-06-15 14:47:17.299504 neptune-1.3.0/src/neptune/internal/utils/iteration.py
+-rw-r--r--   0        0        0     3053 2023-06-15 14:47:17.299504 neptune-1.3.0/src/neptune/internal/utils/json_file_splitter.py
+-rw-r--r--   0        0        0     1633 2023-06-15 14:47:17.299504 neptune-1.3.0/src/neptune/internal/utils/limits.py
+-rw-r--r--   0        0        0     1488 2023-06-15 14:47:17.299504 neptune-1.3.0/src/neptune/internal/utils/logger.py
+-rw-r--r--   0        0        0     1042 2023-06-15 14:47:17.299504 neptune-1.3.0/src/neptune/internal/utils/paths.py
+-rw-r--r--   0        0        0     2049 2023-06-15 14:47:17.299504 neptune-1.3.0/src/neptune/internal/utils/ping_background_job.py
+-rw-r--r--   0        0        0     1809 2023-06-15 14:47:17.299504 neptune-1.3.0/src/neptune/internal/utils/process_killer.py
+-rw-r--r--   0        0        0     1564 2023-06-15 14:47:17.299504 neptune-1.3.0/src/neptune/internal/utils/run_state.py
+-rw-r--r--   0        0        0     1207 2023-06-15 14:47:17.299504 neptune-1.3.0/src/neptune/internal/utils/runningmode.py
+-rw-r--r--   0        0        0     1340 2023-06-15 14:47:17.299504 neptune-1.3.0/src/neptune/internal/utils/s3.py
+-rw-r--r--   0        0        0     2270 2023-06-15 14:47:17.299504 neptune-1.3.0/src/neptune/internal/utils/source_code.py
+-rw-r--r--   0        0        0     1457 2023-06-15 14:47:17.299504 neptune-1.3.0/src/neptune/internal/utils/sync_offset_file.py
+-rw-r--r--   0        0        0     1927 2023-06-15 14:47:17.299504 neptune-1.3.0/src/neptune/internal/utils/traceback_job.py
+-rw-r--r--   0        0        0     2426 2023-06-15 14:47:17.299504 neptune-1.3.0/src/neptune/internal/utils/uncaught_exception_handler.py
+-rw-r--r--   0        0        0     4462 2023-06-15 14:47:17.299504 neptune-1.3.0/src/neptune/internal/value_to_attribute_visitor.py
+-rw-r--r--   0        0        0      596 2023-06-15 14:47:17.299504 neptune-1.3.0/src/neptune/internal/websockets/__init__.py
+-rw-r--r--   0        0        0     5188 2023-06-15 14:47:17.299504 neptune-1.3.0/src/neptune/internal/websockets/websocket_signals_background_job.py
+-rw-r--r--   0        0        0     1229 2023-06-15 14:47:17.299504 neptune-1.3.0/src/neptune/internal/websockets/websockets_factory.py
+-rw-r--r--   0        0        0    13821 2023-06-15 14:47:17.299504 neptune-1.3.0/src/neptune/legacy/__init__.py
+-rw-r--r--   0        0        0    11218 2023-06-15 14:47:17.299504 neptune-1.3.0/src/neptune/legacy/api_exceptions.py
+-rw-r--r--   0        0        0     4710 2023-06-15 14:47:17.299504 neptune-1.3.0/src/neptune/legacy/backend.py
+-rw-r--r--   0        0        0      737 2023-06-15 14:47:17.299504 neptune-1.3.0/src/neptune/legacy/checkpoint.py
+-rw-r--r--   0        0        0      859 2023-06-15 14:47:17.299504 neptune-1.3.0/src/neptune/legacy/constants.py
+-rw-r--r--   0        0        0      860 2023-06-15 14:47:17.299504 neptune-1.3.0/src/neptune/legacy/envs.py
+-rw-r--r--   0        0        0    12780 2023-06-15 14:47:17.299504 neptune-1.3.0/src/neptune/legacy/exceptions.py
+-rw-r--r--   0        0        0    42888 2023-06-15 14:47:17.299504 neptune-1.3.0/src/neptune/legacy/experiments.py
+-rw-r--r--   0        0        0      663 2023-06-15 14:47:17.299504 neptune-1.3.0/src/neptune/legacy/git_info.py
+-rw-r--r--   0        0        0      596 2023-06-15 14:47:17.299504 neptune-1.3.0/src/neptune/legacy/internal/__init__.py
+-rw-r--r--   0        0        0     1999 2023-06-15 14:47:17.299504 neptune-1.3.0/src/neptune/legacy/internal/abort.py
+-rw-r--r--   0        0        0      888 2023-06-15 14:47:17.299504 neptune-1.3.0/src/neptune/legacy/internal/api_clients/__init__.py
+-rw-r--r--   0        0        0     1148 2023-06-15 14:47:17.299504 neptune-1.3.0/src/neptune/legacy/internal/api_clients/backend_factory.py
+-rw-r--r--   0        0        0     1826 2023-06-15 14:47:17.299504 neptune-1.3.0/src/neptune/legacy/internal/api_clients/client_config.py
+-rw-r--r--   0        0        0     3103 2023-06-15 14:47:17.299504 neptune-1.3.0/src/neptune/legacy/internal/api_clients/credentials.py
+-rw-r--r--   0        0        0      596 2023-06-15 14:47:17.299504 neptune-1.3.0/src/neptune/legacy/internal/api_clients/hosted_api_clients/__init__.py
+-rw-r--r--   0        0        0    46556 2023-06-15 14:47:17.299504 neptune-1.3.0/src/neptune/legacy/internal/api_clients/hosted_api_clients/hosted_alpha_leaderboard_api_client.py
+-rw-r--r--   0        0        0     8710 2023-06-15 14:47:17.299504 neptune-1.3.0/src/neptune/legacy/internal/api_clients/hosted_api_clients/hosted_backend_api_client.py
+-rw-r--r--   0        0        0     4456 2023-06-15 14:47:17.299504 neptune-1.3.0/src/neptune/legacy/internal/api_clients/hosted_api_clients/mixins.py
+-rw-r--r--   0        0        0     3857 2023-06-15 14:47:17.299504 neptune-1.3.0/src/neptune/legacy/internal/api_clients/hosted_api_clients/utils.py
+-rw-r--r--   0        0        0     4631 2023-06-15 14:47:17.303504 neptune-1.3.0/src/neptune/legacy/internal/api_clients/offline_backend.py
+-rw-r--r--   0        0        0      596 2023-06-15 14:47:17.303504 neptune-1.3.0/src/neptune/legacy/internal/backends/__init__.py
+-rw-r--r--   0        0        0      776 2023-06-15 14:47:17.303504 neptune-1.3.0/src/neptune/legacy/internal/backends/hosted_neptune_backend.py
+-rw-r--r--   0        0        0      596 2023-06-15 14:47:17.303504 neptune-1.3.0/src/neptune/legacy/internal/channels/__init__.py
+-rw-r--r--   0        0        0     3903 2023-06-15 14:47:17.303504 neptune-1.3.0/src/neptune/legacy/internal/channels/channels.py
+-rw-r--r--   0        0        0     7087 2023-06-15 14:47:17.303504 neptune-1.3.0/src/neptune/legacy/internal/channels/channels_values_sender.py
+-rw-r--r--   0        0        0      596 2023-06-15 14:47:17.303504 neptune-1.3.0/src/neptune/legacy/internal/execution/__init__.py
+-rw-r--r--   0        0        0     6126 2023-06-15 14:47:17.303504 neptune-1.3.0/src/neptune/legacy/internal/execution/execution_context.py
+-rw-r--r--   0        0        0      596 2023-06-15 14:47:17.303504 neptune-1.3.0/src/neptune/legacy/internal/experiments/__init__.py
+-rw-r--r--   0        0        0      596 2023-06-15 14:47:17.303504 neptune-1.3.0/src/neptune/legacy/internal/notebooks/__init__.py
+-rw-r--r--   0        0        0     1510 2023-06-15 14:47:17.303504 neptune-1.3.0/src/neptune/legacy/internal/notebooks/comm.py
+-rw-r--r--   0        0        0     1711 2023-06-15 14:47:17.303504 neptune-1.3.0/src/neptune/legacy/internal/notebooks/notebooks.py
+-rw-r--r--   0        0        0      596 2023-06-15 14:47:17.303504 neptune-1.3.0/src/neptune/legacy/internal/streams/__init__.py
+-rw-r--r--   0        0        0     2805 2023-06-15 14:47:17.303504 neptune-1.3.0/src/neptune/legacy/internal/streams/channel_writer.py
+-rw-r--r--   0        0        0     1945 2023-06-15 14:47:17.303504 neptune-1.3.0/src/neptune/legacy/internal/streams/stdstream_uploader.py
+-rw-r--r--   0        0        0      596 2023-06-15 14:47:17.303504 neptune-1.3.0/src/neptune/legacy/internal/threads/__init__.py
+-rw-r--r--   0        0        0     2363 2023-06-15 14:47:17.303504 neptune-1.3.0/src/neptune/legacy/internal/threads/aborting_thread.py
+-rw-r--r--   0        0        0     1816 2023-06-15 14:47:17.303504 neptune-1.3.0/src/neptune/legacy/internal/threads/hardware_metric_reporting_thread.py
+-rw-r--r--   0        0        0     1334 2023-06-15 14:47:17.303504 neptune-1.3.0/src/neptune/legacy/internal/threads/neptune_thread.py
+-rw-r--r--   0        0        0     1556 2023-06-15 14:47:17.303504 neptune-1.3.0/src/neptune/legacy/internal/threads/ping_thread.py
+-rw-r--r--   0        0        0      596 2023-06-15 14:47:17.303504 neptune-1.3.0/src/neptune/legacy/internal/utils/__init__.py
+-rw-r--r--   0        0        0     8091 2023-06-15 14:47:17.303504 neptune-1.3.0/src/neptune/legacy/internal/utils/alpha_integration.py
+-rw-r--r--   0        0        0      997 2023-06-15 14:47:17.303504 neptune-1.3.0/src/neptune/legacy/internal/utils/deprecation.py
+-rw-r--r--   0        0        0     2597 2023-06-15 14:47:17.303504 neptune-1.3.0/src/neptune/legacy/internal/utils/http.py
+-rw-r--r--   0        0        0     2597 2023-06-15 14:47:17.303504 neptune-1.3.0/src/neptune/legacy/internal/utils/http_utils.py
+-rw-r--r--   0        0        0     2990 2023-06-15 14:47:17.303504 neptune-1.3.0/src/neptune/legacy/internal/utils/image.py
+-rw-r--r--   0        0        0     3145 2023-06-15 14:47:17.303504 neptune-1.3.0/src/neptune/legacy/internal/utils/source_code.py
+-rw-r--r--   0        0        0      596 2023-06-15 14:47:17.303504 neptune-1.3.0/src/neptune/legacy/internal/websockets/__init__.py
+-rw-r--r--   0        0        0     3542 2023-06-15 14:47:17.303504 neptune-1.3.0/src/neptune/legacy/internal/websockets/message.py
+-rw-r--r--   0        0        0     1097 2023-06-15 14:47:17.303504 neptune-1.3.0/src/neptune/legacy/internal/websockets/reconnecting_websocket_factory.py
+-rw-r--r--   0        0        0     1228 2023-06-15 14:47:17.303504 neptune-1.3.0/src/neptune/legacy/internal/websockets/websocket_message_processor.py
+-rw-r--r--   0        0        0     3938 2023-06-15 14:47:17.303504 neptune-1.3.0/src/neptune/legacy/model.py
+-rw-r--r--   0        0        0     2807 2023-06-15 14:47:17.303504 neptune-1.3.0/src/neptune/legacy/notebook.py
+-rw-r--r--   0        0        0      691 2023-06-15 14:47:17.303504 neptune-1.3.0/src/neptune/legacy/oauth.py
+-rw-r--r--   0        0        0      678 2023-06-15 14:47:17.303504 neptune-1.3.0/src/neptune/legacy/patterns.py
+-rw-r--r--   0        0        0    26377 2023-06-15 14:47:17.303504 neptune-1.3.0/src/neptune/legacy/projects.py
+-rw-r--r--   0        0        0     8992 2023-06-15 14:47:17.303504 neptune-1.3.0/src/neptune/legacy/sessions.py
+-rw-r--r--   0        0        0     1162 2023-06-15 14:47:17.303504 neptune-1.3.0/src/neptune/legacy/utils.py
+-rw-r--r--   0        0        0      660 2023-06-15 14:47:17.303504 neptune-1.3.0/src/neptune/logging/__init__.py
+-rw-r--r--   0        0        0      976 2023-06-15 14:47:17.303504 neptune-1.3.0/src/neptune/logging/logger.py
+-rw-r--r--   0        0        0     4454 2023-06-15 14:47:17.303504 neptune-1.3.0/src/neptune/management/__init__.py
+-rw-r--r--   0        0        0     6943 2023-06-15 14:47:17.303504 neptune-1.3.0/src/neptune/management/exceptions.py
+-rw-r--r--   0        0        0      596 2023-06-15 14:47:17.303504 neptune-1.3.0/src/neptune/management/internal/__init__.py
+-rw-r--r--   0        0        0    36941 2023-06-15 14:47:17.303504 neptune-1.3.0/src/neptune/management/internal/api.py
+-rw-r--r--   0        0        0     2853 2023-06-15 14:47:17.303504 neptune-1.3.0/src/neptune/management/internal/dto.py
+-rw-r--r--   0        0        0     1069 2023-06-15 14:47:17.303504 neptune-1.3.0/src/neptune/management/internal/types.py
+-rw-r--r--   0        0        0     2013 2023-06-15 14:47:17.303504 neptune-1.3.0/src/neptune/management/internal/utils.py
+-rw-r--r--   0        0        0      995 2023-06-15 14:47:17.303504 neptune-1.3.0/src/neptune/metadata_containers/__init__.py
+-rw-r--r--   0        0        0     2063 2023-06-15 14:47:17.303504 neptune-1.3.0/src/neptune/metadata_containers/abstract.py
+-rw-r--r--   0        0        0    20007 2023-06-15 14:47:17.303504 neptune-1.3.0/src/neptune/metadata_containers/metadata_container.py
+-rw-r--r--   0        0        0     9194 2023-06-15 14:47:17.303504 neptune-1.3.0/src/neptune/metadata_containers/metadata_containers_table.py
+-rw-r--r--   0        0        0    12337 2023-06-15 14:47:17.303504 neptune-1.3.0/src/neptune/metadata_containers/model.py
+-rw-r--r--   0        0        0    11428 2023-06-15 14:47:17.303504 neptune-1.3.0/src/neptune/metadata_containers/model_version.py
+-rw-r--r--   0        0        0    15433 2023-06-15 14:47:17.303504 neptune-1.3.0/src/neptune/metadata_containers/project.py
+-rw-r--r--   0        0        0    23734 2023-06-15 14:47:17.307504 neptune-1.3.0/src/neptune/metadata_containers/run.py
+-rw-r--r--   0        0        0     2606 2023-06-15 14:47:17.307504 neptune-1.3.0/src/neptune/new/__init__.py
+-rw-r--r--   0        0        0     1476 2023-06-15 14:47:17.307504 neptune-1.3.0/src/neptune/new/_compatibility.py
+-rw-r--r--   0        0        0      974 2023-06-15 14:47:17.307504 neptune-1.3.0/src/neptune/new/constants.py
+-rw-r--r--   0        0        0     1378 2023-06-15 14:47:17.307504 neptune-1.3.0/src/neptune/new/envs.py
+-rw-r--r--   0        0        0     5846 2023-06-15 14:47:17.307504 neptune-1.3.0/src/neptune/new/exceptions.py
+-rw-r--r--   0        0        0      655 2023-06-15 14:47:17.307504 neptune-1.3.0/src/neptune/new/handler.py
+-rw-r--r--   0        0        0      694 2023-06-15 14:47:17.307504 neptune-1.3.0/src/neptune/new/project.py
+-rw-r--r--   0        0        0     1672 2023-06-15 14:47:17.307504 neptune-1.3.0/src/neptune/new/run.py
+-rw-r--r--   0        0        0     1426 2023-06-15 14:47:17.307504 neptune-1.3.0/src/neptune/new/runs_table.py
+-rw-r--r--   0        0        0      681 2023-06-15 14:47:17.307504 neptune-1.3.0/src/neptune/new/utils.py
+-rw-r--r--   0        0        0      696 2023-06-15 14:47:17.307504 neptune-1.3.0/src/neptune/new/version.py
+-rw-r--r--   0        0        0     1071 2023-06-15 14:47:17.307504 neptune-1.3.0/src/neptune/types/__init__.py
+-rw-r--r--   0        0        0      914 2023-06-15 14:47:17.307504 neptune-1.3.0/src/neptune/types/atoms/__init__.py
+-rw-r--r--   0        0        0     1626 2023-06-15 14:47:17.307504 neptune-1.3.0/src/neptune/types/atoms/artifact.py
+-rw-r--r--   0        0        0      936 2023-06-15 14:47:17.307504 neptune-1.3.0/src/neptune/types/atoms/atom.py
+-rw-r--r--   0        0        0     1302 2023-06-15 14:47:17.307504 neptune-1.3.0/src/neptune/types/atoms/boolean.py
+-rw-r--r--   0        0        0     1435 2023-06-15 14:47:17.307504 neptune-1.3.0/src/neptune/types/atoms/datetime.py
+-rw-r--r--   0        0        0    11695 2023-06-15 14:47:17.307504 neptune-1.3.0/src/neptune/types/atoms/file.py
+-rw-r--r--   0        0        0     1297 2023-06-15 14:47:17.307504 neptune-1.3.0/src/neptune/types/atoms/float.py
+-rw-r--r--   0        0        0     1902 2023-06-15 14:47:17.307504 neptune-1.3.0/src/neptune/types/atoms/git_ref.py
+-rw-r--r--   0        0        0     1299 2023-06-15 14:47:17.307504 neptune-1.3.0/src/neptune/types/atoms/integer.py
+-rw-r--r--   0        0        0     1473 2023-06-15 14:47:17.307504 neptune-1.3.0/src/neptune/types/atoms/string.py
+-rw-r--r--   0        0        0     1485 2023-06-15 14:47:17.307504 neptune-1.3.0/src/neptune/types/file_set.py
+-rw-r--r--   0        0        0      831 2023-06-15 14:47:17.307504 neptune-1.3.0/src/neptune/types/mode.py
+-rw-r--r--   0        0        0      777 2023-06-15 14:47:17.307504 neptune-1.3.0/src/neptune/types/model_version_stage.py
+-rw-r--r--   0        0        0     1144 2023-06-15 14:47:17.307504 neptune-1.3.0/src/neptune/types/namespace.py
+-rw-r--r--   0        0        0      783 2023-06-15 14:47:17.307504 neptune-1.3.0/src/neptune/types/series/__init__.py
+-rw-r--r--   0        0        0     2447 2023-06-15 14:47:17.307504 neptune-1.3.0/src/neptune/types/series/file_series.py
+-rw-r--r--   0        0        0     2553 2023-06-15 14:47:17.307504 neptune-1.3.0/src/neptune/types/series/float_series.py
+-rw-r--r--   0        0        0     1221 2023-06-15 14:47:17.307504 neptune-1.3.0/src/neptune/types/series/series.py
+-rw-r--r--   0        0        0     1353 2023-06-15 14:47:17.307504 neptune-1.3.0/src/neptune/types/series/series_value.py
+-rw-r--r--   0        0        0     2601 2023-06-15 14:47:17.307504 neptune-1.3.0/src/neptune/types/series/string_series.py
+-rw-r--r--   0        0        0      655 2023-06-15 14:47:17.307504 neptune-1.3.0/src/neptune/types/sets/__init__.py
+-rw-r--r--   0        0        0      934 2023-06-15 14:47:17.307504 neptune-1.3.0/src/neptune/types/sets/set.py
+-rw-r--r--   0        0        0     1119 2023-06-15 14:47:17.307504 neptune-1.3.0/src/neptune/types/sets/string_set.py
+-rw-r--r--   0        0        0     3551 2023-06-15 14:47:17.307504 neptune-1.3.0/src/neptune/types/type_casting.py
+-rw-r--r--   0        0        0      892 2023-06-15 14:47:17.307504 neptune-1.3.0/src/neptune/types/value.py
+-rw-r--r--   0        0        0     1634 2023-06-15 14:47:17.307504 neptune-1.3.0/src/neptune/types/value_copy.py
+-rw-r--r--   0        0        0     2596 2023-06-15 14:47:17.307504 neptune-1.3.0/src/neptune/types/value_visitor.py
+-rw-r--r--   0        0        0      698 2023-06-15 14:47:17.307504 neptune-1.3.0/src/neptune/typing.py
+-rw-r--r--   0        0        0     1755 2023-06-15 14:47:17.307504 neptune-1.3.0/src/neptune/utils.py
+-rw-r--r--   0        0        0        0 2023-06-15 14:47:17.307504 neptune-1.3.0/src/neptune/vendor/__init__.py
+-rw-r--r--   0        0        0     6306 2023-06-15 14:47:17.307504 neptune-1.3.0/src/neptune/vendor/lib_programname.py
+-rw-r--r--   0        0        0    68552 2023-06-15 14:47:17.307504 neptune-1.3.0/src/neptune/vendor/pynvml.py
+-rw-r--r--   0        0        0     2228 2023-06-15 14:47:17.307504 neptune-1.3.0/src/neptune/version.py
+-rw-r--r--   0        0        0    18779 1970-01-01 00:00:00.000000 neptune-1.3.0/PKG-INFO
```

### Comparing `neptune-1.2.0/CHANGELOG.md` & `neptune-1.3.0/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+## neptune 1.3.0
+
+### Features
+- Added automatic tracking of dependencies ([#1345](https://github.com/neptune-ai/neptune-client/pull/1345))
+- Added automatic tracking of uncommitted changes ([#1350]https://github.com/neptune-ai/neptune-client/pull/1350)
+
+### Fixes
+- Added support of project visibility exception ([#1343](https://github.com/neptune-ai/neptune-client/pull/1343))
+
+### Changes
+- Added support of active projects limit exception ([#1348](https://github.com/neptune-ai/neptune-client/pull/1348))
+
 ## neptune 1.2.0
 
 ### Changes
 - Neptune objects and universal methods covered with docstrings ([#1309](https://github.com/neptune-ai/neptune-client/pull/1309))
 - Added docstrings for Neptune packages and modules ([#1332](https://github.com/neptune-ai/neptune-client/pull/1332))
 
 ### Features
```

### Comparing `neptune-1.2.0/LICENSE` & `neptune-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/README.md` & `neptune-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/pyproject.toml` & `neptune-1.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 # Missing compatibility layer between Python 2 and Python 3
 six = ">=1.12.0"
 future = ">=0.17.1"
 
 # Utility
 packaging = "*"
 click = ">=7.0"
+pipreqs = ">=0.4"
 
 # Networking
 bravado = "^11.0.0"
 oauthlib = ">=2.1.0"
 PyJWT = "*"
 requests = ">=2.20.0"
 requests-oauthlib = ">=1.0.0"
@@ -59,14 +60,15 @@
 vega_datasets = { version = "*", optional = true }
 Faker = { version = "*", optional = true }
 
 # e2e
 optuna = { version = "*", optional = true }
 scikit-learn = { version = "*", optional = true }
 torchvision = { version = "*", optional = true }
+accelerate = { version = "*", optional = true }
 
 # Additional integrations
 kedro-neptune = { version = "*", optional = true, python = "<3.11" }
 neptune-detectron2 = { version = "*", optional = true, python = ">=3.7"}
 neptune-fastai = { version = "*", optional = true }
 neptune-lightgbm = { version = "*", optional = true }
 pytorch-lightning = { version = "*", optional = true }
@@ -120,28 +122,29 @@
 e2e = [
     # Integrations
     "optuna",
     "pytorch-lightning",
     "scikit-learn",
     "torchvision",
     "transformers",
+    "accelerate",
     "zenml",
 ]
 
 [tool.poetry]
 authors = ["neptune.ai <contact@neptune.ai>"]
 description = "Neptune Client"
 repository = "https://github.com/neptune-ai/neptune-client"
 homepage = "https://neptune.ai/"
 documentation = "https://docs.neptune.ai/"
 include = ["CHANGELOG.md"]
 license = "Apache License 2.0"
 name = "neptune"
 readme = "README.md"
-version = "1.2.0"
+version = "1.3.0"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: Apache Software License",
     "Natural Language :: English",
```

### Comparing `neptune-1.2.0/src/neptune/__init__.py` & `neptune-1.3.0/src/neptune/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/attributes/__init__.py` & `neptune-1.3.0/src/neptune/attributes/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/attributes/atoms/__init__.py` & `neptune-1.3.0/src/neptune/attributes/atoms/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/attributes/atoms/artifact.py` & `neptune-1.3.0/src/neptune/attributes/atoms/artifact.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/attributes/atoms/atom.py` & `neptune-1.3.0/src/neptune/attributes/atoms/atom.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/attributes/atoms/boolean.py` & `neptune-1.3.0/src/neptune/attributes/atoms/boolean.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/attributes/atoms/copiable_atom.py` & `neptune-1.3.0/src/neptune/attributes/atoms/copiable_atom.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/attributes/atoms/datetime.py` & `neptune-1.3.0/src/neptune/attributes/atoms/datetime.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/attributes/atoms/file.py` & `neptune-1.3.0/src/neptune/attributes/atoms/file.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/attributes/atoms/float.py` & `neptune-1.3.0/src/neptune/attributes/atoms/float.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/attributes/atoms/git_ref.py` & `neptune-1.3.0/src/neptune/attributes/atoms/git_ref.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/attributes/atoms/integer.py` & `neptune-1.3.0/src/neptune/attributes/atoms/integer.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/attributes/atoms/notebook_ref.py` & `neptune-1.3.0/src/neptune/attributes/atoms/notebook_ref.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/attributes/atoms/run_state.py` & `neptune-1.3.0/src/neptune/attributes/atoms/run_state.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/attributes/atoms/string.py` & `neptune-1.3.0/src/neptune/attributes/atoms/string.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/attributes/attribute.py` & `neptune-1.3.0/src/neptune/attributes/attribute.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/attributes/constants.py` & `neptune-1.3.0/src/neptune/attributes/constants.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 __all__ = [
     "ARTIFACT_ATTRIBUTE_SPACE",
+    "DIFF_HEAD_INDEX_PATH",
     "LOG_ATTRIBUTE_SPACE",
     "MONITORING_ATTRIBUTE_SPACE",
     "MONITORING_STDERR_ATTRIBUTE_PATH",
     "MONITORING_STDOUT_ATTRIBUTE_PATH",
     "MONITORING_TRACEBACK_ATTRIBUTE_PATH",
     "PARAMETERS_ATTRIBUTE_SPACE",
     "PROPERTIES_ATTRIBUTE_SPACE",
@@ -31,14 +32,15 @@
     "SYSTEM_NAME_ATTRIBUTE_PATH",
     "SYSTEM_STATE_ATTRIBUTE_PATH",
     "SYSTEM_TAGS_ATTRIBUTE_PATH",
     "SYSTEM_FAILED_ATTRIBUTE_PATH",
     "SYSTEM_STAGE_ATTRIBUTE_PATH",
     "SIGNAL_TYPE_STOP",
     "SIGNAL_TYPE_ABORT",
+    "UPSTREAM_INDEX_DIFF",
 ]
 
 ARTIFACT_ATTRIBUTE_SPACE = "artifacts/"
 
 LOG_ATTRIBUTE_SPACE = "logs/"
 
 MONITORING_ATTRIBUTE_SPACE = "monitoring/"
@@ -61,7 +63,10 @@
 SYSTEM_STATE_ATTRIBUTE_PATH = f"{SYSTEM_ATTRIBUTE_SPACE}state"
 SYSTEM_TAGS_ATTRIBUTE_PATH = f"{SYSTEM_ATTRIBUTE_SPACE}tags"
 SYSTEM_FAILED_ATTRIBUTE_PATH = f"{SYSTEM_ATTRIBUTE_SPACE}failed"
 SYSTEM_STAGE_ATTRIBUTE_PATH = f"{SYSTEM_ATTRIBUTE_SPACE}stage"
 
 SIGNAL_TYPE_STOP = "neptune/stop"
 SIGNAL_TYPE_ABORT = "neptune/abort"
+
+DIFF_HEAD_INDEX_PATH = f"{SOURCE_CODE_ATTRIBUTE_SPACE}diff"
+UPSTREAM_INDEX_DIFF = f"{SOURCE_CODE_ATTRIBUTE_SPACE}upstream_diff_"
```

### Comparing `neptune-1.2.0/src/neptune/attributes/file_set.py` & `neptune-1.3.0/src/neptune/attributes/file_set.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/attributes/namespace.py` & `neptune-1.3.0/src/neptune/attributes/namespace.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/attributes/series/__init__.py` & `neptune-1.3.0/src/neptune/attributes/series/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/attributes/series/fetchable_series.py` & `neptune-1.3.0/src/neptune/attributes/series/fetchable_series.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/attributes/series/file_series.py` & `neptune-1.3.0/src/neptune/attributes/series/file_series.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/attributes/series/float_series.py` & `neptune-1.3.0/src/neptune/attributes/series/float_series.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/attributes/series/series.py` & `neptune-1.3.0/src/neptune/attributes/series/series.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/attributes/series/string_series.py` & `neptune-1.3.0/src/neptune/attributes/series/string_series.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/attributes/sets/__init__.py` & `neptune-1.3.0/src/neptune/attributes/sets/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/attributes/sets/set.py` & `neptune-1.3.0/src/neptune/attributes/sets/set.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/attributes/sets/string_set.py` & `neptune-1.3.0/src/neptune/attributes/sets/string_set.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/attributes/utils.py` & `neptune-1.3.0/src/neptune/attributes/utils.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/cli/__init__.py` & `neptune-1.3.0/src/neptune/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/cli/__main__.py` & `neptune-1.3.0/src/neptune/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/cli/abstract_backend_runner.py` & `neptune-1.3.0/src/neptune/cli/abstract_backend_runner.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/cli/clear.py` & `neptune-1.3.0/src/neptune/cli/clear.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/cli/commands.py` & `neptune-1.3.0/src/neptune/cli/commands.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/cli/container_manager.py` & `neptune-1.3.0/src/neptune/cli/container_manager.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/cli/path_option.py` & `neptune-1.3.0/src/neptune/cli/path_option.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/cli/status.py` & `neptune-1.3.0/src/neptune/cli/status.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/cli/sync.py` & `neptune-1.3.0/src/neptune/cli/sync.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/cli/utils.py` & `neptune-1.3.0/src/neptune/cli/utils.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/common/__init__.py` & `neptune-1.3.0/src/neptune/common/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/common/backends/__init__.py` & `neptune-1.3.0/src/neptune/common/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/common/backends/api_model.py` & `neptune-1.3.0/src/neptune/common/backends/api_model.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/common/backends/utils.py` & `neptune-1.3.0/src/neptune/common/backends/utils.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/common/envs.py` & `neptune-1.3.0/src/neptune/common/envs.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/common/exceptions.py` & `neptune-1.3.0/src/neptune/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/common/experiments.py` & `neptune-1.3.0/src/neptune/common/experiments.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/common/git_info.py` & `neptune-1.3.0/src/neptune/common/git_info.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/common/hardware/__init__.py` & `neptune-1.3.0/src/neptune/common/hardware/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/common/hardware/cgroup/__init__.py` & `neptune-1.3.0/src/neptune/common/hardware/cgroup/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/common/hardware/cgroup/cgroup_filesystem_reader.py` & `neptune-1.3.0/src/neptune/common/hardware/cgroup/cgroup_filesystem_reader.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/common/hardware/cgroup/cgroup_monitor.py` & `neptune-1.3.0/src/neptune/common/hardware/cgroup/cgroup_monitor.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/common/hardware/constants.py` & `neptune-1.3.0/src/neptune/common/hardware/constants.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/common/hardware/gauges/__init__.py` & `neptune-1.3.0/src/neptune/common/hardware/gauges/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/common/hardware/gauges/cpu.py` & `neptune-1.3.0/src/neptune/common/hardware/gauges/cpu.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/common/hardware/gauges/gauge.py` & `neptune-1.3.0/src/neptune/common/hardware/gauges/gauge.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/common/hardware/gauges/gauge_factory.py` & `neptune-1.3.0/src/neptune/common/hardware/gauges/gauge_factory.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/common/hardware/gauges/gauge_mode.py` & `neptune-1.3.0/src/neptune/common/hardware/gauges/gauge_mode.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/common/hardware/gauges/gpu.py` & `neptune-1.3.0/src/neptune/common/hardware/gauges/gpu.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/common/hardware/gauges/memory.py` & `neptune-1.3.0/src/neptune/common/hardware/gauges/memory.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/common/hardware/gpu/__init__.py` & `neptune-1.3.0/src/neptune/common/hardware/gpu/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/common/hardware/gpu/gpu_monitor.py` & `neptune-1.3.0/src/neptune/common/hardware/gpu/gpu_monitor.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/common/hardware/metrics/__init__.py` & `neptune-1.3.0/src/neptune/common/hardware/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/common/hardware/metrics/metric.py` & `neptune-1.3.0/src/neptune/common/hardware/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/common/hardware/metrics/metrics_container.py` & `neptune-1.3.0/src/neptune/common/hardware/metrics/metrics_container.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/common/hardware/metrics/metrics_factory.py` & `neptune-1.3.0/src/neptune/common/hardware/metrics/metrics_factory.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/common/hardware/metrics/reports/__init__.py` & `neptune-1.3.0/src/neptune/common/hardware/metrics/reports/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/common/hardware/metrics/reports/metric_report.py` & `neptune-1.3.0/src/neptune/common/hardware/metrics/reports/metric_report.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/common/hardware/metrics/reports/metric_reporter.py` & `neptune-1.3.0/src/neptune/common/hardware/metrics/reports/metric_reporter.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/common/hardware/metrics/reports/metric_reporter_factory.py` & `neptune-1.3.0/src/neptune/common/hardware/metrics/reports/metric_reporter_factory.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/common/hardware/metrics/service/__init__.py` & `neptune-1.3.0/src/neptune/common/hardware/metrics/service/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/common/hardware/metrics/service/metric_service.py` & `neptune-1.3.0/src/neptune/common/hardware/metrics/service/metric_service.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/common/hardware/metrics/service/metric_service_factory.py` & `neptune-1.3.0/src/neptune/common/hardware/metrics/service/metric_service_factory.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/common/hardware/resources/__init__.py` & `neptune-1.3.0/src/neptune/common/hardware/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/common/hardware/resources/gpu_card_indices_provider.py` & `neptune-1.3.0/src/neptune/common/hardware/resources/gpu_card_indices_provider.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/common/hardware/resources/system_resource_info.py` & `neptune-1.3.0/src/neptune/common/hardware/resources/system_resource_info.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/common/hardware/resources/system_resource_info_factory.py` & `neptune-1.3.0/src/neptune/common/hardware/resources/system_resource_info_factory.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/common/hardware/system/__init__.py` & `neptune-1.3.0/src/neptune/common/hardware/system/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/common/hardware/system/system_monitor.py` & `neptune-1.3.0/src/neptune/common/hardware/system/system_monitor.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/common/oauth.py` & `neptune-1.3.0/src/neptune/common/oauth.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/common/patches/__init__.py` & `neptune-1.3.0/src/neptune/common/patches/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/common/patches/bravado.py` & `neptune-1.3.0/src/neptune/common/patches/bravado.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/common/patterns.py` & `neptune-1.3.0/src/neptune/common/patterns.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/common/storage/__init__.py` & `neptune-1.3.0/src/neptune/common/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/common/storage/datastream.py` & `neptune-1.3.0/src/neptune/common/storage/datastream.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/common/storage/storage_utils.py` & `neptune-1.3.0/src/neptune/common/storage/storage_utils.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/common/utils.py` & `neptune-1.3.0/src/neptune/common/utils.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/common/warnings.py` & `neptune-1.3.0/src/neptune/common/warnings.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/common/websockets/__init__.py` & `neptune-1.3.0/src/neptune/common/websockets/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/common/websockets/reconnecting_websocket.py` & `neptune-1.3.0/src/neptune/common/websockets/reconnecting_websocket.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/common/websockets/websocket_client_adapter.py` & `neptune-1.3.0/src/neptune/common/websockets/websocket_client_adapter.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/constants.py` & `neptune-1.3.0/src/neptune/constants.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/envs.py` & `neptune-1.3.0/src/neptune/envs.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/exceptions.py` & `neptune-1.3.0/src/neptune/exceptions.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/handler.py` & `neptune-1.3.0/src/neptune/handler.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/integrations/__init__.py` & `neptune-1.3.0/src/neptune/integrations/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/integrations/aws/__init__.py` & `neptune-1.3.0/src/neptune/integrations/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/integrations/detectron2/__init__.py` & `neptune-1.3.0/src/neptune/integrations/detectron2/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/integrations/fastai/__init__.py` & `neptune-1.3.0/src/neptune/integrations/fastai/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/integrations/kedro/__init__.py` & `neptune-1.3.0/src/neptune/integrations/kedro/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/integrations/lightgbm/__init__.py` & `neptune-1.3.0/src/neptune/integrations/lightgbm/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/integrations/optuna/__init__.py` & `neptune-1.3.0/src/neptune/integrations/optuna/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/integrations/prophet/__init__.py` & `neptune-1.3.0/src/neptune/integrations/prophet/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/integrations/python_logger.py` & `neptune-1.3.0/src/neptune/integrations/python_logger.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/integrations/pytorch/__init__.py` & `neptune-1.3.0/src/neptune/integrations/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/integrations/pytorch_lightning/__init__.py` & `neptune-1.3.0/src/neptune/integrations/pytorch_lightning/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/integrations/sacred/__init__.py` & `neptune-1.3.0/src/neptune/integrations/sacred/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/integrations/sklearn/__init__.py` & `neptune-1.3.0/src/neptune/integrations/sklearn/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/integrations/tensorflow_keras/__init__.py` & `neptune-1.3.0/src/neptune/integrations/tensorflow_keras/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/integrations/transformers/__init__.py` & `neptune-1.3.0/src/neptune/integrations/transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/integrations/utils.py` & `neptune-1.3.0/src/neptune/integrations/utils.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/integrations/xgboost/__init__.py` & `neptune-1.3.0/src/neptune/integrations/xgboost/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/internal/__init__.py` & `neptune-1.3.0/src/neptune/internal/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/internal/artifacts/__init__.py` & `neptune-1.3.0/src/neptune/internal/artifacts/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/internal/artifacts/drivers/__init__.py` & `neptune-1.3.0/src/neptune/internal/artifacts/drivers/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/internal/artifacts/drivers/local.py` & `neptune-1.3.0/src/neptune/internal/artifacts/drivers/local.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/internal/artifacts/drivers/s3.py` & `neptune-1.3.0/src/neptune/internal/artifacts/drivers/s3.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/internal/artifacts/file_hasher.py` & `neptune-1.3.0/src/neptune/internal/artifacts/file_hasher.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/internal/artifacts/local_file_hash_storage.py` & `neptune-1.3.0/src/neptune/internal/artifacts/local_file_hash_storage.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/internal/artifacts/types.py` & `neptune-1.3.0/src/neptune/internal/artifacts/types.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/internal/artifacts/utils.py` & `neptune-1.3.0/src/neptune/internal/artifacts/utils.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/internal/backends/__init__.py` & `neptune-1.3.0/src/neptune/internal/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/internal/backends/api_model.py` & `neptune-1.3.0/src/neptune/internal/backends/api_model.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/internal/backends/factory.py` & `neptune-1.3.0/src/neptune/internal/backends/factory.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/internal/backends/hosted_artifact_operations.py` & `neptune-1.3.0/src/neptune/internal/backends/hosted_artifact_operations.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/internal/backends/hosted_client.py` & `neptune-1.3.0/src/neptune/internal/backends/hosted_client.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/internal/backends/hosted_file_operations.py` & `neptune-1.3.0/src/neptune/internal/backends/hosted_file_operations.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/internal/backends/hosted_neptune_backend.py` & `neptune-1.3.0/src/neptune/internal/backends/hosted_neptune_backend.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/internal/backends/neptune_backend.py` & `neptune-1.3.0/src/neptune/internal/backends/neptune_backend.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/internal/backends/neptune_backend_mock.py` & `neptune-1.3.0/src/neptune/internal/backends/neptune_backend_mock.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/internal/backends/nql.py` & `neptune-1.3.0/src/neptune/internal/backends/nql.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/internal/backends/offline_neptune_backend.py` & `neptune-1.3.0/src/neptune/internal/backends/offline_neptune_backend.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/internal/backends/operation_api_name_visitor.py` & `neptune-1.3.0/src/neptune/internal/backends/operation_api_name_visitor.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/internal/backends/operation_api_object_converter.py` & `neptune-1.3.0/src/neptune/internal/backends/operation_api_object_converter.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/internal/backends/operations_preprocessor.py` & `neptune-1.3.0/src/neptune/internal/backends/operations_preprocessor.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/internal/backends/project_name_lookup.py` & `neptune-1.3.0/src/neptune/internal/backends/project_name_lookup.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/internal/backends/utils.py` & `neptune-1.3.0/src/neptune/internal/backends/utils.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/internal/backgroud_job_list.py` & `neptune-1.3.0/src/neptune/internal/backgroud_job_list.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/internal/background_job.py` & `neptune-1.3.0/src/neptune/internal/background_job.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/internal/container_structure.py` & `neptune-1.3.0/src/neptune/internal/container_structure.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/internal/container_type.py` & `neptune-1.3.0/src/neptune/internal/container_type.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/internal/credentials.py` & `neptune-1.3.0/src/neptune/internal/credentials.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/internal/disk_queue.py` & `neptune-1.3.0/src/neptune/internal/disk_queue.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/internal/exceptions.py` & `neptune-1.3.0/src/neptune/internal/exceptions.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/internal/hardware/__init__.py` & `neptune-1.3.0/src/neptune/internal/hardware/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/internal/hardware/gpu/__init__.py` & `neptune-1.3.0/src/neptune/internal/hardware/gpu/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/internal/hardware/gpu/gpu_monitor.py` & `neptune-1.3.0/src/neptune/internal/hardware/gpu/gpu_monitor.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/internal/hardware/hardware_metric_reporting_job.py` & `neptune-1.3.0/src/neptune/internal/hardware/hardware_metric_reporting_job.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/internal/id_formats.py` & `neptune-1.3.0/src/neptune/internal/id_formats.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/internal/init/__init__.py` & `neptune-1.3.0/src/neptune/internal/init/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/internal/init/parameters.py` & `neptune-1.3.0/src/neptune/internal/init/parameters.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/internal/notebooks/__init__.py` & `neptune-1.3.0/src/neptune/internal/notebooks/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/internal/notebooks/comm.py` & `neptune-1.3.0/src/neptune/internal/notebooks/comm.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/internal/notebooks/notebooks.py` & `neptune-1.3.0/src/neptune/internal/notebooks/notebooks.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/internal/operation.py` & `neptune-1.3.0/src/neptune/internal/operation.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/internal/operation_processors/__init__.py` & `neptune-1.3.0/src/neptune/internal/operation_processors/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/internal/operation_processors/async_operation_processor.py` & `neptune-1.3.0/src/neptune/internal/operation_processors/async_operation_processor.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/internal/operation_processors/factory.py` & `neptune-1.3.0/src/neptune/internal/operation_processors/factory.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/internal/operation_processors/offline_operation_processor.py` & `neptune-1.3.0/src/neptune/internal/operation_processors/offline_operation_processor.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/internal/operation_processors/operation_processor.py` & `neptune-1.3.0/src/neptune/internal/operation_processors/operation_processor.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/internal/operation_processors/operation_storage.py` & `neptune-1.3.0/src/neptune/internal/operation_processors/operation_storage.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/internal/operation_processors/read_only_operation_processor.py` & `neptune-1.3.0/src/neptune/internal/operation_processors/read_only_operation_processor.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/internal/operation_processors/sync_operation_processor.py` & `neptune-1.3.0/src/neptune/internal/operation_processors/sync_operation_processor.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/internal/operation_visitor.py` & `neptune-1.3.0/src/neptune/internal/operation_visitor.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/internal/state.py` & `neptune-1.3.0/src/neptune/internal/state.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/internal/streams/__init__.py` & `neptune-1.3.0/src/neptune/internal/streams/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/internal/streams/std_capture_background_job.py` & `neptune-1.3.0/src/neptune/internal/streams/std_capture_background_job.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/internal/streams/std_stream_capture_logger.py` & `neptune-1.3.0/src/neptune/internal/streams/std_stream_capture_logger.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/internal/threading/__init__.py` & `neptune-1.3.0/src/neptune/internal/threading/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/internal/threading/daemon.py` & `neptune-1.3.0/src/neptune/internal/threading/daemon.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/internal/types/__init__.py` & `neptune-1.3.0/src/neptune/internal/types/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/internal/types/file_types.py` & `neptune-1.3.0/src/neptune/internal/types/file_types.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/internal/types/stringify_value.py` & `neptune-1.3.0/src/neptune/internal/types/stringify_value.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/internal/utils/__init__.py` & `neptune-1.3.0/src/neptune/internal/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/internal/utils/deprecation.py` & `neptune-1.3.0/src/neptune/internal/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/internal/utils/generic_attribute_mapper.py` & `neptune-1.3.0/src/neptune/internal/utils/generic_attribute_mapper.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/internal/utils/hashing.py` & `neptune-1.3.0/src/neptune/internal/utils/hashing.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/internal/utils/images.py` & `neptune-1.3.0/src/neptune/internal/utils/images.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/internal/utils/iteration.py` & `neptune-1.3.0/src/neptune/internal/utils/iteration.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/internal/utils/json_file_splitter.py` & `neptune-1.3.0/src/neptune/internal/utils/json_file_splitter.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/internal/utils/limits.py` & `neptune-1.3.0/src/neptune/internal/utils/limits.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/internal/utils/logger.py` & `neptune-1.3.0/src/neptune/internal/utils/logger.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/internal/utils/paths.py` & `neptune-1.3.0/src/neptune/internal/utils/paths.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/internal/utils/ping_background_job.py` & `neptune-1.3.0/src/neptune/internal/utils/ping_background_job.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/internal/utils/process_killer.py` & `neptune-1.3.0/src/neptune/internal/utils/process_killer.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/internal/utils/run_state.py` & `neptune-1.3.0/src/neptune/internal/utils/run_state.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/internal/utils/runningmode.py` & `neptune-1.3.0/src/neptune/internal/utils/runningmode.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/internal/utils/s3.py` & `neptune-1.3.0/src/neptune/internal/utils/s3.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/internal/utils/source_code.py` & `neptune-1.3.0/src/neptune/internal/utils/source_code.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/internal/utils/sync_offset_file.py` & `neptune-1.3.0/src/neptune/internal/utils/sync_offset_file.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/internal/utils/traceback_job.py` & `neptune-1.3.0/src/neptune/internal/utils/traceback_job.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/internal/utils/uncaught_exception_handler.py` & `neptune-1.3.0/src/neptune/internal/utils/uncaught_exception_handler.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/internal/value_to_attribute_visitor.py` & `neptune-1.3.0/src/neptune/internal/value_to_attribute_visitor.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/internal/websockets/__init__.py` & `neptune-1.3.0/src/neptune/internal/websockets/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/internal/websockets/websocket_signals_background_job.py` & `neptune-1.3.0/src/neptune/internal/websockets/websocket_signals_background_job.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/internal/websockets/websockets_factory.py` & `neptune-1.3.0/src/neptune/internal/websockets/websockets_factory.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/legacy/__init__.py` & `neptune-1.3.0/src/neptune/legacy/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/legacy/api_exceptions.py` & `neptune-1.3.0/src/neptune/legacy/api_exceptions.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/legacy/backend.py` & `neptune-1.3.0/src/neptune/legacy/backend.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/legacy/checkpoint.py` & `neptune-1.3.0/src/neptune/legacy/checkpoint.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/legacy/constants.py` & `neptune-1.3.0/src/neptune/legacy/constants.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/legacy/envs.py` & `neptune-1.3.0/src/neptune/legacy/envs.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/legacy/exceptions.py` & `neptune-1.3.0/src/neptune/legacy/exceptions.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/legacy/experiments.py` & `neptune-1.3.0/src/neptune/legacy/experiments.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/legacy/git_info.py` & `neptune-1.3.0/src/neptune/legacy/git_info.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/legacy/internal/__init__.py` & `neptune-1.3.0/src/neptune/legacy/internal/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/legacy/internal/abort.py` & `neptune-1.3.0/src/neptune/legacy/internal/abort.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/legacy/internal/api_clients/__init__.py` & `neptune-1.3.0/src/neptune/legacy/internal/api_clients/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/legacy/internal/api_clients/backend_factory.py` & `neptune-1.3.0/src/neptune/legacy/internal/api_clients/backend_factory.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/legacy/internal/api_clients/client_config.py` & `neptune-1.3.0/src/neptune/legacy/internal/api_clients/client_config.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/legacy/internal/api_clients/credentials.py` & `neptune-1.3.0/src/neptune/legacy/internal/api_clients/credentials.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/legacy/internal/api_clients/hosted_api_clients/__init__.py` & `neptune-1.3.0/src/neptune/legacy/internal/api_clients/hosted_api_clients/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/legacy/internal/api_clients/hosted_api_clients/hosted_alpha_leaderboard_api_client.py` & `neptune-1.3.0/src/neptune/legacy/internal/api_clients/hosted_api_clients/hosted_alpha_leaderboard_api_client.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/legacy/internal/api_clients/hosted_api_clients/hosted_backend_api_client.py` & `neptune-1.3.0/src/neptune/legacy/internal/api_clients/hosted_api_clients/hosted_backend_api_client.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/legacy/internal/api_clients/hosted_api_clients/mixins.py` & `neptune-1.3.0/src/neptune/legacy/internal/api_clients/hosted_api_clients/mixins.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/legacy/internal/api_clients/hosted_api_clients/utils.py` & `neptune-1.3.0/src/neptune/legacy/internal/api_clients/hosted_api_clients/utils.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/legacy/internal/api_clients/offline_backend.py` & `neptune-1.3.0/src/neptune/legacy/internal/api_clients/offline_backend.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/legacy/internal/backends/__init__.py` & `neptune-1.3.0/src/neptune/legacy/internal/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/legacy/internal/backends/hosted_neptune_backend.py` & `neptune-1.3.0/src/neptune/legacy/internal/backends/hosted_neptune_backend.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/legacy/internal/channels/__init__.py` & `neptune-1.3.0/src/neptune/legacy/internal/channels/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/legacy/internal/channels/channels.py` & `neptune-1.3.0/src/neptune/legacy/internal/channels/channels.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/legacy/internal/channels/channels_values_sender.py` & `neptune-1.3.0/src/neptune/legacy/internal/channels/channels_values_sender.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/legacy/internal/execution/__init__.py` & `neptune-1.3.0/src/neptune/legacy/internal/execution/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/legacy/internal/execution/execution_context.py` & `neptune-1.3.0/src/neptune/legacy/internal/execution/execution_context.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/legacy/internal/experiments/__init__.py` & `neptune-1.3.0/src/neptune/legacy/internal/experiments/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/legacy/internal/notebooks/__init__.py` & `neptune-1.3.0/src/neptune/legacy/internal/notebooks/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/legacy/internal/notebooks/comm.py` & `neptune-1.3.0/src/neptune/legacy/internal/notebooks/comm.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/legacy/internal/notebooks/notebooks.py` & `neptune-1.3.0/src/neptune/legacy/internal/notebooks/notebooks.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/legacy/internal/streams/__init__.py` & `neptune-1.3.0/src/neptune/legacy/internal/streams/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/legacy/internal/streams/channel_writer.py` & `neptune-1.3.0/src/neptune/legacy/internal/streams/channel_writer.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/legacy/internal/streams/stdstream_uploader.py` & `neptune-1.3.0/src/neptune/legacy/internal/streams/stdstream_uploader.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/legacy/internal/threads/__init__.py` & `neptune-1.3.0/src/neptune/legacy/internal/threads/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/legacy/internal/threads/aborting_thread.py` & `neptune-1.3.0/src/neptune/legacy/internal/threads/aborting_thread.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/legacy/internal/threads/hardware_metric_reporting_thread.py` & `neptune-1.3.0/src/neptune/legacy/internal/threads/hardware_metric_reporting_thread.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/legacy/internal/threads/neptune_thread.py` & `neptune-1.3.0/src/neptune/legacy/internal/threads/neptune_thread.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/legacy/internal/threads/ping_thread.py` & `neptune-1.3.0/src/neptune/legacy/internal/threads/ping_thread.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/legacy/internal/utils/__init__.py` & `neptune-1.3.0/src/neptune/legacy/internal/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/legacy/internal/utils/alpha_integration.py` & `neptune-1.3.0/src/neptune/legacy/internal/utils/alpha_integration.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/legacy/internal/utils/deprecation.py` & `neptune-1.3.0/src/neptune/legacy/internal/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/legacy/internal/utils/http.py` & `neptune-1.3.0/src/neptune/legacy/internal/utils/http.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/legacy/internal/utils/http_utils.py` & `neptune-1.3.0/src/neptune/legacy/internal/utils/http_utils.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/legacy/internal/utils/image.py` & `neptune-1.3.0/src/neptune/legacy/internal/utils/image.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/legacy/internal/utils/source_code.py` & `neptune-1.3.0/src/neptune/legacy/internal/utils/source_code.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/legacy/internal/websockets/__init__.py` & `neptune-1.3.0/src/neptune/legacy/internal/websockets/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/legacy/internal/websockets/message.py` & `neptune-1.3.0/src/neptune/legacy/internal/websockets/message.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/legacy/internal/websockets/reconnecting_websocket_factory.py` & `neptune-1.3.0/src/neptune/legacy/internal/websockets/reconnecting_websocket_factory.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/legacy/internal/websockets/websocket_message_processor.py` & `neptune-1.3.0/src/neptune/legacy/internal/websockets/websocket_message_processor.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/legacy/model.py` & `neptune-1.3.0/src/neptune/legacy/model.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/legacy/notebook.py` & `neptune-1.3.0/src/neptune/legacy/notebook.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/legacy/oauth.py` & `neptune-1.3.0/src/neptune/legacy/oauth.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/legacy/patterns.py` & `neptune-1.3.0/src/neptune/legacy/patterns.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/legacy/projects.py` & `neptune-1.3.0/src/neptune/legacy/projects.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/legacy/sessions.py` & `neptune-1.3.0/src/neptune/legacy/sessions.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/legacy/utils.py` & `neptune-1.3.0/src/neptune/legacy/utils.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/logging/__init__.py` & `neptune-1.3.0/src/neptune/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/logging/logger.py` & `neptune-1.3.0/src/neptune/logging/logger.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/management/__init__.py` & `neptune-1.3.0/src/neptune/management/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/management/exceptions.py` & `neptune-1.3.0/src/neptune/management/exceptions.py`

 * *Files 12% similar despite different names*

```diff
@@ -174,7 +174,39 @@
     code = 23
     description = "Workspace '{workspace}' or user '{user}' could not be found."
 
 
 class UserAlreadyInvited(ManagementOperationFailure):
     code = 24
     description = "User '{user}' has already been invited to the workspace '{workspace}'."
+
+
+class ProjectPrivacyRestrictedException(ManagementOperationFailure):
+    code = 25
+    description = (
+        "Cannot set {requested} visibility for project. {followup}This might be caused by workspace "
+        "settings or limited by your plan."
+    )
+
+    def __init__(self, **kwargs):
+        modified_kwargs = {"followup": ""}
+        allowed = kwargs.get("allowed")
+        if allowed and isinstance(allowed, list):
+            modified_kwargs["followup"] = "Allowed values are: {allowed}. ".format(
+                allowed=", ".join(['"' + option + '"' for option in allowed])
+            )
+        modified_kwargs.update(kwargs)
+        requested = modified_kwargs.get("requested")
+        if not requested:
+            modified_kwargs["requested"] = "the selected"
+        else:
+            modified_kwargs["requested"] = '"' + requested + '"'
+        super().__init__(**modified_kwargs)
+
+
+class ActiveProjectsLimitReachedException(ManagementOperationFailure):
+    code = 26
+    description = (
+        "Limit of active projects reached. You can have up to {currentQuota} active projects simultaneously. "
+        "To create a new project, you need to either archive an active project or increase the quota of active "
+        "projects in the workspace."
+    )
```

### Comparing `neptune-1.2.0/src/neptune/management/internal/__init__.py` & `neptune-1.3.0/src/neptune/management/internal/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/management/internal/api.py` & `neptune-1.3.0/src/neptune/management/internal/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,14 @@
 from neptune.management.exceptions import (
     AccessRevokedOnDeletion,
     AccessRevokedOnMemberRemoval,
     AccessRevokedOnServiceAccountRemoval,
     BadRequestException,
     ProjectAlreadyExists,
     ProjectNotFound,
-    ProjectsLimitReached,
     ServiceAccountAlreadyHasAccess,
     ServiceAccountNotExistsOrWithoutAccess,
     ServiceAccountNotFound,
     UserAlreadyHasAccess,
     UserAlreadyInvited,
     UserNotExistsOrWithoutAccess,
     WorkspaceNotFound,
@@ -257,16 +256,14 @@
     try:
         return backend_client.api.createProject(**params).response()
     except HTTPBadRequest as e:
         validation_errors = parse_validation_errors(error=e)
         if "ERR_NOT_UNIQUE" in validation_errors:
             raise ProjectAlreadyExists(name=project_qualified_name) from e
         raise BadRequestException(validation_errors=validation_errors)
-    except HTTPUnprocessableEntity as e:
-        raise ProjectsLimitReached() from e
 
 
 @with_api_exceptions_handler
 def delete_project(project: str, *, workspace: Optional[str] = None, api_token: Optional[str] = None):
     """Deletes a project from a Neptune workspace.
 
     To delete projects, the user must be a workspace admin.
@@ -588,26 +585,23 @@
             If both are filled, will raise ValueError.
         workspace: Name of your Neptune workspace.
         api_token: Account's API token.
             If None, the value of the NEPTUNE_API_TOKEN environment variable is used.
             Note: To keep your token secure, use the NEPTUNE_API_TOKEN environment variable rather than placing your
             API token in plain text in your source code.
         role: The workspace role that is to be granted to the invited user.
-        You can choose between the following values:
-        - Administrator: `WorkspaceMemberRole.ADMIN`
-        - Member: `WorkspaceMemberRole.MEMBER`
+            You can choose between the following values: "admin" and "member".
         add_to_all_projects: Whether to add the user to all projects in the workspace.
 
     Example:
         >>> from neptune import management
-        >>> from management import WorkspaceMemberRole
         >>> management.invite_to_workspace(
         ...     username="user",
         ...     workspace="ml-team",
-        ...     role=WorkspaceMemberRole.ADMIN,
+        ...     role="admin",
         ... )
 
     You may also want to check the management API reference:
     https://docs.neptune.ai/api/management
     """
     verify_type("workspace", workspace, str)
     verify_type("role", role, (WorkspaceMemberRole, str))
```

### Comparing `neptune-1.2.0/src/neptune/management/internal/dto.py` & `neptune-1.3.0/src/neptune/management/internal/dto.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/management/internal/types.py` & `neptune-1.3.0/src/neptune/management/internal/types.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/management/internal/utils.py` & `neptune-1.3.0/src/neptune/management/internal/utils.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/metadata_containers/__init__.py` & `neptune-1.3.0/src/neptune/metadata_containers/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/metadata_containers/abstract.py` & `neptune-1.3.0/src/neptune/metadata_containers/abstract.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/metadata_containers/metadata_container.py` & `neptune-1.3.0/src/neptune/metadata_containers/metadata_container.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/metadata_containers/metadata_containers_table.py` & `neptune-1.3.0/src/neptune/metadata_containers/metadata_containers_table.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/metadata_containers/model.py` & `neptune-1.3.0/src/neptune/metadata_containers/model.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/metadata_containers/model_version.py` & `neptune-1.3.0/src/neptune/metadata_containers/model_version.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/metadata_containers/project.py` & `neptune-1.3.0/src/neptune/metadata_containers/project.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/metadata_containers/run.py` & `neptune-1.3.0/src/neptune/metadata_containers/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,22 @@
     StderrCaptureBackgroundJob,
     StdoutCaptureBackgroundJob,
 )
 from neptune.internal.utils import (
     verify_collection_type,
     verify_type,
 )
-from neptune.internal.utils.git import to_git_info
+from neptune.internal.utils.dependency_tracking import (
+    FileDependenciesStrategy,
+    InferDependenciesStrategy,
+)
+from neptune.internal.utils.git import (
+    to_git_info,
+    track_uncommitted_changes,
+)
 from neptune.internal.utils.hashing import generate_hash
 from neptune.internal.utils.limits import custom_run_id_exceeds_length
 from neptune.internal.utils.ping_background_job import PingBackgroundJob
 from neptune.internal.utils.runningmode import (
     in_interactive,
     in_notebook,
 )
@@ -135,14 +142,15 @@
         capture_hardware_metrics: Optional[bool] = None,
         fail_on_exception: bool = True,
         monitoring_namespace: Optional[str] = None,
         flush_period: float = DEFAULT_FLUSH_PERIOD,
         proxies: Optional[dict] = None,
         capture_traceback: bool = True,
         git_ref: Optional[Union[GitRef, GitRefDisabled]] = None,
+        dependencies: Optional[Union[str, os.PathLike]] = None,
         **kwargs,
     ):
         """Starts a new tracked run that logs ML model-building metadata to neptune.ai.
 
         You can log metadata by assigning it to the initialized Run object:
 
         ```
@@ -214,14 +222,18 @@
             capture_traceback: Whether to log the traceback of the run in case of an exception.
                 The tracked metadata is stored in the "<monitoring_namespace>/traceback" namespace (see the
                 `monitoring_namespace` parameter).
             git_ref: GitRef object containing information about the Git repository path.
                 If None, Neptune looks for a repository in the path of the script that is executed.
                 To specify a different location, set to GitRef(repository_path="path/to/repo").
                 To turn off Git tracking for the run, set to GitRef.DISABLED.
+            dependencies: To track the project dependencies, pass a path to your dependency file.
+                If None, no dependency file is uploaded.
+                If you pass `"infer"`, Neptune uses [pipreqs](https://pypi.org/project/pipreqs) to upload
+                the requirements.
 
         Returns:
             Run object that is used to manage the tracked run and log metadata to it.
 
         Examples:
 
             Creating a new run:
@@ -304,14 +316,16 @@
         verify_type("capture_stderr", capture_stderr, (bool, type(None)))
         verify_type("capture_hardware_metrics", capture_hardware_metrics, (bool, type(None)))
         verify_type("fail_on_exception", fail_on_exception, bool)
         verify_type("monitoring_namespace", monitoring_namespace, (str, type(None)))
         verify_type("capture_traceback", capture_traceback, bool)
         verify_type("capture_traceback", capture_traceback, bool)
         verify_type("git_ref", git_ref, (GitRef, str, type(None)))
+        verify_type("dependencies", dependencies, (str, os.PathLike, type(None)))
+
         if tags is not None:
             if isinstance(tags, str):
                 tags = [tags]
             else:
                 verify_collection_type("tags", tags, str)
         if source_files is not None:
             if isinstance(source_files, str):
@@ -326,15 +340,16 @@
         self._hostname: str = get_hostname()
         self._pid: int = os.getpid()
         self._tid: int = threading.get_ident()
         self._tags: Optional[List[str]] = tags
         self._source_files: Optional[List[str]] = source_files
         self._fail_on_exception: bool = fail_on_exception
         self._capture_traceback: bool = capture_traceback
-        self._git_ref: Optional[GitRef, GitRefDisabled] = git_ref
+        self._git_ref: Optional[GitRef, GitRefDisabled] = git_ref or GitRef()
+        self._dependencies: Optional[str, os.PathLike] = dependencies
 
         self._monitoring_namespace: str = (
             monitoring_namespace
             or os.getenv(MONITORING_NAMESPACE)
             or generate_monitoring_namespace(self._hostname, self._pid, self._tid)
         )
 
@@ -373,16 +388,15 @@
                 container_id=QualifiedName(project_qualified_name + "/" + self._with_id),
                 expected_container_type=Run.container_type,
             )
         else:
             if self._mode == Mode.READ_ONLY:
                 raise NeedExistingRunForReadOnlyMode()
 
-            git_ref = self._git_ref or GitRef()
-            git_info = to_git_info(git_ref=git_ref)
+            git_info = to_git_info(git_ref=self._git_ref)
 
             custom_run_id = self._custom_run_id
             if custom_run_id_exceeds_length(self._custom_run_id):
                 custom_run_id = None
 
             notebook_id, checkpoint_id = create_notebook_checkpoint(backend=self._backend)
 
@@ -447,14 +461,28 @@
         if self._capture_stderr and not self.exists(self._stderr_path):
             self.define(self._stderr_path, StringSeries([]))
 
         if self._with_id is None or self._source_files is not None:
             # upload default sources ONLY if creating a new run
             upload_source_code(source_files=self._source_files, run=self)
 
+        if self._dependencies:
+            if self._dependencies == "infer":
+                dependency_strategy = InferDependenciesStrategy()
+
+            else:
+                dependency_strategy = FileDependenciesStrategy(path=self._dependencies)
+
+            dependency_strategy.log_dependencies(run=self)
+
+        track_uncommitted_changes(
+            git_ref=self._git_ref,
+            run=self,
+        )
+
     @property
     def monitoring_namespace(self) -> str:
         return self._monitoring_namespace
 
     def _raise_if_stopped(self):
         if self._state == ContainerState.STOPPED:
             raise InactiveRunException(label=self._sys_id)
```

### Comparing `neptune-1.2.0/src/neptune/new/__init__.py` & `neptune-1.3.0/src/neptune/new/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/new/_compatibility.py` & `neptune-1.3.0/src/neptune/new/_compatibility.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/new/constants.py` & `neptune-1.3.0/src/neptune/new/constants.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/new/envs.py` & `neptune-1.3.0/src/neptune/new/envs.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/new/exceptions.py` & `neptune-1.3.0/src/neptune/new/exceptions.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/new/handler.py` & `neptune-1.3.0/src/neptune/new/handler.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/new/project.py` & `neptune-1.3.0/src/neptune/new/project.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/new/run.py` & `neptune-1.3.0/src/neptune/new/run.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/new/runs_table.py` & `neptune-1.3.0/src/neptune/new/runs_table.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/new/utils.py` & `neptune-1.3.0/src/neptune/new/utils.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/new/version.py` & `neptune-1.3.0/src/neptune/new/version.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/types/__init__.py` & `neptune-1.3.0/src/neptune/types/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/types/atoms/__init__.py` & `neptune-1.3.0/src/neptune/types/atoms/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/types/atoms/artifact.py` & `neptune-1.3.0/src/neptune/types/atoms/artifact.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/types/atoms/atom.py` & `neptune-1.3.0/src/neptune/types/atoms/atom.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/types/atoms/boolean.py` & `neptune-1.3.0/src/neptune/types/atoms/boolean.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/types/atoms/datetime.py` & `neptune-1.3.0/src/neptune/types/atoms/datetime.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/types/atoms/file.py` & `neptune-1.3.0/src/neptune/types/atoms/file.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/types/atoms/float.py` & `neptune-1.3.0/src/neptune/types/atoms/float.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/types/atoms/git_ref.py` & `neptune-1.3.0/src/neptune/types/atoms/git_ref.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/types/atoms/integer.py` & `neptune-1.3.0/src/neptune/types/atoms/integer.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/types/atoms/string.py` & `neptune-1.3.0/src/neptune/types/atoms/string.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/types/file_set.py` & `neptune-1.3.0/src/neptune/types/file_set.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/types/mode.py` & `neptune-1.3.0/src/neptune/types/mode.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/types/model_version_stage.py` & `neptune-1.3.0/src/neptune/types/model_version_stage.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/types/namespace.py` & `neptune-1.3.0/src/neptune/types/namespace.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/types/series/__init__.py` & `neptune-1.3.0/src/neptune/types/series/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/types/series/file_series.py` & `neptune-1.3.0/src/neptune/types/series/file_series.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/types/series/float_series.py` & `neptune-1.3.0/src/neptune/types/series/float_series.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/types/series/series.py` & `neptune-1.3.0/src/neptune/types/series/series.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/types/series/series_value.py` & `neptune-1.3.0/src/neptune/types/series/series_value.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/types/series/string_series.py` & `neptune-1.3.0/src/neptune/types/series/string_series.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/types/sets/__init__.py` & `neptune-1.3.0/src/neptune/types/sets/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/types/sets/set.py` & `neptune-1.3.0/src/neptune/types/sets/set.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/types/sets/string_set.py` & `neptune-1.3.0/src/neptune/types/sets/string_set.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/types/type_casting.py` & `neptune-1.3.0/src/neptune/types/type_casting.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/types/value.py` & `neptune-1.3.0/src/neptune/types/value.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/types/value_copy.py` & `neptune-1.3.0/src/neptune/types/value_copy.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/types/value_visitor.py` & `neptune-1.3.0/src/neptune/types/value_visitor.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/typing.py` & `neptune-1.3.0/src/neptune/typing.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/utils.py` & `neptune-1.3.0/src/neptune/utils.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/vendor/lib_programname.py` & `neptune-1.3.0/src/neptune/vendor/lib_programname.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/vendor/pynvml.py` & `neptune-1.3.0/src/neptune/vendor/pynvml.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/src/neptune/version.py` & `neptune-1.3.0/src/neptune/version.py`

 * *Files identical despite different names*

### Comparing `neptune-1.2.0/PKG-INFO` & `neptune-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neptune
-Version: 1.2.0
+Version: 1.3.0
 Summary: Neptune Client
 Home-page: https://neptune.ai/
 License: Apache-2.0
 Keywords: MLOps,ML Experiment Tracking,ML Model Registry,ML Model Store,ML Metadata Store
 Author: neptune.ai
 Author-email: contact@neptune.ai
 Requires-Python: >=3.7,<4.0
@@ -44,14 +44,15 @@
 Provides-Extra: transformers
 Provides-Extra: xgboost
 Provides-Extra: zenml
 Requires-Dist: Faker ; extra == "dev"
 Requires-Dist: GitPython (>=2.0.8)
 Requires-Dist: Pillow (>=1.1.6)
 Requires-Dist: PyJWT
+Requires-Dist: accelerate ; extra == "e2e"
 Requires-Dist: altair ; extra == "dev"
 Requires-Dist: bokeh ; extra == "dev"
 Requires-Dist: boto3 (>=1.16.0)
 Requires-Dist: bravado (>=11.0.0,<12.0.0)
 Requires-Dist: click (>=7.0)
 Requires-Dist: freezegun ; extra == "dev"
 Requires-Dist: future (>=0.17.1)
@@ -72,14 +73,15 @@
 Requires-Dist: neptune-sklearn ; extra == "sklearn"
 Requires-Dist: neptune-tensorflow-keras ; extra == "tensorflow-keras"
 Requires-Dist: neptune-xgboost ; extra == "xgboost"
 Requires-Dist: oauthlib (>=2.1.0)
 Requires-Dist: optuna ; extra == "e2e"
 Requires-Dist: packaging
 Requires-Dist: pandas
+Requires-Dist: pipreqs (>=0.4)
 Requires-Dist: plotly ; extra == "dev"
 Requires-Dist: pre-commit ; extra == "dev"
 Requires-Dist: psutil
 Requires-Dist: pytest ; extra == "dev"
 Requires-Dist: pytest-cov ; extra == "dev"
 Requires-Dist: pytest-mock ; extra == "dev"
 Requires-Dist: pytest-timeout ; extra == "dev"
```

