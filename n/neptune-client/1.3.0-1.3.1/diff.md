# Comparing `tmp/neptune_client-1.3.0.tar.gz` & `tmp/neptune_client-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neptune_client-1.3.0.tar", max compression
+gzip compressed data, was "neptune_client-1.3.1.tar", max compression
```

## Comparing `neptune_client-1.3.0.tar` & `neptune_client-1.3.1.tar`

### file list

```diff
@@ -1,324 +1,324 @@
--rw-r--r--   0        0        0    25669 2023-06-15 14:47:16.402540 neptune_client-1.3.0/CHANGELOG.md
--rw-r--r--   0        0        0    11357 2023-06-15 14:47:16.402540 neptune_client-1.3.0/LICENSE
--rw-r--r--   0        0        0    14357 2023-06-15 14:47:16.402540 neptune_client-1.3.0/README.md
--rw-r--r--   0        0        0     4932 2023-06-15 14:47:36.703741 neptune_client-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     3532 2023-06-15 14:47:16.402540 neptune_client-1.3.0/src/neptune/__init__.py
--rw-r--r--   0        0        0     1218 2023-06-15 14:47:16.402540 neptune_client-1.3.0/src/neptune/attributes/__init__.py
--rw-r--r--   0        0        0     1011 2023-06-15 14:47:16.402540 neptune_client-1.3.0/src/neptune/attributes/atoms/__init__.py
--rw-r--r--   0        0        0     3048 2023-06-15 14:47:16.402540 neptune_client-1.3.0/src/neptune/attributes/atoms/artifact.py
--rw-r--r--   0        0        0      701 2023-06-15 14:47:16.402540 neptune_client-1.3.0/src/neptune/attributes/atoms/atom.py
--rw-r--r--   0        0        0     1709 2023-06-15 14:47:16.402540 neptune_client-1.3.0/src/neptune/attributes/atoms/boolean.py
--rw-r--r--   0        0        0     2121 2023-06-15 14:47:16.402540 neptune_client-1.3.0/src/neptune/attributes/atoms/copiable_atom.py
--rw-r--r--   0        0        0     2075 2023-06-15 14:47:16.402540 neptune_client-1.3.0/src/neptune/attributes/atoms/datetime.py
--rw-r--r--   0        0        0     1788 2023-06-15 14:47:16.402540 neptune_client-1.3.0/src/neptune/attributes/atoms/file.py
--rw-r--r--   0        0        0     1704 2023-06-15 14:47:16.402540 neptune_client-1.3.0/src/neptune/attributes/atoms/float.py
--rw-r--r--   0        0        0      696 2023-06-15 14:47:16.402540 neptune_client-1.3.0/src/neptune/attributes/atoms/git_ref.py
--rw-r--r--   0        0        0     2395 2023-06-15 14:47:16.402540 neptune_client-1.3.0/src/neptune/attributes/atoms/integer.py
--rw-r--r--   0        0        0      707 2023-06-15 14:47:16.402540 neptune_client-1.3.0/src/neptune/attributes/atoms/notebook_ref.py
--rw-r--r--   0        0        0      700 2023-06-15 14:47:16.402540 neptune_client-1.3.0/src/neptune/attributes/atoms/run_state.py
--rw-r--r--   0        0        0     2658 2023-06-15 14:47:16.402540 neptune_client-1.3.0/src/neptune/attributes/atoms/string.py
--rw-r--r--   0        0        0     2159 2023-06-15 14:47:16.402540 neptune_client-1.3.0/src/neptune/attributes/attribute.py
--rw-r--r--   0        0        0     2723 2023-06-15 14:47:16.406540 neptune_client-1.3.0/src/neptune/attributes/constants.py
--rw-r--r--   0        0        0     2642 2023-06-15 14:47:16.406540 neptune_client-1.3.0/src/neptune/attributes/file_set.py
--rw-r--r--   0        0        0     4266 2023-06-15 14:47:16.406540 neptune_client-1.3.0/src/neptune/attributes/namespace.py
--rw-r--r--   0        0        0      782 2023-06-15 14:47:16.406540 neptune_client-1.3.0/src/neptune/attributes/series/__init__.py
--rw-r--r--   0        0        0     1949 2023-06-15 14:47:16.406540 neptune_client-1.3.0/src/neptune/attributes/series/fetchable_series.py
--rw-r--r--   0        0        0     4292 2023-06-15 14:47:16.406540 neptune_client-1.3.0/src/neptune/attributes/series/file_series.py
--rw-r--r--   0        0        0     2656 2023-06-15 14:47:16.406540 neptune_client-1.3.0/src/neptune/attributes/series/float_series.py
--rw-r--r--   0        0        0     6003 2023-06-15 14:47:16.406540 neptune_client-1.3.0/src/neptune/attributes/series/series.py
--rw-r--r--   0        0        0     3498 2023-06-15 14:47:16.406540 neptune_client-1.3.0/src/neptune/attributes/series/string_series.py
--rw-r--r--   0        0        0      662 2023-06-15 14:47:16.406540 neptune_client-1.3.0/src/neptune/attributes/sets/__init__.py
--rw-r--r--   0        0        0      699 2023-06-15 14:47:16.406540 neptune_client-1.3.0/src/neptune/attributes/sets/set.py
--rw-r--r--   0        0        0     2627 2023-06-15 14:47:16.406540 neptune_client-1.3.0/src/neptune/attributes/sets/string_set.py
--rw-r--r--   0        0        0     2157 2023-06-15 14:47:16.406540 neptune_client-1.3.0/src/neptune/attributes/utils.py
--rw-r--r--   0        0        0      686 2023-06-15 14:47:16.406540 neptune_client-1.3.0/src/neptune/cli/__init__.py
--rw-r--r--   0        0        0     1017 2023-06-15 14:47:16.406540 neptune_client-1.3.0/src/neptune/cli/__main__.py
--rw-r--r--   0        0        0      866 2023-06-15 14:47:16.406540 neptune_client-1.3.0/src/neptune/cli/abstract_backend_runner.py
--rw-r--r--   0        0        0     3436 2023-06-15 14:47:16.406540 neptune_client-1.3.0/src/neptune/cli/clear.py
--rw-r--r--   0        0        0     5574 2023-06-15 14:47:16.406540 neptune_client-1.3.0/src/neptune/cli/commands.py
--rw-r--r--   0        0        0     2814 2023-06-15 14:47:16.406540 neptune_client-1.3.0/src/neptune/cli/container_manager.py
--rw-r--r--   0        0        0     1947 2023-06-15 14:47:16.406540 neptune_client-1.3.0/src/neptune/cli/path_option.py
--rw-r--r--   0        0        0     3899 2023-06-15 14:47:16.406540 neptune_client-1.3.0/src/neptune/cli/status.py
--rw-r--r--   0        0        0     9995 2023-06-15 14:47:16.406540 neptune_client-1.3.0/src/neptune/cli/sync.py
--rw-r--r--   0        0        0     5028 2023-06-15 14:47:16.406540 neptune_client-1.3.0/src/neptune/cli/utils.py
--rw-r--r--   0        0        0      596 2023-06-15 14:47:16.406540 neptune_client-1.3.0/src/neptune/common/__init__.py
--rw-r--r--   0        0        0      596 2023-06-15 14:47:16.406540 neptune_client-1.3.0/src/neptune/common/backends/__init__.py
--rw-r--r--   0        0        0     1038 2023-06-15 14:47:16.406540 neptune_client-1.3.0/src/neptune/common/backends/api_model.py
--rw-r--r--   0        0        0     4230 2023-06-15 14:47:16.406540 neptune_client-1.3.0/src/neptune/common/backends/utils.py
--rw-r--r--   0        0        0      859 2023-06-15 14:47:16.406540 neptune_client-1.3.0/src/neptune/common/envs.py
--rw-r--r--   0        0        0    14106 2023-06-15 14:47:16.406540 neptune_client-1.3.0/src/neptune/common/exceptions.py
--rw-r--r--   0        0        0      629 2023-06-15 14:47:16.406540 neptune_client-1.3.0/src/neptune/common/experiments.py
--rw-r--r--   0        0        0     2490 2023-06-15 14:47:16.406540 neptune_client-1.3.0/src/neptune/common/git_info.py
--rw-r--r--   0        0        0      596 2023-06-15 14:47:16.406540 neptune_client-1.3.0/src/neptune/common/hardware/__init__.py
--rw-r--r--   0        0        0      596 2023-06-15 14:47:16.406540 neptune_client-1.3.0/src/neptune/common/hardware/cgroup/__init__.py
--rw-r--r--   0        0        0     2638 2023-06-15 14:47:16.406540 neptune_client-1.3.0/src/neptune/common/hardware/cgroup/cgroup_filesystem_reader.py
--rw-r--r--   0        0        0     3212 2023-06-15 14:47:16.406540 neptune_client-1.3.0/src/neptune/common/hardware/cgroup/cgroup_monitor.py
--rw-r--r--   0        0        0      694 2023-06-15 14:47:16.406540 neptune_client-1.3.0/src/neptune/common/hardware/constants.py
--rw-r--r--   0        0        0      596 2023-06-15 14:47:16.406540 neptune_client-1.3.0/src/neptune/common/hardware/gauges/__init__.py
--rw-r--r--   0        0        0     1554 2023-06-15 14:47:16.406540 neptune_client-1.3.0/src/neptune/common/hardware/gauges/cpu.py
--rw-r--r--   0        0        0      979 2023-06-15 14:47:16.406540 neptune_client-1.3.0/src/neptune/common/hardware/gauges/gauge.py
--rw-r--r--   0        0        0     2023 2023-06-15 14:47:16.406540 neptune_client-1.3.0/src/neptune/common/hardware/gauges/gauge_factory.py
--rw-r--r--   0        0        0      667 2023-06-15 14:47:16.406540 neptune_client-1.3.0/src/neptune/common/hardware/gauges/gauge_mode.py
--rw-r--r--   0        0        0     1766 2023-06-15 14:47:16.406540 neptune_client-1.3.0/src/neptune/common/hardware/gauges/gpu.py
--rw-r--r--   0        0        0     1748 2023-06-15 14:47:16.406540 neptune_client-1.3.0/src/neptune/common/hardware/gauges/memory.py
--rw-r--r--   0        0        0      596 2023-06-15 14:47:16.406540 neptune_client-1.3.0/src/neptune/common/hardware/gpu/__init__.py
--rw-r--r--   0        0        0     2568 2023-06-15 14:47:16.406540 neptune_client-1.3.0/src/neptune/common/hardware/gpu/gpu_monitor.py
--rw-r--r--   0        0        0      596 2023-06-15 14:47:16.406540 neptune_client-1.3.0/src/neptune/common/hardware/metrics/__init__.py
--rw-r--r--   0        0        0     2432 2023-06-15 14:47:16.406540 neptune_client-1.3.0/src/neptune/common/hardware/metrics/metric.py
--rw-r--r--   0        0        0     1216 2023-06-15 14:47:16.406540 neptune_client-1.3.0/src/neptune/common/hardware/metrics/metrics_container.py
--rw-r--r--   0        0        0     3490 2023-06-15 14:47:16.406540 neptune_client-1.3.0/src/neptune/common/hardware/metrics/metrics_factory.py
--rw-r--r--   0        0        0      596 2023-06-15 14:47:16.406540 neptune_client-1.3.0/src/neptune/common/hardware/metrics/reports/__init__.py
--rw-r--r--   0        0        0      792 2023-06-15 14:47:16.406540 neptune_client-1.3.0/src/neptune/common/hardware/metrics/reports/metric_report.py
--rw-r--r--   0        0        0     1679 2023-06-15 14:47:16.406540 neptune_client-1.3.0/src/neptune/common/hardware/metrics/reports/metric_reporter.py
--rw-r--r--   0        0        0      947 2023-06-15 14:47:16.406540 neptune_client-1.3.0/src/neptune/common/hardware/metrics/reports/metric_reporter_factory.py
--rw-r--r--   0        0        0      596 2023-06-15 14:47:16.406540 neptune_client-1.3.0/src/neptune/common/hardware/metrics/service/__init__.py
--rw-r--r--   0        0        0     1106 2023-06-15 14:47:16.406540 neptune_client-1.3.0/src/neptune/common/hardware/metrics/service/metric_service.py
--rw-r--r--   0        0        0     2309 2023-06-15 14:47:16.410540 neptune_client-1.3.0/src/neptune/common/hardware/metrics/service/metric_service_factory.py
--rw-r--r--   0        0        0      596 2023-06-15 14:47:16.410540 neptune_client-1.3.0/src/neptune/common/hardware/resources/__init__.py
--rw-r--r--   0        0        0     1821 2023-06-15 14:47:16.410540 neptune_client-1.3.0/src/neptune/common/hardware/resources/gpu_card_indices_provider.py
--rw-r--r--   0        0        0     1574 2023-06-15 14:47:16.410540 neptune_client-1.3.0/src/neptune/common/hardware/resources/system_resource_info.py
--rw-r--r--   0        0        0     2504 2023-06-15 14:47:16.410540 neptune_client-1.3.0/src/neptune/common/hardware/resources/system_resource_info_factory.py
--rw-r--r--   0        0        0      596 2023-06-15 14:47:16.410540 neptune_client-1.3.0/src/neptune/common/hardware/system/__init__.py
--rw-r--r--   0        0        0      964 2023-06-15 14:47:16.410540 neptune_client-1.3.0/src/neptune/common/hardware/system/system_monitor.py
--rw-r--r--   0        0        0     4772 2023-06-15 14:47:16.410540 neptune_client-1.3.0/src/neptune/common/oauth.py
--rw-r--r--   0        0        0      884 2023-06-15 14:47:16.410540 neptune_client-1.3.0/src/neptune/common/patches/__init__.py
--rw-r--r--   0        0        0     2731 2023-06-15 14:47:16.410540 neptune_client-1.3.0/src/neptune/common/patches/bravado.py
--rw-r--r--   0        0        0      726 2023-06-15 14:47:16.410540 neptune_client-1.3.0/src/neptune/common/patterns.py
--rw-r--r--   0        0        0      596 2023-06-15 14:47:16.410540 neptune_client-1.3.0/src/neptune/common/storage/__init__.py
--rw-r--r--   0        0        0     3223 2023-06-15 14:47:16.410540 neptune_client-1.3.0/src/neptune/common/storage/datastream.py
--rw-r--r--   0        0        0     7335 2023-06-15 14:47:16.410540 neptune_client-1.3.0/src/neptune/common/storage/storage_utils.py
--rw-r--r--   0        0        0     7075 2023-06-15 14:47:16.410540 neptune_client-1.3.0/src/neptune/common/utils.py
--rw-r--r--   0        0        0     2206 2023-06-15 14:47:16.410540 neptune_client-1.3.0/src/neptune/common/warnings.py
--rw-r--r--   0        0        0      596 2023-06-15 14:47:16.410540 neptune_client-1.3.0/src/neptune/common/websockets/__init__.py
--rw-r--r--   0        0        0     3589 2023-06-15 14:47:16.410540 neptune_client-1.3.0/src/neptune/common/websockets/reconnecting_websocket.py
--rw-r--r--   0        0        0     2693 2023-06-15 14:47:16.410540 neptune_client-1.3.0/src/neptune/common/websockets/websocket_client_adapter.py
--rw-r--r--   0        0        0      985 2023-06-15 14:47:16.410540 neptune_client-1.3.0/src/neptune/constants.py
--rw-r--r--   0        0        0     1863 2023-06-15 14:47:16.410540 neptune_client-1.3.0/src/neptune/envs.py
--rw-r--r--   0        0        0    41966 2023-06-15 14:47:16.410540 neptune_client-1.3.0/src/neptune/exceptions.py
--rw-r--r--   0        0        0    29698 2023-06-15 14:47:16.410540 neptune_client-1.3.0/src/neptune/handler.py
--rw-r--r--   0        0        0      596 2023-06-15 14:47:16.410540 neptune_client-1.3.0/src/neptune/integrations/__init__.py
--rw-r--r--   0        0        0      973 2023-06-15 14:47:16.410540 neptune_client-1.3.0/src/neptune/integrations/aws/__init__.py
--rw-r--r--   0        0        0     1014 2023-06-15 14:47:16.410540 neptune_client-1.3.0/src/neptune/integrations/detectron2/__init__.py
--rw-r--r--   0        0        0      985 2023-06-15 14:47:16.410540 neptune_client-1.3.0/src/neptune/integrations/fastai/__init__.py
--rw-r--r--   0        0        0      976 2023-06-15 14:47:16.410540 neptune_client-1.3.0/src/neptune/integrations/kedro/__init__.py
--rw-r--r--   0        0        0      993 2023-06-15 14:47:16.410540 neptune_client-1.3.0/src/neptune/integrations/lightgbm/__init__.py
--rw-r--r--   0        0        0      985 2023-06-15 14:47:16.410540 neptune_client-1.3.0/src/neptune/integrations/optuna/__init__.py
--rw-r--r--   0        0        0      989 2023-06-15 14:47:16.410540 neptune_client-1.3.0/src/neptune/integrations/prophet/__init__.py
--rw-r--r--   0        0        0     3084 2023-06-15 14:47:16.410540 neptune_client-1.3.0/src/neptune/integrations/python_logger.py
--rw-r--r--   0        0        0     1006 2023-06-15 14:47:16.410540 neptune_client-1.3.0/src/neptune/integrations/pytorch/__init__.py
--rw-r--r--   0        0        0     1042 2023-06-15 14:47:16.410540 neptune_client-1.3.0/src/neptune/integrations/pytorch_lightning/__init__.py
--rw-r--r--   0        0        0      985 2023-06-15 14:47:16.410540 neptune_client-1.3.0/src/neptune/integrations/sacred/__init__.py
--rw-r--r--   0        0        0      989 2023-06-15 14:47:16.410540 neptune_client-1.3.0/src/neptune/integrations/sklearn/__init__.py
--rw-r--r--   0        0        0     1038 2023-06-15 14:47:16.410540 neptune_client-1.3.0/src/neptune/integrations/tensorflow_keras/__init__.py
--rw-r--r--   0        0        0     1032 2023-06-15 14:47:16.410540 neptune_client-1.3.0/src/neptune/integrations/transformers/__init__.py
--rw-r--r--   0        0        0     1164 2023-06-15 14:47:16.410540 neptune_client-1.3.0/src/neptune/integrations/utils.py
--rw-r--r--   0        0        0      989 2023-06-15 14:47:16.410540 neptune_client-1.3.0/src/neptune/integrations/xgboost/__init__.py
--rw-r--r--   0        0        0      596 2023-06-15 14:47:16.410540 neptune_client-1.3.0/src/neptune/internal/__init__.py
--rw-r--r--   0        0        0      760 2023-06-15 14:47:16.410540 neptune_client-1.3.0/src/neptune/internal/artifacts/__init__.py
--rw-r--r--   0        0        0      791 2023-06-15 14:47:16.410540 neptune_client-1.3.0/src/neptune/internal/artifacts/drivers/__init__.py
--rw-r--r--   0        0        0     4240 2023-06-15 14:47:16.410540 neptune_client-1.3.0/src/neptune/internal/artifacts/drivers/local.py
--rw-r--r--   0        0        0     4810 2023-06-15 14:47:16.410540 neptune_client-1.3.0/src/neptune/internal/artifacts/drivers/s3.py
--rw-r--r--   0        0        0     4017 2023-06-15 14:47:16.410540 neptune_client-1.3.0/src/neptune/internal/artifacts/file_hasher.py
--rw-r--r--   0        0        0     2318 2023-06-15 14:47:16.410540 neptune_client-1.3.0/src/neptune/internal/artifacts/local_file_hash_storage.py
--rw-r--r--   0        0        0     3578 2023-06-15 14:47:16.410540 neptune_client-1.3.0/src/neptune/internal/artifacts/types.py
--rw-r--r--   0        0        0      999 2023-06-15 14:47:16.414540 neptune_client-1.3.0/src/neptune/internal/artifacts/utils.py
--rw-r--r--   0        0        0      596 2023-06-15 14:47:16.414540 neptune_client-1.3.0/src/neptune/internal/backends/__init__.py
--rw-r--r--   0        0        0     7169 2023-06-15 14:47:16.414540 neptune_client-1.3.0/src/neptune/internal/backends/api_model.py
--rw-r--r--   0        0        0     1703 2023-06-15 14:47:16.414540 neptune_client-1.3.0/src/neptune/internal/backends/factory.py
--rw-r--r--   0        0        0     6700 2023-06-15 14:47:16.414540 neptune_client-1.3.0/src/neptune/internal/backends/hosted_artifact_operations.py
--rw-r--r--   0        0        0     5942 2023-06-15 14:47:16.414540 neptune_client-1.3.0/src/neptune/internal/backends/hosted_client.py
--rw-r--r--   0        0        0    17136 2023-06-15 14:47:16.414540 neptune_client-1.3.0/src/neptune/internal/backends/hosted_file_operations.py
--rw-r--r--   0        0        0    40705 2023-06-15 14:47:16.414540 neptune_client-1.3.0/src/neptune/internal/backends/hosted_neptune_backend.py
--rw-r--r--   0        0        0     8506 2023-06-15 14:47:16.414540 neptune_client-1.3.0/src/neptune/internal/backends/neptune_backend.py
--rw-r--r--   0        0        0    31714 2023-06-15 14:47:16.414540 neptune_client-1.3.0/src/neptune/internal/backends/neptune_backend_mock.py
--rw-r--r--   0        0        0     1942 2023-06-15 14:47:16.414540 neptune_client-1.3.0/src/neptune/internal/backends/nql.py
--rw-r--r--   0        0        0     4471 2023-06-15 14:47:16.414540 neptune_client-1.3.0/src/neptune/internal/backends/offline_neptune_backend.py
--rw-r--r--   0        0        0     3946 2023-06-15 14:47:16.414540 neptune_client-1.3.0/src/neptune/internal/backends/operation_api_name_visitor.py
--rw-r--r--   0        0        0     5003 2023-06-15 14:47:16.414540 neptune_client-1.3.0/src/neptune/internal/backends/operation_api_object_converter.py
--rw-r--r--   0        0        0    13841 2023-06-15 14:47:16.414540 neptune_client-1.3.0/src/neptune/internal/backends/operations_preprocessor.py
--rw-r--r--   0        0        0     1619 2023-06-15 14:47:16.414540 neptune_client-1.3.0/src/neptune/internal/backends/project_name_lookup.py
--rw-r--r--   0        0        0     5246 2023-06-15 14:47:16.414540 neptune_client-1.3.0/src/neptune/internal/backends/swagger_client_wrapper.py
--rw-r--r--   0        0        0     8765 2023-06-15 14:47:16.414540 neptune_client-1.3.0/src/neptune/internal/backends/utils.py
--rw-r--r--   0        0        0     1381 2023-06-15 14:47:16.414540 neptune_client-1.3.0/src/neptune/internal/backgroud_job_list.py
--rw-r--r--   0        0        0     1035 2023-06-15 14:47:16.414540 neptune_client-1.3.0/src/neptune/internal/background_job.py
--rw-r--r--   0        0        0      350 2023-06-15 14:47:16.414540 neptune_client-1.3.0/src/neptune/internal/constants.py
--rw-r--r--   0        0        0     4486 2023-06-15 14:47:16.414540 neptune_client-1.3.0/src/neptune/internal/container_structure.py
--rw-r--r--   0        0        0     1302 2023-06-15 14:47:16.414540 neptune_client-1.3.0/src/neptune/internal/container_type.py
--rw-r--r--   0        0        0     2345 2023-06-15 14:47:16.414540 neptune_client-1.3.0/src/neptune/internal/credentials.py
--rw-r--r--   0        0        0     8468 2023-06-15 14:47:16.414540 neptune_client-1.3.0/src/neptune/internal/disk_queue.py
--rw-r--r--   0        0        0      689 2023-06-15 14:47:16.414540 neptune_client-1.3.0/src/neptune/internal/exceptions.py
--rw-r--r--   0        0        0      596 2023-06-15 14:47:16.414540 neptune_client-1.3.0/src/neptune/internal/hardware/__init__.py
--rw-r--r--   0        0        0      596 2023-06-15 14:47:16.414540 neptune_client-1.3.0/src/neptune/internal/hardware/gpu/__init__.py
--rw-r--r--   0        0        0     2466 2023-06-15 14:47:16.414540 neptune_client-1.3.0/src/neptune/internal/hardware/gpu/gpu_monitor.py
--rw-r--r--   0        0        0     4997 2023-06-15 14:47:16.414540 neptune_client-1.3.0/src/neptune/internal/hardware/hardware_metric_reporting_job.py
--rw-r--r--   0        0        0      933 2023-06-15 14:47:16.414540 neptune_client-1.3.0/src/neptune/internal/id_formats.py
--rw-r--r--   0        0        0      596 2023-06-15 14:47:16.414540 neptune_client-1.3.0/src/neptune/internal/init/__init__.py
--rw-r--r--   0        0        0      796 2023-06-15 14:47:16.414540 neptune_client-1.3.0/src/neptune/internal/init/parameters.py
--rw-r--r--   0        0        0      596 2023-06-15 14:47:16.414540 neptune_client-1.3.0/src/neptune/internal/notebooks/__init__.py
--rw-r--r--   0        0        0     1572 2023-06-15 14:47:16.414540 neptune_client-1.3.0/src/neptune/internal/notebooks/comm.py
--rw-r--r--   0        0        0     1831 2023-06-15 14:47:16.414540 neptune_client-1.3.0/src/neptune/internal/notebooks/notebooks.py
--rw-r--r--   0        0        0    17310 2023-06-15 14:47:16.414540 neptune_client-1.3.0/src/neptune/internal/operation.py
--rw-r--r--   0        0        0      596 2023-06-15 14:47:16.414540 neptune_client-1.3.0/src/neptune/internal/operation_processors/__init__.py
--rw-r--r--   0        0        0    10851 2023-06-15 14:47:16.414540 neptune_client-1.3.0/src/neptune/internal/operation_processors/async_operation_processor.py
--rw-r--r--   0        0        0     2177 2023-06-15 14:47:16.414540 neptune_client-1.3.0/src/neptune/internal/operation_processors/factory.py
--rw-r--r--   0        0        0     2136 2023-06-15 14:47:16.414540 neptune_client-1.3.0/src/neptune/internal/operation_processors/offline_operation_processor.py
--rw-r--r--   0        0        0     1140 2023-06-15 14:47:16.414540 neptune_client-1.3.0/src/neptune/internal/operation_processors/operation_processor.py
--rw-r--r--   0        0        0     1998 2023-06-15 14:47:16.414540 neptune_client-1.3.0/src/neptune/internal/operation_processors/operation_storage.py
--rw-r--r--   0        0        0     1577 2023-06-15 14:47:16.414540 neptune_client-1.3.0/src/neptune/internal/operation_processors/read_only_operation_processor.py
--rw-r--r--   0        0        0     2483 2023-06-15 14:47:16.414540 neptune_client-1.3.0/src/neptune/internal/operation_processors/sync_operation_processor.py
--rw-r--r--   0        0        0     3724 2023-06-15 14:47:16.414540 neptune_client-1.3.0/src/neptune/internal/operation_visitor.py
--rw-r--r--   0        0        0      776 2023-06-15 14:47:16.414540 neptune_client-1.3.0/src/neptune/internal/state.py
--rw-r--r--   0        0        0      596 2023-06-15 14:47:16.414540 neptune_client-1.3.0/src/neptune/internal/streams/__init__.py
--rw-r--r--   0        0        0     1815 2023-06-15 14:47:16.414540 neptune_client-1.3.0/src/neptune/internal/streams/std_capture_background_job.py
--rw-r--r--   0        0        0     2418 2023-06-15 14:47:16.414540 neptune_client-1.3.0/src/neptune/internal/streams/std_stream_capture_logger.py
--rw-r--r--   0        0        0      596 2023-06-15 14:47:16.414540 neptune_client-1.3.0/src/neptune/internal/threading/__init__.py
--rw-r--r--   0        0        0     3567 2023-06-15 14:47:16.414540 neptune_client-1.3.0/src/neptune/internal/threading/daemon.py
--rw-r--r--   0        0        0      596 2023-06-15 14:47:16.414540 neptune_client-1.3.0/src/neptune/internal/types/__init__.py
--rw-r--r--   0        0        0     4584 2023-06-15 14:47:16.414540 neptune_client-1.3.0/src/neptune/internal/types/file_types.py
--rw-r--r--   0        0        0     1665 2023-06-15 14:47:16.414540 neptune_client-1.3.0/src/neptune/internal/types/stringify_value.py
--rw-r--r--   0        0        0     4856 2023-06-15 14:47:16.414540 neptune_client-1.3.0/src/neptune/internal/utils/__init__.py
--rw-r--r--   0        0        0     1171 2023-06-15 14:47:16.414540 neptune_client-1.3.0/src/neptune/internal/utils/dependency_tracking.py
--rw-r--r--   0        0        0     2114 2023-06-15 14:47:16.414540 neptune_client-1.3.0/src/neptune/internal/utils/deprecation.py
--rw-r--r--   0        0        0     2374 2023-06-15 14:47:16.414540 neptune_client-1.3.0/src/neptune/internal/utils/generic_attribute_mapper.py
--rw-r--r--   0        0        0     5537 2023-06-15 14:47:16.414540 neptune_client-1.3.0/src/neptune/internal/utils/git.py
--rw-r--r--   0        0        0      849 2023-06-15 14:47:16.414540 neptune_client-1.3.0/src/neptune/internal/utils/hashing.py
--rw-r--r--   0        0        0     9732 2023-06-15 14:47:16.414540 neptune_client-1.3.0/src/neptune/internal/utils/images.py
--rw-r--r--   0        0        0     1288 2023-06-15 14:47:16.418541 neptune_client-1.3.0/src/neptune/internal/utils/iteration.py
--rw-r--r--   0        0        0     3053 2023-06-15 14:47:16.418541 neptune_client-1.3.0/src/neptune/internal/utils/json_file_splitter.py
--rw-r--r--   0        0        0     1633 2023-06-15 14:47:16.418541 neptune_client-1.3.0/src/neptune/internal/utils/limits.py
--rw-r--r--   0        0        0     1488 2023-06-15 14:47:16.418541 neptune_client-1.3.0/src/neptune/internal/utils/logger.py
--rw-r--r--   0        0        0     1042 2023-06-15 14:47:16.418541 neptune_client-1.3.0/src/neptune/internal/utils/paths.py
--rw-r--r--   0        0        0     2049 2023-06-15 14:47:16.418541 neptune_client-1.3.0/src/neptune/internal/utils/ping_background_job.py
--rw-r--r--   0        0        0     1809 2023-06-15 14:47:16.418541 neptune_client-1.3.0/src/neptune/internal/utils/process_killer.py
--rw-r--r--   0        0        0     1564 2023-06-15 14:47:16.418541 neptune_client-1.3.0/src/neptune/internal/utils/run_state.py
--rw-r--r--   0        0        0     1207 2023-06-15 14:47:16.418541 neptune_client-1.3.0/src/neptune/internal/utils/runningmode.py
--rw-r--r--   0        0        0     1340 2023-06-15 14:47:16.418541 neptune_client-1.3.0/src/neptune/internal/utils/s3.py
--rw-r--r--   0        0        0     2270 2023-06-15 14:47:16.418541 neptune_client-1.3.0/src/neptune/internal/utils/source_code.py
--rw-r--r--   0        0        0     1457 2023-06-15 14:47:16.418541 neptune_client-1.3.0/src/neptune/internal/utils/sync_offset_file.py
--rw-r--r--   0        0        0     1927 2023-06-15 14:47:16.418541 neptune_client-1.3.0/src/neptune/internal/utils/traceback_job.py
--rw-r--r--   0        0        0     2426 2023-06-15 14:47:16.418541 neptune_client-1.3.0/src/neptune/internal/utils/uncaught_exception_handler.py
--rw-r--r--   0        0        0     4462 2023-06-15 14:47:16.418541 neptune_client-1.3.0/src/neptune/internal/value_to_attribute_visitor.py
--rw-r--r--   0        0        0      596 2023-06-15 14:47:16.418541 neptune_client-1.3.0/src/neptune/internal/websockets/__init__.py
--rw-r--r--   0        0        0     5188 2023-06-15 14:47:16.418541 neptune_client-1.3.0/src/neptune/internal/websockets/websocket_signals_background_job.py
--rw-r--r--   0        0        0     1229 2023-06-15 14:47:16.418541 neptune_client-1.3.0/src/neptune/internal/websockets/websockets_factory.py
--rw-r--r--   0        0        0    13821 2023-06-15 14:47:16.418541 neptune_client-1.3.0/src/neptune/legacy/__init__.py
--rw-r--r--   0        0        0    11218 2023-06-15 14:47:16.418541 neptune_client-1.3.0/src/neptune/legacy/api_exceptions.py
--rw-r--r--   0        0        0     4710 2023-06-15 14:47:16.418541 neptune_client-1.3.0/src/neptune/legacy/backend.py
--rw-r--r--   0        0        0      737 2023-06-15 14:47:16.418541 neptune_client-1.3.0/src/neptune/legacy/checkpoint.py
--rw-r--r--   0        0        0      859 2023-06-15 14:47:16.418541 neptune_client-1.3.0/src/neptune/legacy/constants.py
--rw-r--r--   0        0        0      860 2023-06-15 14:47:16.418541 neptune_client-1.3.0/src/neptune/legacy/envs.py
--rw-r--r--   0        0        0    12780 2023-06-15 14:47:16.418541 neptune_client-1.3.0/src/neptune/legacy/exceptions.py
--rw-r--r--   0        0        0    42888 2023-06-15 14:47:16.418541 neptune_client-1.3.0/src/neptune/legacy/experiments.py
--rw-r--r--   0        0        0      663 2023-06-15 14:47:16.418541 neptune_client-1.3.0/src/neptune/legacy/git_info.py
--rw-r--r--   0        0        0      596 2023-06-15 14:47:16.418541 neptune_client-1.3.0/src/neptune/legacy/internal/__init__.py
--rw-r--r--   0        0        0     1999 2023-06-15 14:47:16.418541 neptune_client-1.3.0/src/neptune/legacy/internal/abort.py
--rw-r--r--   0        0        0      888 2023-06-15 14:47:16.418541 neptune_client-1.3.0/src/neptune/legacy/internal/api_clients/__init__.py
--rw-r--r--   0        0        0     1148 2023-06-15 14:47:16.418541 neptune_client-1.3.0/src/neptune/legacy/internal/api_clients/backend_factory.py
--rw-r--r--   0        0        0     1826 2023-06-15 14:47:16.418541 neptune_client-1.3.0/src/neptune/legacy/internal/api_clients/client_config.py
--rw-r--r--   0        0        0     3103 2023-06-15 14:47:16.418541 neptune_client-1.3.0/src/neptune/legacy/internal/api_clients/credentials.py
--rw-r--r--   0        0        0      596 2023-06-15 14:47:16.418541 neptune_client-1.3.0/src/neptune/legacy/internal/api_clients/hosted_api_clients/__init__.py
--rw-r--r--   0        0        0    46556 2023-06-15 14:47:16.418541 neptune_client-1.3.0/src/neptune/legacy/internal/api_clients/hosted_api_clients/hosted_alpha_leaderboard_api_client.py
--rw-r--r--   0        0        0     8710 2023-06-15 14:47:16.418541 neptune_client-1.3.0/src/neptune/legacy/internal/api_clients/hosted_api_clients/hosted_backend_api_client.py
--rw-r--r--   0        0        0     4456 2023-06-15 14:47:16.418541 neptune_client-1.3.0/src/neptune/legacy/internal/api_clients/hosted_api_clients/mixins.py
--rw-r--r--   0        0        0     3857 2023-06-15 14:47:16.418541 neptune_client-1.3.0/src/neptune/legacy/internal/api_clients/hosted_api_clients/utils.py
--rw-r--r--   0        0        0     4631 2023-06-15 14:47:16.418541 neptune_client-1.3.0/src/neptune/legacy/internal/api_clients/offline_backend.py
--rw-r--r--   0        0        0      596 2023-06-15 14:47:16.418541 neptune_client-1.3.0/src/neptune/legacy/internal/backends/__init__.py
--rw-r--r--   0        0        0      776 2023-06-15 14:47:16.418541 neptune_client-1.3.0/src/neptune/legacy/internal/backends/hosted_neptune_backend.py
--rw-r--r--   0        0        0      596 2023-06-15 14:47:16.418541 neptune_client-1.3.0/src/neptune/legacy/internal/channels/__init__.py
--rw-r--r--   0        0        0     3903 2023-06-15 14:47:16.418541 neptune_client-1.3.0/src/neptune/legacy/internal/channels/channels.py
--rw-r--r--   0        0        0     7087 2023-06-15 14:47:16.418541 neptune_client-1.3.0/src/neptune/legacy/internal/channels/channels_values_sender.py
--rw-r--r--   0        0        0      596 2023-06-15 14:47:16.418541 neptune_client-1.3.0/src/neptune/legacy/internal/execution/__init__.py
--rw-r--r--   0        0        0     6126 2023-06-15 14:47:16.418541 neptune_client-1.3.0/src/neptune/legacy/internal/execution/execution_context.py
--rw-r--r--   0        0        0      596 2023-06-15 14:47:16.418541 neptune_client-1.3.0/src/neptune/legacy/internal/experiments/__init__.py
--rw-r--r--   0        0        0      596 2023-06-15 14:47:16.422541 neptune_client-1.3.0/src/neptune/legacy/internal/notebooks/__init__.py
--rw-r--r--   0        0        0     1510 2023-06-15 14:47:16.422541 neptune_client-1.3.0/src/neptune/legacy/internal/notebooks/comm.py
--rw-r--r--   0        0        0     1711 2023-06-15 14:47:16.422541 neptune_client-1.3.0/src/neptune/legacy/internal/notebooks/notebooks.py
--rw-r--r--   0        0        0      596 2023-06-15 14:47:16.422541 neptune_client-1.3.0/src/neptune/legacy/internal/streams/__init__.py
--rw-r--r--   0        0        0     2805 2023-06-15 14:47:16.422541 neptune_client-1.3.0/src/neptune/legacy/internal/streams/channel_writer.py
--rw-r--r--   0        0        0     1945 2023-06-15 14:47:16.422541 neptune_client-1.3.0/src/neptune/legacy/internal/streams/stdstream_uploader.py
--rw-r--r--   0        0        0      596 2023-06-15 14:47:16.422541 neptune_client-1.3.0/src/neptune/legacy/internal/threads/__init__.py
--rw-r--r--   0        0        0     2363 2023-06-15 14:47:16.422541 neptune_client-1.3.0/src/neptune/legacy/internal/threads/aborting_thread.py
--rw-r--r--   0        0        0     1816 2023-06-15 14:47:16.422541 neptune_client-1.3.0/src/neptune/legacy/internal/threads/hardware_metric_reporting_thread.py
--rw-r--r--   0        0        0     1334 2023-06-15 14:47:16.422541 neptune_client-1.3.0/src/neptune/legacy/internal/threads/neptune_thread.py
--rw-r--r--   0        0        0     1556 2023-06-15 14:47:16.422541 neptune_client-1.3.0/src/neptune/legacy/internal/threads/ping_thread.py
--rw-r--r--   0        0        0      596 2023-06-15 14:47:16.422541 neptune_client-1.3.0/src/neptune/legacy/internal/utils/__init__.py
--rw-r--r--   0        0        0     8091 2023-06-15 14:47:16.422541 neptune_client-1.3.0/src/neptune/legacy/internal/utils/alpha_integration.py
--rw-r--r--   0        0        0      997 2023-06-15 14:47:16.422541 neptune_client-1.3.0/src/neptune/legacy/internal/utils/deprecation.py
--rw-r--r--   0        0        0     2597 2023-06-15 14:47:16.422541 neptune_client-1.3.0/src/neptune/legacy/internal/utils/http.py
--rw-r--r--   0        0        0     2597 2023-06-15 14:47:16.422541 neptune_client-1.3.0/src/neptune/legacy/internal/utils/http_utils.py
--rw-r--r--   0        0        0     2990 2023-06-15 14:47:16.422541 neptune_client-1.3.0/src/neptune/legacy/internal/utils/image.py
--rw-r--r--   0        0        0     3145 2023-06-15 14:47:16.422541 neptune_client-1.3.0/src/neptune/legacy/internal/utils/source_code.py
--rw-r--r--   0        0        0      596 2023-06-15 14:47:16.422541 neptune_client-1.3.0/src/neptune/legacy/internal/websockets/__init__.py
--rw-r--r--   0        0        0     3542 2023-06-15 14:47:16.422541 neptune_client-1.3.0/src/neptune/legacy/internal/websockets/message.py
--rw-r--r--   0        0        0     1097 2023-06-15 14:47:16.422541 neptune_client-1.3.0/src/neptune/legacy/internal/websockets/reconnecting_websocket_factory.py
--rw-r--r--   0        0        0     1228 2023-06-15 14:47:16.422541 neptune_client-1.3.0/src/neptune/legacy/internal/websockets/websocket_message_processor.py
--rw-r--r--   0        0        0     3938 2023-06-15 14:47:16.422541 neptune_client-1.3.0/src/neptune/legacy/model.py
--rw-r--r--   0        0        0     2807 2023-06-15 14:47:16.422541 neptune_client-1.3.0/src/neptune/legacy/notebook.py
--rw-r--r--   0        0        0      691 2023-06-15 14:47:16.422541 neptune_client-1.3.0/src/neptune/legacy/oauth.py
--rw-r--r--   0        0        0      678 2023-06-15 14:47:16.422541 neptune_client-1.3.0/src/neptune/legacy/patterns.py
--rw-r--r--   0        0        0    26377 2023-06-15 14:47:16.422541 neptune_client-1.3.0/src/neptune/legacy/projects.py
--rw-r--r--   0        0        0     8992 2023-06-15 14:47:16.422541 neptune_client-1.3.0/src/neptune/legacy/sessions.py
--rw-r--r--   0        0        0     1162 2023-06-15 14:47:16.422541 neptune_client-1.3.0/src/neptune/legacy/utils.py
--rw-r--r--   0        0        0      660 2023-06-15 14:47:16.422541 neptune_client-1.3.0/src/neptune/logging/__init__.py
--rw-r--r--   0        0        0      976 2023-06-15 14:47:16.422541 neptune_client-1.3.0/src/neptune/logging/logger.py
--rw-r--r--   0        0        0     4454 2023-06-15 14:47:16.422541 neptune_client-1.3.0/src/neptune/management/__init__.py
--rw-r--r--   0        0        0     6943 2023-06-15 14:47:16.422541 neptune_client-1.3.0/src/neptune/management/exceptions.py
--rw-r--r--   0        0        0      596 2023-06-15 14:47:16.422541 neptune_client-1.3.0/src/neptune/management/internal/__init__.py
--rw-r--r--   0        0        0    36941 2023-06-15 14:47:16.422541 neptune_client-1.3.0/src/neptune/management/internal/api.py
--rw-r--r--   0        0        0     2853 2023-06-15 14:47:16.422541 neptune_client-1.3.0/src/neptune/management/internal/dto.py
--rw-r--r--   0        0        0     1069 2023-06-15 14:47:16.422541 neptune_client-1.3.0/src/neptune/management/internal/types.py
--rw-r--r--   0        0        0     2013 2023-06-15 14:47:16.422541 neptune_client-1.3.0/src/neptune/management/internal/utils.py
--rw-r--r--   0        0        0      995 2023-06-15 14:47:16.422541 neptune_client-1.3.0/src/neptune/metadata_containers/__init__.py
--rw-r--r--   0        0        0     2063 2023-06-15 14:47:16.422541 neptune_client-1.3.0/src/neptune/metadata_containers/abstract.py
--rw-r--r--   0        0        0    20007 2023-06-15 14:47:16.422541 neptune_client-1.3.0/src/neptune/metadata_containers/metadata_container.py
--rw-r--r--   0        0        0     9194 2023-06-15 14:47:16.422541 neptune_client-1.3.0/src/neptune/metadata_containers/metadata_containers_table.py
--rw-r--r--   0        0        0    12337 2023-06-15 14:47:16.422541 neptune_client-1.3.0/src/neptune/metadata_containers/model.py
--rw-r--r--   0        0        0    11428 2023-06-15 14:47:16.422541 neptune_client-1.3.0/src/neptune/metadata_containers/model_version.py
--rw-r--r--   0        0        0    15433 2023-06-15 14:47:16.422541 neptune_client-1.3.0/src/neptune/metadata_containers/project.py
--rw-r--r--   0        0        0    23734 2023-06-15 14:47:16.422541 neptune_client-1.3.0/src/neptune/metadata_containers/run.py
--rw-r--r--   0        0        0     2606 2023-06-15 14:47:16.422541 neptune_client-1.3.0/src/neptune/new/__init__.py
--rw-r--r--   0        0        0     1476 2023-06-15 14:47:16.422541 neptune_client-1.3.0/src/neptune/new/_compatibility.py
--rw-r--r--   0        0        0      974 2023-06-15 14:47:16.422541 neptune_client-1.3.0/src/neptune/new/constants.py
--rw-r--r--   0        0        0     1378 2023-06-15 14:47:16.422541 neptune_client-1.3.0/src/neptune/new/envs.py
--rw-r--r--   0        0        0     5846 2023-06-15 14:47:16.422541 neptune_client-1.3.0/src/neptune/new/exceptions.py
--rw-r--r--   0        0        0      655 2023-06-15 14:47:16.426541 neptune_client-1.3.0/src/neptune/new/handler.py
--rw-r--r--   0        0        0      694 2023-06-15 14:47:16.426541 neptune_client-1.3.0/src/neptune/new/project.py
--rw-r--r--   0        0        0     1672 2023-06-15 14:47:16.426541 neptune_client-1.3.0/src/neptune/new/run.py
--rw-r--r--   0        0        0     1426 2023-06-15 14:47:16.426541 neptune_client-1.3.0/src/neptune/new/runs_table.py
--rw-r--r--   0        0        0      681 2023-06-15 14:47:16.426541 neptune_client-1.3.0/src/neptune/new/utils.py
--rw-r--r--   0        0        0      696 2023-06-15 14:47:16.426541 neptune_client-1.3.0/src/neptune/new/version.py
--rw-r--r--   0        0        0     1071 2023-06-15 14:47:16.426541 neptune_client-1.3.0/src/neptune/types/__init__.py
--rw-r--r--   0        0        0      914 2023-06-15 14:47:16.426541 neptune_client-1.3.0/src/neptune/types/atoms/__init__.py
--rw-r--r--   0        0        0     1626 2023-06-15 14:47:16.426541 neptune_client-1.3.0/src/neptune/types/atoms/artifact.py
--rw-r--r--   0        0        0      936 2023-06-15 14:47:16.426541 neptune_client-1.3.0/src/neptune/types/atoms/atom.py
--rw-r--r--   0        0        0     1302 2023-06-15 14:47:16.426541 neptune_client-1.3.0/src/neptune/types/atoms/boolean.py
--rw-r--r--   0        0        0     1435 2023-06-15 14:47:16.426541 neptune_client-1.3.0/src/neptune/types/atoms/datetime.py
--rw-r--r--   0        0        0    11695 2023-06-15 14:47:16.426541 neptune_client-1.3.0/src/neptune/types/atoms/file.py
--rw-r--r--   0        0        0     1297 2023-06-15 14:47:16.426541 neptune_client-1.3.0/src/neptune/types/atoms/float.py
--rw-r--r--   0        0        0     1902 2023-06-15 14:47:16.426541 neptune_client-1.3.0/src/neptune/types/atoms/git_ref.py
--rw-r--r--   0        0        0     1299 2023-06-15 14:47:16.426541 neptune_client-1.3.0/src/neptune/types/atoms/integer.py
--rw-r--r--   0        0        0     1473 2023-06-15 14:47:16.426541 neptune_client-1.3.0/src/neptune/types/atoms/string.py
--rw-r--r--   0        0        0     1485 2023-06-15 14:47:16.426541 neptune_client-1.3.0/src/neptune/types/file_set.py
--rw-r--r--   0        0        0      831 2023-06-15 14:47:16.426541 neptune_client-1.3.0/src/neptune/types/mode.py
--rw-r--r--   0        0        0      777 2023-06-15 14:47:16.426541 neptune_client-1.3.0/src/neptune/types/model_version_stage.py
--rw-r--r--   0        0        0     1144 2023-06-15 14:47:16.426541 neptune_client-1.3.0/src/neptune/types/namespace.py
--rw-r--r--   0        0        0      783 2023-06-15 14:47:16.426541 neptune_client-1.3.0/src/neptune/types/series/__init__.py
--rw-r--r--   0        0        0     2447 2023-06-15 14:47:16.426541 neptune_client-1.3.0/src/neptune/types/series/file_series.py
--rw-r--r--   0        0        0     2553 2023-06-15 14:47:16.426541 neptune_client-1.3.0/src/neptune/types/series/float_series.py
--rw-r--r--   0        0        0     1221 2023-06-15 14:47:16.426541 neptune_client-1.3.0/src/neptune/types/series/series.py
--rw-r--r--   0        0        0     1353 2023-06-15 14:47:16.426541 neptune_client-1.3.0/src/neptune/types/series/series_value.py
--rw-r--r--   0        0        0     2601 2023-06-15 14:47:16.426541 neptune_client-1.3.0/src/neptune/types/series/string_series.py
--rw-r--r--   0        0        0      655 2023-06-15 14:47:16.426541 neptune_client-1.3.0/src/neptune/types/sets/__init__.py
--rw-r--r--   0        0        0      934 2023-06-15 14:47:16.426541 neptune_client-1.3.0/src/neptune/types/sets/set.py
--rw-r--r--   0        0        0     1119 2023-06-15 14:47:16.426541 neptune_client-1.3.0/src/neptune/types/sets/string_set.py
--rw-r--r--   0        0        0     3551 2023-06-15 14:47:16.426541 neptune_client-1.3.0/src/neptune/types/type_casting.py
--rw-r--r--   0        0        0      892 2023-06-15 14:47:16.426541 neptune_client-1.3.0/src/neptune/types/value.py
--rw-r--r--   0        0        0     1634 2023-06-15 14:47:16.426541 neptune_client-1.3.0/src/neptune/types/value_copy.py
--rw-r--r--   0        0        0     2596 2023-06-15 14:47:16.426541 neptune_client-1.3.0/src/neptune/types/value_visitor.py
--rw-r--r--   0        0        0      698 2023-06-15 14:47:16.426541 neptune_client-1.3.0/src/neptune/typing.py
--rw-r--r--   0        0        0     1755 2023-06-15 14:47:16.426541 neptune_client-1.3.0/src/neptune/utils.py
--rw-r--r--   0        0        0        0 2023-06-15 14:47:16.426541 neptune_client-1.3.0/src/neptune/vendor/__init__.py
--rw-r--r--   0        0        0     6306 2023-06-15 14:47:16.426541 neptune_client-1.3.0/src/neptune/vendor/lib_programname.py
--rw-r--r--   0        0        0    68552 2023-06-15 14:47:16.426541 neptune_client-1.3.0/src/neptune/vendor/pynvml.py
--rw-r--r--   0        0        0     2228 2023-06-15 14:47:16.426541 neptune_client-1.3.0/src/neptune/version.py
--rw-r--r--   0        0        0    18640 1970-01-01 00:00:00.000000 neptune_client-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0    25802 2023-06-15 17:45:30.434589 neptune_client-1.3.1/CHANGELOG.md
+-rw-r--r--   0        0        0    11357 2023-06-15 17:45:30.438589 neptune_client-1.3.1/LICENSE
+-rw-r--r--   0        0        0    13935 2023-06-15 17:45:30.438589 neptune_client-1.3.1/README.md
+-rw-r--r--   0        0        0     4932 2023-06-15 17:45:45.706697 neptune_client-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0     3532 2023-06-15 17:45:30.438589 neptune_client-1.3.1/src/neptune/__init__.py
+-rw-r--r--   0        0        0     1218 2023-06-15 17:45:30.438589 neptune_client-1.3.1/src/neptune/attributes/__init__.py
+-rw-r--r--   0        0        0     1011 2023-06-15 17:45:30.438589 neptune_client-1.3.1/src/neptune/attributes/atoms/__init__.py
+-rw-r--r--   0        0        0     3048 2023-06-15 17:45:30.438589 neptune_client-1.3.1/src/neptune/attributes/atoms/artifact.py
+-rw-r--r--   0        0        0      701 2023-06-15 17:45:30.438589 neptune_client-1.3.1/src/neptune/attributes/atoms/atom.py
+-rw-r--r--   0        0        0     1709 2023-06-15 17:45:30.438589 neptune_client-1.3.1/src/neptune/attributes/atoms/boolean.py
+-rw-r--r--   0        0        0     2121 2023-06-15 17:45:30.438589 neptune_client-1.3.1/src/neptune/attributes/atoms/copiable_atom.py
+-rw-r--r--   0        0        0     2075 2023-06-15 17:45:30.438589 neptune_client-1.3.1/src/neptune/attributes/atoms/datetime.py
+-rw-r--r--   0        0        0     1788 2023-06-15 17:45:30.438589 neptune_client-1.3.1/src/neptune/attributes/atoms/file.py
+-rw-r--r--   0        0        0     1704 2023-06-15 17:45:30.438589 neptune_client-1.3.1/src/neptune/attributes/atoms/float.py
+-rw-r--r--   0        0        0      696 2023-06-15 17:45:30.438589 neptune_client-1.3.1/src/neptune/attributes/atoms/git_ref.py
+-rw-r--r--   0        0        0     2395 2023-06-15 17:45:30.438589 neptune_client-1.3.1/src/neptune/attributes/atoms/integer.py
+-rw-r--r--   0        0        0      707 2023-06-15 17:45:30.438589 neptune_client-1.3.1/src/neptune/attributes/atoms/notebook_ref.py
+-rw-r--r--   0        0        0      700 2023-06-15 17:45:30.438589 neptune_client-1.3.1/src/neptune/attributes/atoms/run_state.py
+-rw-r--r--   0        0        0     2658 2023-06-15 17:45:30.438589 neptune_client-1.3.1/src/neptune/attributes/atoms/string.py
+-rw-r--r--   0        0        0     2159 2023-06-15 17:45:30.438589 neptune_client-1.3.1/src/neptune/attributes/attribute.py
+-rw-r--r--   0        0        0     2723 2023-06-15 17:45:30.438589 neptune_client-1.3.1/src/neptune/attributes/constants.py
+-rw-r--r--   0        0        0     2642 2023-06-15 17:45:30.438589 neptune_client-1.3.1/src/neptune/attributes/file_set.py
+-rw-r--r--   0        0        0     4266 2023-06-15 17:45:30.438589 neptune_client-1.3.1/src/neptune/attributes/namespace.py
+-rw-r--r--   0        0        0      782 2023-06-15 17:45:30.438589 neptune_client-1.3.1/src/neptune/attributes/series/__init__.py
+-rw-r--r--   0        0        0     1949 2023-06-15 17:45:30.438589 neptune_client-1.3.1/src/neptune/attributes/series/fetchable_series.py
+-rw-r--r--   0        0        0     4292 2023-06-15 17:45:30.438589 neptune_client-1.3.1/src/neptune/attributes/series/file_series.py
+-rw-r--r--   0        0        0     2656 2023-06-15 17:45:30.438589 neptune_client-1.3.1/src/neptune/attributes/series/float_series.py
+-rw-r--r--   0        0        0     6003 2023-06-15 17:45:30.438589 neptune_client-1.3.1/src/neptune/attributes/series/series.py
+-rw-r--r--   0        0        0     3498 2023-06-15 17:45:30.438589 neptune_client-1.3.1/src/neptune/attributes/series/string_series.py
+-rw-r--r--   0        0        0      662 2023-06-15 17:45:30.438589 neptune_client-1.3.1/src/neptune/attributes/sets/__init__.py
+-rw-r--r--   0        0        0      699 2023-06-15 17:45:30.438589 neptune_client-1.3.1/src/neptune/attributes/sets/set.py
+-rw-r--r--   0        0        0     2627 2023-06-15 17:45:30.438589 neptune_client-1.3.1/src/neptune/attributes/sets/string_set.py
+-rw-r--r--   0        0        0     2157 2023-06-15 17:45:30.438589 neptune_client-1.3.1/src/neptune/attributes/utils.py
+-rw-r--r--   0        0        0      686 2023-06-15 17:45:30.438589 neptune_client-1.3.1/src/neptune/cli/__init__.py
+-rw-r--r--   0        0        0     1017 2023-06-15 17:45:30.438589 neptune_client-1.3.1/src/neptune/cli/__main__.py
+-rw-r--r--   0        0        0      866 2023-06-15 17:45:30.438589 neptune_client-1.3.1/src/neptune/cli/abstract_backend_runner.py
+-rw-r--r--   0        0        0     3436 2023-06-15 17:45:30.438589 neptune_client-1.3.1/src/neptune/cli/clear.py
+-rw-r--r--   0        0        0     5574 2023-06-15 17:45:30.438589 neptune_client-1.3.1/src/neptune/cli/commands.py
+-rw-r--r--   0        0        0     2814 2023-06-15 17:45:30.438589 neptune_client-1.3.1/src/neptune/cli/container_manager.py
+-rw-r--r--   0        0        0     1947 2023-06-15 17:45:30.438589 neptune_client-1.3.1/src/neptune/cli/path_option.py
+-rw-r--r--   0        0        0     3899 2023-06-15 17:45:30.438589 neptune_client-1.3.1/src/neptune/cli/status.py
+-rw-r--r--   0        0        0     9995 2023-06-15 17:45:30.438589 neptune_client-1.3.1/src/neptune/cli/sync.py
+-rw-r--r--   0        0        0     5028 2023-06-15 17:45:30.438589 neptune_client-1.3.1/src/neptune/cli/utils.py
+-rw-r--r--   0        0        0      596 2023-06-15 17:45:30.438589 neptune_client-1.3.1/src/neptune/common/__init__.py
+-rw-r--r--   0        0        0      596 2023-06-15 17:45:30.438589 neptune_client-1.3.1/src/neptune/common/backends/__init__.py
+-rw-r--r--   0        0        0     1038 2023-06-15 17:45:30.438589 neptune_client-1.3.1/src/neptune/common/backends/api_model.py
+-rw-r--r--   0        0        0     4230 2023-06-15 17:45:30.438589 neptune_client-1.3.1/src/neptune/common/backends/utils.py
+-rw-r--r--   0        0        0      859 2023-06-15 17:45:30.438589 neptune_client-1.3.1/src/neptune/common/envs.py
+-rw-r--r--   0        0        0    14106 2023-06-15 17:45:30.438589 neptune_client-1.3.1/src/neptune/common/exceptions.py
+-rw-r--r--   0        0        0      629 2023-06-15 17:45:30.438589 neptune_client-1.3.1/src/neptune/common/experiments.py
+-rw-r--r--   0        0        0     2490 2023-06-15 17:45:30.438589 neptune_client-1.3.1/src/neptune/common/git_info.py
+-rw-r--r--   0        0        0      596 2023-06-15 17:45:30.438589 neptune_client-1.3.1/src/neptune/common/hardware/__init__.py
+-rw-r--r--   0        0        0      596 2023-06-15 17:45:30.438589 neptune_client-1.3.1/src/neptune/common/hardware/cgroup/__init__.py
+-rw-r--r--   0        0        0     2638 2023-06-15 17:45:30.438589 neptune_client-1.3.1/src/neptune/common/hardware/cgroup/cgroup_filesystem_reader.py
+-rw-r--r--   0        0        0     3212 2023-06-15 17:45:30.438589 neptune_client-1.3.1/src/neptune/common/hardware/cgroup/cgroup_monitor.py
+-rw-r--r--   0        0        0      694 2023-06-15 17:45:30.438589 neptune_client-1.3.1/src/neptune/common/hardware/constants.py
+-rw-r--r--   0        0        0      596 2023-06-15 17:45:30.438589 neptune_client-1.3.1/src/neptune/common/hardware/gauges/__init__.py
+-rw-r--r--   0        0        0     1554 2023-06-15 17:45:30.442589 neptune_client-1.3.1/src/neptune/common/hardware/gauges/cpu.py
+-rw-r--r--   0        0        0      979 2023-06-15 17:45:30.442589 neptune_client-1.3.1/src/neptune/common/hardware/gauges/gauge.py
+-rw-r--r--   0        0        0     2023 2023-06-15 17:45:30.442589 neptune_client-1.3.1/src/neptune/common/hardware/gauges/gauge_factory.py
+-rw-r--r--   0        0        0      667 2023-06-15 17:45:30.442589 neptune_client-1.3.1/src/neptune/common/hardware/gauges/gauge_mode.py
+-rw-r--r--   0        0        0     1766 2023-06-15 17:45:30.442589 neptune_client-1.3.1/src/neptune/common/hardware/gauges/gpu.py
+-rw-r--r--   0        0        0     1748 2023-06-15 17:45:30.442589 neptune_client-1.3.1/src/neptune/common/hardware/gauges/memory.py
+-rw-r--r--   0        0        0      596 2023-06-15 17:45:30.442589 neptune_client-1.3.1/src/neptune/common/hardware/gpu/__init__.py
+-rw-r--r--   0        0        0     2568 2023-06-15 17:45:30.442589 neptune_client-1.3.1/src/neptune/common/hardware/gpu/gpu_monitor.py
+-rw-r--r--   0        0        0      596 2023-06-15 17:45:30.442589 neptune_client-1.3.1/src/neptune/common/hardware/metrics/__init__.py
+-rw-r--r--   0        0        0     2432 2023-06-15 17:45:30.442589 neptune_client-1.3.1/src/neptune/common/hardware/metrics/metric.py
+-rw-r--r--   0        0        0     1216 2023-06-15 17:45:30.442589 neptune_client-1.3.1/src/neptune/common/hardware/metrics/metrics_container.py
+-rw-r--r--   0        0        0     3490 2023-06-15 17:45:30.442589 neptune_client-1.3.1/src/neptune/common/hardware/metrics/metrics_factory.py
+-rw-r--r--   0        0        0      596 2023-06-15 17:45:30.442589 neptune_client-1.3.1/src/neptune/common/hardware/metrics/reports/__init__.py
+-rw-r--r--   0        0        0      792 2023-06-15 17:45:30.442589 neptune_client-1.3.1/src/neptune/common/hardware/metrics/reports/metric_report.py
+-rw-r--r--   0        0        0     1679 2023-06-15 17:45:30.442589 neptune_client-1.3.1/src/neptune/common/hardware/metrics/reports/metric_reporter.py
+-rw-r--r--   0        0        0      947 2023-06-15 17:45:30.442589 neptune_client-1.3.1/src/neptune/common/hardware/metrics/reports/metric_reporter_factory.py
+-rw-r--r--   0        0        0      596 2023-06-15 17:45:30.442589 neptune_client-1.3.1/src/neptune/common/hardware/metrics/service/__init__.py
+-rw-r--r--   0        0        0     1106 2023-06-15 17:45:30.442589 neptune_client-1.3.1/src/neptune/common/hardware/metrics/service/metric_service.py
+-rw-r--r--   0        0        0     2309 2023-06-15 17:45:30.442589 neptune_client-1.3.1/src/neptune/common/hardware/metrics/service/metric_service_factory.py
+-rw-r--r--   0        0        0      596 2023-06-15 17:45:30.442589 neptune_client-1.3.1/src/neptune/common/hardware/resources/__init__.py
+-rw-r--r--   0        0        0     1821 2023-06-15 17:45:30.442589 neptune_client-1.3.1/src/neptune/common/hardware/resources/gpu_card_indices_provider.py
+-rw-r--r--   0        0        0     1574 2023-06-15 17:45:30.442589 neptune_client-1.3.1/src/neptune/common/hardware/resources/system_resource_info.py
+-rw-r--r--   0        0        0     2504 2023-06-15 17:45:30.442589 neptune_client-1.3.1/src/neptune/common/hardware/resources/system_resource_info_factory.py
+-rw-r--r--   0        0        0      596 2023-06-15 17:45:30.442589 neptune_client-1.3.1/src/neptune/common/hardware/system/__init__.py
+-rw-r--r--   0        0        0      964 2023-06-15 17:45:30.442589 neptune_client-1.3.1/src/neptune/common/hardware/system/system_monitor.py
+-rw-r--r--   0        0        0     4772 2023-06-15 17:45:30.442589 neptune_client-1.3.1/src/neptune/common/oauth.py
+-rw-r--r--   0        0        0      884 2023-06-15 17:45:30.442589 neptune_client-1.3.1/src/neptune/common/patches/__init__.py
+-rw-r--r--   0        0        0     2731 2023-06-15 17:45:30.442589 neptune_client-1.3.1/src/neptune/common/patches/bravado.py
+-rw-r--r--   0        0        0      726 2023-06-15 17:45:30.442589 neptune_client-1.3.1/src/neptune/common/patterns.py
+-rw-r--r--   0        0        0      596 2023-06-15 17:45:30.442589 neptune_client-1.3.1/src/neptune/common/storage/__init__.py
+-rw-r--r--   0        0        0     3223 2023-06-15 17:45:30.442589 neptune_client-1.3.1/src/neptune/common/storage/datastream.py
+-rw-r--r--   0        0        0     7335 2023-06-15 17:45:30.442589 neptune_client-1.3.1/src/neptune/common/storage/storage_utils.py
+-rw-r--r--   0        0        0     7075 2023-06-15 17:45:30.442589 neptune_client-1.3.1/src/neptune/common/utils.py
+-rw-r--r--   0        0        0     2206 2023-06-15 17:45:30.442589 neptune_client-1.3.1/src/neptune/common/warnings.py
+-rw-r--r--   0        0        0      596 2023-06-15 17:45:30.442589 neptune_client-1.3.1/src/neptune/common/websockets/__init__.py
+-rw-r--r--   0        0        0     3589 2023-06-15 17:45:30.442589 neptune_client-1.3.1/src/neptune/common/websockets/reconnecting_websocket.py
+-rw-r--r--   0        0        0     2693 2023-06-15 17:45:30.442589 neptune_client-1.3.1/src/neptune/common/websockets/websocket_client_adapter.py
+-rw-r--r--   0        0        0      985 2023-06-15 17:45:30.442589 neptune_client-1.3.1/src/neptune/constants.py
+-rw-r--r--   0        0        0     1863 2023-06-15 17:45:30.442589 neptune_client-1.3.1/src/neptune/envs.py
+-rw-r--r--   0        0        0    41966 2023-06-15 17:45:30.442589 neptune_client-1.3.1/src/neptune/exceptions.py
+-rw-r--r--   0        0        0    29698 2023-06-15 17:45:30.442589 neptune_client-1.3.1/src/neptune/handler.py
+-rw-r--r--   0        0        0      596 2023-06-15 17:45:30.442589 neptune_client-1.3.1/src/neptune/integrations/__init__.py
+-rw-r--r--   0        0        0      973 2023-06-15 17:45:30.442589 neptune_client-1.3.1/src/neptune/integrations/aws/__init__.py
+-rw-r--r--   0        0        0     1014 2023-06-15 17:45:30.442589 neptune_client-1.3.1/src/neptune/integrations/detectron2/__init__.py
+-rw-r--r--   0        0        0      985 2023-06-15 17:45:30.442589 neptune_client-1.3.1/src/neptune/integrations/fastai/__init__.py
+-rw-r--r--   0        0        0      976 2023-06-15 17:45:30.442589 neptune_client-1.3.1/src/neptune/integrations/kedro/__init__.py
+-rw-r--r--   0        0        0      993 2023-06-15 17:45:30.442589 neptune_client-1.3.1/src/neptune/integrations/lightgbm/__init__.py
+-rw-r--r--   0        0        0      985 2023-06-15 17:45:30.442589 neptune_client-1.3.1/src/neptune/integrations/optuna/__init__.py
+-rw-r--r--   0        0        0      989 2023-06-15 17:45:30.442589 neptune_client-1.3.1/src/neptune/integrations/prophet/__init__.py
+-rw-r--r--   0        0        0     3084 2023-06-15 17:45:30.442589 neptune_client-1.3.1/src/neptune/integrations/python_logger.py
+-rw-r--r--   0        0        0     1006 2023-06-15 17:45:30.442589 neptune_client-1.3.1/src/neptune/integrations/pytorch/__init__.py
+-rw-r--r--   0        0        0     1042 2023-06-15 17:45:30.442589 neptune_client-1.3.1/src/neptune/integrations/pytorch_lightning/__init__.py
+-rw-r--r--   0        0        0      985 2023-06-15 17:45:30.442589 neptune_client-1.3.1/src/neptune/integrations/sacred/__init__.py
+-rw-r--r--   0        0        0      989 2023-06-15 17:45:30.442589 neptune_client-1.3.1/src/neptune/integrations/sklearn/__init__.py
+-rw-r--r--   0        0        0     1038 2023-06-15 17:45:30.442589 neptune_client-1.3.1/src/neptune/integrations/tensorflow_keras/__init__.py
+-rw-r--r--   0        0        0     1032 2023-06-15 17:45:30.442589 neptune_client-1.3.1/src/neptune/integrations/transformers/__init__.py
+-rw-r--r--   0        0        0     1164 2023-06-15 17:45:30.442589 neptune_client-1.3.1/src/neptune/integrations/utils.py
+-rw-r--r--   0        0        0      989 2023-06-15 17:45:30.442589 neptune_client-1.3.1/src/neptune/integrations/xgboost/__init__.py
+-rw-r--r--   0        0        0      596 2023-06-15 17:45:30.442589 neptune_client-1.3.1/src/neptune/internal/__init__.py
+-rw-r--r--   0        0        0      760 2023-06-15 17:45:30.442589 neptune_client-1.3.1/src/neptune/internal/artifacts/__init__.py
+-rw-r--r--   0        0        0      791 2023-06-15 17:45:30.442589 neptune_client-1.3.1/src/neptune/internal/artifacts/drivers/__init__.py
+-rw-r--r--   0        0        0     4240 2023-06-15 17:45:30.442589 neptune_client-1.3.1/src/neptune/internal/artifacts/drivers/local.py
+-rw-r--r--   0        0        0     4810 2023-06-15 17:45:30.442589 neptune_client-1.3.1/src/neptune/internal/artifacts/drivers/s3.py
+-rw-r--r--   0        0        0     4017 2023-06-15 17:45:30.442589 neptune_client-1.3.1/src/neptune/internal/artifacts/file_hasher.py
+-rw-r--r--   0        0        0     2318 2023-06-15 17:45:30.442589 neptune_client-1.3.1/src/neptune/internal/artifacts/local_file_hash_storage.py
+-rw-r--r--   0        0        0     3578 2023-06-15 17:45:30.442589 neptune_client-1.3.1/src/neptune/internal/artifacts/types.py
+-rw-r--r--   0        0        0      999 2023-06-15 17:45:30.442589 neptune_client-1.3.1/src/neptune/internal/artifacts/utils.py
+-rw-r--r--   0        0        0      596 2023-06-15 17:45:30.442589 neptune_client-1.3.1/src/neptune/internal/backends/__init__.py
+-rw-r--r--   0        0        0     7169 2023-06-15 17:45:30.442589 neptune_client-1.3.1/src/neptune/internal/backends/api_model.py
+-rw-r--r--   0        0        0     1703 2023-06-15 17:45:30.442589 neptune_client-1.3.1/src/neptune/internal/backends/factory.py
+-rw-r--r--   0        0        0     6700 2023-06-15 17:45:30.442589 neptune_client-1.3.1/src/neptune/internal/backends/hosted_artifact_operations.py
+-rw-r--r--   0        0        0     5942 2023-06-15 17:45:30.442589 neptune_client-1.3.1/src/neptune/internal/backends/hosted_client.py
+-rw-r--r--   0        0        0    17136 2023-06-15 17:45:30.446589 neptune_client-1.3.1/src/neptune/internal/backends/hosted_file_operations.py
+-rw-r--r--   0        0        0    40705 2023-06-15 17:45:30.446589 neptune_client-1.3.1/src/neptune/internal/backends/hosted_neptune_backend.py
+-rw-r--r--   0        0        0     8506 2023-06-15 17:45:30.446589 neptune_client-1.3.1/src/neptune/internal/backends/neptune_backend.py
+-rw-r--r--   0        0        0    31714 2023-06-15 17:45:30.446589 neptune_client-1.3.1/src/neptune/internal/backends/neptune_backend_mock.py
+-rw-r--r--   0        0        0     1942 2023-06-15 17:45:30.446589 neptune_client-1.3.1/src/neptune/internal/backends/nql.py
+-rw-r--r--   0        0        0     4471 2023-06-15 17:45:30.446589 neptune_client-1.3.1/src/neptune/internal/backends/offline_neptune_backend.py
+-rw-r--r--   0        0        0     3946 2023-06-15 17:45:30.446589 neptune_client-1.3.1/src/neptune/internal/backends/operation_api_name_visitor.py
+-rw-r--r--   0        0        0     5003 2023-06-15 17:45:30.446589 neptune_client-1.3.1/src/neptune/internal/backends/operation_api_object_converter.py
+-rw-r--r--   0        0        0    13841 2023-06-15 17:45:30.446589 neptune_client-1.3.1/src/neptune/internal/backends/operations_preprocessor.py
+-rw-r--r--   0        0        0     1619 2023-06-15 17:45:30.446589 neptune_client-1.3.1/src/neptune/internal/backends/project_name_lookup.py
+-rw-r--r--   0        0        0     5246 2023-06-15 17:45:30.446589 neptune_client-1.3.1/src/neptune/internal/backends/swagger_client_wrapper.py
+-rw-r--r--   0        0        0     8765 2023-06-15 17:45:30.446589 neptune_client-1.3.1/src/neptune/internal/backends/utils.py
+-rw-r--r--   0        0        0     1381 2023-06-15 17:45:30.446589 neptune_client-1.3.1/src/neptune/internal/backgroud_job_list.py
+-rw-r--r--   0        0        0     1035 2023-06-15 17:45:30.446589 neptune_client-1.3.1/src/neptune/internal/background_job.py
+-rw-r--r--   0        0        0      350 2023-06-15 17:45:30.446589 neptune_client-1.3.1/src/neptune/internal/constants.py
+-rw-r--r--   0        0        0     4486 2023-06-15 17:45:30.446589 neptune_client-1.3.1/src/neptune/internal/container_structure.py
+-rw-r--r--   0        0        0     1302 2023-06-15 17:45:30.446589 neptune_client-1.3.1/src/neptune/internal/container_type.py
+-rw-r--r--   0        0        0     2345 2023-06-15 17:45:30.446589 neptune_client-1.3.1/src/neptune/internal/credentials.py
+-rw-r--r--   0        0        0     8468 2023-06-15 17:45:30.446589 neptune_client-1.3.1/src/neptune/internal/disk_queue.py
+-rw-r--r--   0        0        0      689 2023-06-15 17:45:30.446589 neptune_client-1.3.1/src/neptune/internal/exceptions.py
+-rw-r--r--   0        0        0      596 2023-06-15 17:45:30.446589 neptune_client-1.3.1/src/neptune/internal/hardware/__init__.py
+-rw-r--r--   0        0        0      596 2023-06-15 17:45:30.446589 neptune_client-1.3.1/src/neptune/internal/hardware/gpu/__init__.py
+-rw-r--r--   0        0        0     2466 2023-06-15 17:45:30.446589 neptune_client-1.3.1/src/neptune/internal/hardware/gpu/gpu_monitor.py
+-rw-r--r--   0        0        0     4997 2023-06-15 17:45:30.446589 neptune_client-1.3.1/src/neptune/internal/hardware/hardware_metric_reporting_job.py
+-rw-r--r--   0        0        0      933 2023-06-15 17:45:30.446589 neptune_client-1.3.1/src/neptune/internal/id_formats.py
+-rw-r--r--   0        0        0      596 2023-06-15 17:45:30.446589 neptune_client-1.3.1/src/neptune/internal/init/__init__.py
+-rw-r--r--   0        0        0      796 2023-06-15 17:45:30.446589 neptune_client-1.3.1/src/neptune/internal/init/parameters.py
+-rw-r--r--   0        0        0      596 2023-06-15 17:45:30.446589 neptune_client-1.3.1/src/neptune/internal/notebooks/__init__.py
+-rw-r--r--   0        0        0     1572 2023-06-15 17:45:30.446589 neptune_client-1.3.1/src/neptune/internal/notebooks/comm.py
+-rw-r--r--   0        0        0     1831 2023-06-15 17:45:30.446589 neptune_client-1.3.1/src/neptune/internal/notebooks/notebooks.py
+-rw-r--r--   0        0        0    17310 2023-06-15 17:45:30.446589 neptune_client-1.3.1/src/neptune/internal/operation.py
+-rw-r--r--   0        0        0      596 2023-06-15 17:45:30.446589 neptune_client-1.3.1/src/neptune/internal/operation_processors/__init__.py
+-rw-r--r--   0        0        0    10851 2023-06-15 17:45:30.446589 neptune_client-1.3.1/src/neptune/internal/operation_processors/async_operation_processor.py
+-rw-r--r--   0        0        0     2177 2023-06-15 17:45:30.446589 neptune_client-1.3.1/src/neptune/internal/operation_processors/factory.py
+-rw-r--r--   0        0        0     2136 2023-06-15 17:45:30.446589 neptune_client-1.3.1/src/neptune/internal/operation_processors/offline_operation_processor.py
+-rw-r--r--   0        0        0     1140 2023-06-15 17:45:30.446589 neptune_client-1.3.1/src/neptune/internal/operation_processors/operation_processor.py
+-rw-r--r--   0        0        0     1998 2023-06-15 17:45:30.446589 neptune_client-1.3.1/src/neptune/internal/operation_processors/operation_storage.py
+-rw-r--r--   0        0        0     1577 2023-06-15 17:45:30.446589 neptune_client-1.3.1/src/neptune/internal/operation_processors/read_only_operation_processor.py
+-rw-r--r--   0        0        0     2483 2023-06-15 17:45:30.446589 neptune_client-1.3.1/src/neptune/internal/operation_processors/sync_operation_processor.py
+-rw-r--r--   0        0        0     3724 2023-06-15 17:45:30.446589 neptune_client-1.3.1/src/neptune/internal/operation_visitor.py
+-rw-r--r--   0        0        0      776 2023-06-15 17:45:30.446589 neptune_client-1.3.1/src/neptune/internal/state.py
+-rw-r--r--   0        0        0      596 2023-06-15 17:45:30.446589 neptune_client-1.3.1/src/neptune/internal/streams/__init__.py
+-rw-r--r--   0        0        0     1815 2023-06-15 17:45:30.446589 neptune_client-1.3.1/src/neptune/internal/streams/std_capture_background_job.py
+-rw-r--r--   0        0        0     2418 2023-06-15 17:45:30.446589 neptune_client-1.3.1/src/neptune/internal/streams/std_stream_capture_logger.py
+-rw-r--r--   0        0        0      596 2023-06-15 17:45:30.446589 neptune_client-1.3.1/src/neptune/internal/threading/__init__.py
+-rw-r--r--   0        0        0     3567 2023-06-15 17:45:30.446589 neptune_client-1.3.1/src/neptune/internal/threading/daemon.py
+-rw-r--r--   0        0        0      596 2023-06-15 17:45:30.446589 neptune_client-1.3.1/src/neptune/internal/types/__init__.py
+-rw-r--r--   0        0        0     4584 2023-06-15 17:45:30.446589 neptune_client-1.3.1/src/neptune/internal/types/file_types.py
+-rw-r--r--   0        0        0     1665 2023-06-15 17:45:30.446589 neptune_client-1.3.1/src/neptune/internal/types/stringify_value.py
+-rw-r--r--   0        0        0     4856 2023-06-15 17:45:30.446589 neptune_client-1.3.1/src/neptune/internal/utils/__init__.py
+-rw-r--r--   0        0        0     1171 2023-06-15 17:45:30.446589 neptune_client-1.3.1/src/neptune/internal/utils/dependency_tracking.py
+-rw-r--r--   0        0        0     2114 2023-06-15 17:45:30.446589 neptune_client-1.3.1/src/neptune/internal/utils/deprecation.py
+-rw-r--r--   0        0        0     2374 2023-06-15 17:45:30.446589 neptune_client-1.3.1/src/neptune/internal/utils/generic_attribute_mapper.py
+-rw-r--r--   0        0        0     5888 2023-06-15 17:45:30.446589 neptune_client-1.3.1/src/neptune/internal/utils/git.py
+-rw-r--r--   0        0        0      849 2023-06-15 17:45:30.446589 neptune_client-1.3.1/src/neptune/internal/utils/hashing.py
+-rw-r--r--   0        0        0     9732 2023-06-15 17:45:30.446589 neptune_client-1.3.1/src/neptune/internal/utils/images.py
+-rw-r--r--   0        0        0     1288 2023-06-15 17:45:30.446589 neptune_client-1.3.1/src/neptune/internal/utils/iteration.py
+-rw-r--r--   0        0        0     3053 2023-06-15 17:45:30.446589 neptune_client-1.3.1/src/neptune/internal/utils/json_file_splitter.py
+-rw-r--r--   0        0        0     1633 2023-06-15 17:45:30.446589 neptune_client-1.3.1/src/neptune/internal/utils/limits.py
+-rw-r--r--   0        0        0     1488 2023-06-15 17:45:30.446589 neptune_client-1.3.1/src/neptune/internal/utils/logger.py
+-rw-r--r--   0        0        0     1042 2023-06-15 17:45:30.446589 neptune_client-1.3.1/src/neptune/internal/utils/paths.py
+-rw-r--r--   0        0        0     2049 2023-06-15 17:45:30.446589 neptune_client-1.3.1/src/neptune/internal/utils/ping_background_job.py
+-rw-r--r--   0        0        0     1809 2023-06-15 17:45:30.446589 neptune_client-1.3.1/src/neptune/internal/utils/process_killer.py
+-rw-r--r--   0        0        0     1564 2023-06-15 17:45:30.446589 neptune_client-1.3.1/src/neptune/internal/utils/run_state.py
+-rw-r--r--   0        0        0     1207 2023-06-15 17:45:30.446589 neptune_client-1.3.1/src/neptune/internal/utils/runningmode.py
+-rw-r--r--   0        0        0     1340 2023-06-15 17:45:30.446589 neptune_client-1.3.1/src/neptune/internal/utils/s3.py
+-rw-r--r--   0        0        0     2270 2023-06-15 17:45:30.446589 neptune_client-1.3.1/src/neptune/internal/utils/source_code.py
+-rw-r--r--   0        0        0     1457 2023-06-15 17:45:30.446589 neptune_client-1.3.1/src/neptune/internal/utils/sync_offset_file.py
+-rw-r--r--   0        0        0     1927 2023-06-15 17:45:30.446589 neptune_client-1.3.1/src/neptune/internal/utils/traceback_job.py
+-rw-r--r--   0        0        0     2426 2023-06-15 17:45:30.446589 neptune_client-1.3.1/src/neptune/internal/utils/uncaught_exception_handler.py
+-rw-r--r--   0        0        0     4462 2023-06-15 17:45:30.446589 neptune_client-1.3.1/src/neptune/internal/value_to_attribute_visitor.py
+-rw-r--r--   0        0        0      596 2023-06-15 17:45:30.446589 neptune_client-1.3.1/src/neptune/internal/websockets/__init__.py
+-rw-r--r--   0        0        0     5188 2023-06-15 17:45:30.446589 neptune_client-1.3.1/src/neptune/internal/websockets/websocket_signals_background_job.py
+-rw-r--r--   0        0        0     1229 2023-06-15 17:45:30.446589 neptune_client-1.3.1/src/neptune/internal/websockets/websockets_factory.py
+-rw-r--r--   0        0        0    13821 2023-06-15 17:45:30.446589 neptune_client-1.3.1/src/neptune/legacy/__init__.py
+-rw-r--r--   0        0        0    11218 2023-06-15 17:45:30.446589 neptune_client-1.3.1/src/neptune/legacy/api_exceptions.py
+-rw-r--r--   0        0        0     4710 2023-06-15 17:45:30.450589 neptune_client-1.3.1/src/neptune/legacy/backend.py
+-rw-r--r--   0        0        0      737 2023-06-15 17:45:30.450589 neptune_client-1.3.1/src/neptune/legacy/checkpoint.py
+-rw-r--r--   0        0        0      859 2023-06-15 17:45:30.450589 neptune_client-1.3.1/src/neptune/legacy/constants.py
+-rw-r--r--   0        0        0      860 2023-06-15 17:45:30.450589 neptune_client-1.3.1/src/neptune/legacy/envs.py
+-rw-r--r--   0        0        0    12780 2023-06-15 17:45:30.450589 neptune_client-1.3.1/src/neptune/legacy/exceptions.py
+-rw-r--r--   0        0        0    42888 2023-06-15 17:45:30.450589 neptune_client-1.3.1/src/neptune/legacy/experiments.py
+-rw-r--r--   0        0        0      663 2023-06-15 17:45:30.450589 neptune_client-1.3.1/src/neptune/legacy/git_info.py
+-rw-r--r--   0        0        0      596 2023-06-15 17:45:30.450589 neptune_client-1.3.1/src/neptune/legacy/internal/__init__.py
+-rw-r--r--   0        0        0     1999 2023-06-15 17:45:30.450589 neptune_client-1.3.1/src/neptune/legacy/internal/abort.py
+-rw-r--r--   0        0        0      888 2023-06-15 17:45:30.450589 neptune_client-1.3.1/src/neptune/legacy/internal/api_clients/__init__.py
+-rw-r--r--   0        0        0     1148 2023-06-15 17:45:30.450589 neptune_client-1.3.1/src/neptune/legacy/internal/api_clients/backend_factory.py
+-rw-r--r--   0        0        0     1826 2023-06-15 17:45:30.450589 neptune_client-1.3.1/src/neptune/legacy/internal/api_clients/client_config.py
+-rw-r--r--   0        0        0     3103 2023-06-15 17:45:30.450589 neptune_client-1.3.1/src/neptune/legacy/internal/api_clients/credentials.py
+-rw-r--r--   0        0        0      596 2023-06-15 17:45:30.450589 neptune_client-1.3.1/src/neptune/legacy/internal/api_clients/hosted_api_clients/__init__.py
+-rw-r--r--   0        0        0    46556 2023-06-15 17:45:30.450589 neptune_client-1.3.1/src/neptune/legacy/internal/api_clients/hosted_api_clients/hosted_alpha_leaderboard_api_client.py
+-rw-r--r--   0        0        0     8710 2023-06-15 17:45:30.450589 neptune_client-1.3.1/src/neptune/legacy/internal/api_clients/hosted_api_clients/hosted_backend_api_client.py
+-rw-r--r--   0        0        0     4456 2023-06-15 17:45:30.450589 neptune_client-1.3.1/src/neptune/legacy/internal/api_clients/hosted_api_clients/mixins.py
+-rw-r--r--   0        0        0     3857 2023-06-15 17:45:30.450589 neptune_client-1.3.1/src/neptune/legacy/internal/api_clients/hosted_api_clients/utils.py
+-rw-r--r--   0        0        0     4631 2023-06-15 17:45:30.450589 neptune_client-1.3.1/src/neptune/legacy/internal/api_clients/offline_backend.py
+-rw-r--r--   0        0        0      596 2023-06-15 17:45:30.450589 neptune_client-1.3.1/src/neptune/legacy/internal/backends/__init__.py
+-rw-r--r--   0        0        0      776 2023-06-15 17:45:30.450589 neptune_client-1.3.1/src/neptune/legacy/internal/backends/hosted_neptune_backend.py
+-rw-r--r--   0        0        0      596 2023-06-15 17:45:30.450589 neptune_client-1.3.1/src/neptune/legacy/internal/channels/__init__.py
+-rw-r--r--   0        0        0     3903 2023-06-15 17:45:30.450589 neptune_client-1.3.1/src/neptune/legacy/internal/channels/channels.py
+-rw-r--r--   0        0        0     7087 2023-06-15 17:45:30.450589 neptune_client-1.3.1/src/neptune/legacy/internal/channels/channels_values_sender.py
+-rw-r--r--   0        0        0      596 2023-06-15 17:45:30.450589 neptune_client-1.3.1/src/neptune/legacy/internal/execution/__init__.py
+-rw-r--r--   0        0        0     6126 2023-06-15 17:45:30.450589 neptune_client-1.3.1/src/neptune/legacy/internal/execution/execution_context.py
+-rw-r--r--   0        0        0      596 2023-06-15 17:45:30.450589 neptune_client-1.3.1/src/neptune/legacy/internal/experiments/__init__.py
+-rw-r--r--   0        0        0      596 2023-06-15 17:45:30.450589 neptune_client-1.3.1/src/neptune/legacy/internal/notebooks/__init__.py
+-rw-r--r--   0        0        0     1510 2023-06-15 17:45:30.450589 neptune_client-1.3.1/src/neptune/legacy/internal/notebooks/comm.py
+-rw-r--r--   0        0        0     1711 2023-06-15 17:45:30.450589 neptune_client-1.3.1/src/neptune/legacy/internal/notebooks/notebooks.py
+-rw-r--r--   0        0        0      596 2023-06-15 17:45:30.450589 neptune_client-1.3.1/src/neptune/legacy/internal/streams/__init__.py
+-rw-r--r--   0        0        0     2805 2023-06-15 17:45:30.450589 neptune_client-1.3.1/src/neptune/legacy/internal/streams/channel_writer.py
+-rw-r--r--   0        0        0     1945 2023-06-15 17:45:30.450589 neptune_client-1.3.1/src/neptune/legacy/internal/streams/stdstream_uploader.py
+-rw-r--r--   0        0        0      596 2023-06-15 17:45:30.450589 neptune_client-1.3.1/src/neptune/legacy/internal/threads/__init__.py
+-rw-r--r--   0        0        0     2363 2023-06-15 17:45:30.450589 neptune_client-1.3.1/src/neptune/legacy/internal/threads/aborting_thread.py
+-rw-r--r--   0        0        0     1816 2023-06-15 17:45:30.450589 neptune_client-1.3.1/src/neptune/legacy/internal/threads/hardware_metric_reporting_thread.py
+-rw-r--r--   0        0        0     1334 2023-06-15 17:45:30.450589 neptune_client-1.3.1/src/neptune/legacy/internal/threads/neptune_thread.py
+-rw-r--r--   0        0        0     1556 2023-06-15 17:45:30.450589 neptune_client-1.3.1/src/neptune/legacy/internal/threads/ping_thread.py
+-rw-r--r--   0        0        0      596 2023-06-15 17:45:30.450589 neptune_client-1.3.1/src/neptune/legacy/internal/utils/__init__.py
+-rw-r--r--   0        0        0     8091 2023-06-15 17:45:30.450589 neptune_client-1.3.1/src/neptune/legacy/internal/utils/alpha_integration.py
+-rw-r--r--   0        0        0      997 2023-06-15 17:45:30.450589 neptune_client-1.3.1/src/neptune/legacy/internal/utils/deprecation.py
+-rw-r--r--   0        0        0     2597 2023-06-15 17:45:30.450589 neptune_client-1.3.1/src/neptune/legacy/internal/utils/http.py
+-rw-r--r--   0        0        0     2597 2023-06-15 17:45:30.450589 neptune_client-1.3.1/src/neptune/legacy/internal/utils/http_utils.py
+-rw-r--r--   0        0        0     2990 2023-06-15 17:45:30.450589 neptune_client-1.3.1/src/neptune/legacy/internal/utils/image.py
+-rw-r--r--   0        0        0     3145 2023-06-15 17:45:30.450589 neptune_client-1.3.1/src/neptune/legacy/internal/utils/source_code.py
+-rw-r--r--   0        0        0      596 2023-06-15 17:45:30.450589 neptune_client-1.3.1/src/neptune/legacy/internal/websockets/__init__.py
+-rw-r--r--   0        0        0     3542 2023-06-15 17:45:30.450589 neptune_client-1.3.1/src/neptune/legacy/internal/websockets/message.py
+-rw-r--r--   0        0        0     1097 2023-06-15 17:45:30.450589 neptune_client-1.3.1/src/neptune/legacy/internal/websockets/reconnecting_websocket_factory.py
+-rw-r--r--   0        0        0     1228 2023-06-15 17:45:30.450589 neptune_client-1.3.1/src/neptune/legacy/internal/websockets/websocket_message_processor.py
+-rw-r--r--   0        0        0     3938 2023-06-15 17:45:30.450589 neptune_client-1.3.1/src/neptune/legacy/model.py
+-rw-r--r--   0        0        0     2807 2023-06-15 17:45:30.450589 neptune_client-1.3.1/src/neptune/legacy/notebook.py
+-rw-r--r--   0        0        0      691 2023-06-15 17:45:30.450589 neptune_client-1.3.1/src/neptune/legacy/oauth.py
+-rw-r--r--   0        0        0      678 2023-06-15 17:45:30.450589 neptune_client-1.3.1/src/neptune/legacy/patterns.py
+-rw-r--r--   0        0        0    26377 2023-06-15 17:45:30.450589 neptune_client-1.3.1/src/neptune/legacy/projects.py
+-rw-r--r--   0        0        0     8992 2023-06-15 17:45:30.450589 neptune_client-1.3.1/src/neptune/legacy/sessions.py
+-rw-r--r--   0        0        0     1162 2023-06-15 17:45:30.450589 neptune_client-1.3.1/src/neptune/legacy/utils.py
+-rw-r--r--   0        0        0      660 2023-06-15 17:45:30.450589 neptune_client-1.3.1/src/neptune/logging/__init__.py
+-rw-r--r--   0        0        0      976 2023-06-15 17:45:30.450589 neptune_client-1.3.1/src/neptune/logging/logger.py
+-rw-r--r--   0        0        0     4454 2023-06-15 17:45:30.454589 neptune_client-1.3.1/src/neptune/management/__init__.py
+-rw-r--r--   0        0        0     6943 2023-06-15 17:45:30.454589 neptune_client-1.3.1/src/neptune/management/exceptions.py
+-rw-r--r--   0        0        0      596 2023-06-15 17:45:30.454589 neptune_client-1.3.1/src/neptune/management/internal/__init__.py
+-rw-r--r--   0        0        0    36941 2023-06-15 17:45:30.454589 neptune_client-1.3.1/src/neptune/management/internal/api.py
+-rw-r--r--   0        0        0     2853 2023-06-15 17:45:30.454589 neptune_client-1.3.1/src/neptune/management/internal/dto.py
+-rw-r--r--   0        0        0     1069 2023-06-15 17:45:30.454589 neptune_client-1.3.1/src/neptune/management/internal/types.py
+-rw-r--r--   0        0        0     2013 2023-06-15 17:45:30.454589 neptune_client-1.3.1/src/neptune/management/internal/utils.py
+-rw-r--r--   0        0        0      995 2023-06-15 17:45:30.454589 neptune_client-1.3.1/src/neptune/metadata_containers/__init__.py
+-rw-r--r--   0        0        0     2063 2023-06-15 17:45:30.454589 neptune_client-1.3.1/src/neptune/metadata_containers/abstract.py
+-rw-r--r--   0        0        0    20007 2023-06-15 17:45:30.454589 neptune_client-1.3.1/src/neptune/metadata_containers/metadata_container.py
+-rw-r--r--   0        0        0     9194 2023-06-15 17:45:30.454589 neptune_client-1.3.1/src/neptune/metadata_containers/metadata_containers_table.py
+-rw-r--r--   0        0        0    12337 2023-06-15 17:45:30.454589 neptune_client-1.3.1/src/neptune/metadata_containers/model.py
+-rw-r--r--   0        0        0    11428 2023-06-15 17:45:30.454589 neptune_client-1.3.1/src/neptune/metadata_containers/model_version.py
+-rw-r--r--   0        0        0    15433 2023-06-15 17:45:30.454589 neptune_client-1.3.1/src/neptune/metadata_containers/project.py
+-rw-r--r--   0        0        0    23734 2023-06-15 17:45:30.454589 neptune_client-1.3.1/src/neptune/metadata_containers/run.py
+-rw-r--r--   0        0        0     2606 2023-06-15 17:45:30.454589 neptune_client-1.3.1/src/neptune/new/__init__.py
+-rw-r--r--   0        0        0     1476 2023-06-15 17:45:30.454589 neptune_client-1.3.1/src/neptune/new/_compatibility.py
+-rw-r--r--   0        0        0      974 2023-06-15 17:45:30.454589 neptune_client-1.3.1/src/neptune/new/constants.py
+-rw-r--r--   0        0        0     1378 2023-06-15 17:45:30.454589 neptune_client-1.3.1/src/neptune/new/envs.py
+-rw-r--r--   0        0        0     5846 2023-06-15 17:45:30.454589 neptune_client-1.3.1/src/neptune/new/exceptions.py
+-rw-r--r--   0        0        0      655 2023-06-15 17:45:30.454589 neptune_client-1.3.1/src/neptune/new/handler.py
+-rw-r--r--   0        0        0      694 2023-06-15 17:45:30.454589 neptune_client-1.3.1/src/neptune/new/project.py
+-rw-r--r--   0        0        0     1672 2023-06-15 17:45:30.454589 neptune_client-1.3.1/src/neptune/new/run.py
+-rw-r--r--   0        0        0     1426 2023-06-15 17:45:30.454589 neptune_client-1.3.1/src/neptune/new/runs_table.py
+-rw-r--r--   0        0        0      681 2023-06-15 17:45:30.454589 neptune_client-1.3.1/src/neptune/new/utils.py
+-rw-r--r--   0        0        0      696 2023-06-15 17:45:30.454589 neptune_client-1.3.1/src/neptune/new/version.py
+-rw-r--r--   0        0        0     1071 2023-06-15 17:45:30.454589 neptune_client-1.3.1/src/neptune/types/__init__.py
+-rw-r--r--   0        0        0      914 2023-06-15 17:45:30.454589 neptune_client-1.3.1/src/neptune/types/atoms/__init__.py
+-rw-r--r--   0        0        0     1626 2023-06-15 17:45:30.454589 neptune_client-1.3.1/src/neptune/types/atoms/artifact.py
+-rw-r--r--   0        0        0      936 2023-06-15 17:45:30.454589 neptune_client-1.3.1/src/neptune/types/atoms/atom.py
+-rw-r--r--   0        0        0     1302 2023-06-15 17:45:30.454589 neptune_client-1.3.1/src/neptune/types/atoms/boolean.py
+-rw-r--r--   0        0        0     1435 2023-06-15 17:45:30.454589 neptune_client-1.3.1/src/neptune/types/atoms/datetime.py
+-rw-r--r--   0        0        0    11695 2023-06-15 17:45:30.454589 neptune_client-1.3.1/src/neptune/types/atoms/file.py
+-rw-r--r--   0        0        0     1297 2023-06-15 17:45:30.454589 neptune_client-1.3.1/src/neptune/types/atoms/float.py
+-rw-r--r--   0        0        0     1902 2023-06-15 17:45:30.454589 neptune_client-1.3.1/src/neptune/types/atoms/git_ref.py
+-rw-r--r--   0        0        0     1299 2023-06-15 17:45:30.454589 neptune_client-1.3.1/src/neptune/types/atoms/integer.py
+-rw-r--r--   0        0        0     1473 2023-06-15 17:45:30.454589 neptune_client-1.3.1/src/neptune/types/atoms/string.py
+-rw-r--r--   0        0        0     1485 2023-06-15 17:45:30.454589 neptune_client-1.3.1/src/neptune/types/file_set.py
+-rw-r--r--   0        0        0      831 2023-06-15 17:45:30.454589 neptune_client-1.3.1/src/neptune/types/mode.py
+-rw-r--r--   0        0        0      777 2023-06-15 17:45:30.454589 neptune_client-1.3.1/src/neptune/types/model_version_stage.py
+-rw-r--r--   0        0        0     1144 2023-06-15 17:45:30.454589 neptune_client-1.3.1/src/neptune/types/namespace.py
+-rw-r--r--   0        0        0      783 2023-06-15 17:45:30.454589 neptune_client-1.3.1/src/neptune/types/series/__init__.py
+-rw-r--r--   0        0        0     2447 2023-06-15 17:45:30.454589 neptune_client-1.3.1/src/neptune/types/series/file_series.py
+-rw-r--r--   0        0        0     2553 2023-06-15 17:45:30.454589 neptune_client-1.3.1/src/neptune/types/series/float_series.py
+-rw-r--r--   0        0        0     1221 2023-06-15 17:45:30.454589 neptune_client-1.3.1/src/neptune/types/series/series.py
+-rw-r--r--   0        0        0     1353 2023-06-15 17:45:30.454589 neptune_client-1.3.1/src/neptune/types/series/series_value.py
+-rw-r--r--   0        0        0     2601 2023-06-15 17:45:30.454589 neptune_client-1.3.1/src/neptune/types/series/string_series.py
+-rw-r--r--   0        0        0      655 2023-06-15 17:45:30.454589 neptune_client-1.3.1/src/neptune/types/sets/__init__.py
+-rw-r--r--   0        0        0      934 2023-06-15 17:45:30.454589 neptune_client-1.3.1/src/neptune/types/sets/set.py
+-rw-r--r--   0        0        0     1119 2023-06-15 17:45:30.454589 neptune_client-1.3.1/src/neptune/types/sets/string_set.py
+-rw-r--r--   0        0        0     3551 2023-06-15 17:45:30.454589 neptune_client-1.3.1/src/neptune/types/type_casting.py
+-rw-r--r--   0        0        0      892 2023-06-15 17:45:30.454589 neptune_client-1.3.1/src/neptune/types/value.py
+-rw-r--r--   0        0        0     1634 2023-06-15 17:45:30.454589 neptune_client-1.3.1/src/neptune/types/value_copy.py
+-rw-r--r--   0        0        0     2596 2023-06-15 17:45:30.454589 neptune_client-1.3.1/src/neptune/types/value_visitor.py
+-rw-r--r--   0        0        0      698 2023-06-15 17:45:30.454589 neptune_client-1.3.1/src/neptune/typing.py
+-rw-r--r--   0        0        0     1755 2023-06-15 17:45:30.454589 neptune_client-1.3.1/src/neptune/utils.py
+-rw-r--r--   0        0        0        0 2023-06-15 17:45:30.454589 neptune_client-1.3.1/src/neptune/vendor/__init__.py
+-rw-r--r--   0        0        0     6306 2023-06-15 17:45:30.454589 neptune_client-1.3.1/src/neptune/vendor/lib_programname.py
+-rw-r--r--   0        0        0    68552 2023-06-15 17:45:30.454589 neptune_client-1.3.1/src/neptune/vendor/pynvml.py
+-rw-r--r--   0        0        0     2228 2023-06-15 17:45:30.454589 neptune_client-1.3.1/src/neptune/version.py
+-rw-r--r--   0        0        0    18218 1970-01-01 00:00:00.000000 neptune_client-1.3.1/PKG-INFO
```

### Comparing `neptune_client-1.3.0/CHANGELOG.md` & `neptune_client-1.3.1/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+## neptune 1.3.1
+
+### Fixes
+- Fix ImportError when git is missing ([#1359](https://github.com/neptune-ai/neptune-client/pull/1359))
+
 ## neptune 1.3.0
 
 ### Features
 - Added automatic tracking of dependencies ([#1345](https://github.com/neptune-ai/neptune-client/pull/1345))
 - Added automatic tracking of uncommitted changes ([#1350]https://github.com/neptune-ai/neptune-client/pull/1350)
 
 ### Fixes
```

### Comparing `neptune_client-1.3.0/LICENSE` & `neptune_client-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/README.md` & `neptune_client-1.3.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -27,22 +27,22 @@
 * Automate and standardize as your modeling team grows.
 * Collaborate on models and results with your team and across the org.
 * Use hosted, deploy on-premises, or in a private cloud. Integrate with any MLOps stack.
 &nbsp;
 
 &nbsp;
 <div align="center">
-    <a href="https://youtu.be/L2CAYip0DmI">
+    <a href="https://www.youtube.com/watch?v=bQzgnqM5J6U">
       <img border="0" alt="neptune.ai explainer video" src="https://raw.githubusercontent.com/neptune-ai/neptune-client/assets/readme/github-explainer-video.png" width="600">
     </a>
 </div>
 &nbsp;
 
 &nbsp;
-<a href="https://app.neptune.ai/showcase/example-project-tensorflow-keras/experiments?split=tbl&dash=charts&viewId=eccd5adf-42b3-497e-9cc2-9fa2655429b3"><b>Play with a live neptune.ai app →</b></a>
+<a href="https://app.neptune.ai/o/showcase/org/onboarding-project/runs/table?viewId=98f66b32-2279-4b73-8210-863021c440ac&product_tour_id=444083"><b>Play with a live neptune.ai app →</b></a>
 &nbsp;
 
 &nbsp;
 ## Getting started
 
 **Step 1:** Create a **[free account](https://neptune.ai/register)**
 
@@ -78,59 +78,59 @@
 * <a href="https://docs.neptune.ai/logging/what_you_can_log/"><b>Any metadata type:</b></a> metrics, parameters, dataset and model versions, images, interactive plots, videos, hardware (GPU, CPU, memory), code state.
 
 * <a href="https://docs.neptune.ai/usage/pipelines/"><b>From anywhere in your ML pipeline:</b></a> multinode pipelines, distributed computing, log during or after execution, log offline, and sync when you are back online.
 &nbsp;
 
 &nbsp;
 <div align="center">
-      <img border="0" alt="all metadata metrics" src="https://raw.githubusercontent.com/neptune-ai/neptune-client/assets/readme/all-metadata-metrics.gif" width="600">
+      <img border="0" alt="all metadata metrics" src="https://neptune.ai/wp-content/uploads/2023/06/log_metrics.gif" width="600">
     </a>
 </div>
 &nbsp;
 
 &nbsp;
 
 **Organize experiments**
 
 Organize logs in a fully customizable nested structure. Display model metadata in user-defined dashboard templates.
 
-* <a href="https://app.neptune.ai/o/showcase/org/example-project-tensorflow-keras/experiments?split=tbl&dash=charts&viewId=4a21e7e9-abab-4f9f-8723-41f5ae4f71e8&product_tour_id=314370"><b>Nested metadata structure:</b></a> flexible API lets you customize the metadata logging structure however you want. Talk to a dictionary at the code level. See the folder structure in the app. Organize nested parameter configs or the results on k-fold validation splits the way they should be.
+* <a href="https://app.neptune.ai/o/showcase/org/onboarding-project/runs/table?viewId=98f66b32-2279-4b73-8210-863021c440ac&product_tour_id=444083"><b>Nested metadata structure:</b></a> flexible API lets you customize the metadata logging structure however you want. Talk to a dictionary at the code level. See the folder structure in the app. Organize nested parameter configs or the results on k-fold validation splits the way they should be.
 
-* <a href="https://app.neptune.ai/o/showcase/org/example-project-tensorflow-keras/experiments?split=tbl&dash=charts&viewId=4a21e7e9-abab-4f9f-8723-41f5ae4f71e8&product_tour_id=314370"><b>Custom dashboards:</b></a> combine different metadata types in one view. Define it for one run. Use anywhere. Look at GPU, memory consumption, and load times to debug training speed. See learning curves, image predictions, and confusion matrix to debug model quality.
+* <a href="https://app.neptune.ai/o/showcase/org/onboarding-project/runs/table?viewId=98f66b32-2279-4b73-8210-863021c440ac&product_tour_id=444083"><b>Custom dashboards:</b></a> combine different metadata types in one view. Define it for one run. Use anywhere. Look at GPU, memory consumption, and load times to debug training speed. See learning curves, image predictions, and confusion matrix to debug model quality.
 
-* <a href="https://app.neptune.ai/o/showcase/org/example-project-tensorflow-keras/experiments?split=tbl&dash=charts&viewId=4a21e7e9-abab-4f9f-8723-41f5ae4f71e8&product_tour_id=314370"><b>Table views:</b></a> create different views of the runs table and save them for later. You can have separate table views for debugging, comparing parameter sets, or best experiments.
+* <a href="https://app.neptune.ai/o/showcase/org/onboarding-project/runs/table?viewId=98f66b32-2279-4b73-8210-863021c440ac&product_tour_id=444083"><b>Table views:</b></a> create different views of the runs table and save them for later. You can have separate table views for debugging, comparing parameter sets, or best experiments.
 &nbsp;
 
 &nbsp;
 <div align="center">
-      <img border="0" alt="organize dashboards" src="https://raw.githubusercontent.com/neptune-ai/neptune-client/assets/readme/organize-dashboards.gif" width="600">
+      <img border="0" alt="organize dashboards" src="https://neptune.ai/wp-content/uploads/2023/06/organize_custom_dashboards.gif" width="600">
     </a>
 </div>
 &nbsp;
 
 &nbsp;
 
 **Compare results**
 
 Visualize training live in the neptune.ai web app. See how different parameters and configs affect the results. Optimize models quicker.
 
-* <a href="https://app.neptune.ai/o/showcase/org/example-project-tensorflow-keras/experiments?split=tbl&dash=charts&viewId=4a21e7e9-abab-4f9f-8723-41f5ae4f71e8&product_tour_id=314370"><b>Compare:</b></a> learning curves, parameters, images, datasets.
+* <a href="https://app.neptune.ai/o/showcase/org/onboarding-project/runs/table?viewId=98f66b32-2279-4b73-8210-863021c440ac&product_tour_id=444083"><b>Compare:</b></a> learning curves, parameters, images, datasets.
 
-* <a href="https://app.neptune.ai/o/showcase/org/example-project-tensorflow-keras/experiments?split=tbl&dash=charts&viewId=4a21e7e9-abab-4f9f-8723-41f5ae4f71e8&product_tour_id=314370"><b>Search, sort, and filter:</b></a> experiments by any field you logged. Use our query language to filter runs based on parameter values, metrics, execution times, or anything else.
+* <a href="https://app.neptune.ai/o/showcase/org/onboarding-project/runs/table?viewId=98f66b32-2279-4b73-8210-863021c440ac&product_tour_id=444083"><b>Search, sort, and filter:</b></a> experiments by any field you logged. Use our query language to filter runs based on parameter values, metrics, execution times, or anything else.
 
-* <a href="https://app.neptune.ai/o/showcase/org/example-project-tensorflow-keras/experiments?split=tbl&dash=charts&viewId=4a21e7e9-abab-4f9f-8723-41f5ae4f71e8&product_tour_id=314370"><b>Visualize and display:</b></a> runs table, interactive display, folder structure, dashboards.
+* <a href="https://app.neptune.ai/o/showcase/org/onboarding-project/runs/table?viewId=98f66b32-2279-4b73-8210-863021c440ac&product_tour_id=444083"><b>Visualize and display:</b></a> runs table, interactive display, folder structure, dashboards.
 
-* <a href="https://app.neptune.ai/o/showcase/org/example-project-tensorflow-keras/experiments?split=tbl&dash=charts&viewId=4a21e7e9-abab-4f9f-8723-41f5ae4f71e8&product_tour_id=314370"><b>Monitor live:</b></a> hardware consumption metrics, GPU, CPU, memory.
+* <a href="https://app.neptune.ai/o/showcase/org/onboarding-project/runs/table?viewId=98f66b32-2279-4b73-8210-863021c440ac&product_tour_id=444083"><b>Monitor live:</b></a> hardware consumption metrics, GPU, CPU, memory.
 
-* <a href="https://app.neptune.ai/o/showcase/org/example-project-tensorflow-keras/experiments?split=tbl&dash=charts&viewId=4a21e7e9-abab-4f9f-8723-41f5ae4f71e8&product_tour_id=314370"><b>Group by:</b></a> dataset versions, parameters.
+* <a href="https://app.neptune.ai/o/showcase/org/onboarding-project/runs/table?viewId=98f66b32-2279-4b73-8210-863021c440ac&product_tour_id=444083"><b>Group by:</b></a> dataset versions, parameters.
 &nbsp;
 
 &nbsp;
 <div align="center">
-      <img border="0" alt="compare, search, filter" src="https://raw.githubusercontent.com/neptune-ai/neptune-client/assets/readme/compare-search-filter.gif" width="600">
+      <img border="0" alt="compare, search, filter" src="https://neptune.ai/wp-content/uploads/2023/06/organize_search_sort_filter.gif" width="600">
     </a>
 </div>
 &nbsp;
 
 &nbsp;
 
 **Register models**
@@ -142,37 +142,37 @@
 * <a href="https://docs.neptune.ai/model_registry/managing_stage/"><b>Review and change stages:</b></a> look at the validation, test metrics and other model metadata. You can move models between None/Staging/Production/Archived.
 
 * <a href="https://docs.neptune.ai/model_registry/overview/"><b>Access and share models:</b></a> every model and model version is accessible via the neptune.ai web app or through the API.
 &nbsp;
 
 &nbsp;
 <div align="center">
-      <img border="0" alt="register stages" src="https://raw.githubusercontent.com/neptune-ai/neptune-client/assets/readme/register-stages.gif" width="600">
+      <img border="0" alt="register models" src="https://neptune.ai/wp-content/uploads/2023/06/register_models.gif" width="600">
     </a>
 </div>
 &nbsp;
 
 &nbsp;
 
 **Share results**
 
 Have a single place where your team can see the results and access all models and experiments.
 
 * <a href="https://docs.neptune.ai/about/collaboration/"><b>Send a link:</b></a> share every chart, dashboard, table view, or anything else you see in the neptune.ai app by copying and sending persistent URLs.
 
 * <a href="https://docs.neptune.ai/usage/querying_metadata/"><b>Query API:</b></a> access all model metadata via neptune.ai API. Whatever you logged, you can query in a similar way.
 
-* <a href="https://neptune.ai/pricing"><b>Manage users and projects:</b></a> create different projects, add users to them, and grant different permissions levels.
+* <a href="https://docs.neptune.ai/management/"><b>Manage users and projects:</b></a> create different projects, add users to them, and grant different permissions levels.
 
 * <a href="https://neptune.ai/pricing"><b>Add your entire org:</b></a> get unlimited users on every paid plan. So you can invite your entire organization, including product managers and subject matter experts at no extra cost.
 &nbsp;
 
 &nbsp;
 <div align="center">
-      <img border="0" alt="share persistent link" src="https://raw.githubusercontent.com/neptune-ai/neptune-client/assets/readme/share-persistent-link.gif" width="600">
+      <img border="0" alt="share persistent link" src="https://neptune.ai/wp-content/uploads/2023/06/share_send_link.gif" width="600">
     </a>
 </div>
 &nbsp;
 
 &nbsp;
 ## Integrate with any MLOps stack
 neptune.ai integrates with <a href="https://docs.neptune.ai/integrations/"><b>25+ frameworks:</b></a> PyTorch, PyTorch Lightning, TensorFlow/Keras, LightGBM, scikit-learn, XGBoost, Optuna, Kedro, 🤗 Transformers, fastai, Prophet, and more.
```

#### html2text {}

```diff
@@ -53,15 +53,15 @@
     **Register models** Version, review, and access production-ready models and
 metadata associated with them in a single place. * Version_models: register
 models, create model versions, version external model artifacts. * Review_and
 change_stages: look at the validation, test metrics and other model metadata.
 You can move models between None/Staging/Production/Archived. * Access_and
 share_models: every model and model version is accessible via the neptune.ai
 web app or through the API.    
-                               [register stages]
+                               [register models]
     **Share results** Have a single place where your team can see the results
 and access all models and experiments. * Send_a_link: share every chart,
 dashboard, table view, or anything else you see in the neptune.ai app by
 copying and sending persistent URLs. * Query_API: access all model metadata via
 neptune.ai API. Whatever you logged, you can query in a similar way. * Manage
 users_and_projects: create different projects, add users to them, and grant
 different permissions levels. * Add_your_entire_org: get unlimited users on
```

### Comparing `neptune_client-1.3.0/pyproject.toml` & `neptune_client-1.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -131,15 +131,15 @@
 repository = "https://github.com/neptune-ai/neptune-client"
 homepage = "https://neptune.ai/"
 documentation = "https://docs.neptune.ai/"
 include = ["CHANGELOG.md"]
 license = "Apache License 2.0"
 name = "neptune-client"
 readme = "README.md"
-version = "1.3.0"
+version = "1.3.1"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: Apache Software License",
     "Natural Language :: English",
```

### Comparing `neptune_client-1.3.0/src/neptune/__init__.py` & `neptune_client-1.3.1/src/neptune/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/attributes/__init__.py` & `neptune_client-1.3.1/src/neptune/attributes/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/attributes/atoms/__init__.py` & `neptune_client-1.3.1/src/neptune/attributes/atoms/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/attributes/atoms/artifact.py` & `neptune_client-1.3.1/src/neptune/attributes/atoms/artifact.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/attributes/atoms/atom.py` & `neptune_client-1.3.1/src/neptune/attributes/atoms/atom.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/attributes/atoms/boolean.py` & `neptune_client-1.3.1/src/neptune/attributes/atoms/boolean.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/attributes/atoms/copiable_atom.py` & `neptune_client-1.3.1/src/neptune/attributes/atoms/copiable_atom.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/attributes/atoms/datetime.py` & `neptune_client-1.3.1/src/neptune/attributes/atoms/datetime.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/attributes/atoms/file.py` & `neptune_client-1.3.1/src/neptune/attributes/atoms/file.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/attributes/atoms/float.py` & `neptune_client-1.3.1/src/neptune/attributes/atoms/float.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/attributes/atoms/git_ref.py` & `neptune_client-1.3.1/src/neptune/attributes/atoms/git_ref.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/attributes/atoms/integer.py` & `neptune_client-1.3.1/src/neptune/attributes/atoms/integer.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/attributes/atoms/notebook_ref.py` & `neptune_client-1.3.1/src/neptune/attributes/atoms/notebook_ref.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/attributes/atoms/run_state.py` & `neptune_client-1.3.1/src/neptune/attributes/atoms/run_state.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/attributes/atoms/string.py` & `neptune_client-1.3.1/src/neptune/attributes/atoms/string.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/attributes/attribute.py` & `neptune_client-1.3.1/src/neptune/attributes/attribute.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/attributes/constants.py` & `neptune_client-1.3.1/src/neptune/attributes/constants.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/attributes/file_set.py` & `neptune_client-1.3.1/src/neptune/attributes/file_set.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/attributes/namespace.py` & `neptune_client-1.3.1/src/neptune/attributes/namespace.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/attributes/series/__init__.py` & `neptune_client-1.3.1/src/neptune/attributes/series/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/attributes/series/fetchable_series.py` & `neptune_client-1.3.1/src/neptune/attributes/series/fetchable_series.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/attributes/series/file_series.py` & `neptune_client-1.3.1/src/neptune/attributes/series/file_series.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/attributes/series/float_series.py` & `neptune_client-1.3.1/src/neptune/attributes/series/float_series.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/attributes/series/series.py` & `neptune_client-1.3.1/src/neptune/attributes/series/series.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/attributes/series/string_series.py` & `neptune_client-1.3.1/src/neptune/attributes/series/string_series.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/attributes/sets/__init__.py` & `neptune_client-1.3.1/src/neptune/attributes/sets/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/attributes/sets/set.py` & `neptune_client-1.3.1/src/neptune/attributes/sets/set.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/attributes/sets/string_set.py` & `neptune_client-1.3.1/src/neptune/attributes/sets/string_set.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/attributes/utils.py` & `neptune_client-1.3.1/src/neptune/attributes/utils.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/cli/__init__.py` & `neptune_client-1.3.1/src/neptune/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/cli/__main__.py` & `neptune_client-1.3.1/src/neptune/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/cli/abstract_backend_runner.py` & `neptune_client-1.3.1/src/neptune/cli/abstract_backend_runner.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/cli/clear.py` & `neptune_client-1.3.1/src/neptune/cli/clear.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/cli/commands.py` & `neptune_client-1.3.1/src/neptune/cli/commands.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/cli/container_manager.py` & `neptune_client-1.3.1/src/neptune/cli/container_manager.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/cli/path_option.py` & `neptune_client-1.3.1/src/neptune/cli/path_option.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/cli/status.py` & `neptune_client-1.3.1/src/neptune/cli/status.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/cli/sync.py` & `neptune_client-1.3.1/src/neptune/cli/sync.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/cli/utils.py` & `neptune_client-1.3.1/src/neptune/cli/utils.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/common/__init__.py` & `neptune_client-1.3.1/src/neptune/common/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/common/backends/__init__.py` & `neptune_client-1.3.1/src/neptune/common/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/common/backends/api_model.py` & `neptune_client-1.3.1/src/neptune/common/backends/api_model.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/common/backends/utils.py` & `neptune_client-1.3.1/src/neptune/common/backends/utils.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/common/envs.py` & `neptune_client-1.3.1/src/neptune/common/envs.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/common/exceptions.py` & `neptune_client-1.3.1/src/neptune/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/common/experiments.py` & `neptune_client-1.3.1/src/neptune/common/experiments.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/common/git_info.py` & `neptune_client-1.3.1/src/neptune/common/git_info.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/common/hardware/__init__.py` & `neptune_client-1.3.1/src/neptune/common/hardware/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/common/hardware/cgroup/__init__.py` & `neptune_client-1.3.1/src/neptune/common/hardware/cgroup/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/common/hardware/cgroup/cgroup_filesystem_reader.py` & `neptune_client-1.3.1/src/neptune/common/hardware/cgroup/cgroup_filesystem_reader.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/common/hardware/cgroup/cgroup_monitor.py` & `neptune_client-1.3.1/src/neptune/common/hardware/cgroup/cgroup_monitor.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/common/hardware/constants.py` & `neptune_client-1.3.1/src/neptune/common/hardware/constants.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/common/hardware/gauges/__init__.py` & `neptune_client-1.3.1/src/neptune/common/hardware/gauges/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/common/hardware/gauges/cpu.py` & `neptune_client-1.3.1/src/neptune/common/hardware/gauges/cpu.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/common/hardware/gauges/gauge.py` & `neptune_client-1.3.1/src/neptune/common/hardware/gauges/gauge.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/common/hardware/gauges/gauge_factory.py` & `neptune_client-1.3.1/src/neptune/common/hardware/gauges/gauge_factory.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/common/hardware/gauges/gauge_mode.py` & `neptune_client-1.3.1/src/neptune/common/hardware/gauges/gauge_mode.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/common/hardware/gauges/gpu.py` & `neptune_client-1.3.1/src/neptune/common/hardware/gauges/gpu.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/common/hardware/gauges/memory.py` & `neptune_client-1.3.1/src/neptune/common/hardware/gauges/memory.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/common/hardware/gpu/__init__.py` & `neptune_client-1.3.1/src/neptune/common/hardware/gpu/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/common/hardware/gpu/gpu_monitor.py` & `neptune_client-1.3.1/src/neptune/common/hardware/gpu/gpu_monitor.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/common/hardware/metrics/__init__.py` & `neptune_client-1.3.1/src/neptune/common/hardware/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/common/hardware/metrics/metric.py` & `neptune_client-1.3.1/src/neptune/common/hardware/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/common/hardware/metrics/metrics_container.py` & `neptune_client-1.3.1/src/neptune/common/hardware/metrics/metrics_container.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/common/hardware/metrics/metrics_factory.py` & `neptune_client-1.3.1/src/neptune/common/hardware/metrics/metrics_factory.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/common/hardware/metrics/reports/__init__.py` & `neptune_client-1.3.1/src/neptune/common/hardware/metrics/reports/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/common/hardware/metrics/reports/metric_report.py` & `neptune_client-1.3.1/src/neptune/common/hardware/metrics/reports/metric_report.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/common/hardware/metrics/reports/metric_reporter.py` & `neptune_client-1.3.1/src/neptune/common/hardware/metrics/reports/metric_reporter.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/common/hardware/metrics/reports/metric_reporter_factory.py` & `neptune_client-1.3.1/src/neptune/common/hardware/metrics/reports/metric_reporter_factory.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/common/hardware/metrics/service/__init__.py` & `neptune_client-1.3.1/src/neptune/common/hardware/metrics/service/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/common/hardware/metrics/service/metric_service.py` & `neptune_client-1.3.1/src/neptune/common/hardware/metrics/service/metric_service.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/common/hardware/metrics/service/metric_service_factory.py` & `neptune_client-1.3.1/src/neptune/common/hardware/metrics/service/metric_service_factory.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/common/hardware/resources/__init__.py` & `neptune_client-1.3.1/src/neptune/common/hardware/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/common/hardware/resources/gpu_card_indices_provider.py` & `neptune_client-1.3.1/src/neptune/common/hardware/resources/gpu_card_indices_provider.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/common/hardware/resources/system_resource_info.py` & `neptune_client-1.3.1/src/neptune/common/hardware/resources/system_resource_info.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/common/hardware/resources/system_resource_info_factory.py` & `neptune_client-1.3.1/src/neptune/common/hardware/resources/system_resource_info_factory.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/common/hardware/system/__init__.py` & `neptune_client-1.3.1/src/neptune/common/hardware/system/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/common/hardware/system/system_monitor.py` & `neptune_client-1.3.1/src/neptune/common/hardware/system/system_monitor.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/common/oauth.py` & `neptune_client-1.3.1/src/neptune/common/oauth.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/common/patches/__init__.py` & `neptune_client-1.3.1/src/neptune/common/patches/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/common/patches/bravado.py` & `neptune_client-1.3.1/src/neptune/common/patches/bravado.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/common/patterns.py` & `neptune_client-1.3.1/src/neptune/common/patterns.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/common/storage/__init__.py` & `neptune_client-1.3.1/src/neptune/common/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/common/storage/datastream.py` & `neptune_client-1.3.1/src/neptune/common/storage/datastream.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/common/storage/storage_utils.py` & `neptune_client-1.3.1/src/neptune/common/storage/storage_utils.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/common/utils.py` & `neptune_client-1.3.1/src/neptune/common/utils.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/common/warnings.py` & `neptune_client-1.3.1/src/neptune/common/warnings.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/common/websockets/__init__.py` & `neptune_client-1.3.1/src/neptune/common/websockets/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/common/websockets/reconnecting_websocket.py` & `neptune_client-1.3.1/src/neptune/common/websockets/reconnecting_websocket.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/common/websockets/websocket_client_adapter.py` & `neptune_client-1.3.1/src/neptune/common/websockets/websocket_client_adapter.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/constants.py` & `neptune_client-1.3.1/src/neptune/constants.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/envs.py` & `neptune_client-1.3.1/src/neptune/envs.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/exceptions.py` & `neptune_client-1.3.1/src/neptune/exceptions.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/handler.py` & `neptune_client-1.3.1/src/neptune/handler.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/integrations/__init__.py` & `neptune_client-1.3.1/src/neptune/integrations/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/integrations/aws/__init__.py` & `neptune_client-1.3.1/src/neptune/integrations/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/integrations/detectron2/__init__.py` & `neptune_client-1.3.1/src/neptune/integrations/detectron2/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/integrations/fastai/__init__.py` & `neptune_client-1.3.1/src/neptune/integrations/fastai/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/integrations/kedro/__init__.py` & `neptune_client-1.3.1/src/neptune/integrations/kedro/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/integrations/lightgbm/__init__.py` & `neptune_client-1.3.1/src/neptune/integrations/lightgbm/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/integrations/optuna/__init__.py` & `neptune_client-1.3.1/src/neptune/integrations/optuna/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/integrations/prophet/__init__.py` & `neptune_client-1.3.1/src/neptune/integrations/prophet/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/integrations/python_logger.py` & `neptune_client-1.3.1/src/neptune/integrations/python_logger.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/integrations/pytorch/__init__.py` & `neptune_client-1.3.1/src/neptune/integrations/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/integrations/pytorch_lightning/__init__.py` & `neptune_client-1.3.1/src/neptune/integrations/pytorch_lightning/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/integrations/sacred/__init__.py` & `neptune_client-1.3.1/src/neptune/integrations/sacred/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/integrations/sklearn/__init__.py` & `neptune_client-1.3.1/src/neptune/integrations/sklearn/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/integrations/tensorflow_keras/__init__.py` & `neptune_client-1.3.1/src/neptune/integrations/tensorflow_keras/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/integrations/transformers/__init__.py` & `neptune_client-1.3.1/src/neptune/integrations/transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/integrations/utils.py` & `neptune_client-1.3.1/src/neptune/integrations/utils.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/integrations/xgboost/__init__.py` & `neptune_client-1.3.1/src/neptune/integrations/xgboost/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/internal/__init__.py` & `neptune_client-1.3.1/src/neptune/internal/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/internal/artifacts/__init__.py` & `neptune_client-1.3.1/src/neptune/internal/artifacts/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/internal/artifacts/drivers/__init__.py` & `neptune_client-1.3.1/src/neptune/internal/artifacts/drivers/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/internal/artifacts/drivers/local.py` & `neptune_client-1.3.1/src/neptune/internal/artifacts/drivers/local.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/internal/artifacts/drivers/s3.py` & `neptune_client-1.3.1/src/neptune/internal/artifacts/drivers/s3.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/internal/artifacts/file_hasher.py` & `neptune_client-1.3.1/src/neptune/internal/artifacts/file_hasher.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/internal/artifacts/local_file_hash_storage.py` & `neptune_client-1.3.1/src/neptune/internal/artifacts/local_file_hash_storage.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/internal/artifacts/types.py` & `neptune_client-1.3.1/src/neptune/internal/artifacts/types.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/internal/artifacts/utils.py` & `neptune_client-1.3.1/src/neptune/internal/artifacts/utils.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/internal/backends/__init__.py` & `neptune_client-1.3.1/src/neptune/internal/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/internal/backends/api_model.py` & `neptune_client-1.3.1/src/neptune/internal/backends/api_model.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/internal/backends/factory.py` & `neptune_client-1.3.1/src/neptune/internal/backends/factory.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/internal/backends/hosted_artifact_operations.py` & `neptune_client-1.3.1/src/neptune/internal/backends/hosted_artifact_operations.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/internal/backends/hosted_client.py` & `neptune_client-1.3.1/src/neptune/internal/backends/hosted_client.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/internal/backends/hosted_file_operations.py` & `neptune_client-1.3.1/src/neptune/internal/backends/hosted_file_operations.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/internal/backends/hosted_neptune_backend.py` & `neptune_client-1.3.1/src/neptune/internal/backends/hosted_neptune_backend.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/internal/backends/neptune_backend.py` & `neptune_client-1.3.1/src/neptune/internal/backends/neptune_backend.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/internal/backends/neptune_backend_mock.py` & `neptune_client-1.3.1/src/neptune/internal/backends/neptune_backend_mock.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/internal/backends/nql.py` & `neptune_client-1.3.1/src/neptune/internal/backends/nql.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/internal/backends/offline_neptune_backend.py` & `neptune_client-1.3.1/src/neptune/internal/backends/offline_neptune_backend.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/internal/backends/operation_api_name_visitor.py` & `neptune_client-1.3.1/src/neptune/internal/backends/operation_api_name_visitor.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/internal/backends/operation_api_object_converter.py` & `neptune_client-1.3.1/src/neptune/internal/backends/operation_api_object_converter.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/internal/backends/operations_preprocessor.py` & `neptune_client-1.3.1/src/neptune/internal/backends/operations_preprocessor.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/internal/backends/project_name_lookup.py` & `neptune_client-1.3.1/src/neptune/internal/backends/project_name_lookup.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/internal/backends/swagger_client_wrapper.py` & `neptune_client-1.3.1/src/neptune/internal/backends/swagger_client_wrapper.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/internal/backends/utils.py` & `neptune_client-1.3.1/src/neptune/internal/backends/utils.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/internal/backgroud_job_list.py` & `neptune_client-1.3.1/src/neptune/internal/backgroud_job_list.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/internal/background_job.py` & `neptune_client-1.3.1/src/neptune/internal/background_job.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/internal/container_structure.py` & `neptune_client-1.3.1/src/neptune/internal/container_structure.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/internal/container_type.py` & `neptune_client-1.3.1/src/neptune/internal/container_type.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/internal/credentials.py` & `neptune_client-1.3.1/src/neptune/internal/credentials.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/internal/disk_queue.py` & `neptune_client-1.3.1/src/neptune/internal/disk_queue.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/internal/exceptions.py` & `neptune_client-1.3.1/src/neptune/internal/exceptions.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/internal/hardware/__init__.py` & `neptune_client-1.3.1/src/neptune/internal/hardware/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/internal/hardware/gpu/__init__.py` & `neptune_client-1.3.1/src/neptune/internal/hardware/gpu/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/internal/hardware/gpu/gpu_monitor.py` & `neptune_client-1.3.1/src/neptune/internal/hardware/gpu/gpu_monitor.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/internal/hardware/hardware_metric_reporting_job.py` & `neptune_client-1.3.1/src/neptune/internal/hardware/hardware_metric_reporting_job.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/internal/id_formats.py` & `neptune_client-1.3.1/src/neptune/internal/id_formats.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/internal/init/__init__.py` & `neptune_client-1.3.1/src/neptune/internal/init/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/internal/init/parameters.py` & `neptune_client-1.3.1/src/neptune/internal/init/parameters.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/internal/notebooks/__init__.py` & `neptune_client-1.3.1/src/neptune/internal/notebooks/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/internal/notebooks/comm.py` & `neptune_client-1.3.1/src/neptune/internal/notebooks/comm.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/internal/notebooks/notebooks.py` & `neptune_client-1.3.1/src/neptune/internal/notebooks/notebooks.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/internal/operation.py` & `neptune_client-1.3.1/src/neptune/internal/operation.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/internal/operation_processors/__init__.py` & `neptune_client-1.3.1/src/neptune/internal/operation_processors/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/internal/operation_processors/async_operation_processor.py` & `neptune_client-1.3.1/src/neptune/internal/operation_processors/async_operation_processor.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/internal/operation_processors/factory.py` & `neptune_client-1.3.1/src/neptune/internal/operation_processors/factory.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/internal/operation_processors/offline_operation_processor.py` & `neptune_client-1.3.1/src/neptune/internal/operation_processors/offline_operation_processor.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/internal/operation_processors/operation_processor.py` & `neptune_client-1.3.1/src/neptune/internal/operation_processors/operation_processor.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/internal/operation_processors/operation_storage.py` & `neptune_client-1.3.1/src/neptune/internal/operation_processors/operation_storage.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/internal/operation_processors/read_only_operation_processor.py` & `neptune_client-1.3.1/src/neptune/internal/operation_processors/read_only_operation_processor.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/internal/operation_processors/sync_operation_processor.py` & `neptune_client-1.3.1/src/neptune/internal/operation_processors/sync_operation_processor.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/internal/operation_visitor.py` & `neptune_client-1.3.1/src/neptune/internal/operation_visitor.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/internal/state.py` & `neptune_client-1.3.1/src/neptune/internal/state.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/internal/streams/__init__.py` & `neptune_client-1.3.1/src/neptune/internal/streams/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/internal/streams/std_capture_background_job.py` & `neptune_client-1.3.1/src/neptune/internal/streams/std_capture_background_job.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/internal/streams/std_stream_capture_logger.py` & `neptune_client-1.3.1/src/neptune/internal/streams/std_stream_capture_logger.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/internal/threading/__init__.py` & `neptune_client-1.3.1/src/neptune/internal/threading/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/internal/threading/daemon.py` & `neptune_client-1.3.1/src/neptune/internal/threading/daemon.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/internal/types/__init__.py` & `neptune_client-1.3.1/src/neptune/internal/types/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/internal/types/file_types.py` & `neptune_client-1.3.1/src/neptune/internal/types/file_types.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/internal/types/stringify_value.py` & `neptune_client-1.3.1/src/neptune/internal/types/stringify_value.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/internal/utils/__init__.py` & `neptune_client-1.3.1/src/neptune/internal/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/internal/utils/dependency_tracking.py` & `neptune_client-1.3.1/src/neptune/internal/utils/dependency_tracking.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/internal/utils/deprecation.py` & `neptune_client-1.3.1/src/neptune/internal/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/internal/utils/generic_attribute_mapper.py` & `neptune_client-1.3.1/src/neptune/internal/utils/generic_attribute_mapper.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/internal/utils/git.py` & `neptune_client-1.3.1/src/neptune/internal/utils/git.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,32 +26,27 @@
 from typing import (
     TYPE_CHECKING,
     List,
     Optional,
     Union,
 )
 
-import git
-from git.exc import (
-    GitCommandError,
-    InvalidGitRepositoryError,
-    NoSuchPathError,
-)
-
 from neptune.attributes.constants import (
     DIFF_HEAD_INDEX_PATH,
     UPSTREAM_INDEX_DIFF,
 )
 from neptune.types import File
 from neptune.types.atoms.git_ref import (
     GitRef,
     GitRefDisabled,
 )
 
 if TYPE_CHECKING:
+    import git
+
     from neptune import Run
 
 _logger = logging.getLogger(__name__)
 
 
 @dataclass
 class GitInfo:
@@ -72,25 +67,33 @@
         import git
 
         return git.Repo(repo_path, search_parent_directories=True)
     except ImportError:
         warnings.warn("GitPython could not be initialized")
 
 
-def get_repo_from_git_ref(git_ref: Union[GitRef, GitRefDisabled]) -> Optional[git.Repo]:
+def get_repo_from_git_ref(git_ref: Union[GitRef, GitRefDisabled]) -> Optional["git.Repo"]:
     if git_ref == GitRef.DISABLED:
         return None
 
     initial_repo_path = git_ref.resolve_path()
     if initial_repo_path is None:
         return None
 
     try:
-        return get_git_repo(repo_path=initial_repo_path)
-    except (NoSuchPathError, InvalidGitRepositoryError):
+        from git.exc import (
+            InvalidGitRepositoryError,
+            NoSuchPathError,
+        )
+
+        try:
+            return get_git_repo(repo_path=initial_repo_path)
+        except (NoSuchPathError, InvalidGitRepositoryError):
+            return None
+    except ImportError:
         return None
 
 
 def to_git_info(git_ref: Union[GitRef, GitRefDisabled]) -> Optional[GitInfo]:
     try:
         repo = get_repo_from_git_ref(git_ref)
         commit = repo.head.commit
@@ -122,58 +125,68 @@
 @dataclass
 class UncommittedChanges:
     diff_head: Optional[str]
     diff_upstream: Optional[str]
     upstream_sha: Optional[str]
 
 
-def get_diff(repo: git.Repo, commit_ref: str) -> Optional[str]:
+def get_diff(repo: "git.Repo", commit_ref: str) -> Optional[str]:
     try:
-        return repo.git.diff(commit_ref)
-    except GitCommandError:
-        return
+        from git.exc import GitCommandError
+
+        try:
+            return repo.git.diff(commit_ref)
+        except GitCommandError:
+            return
+    except ImportError:
+        return None
 
 
-def get_relevant_upstream_commit(repo: git.Repo) -> Optional[git.Commit]:
+def get_relevant_upstream_commit(repo: "git.Repo") -> Optional["git.Commit"]:
     try:
         tracking_branch = repo.active_branch.tracking_branch()
     except (TypeError, ValueError):
         return
 
     if tracking_branch:
         return tracking_branch.commit
 
     return search_for_most_recent_ancestor(repo)
 
 
-def search_for_most_recent_ancestor(repo: git.Repo) -> Optional[git.Commit]:
-    most_recent_ancestor: Optional[git.Commit] = None
+def search_for_most_recent_ancestor(repo: "git.Repo") -> Optional["git.Commit"]:
+    most_recent_ancestor: Optional["git.Commit"] = None
 
     try:
-        for branch in repo.heads:
-            tracking_branch = branch.tracking_branch()
-            if tracking_branch:
-                for ancestor in repo.merge_base(repo.head, tracking_branch.commit):
-                    if not most_recent_ancestor or repo.is_ancestor(most_recent_ancestor, ancestor):
-                        most_recent_ancestor = ancestor
-    except GitCommandError:
-        pass
+        from git.exc import GitCommandError
+
+        try:
+            for branch in repo.heads:
+                tracking_branch = branch.tracking_branch()
+                if tracking_branch:
+                    for ancestor in repo.merge_base(repo.head, tracking_branch.commit):
+                        if not most_recent_ancestor or repo.is_ancestor(most_recent_ancestor, ancestor):
+                            most_recent_ancestor = ancestor
+        except GitCommandError:
+            pass
+    except ImportError:
+        return None
 
     return most_recent_ancestor
 
 
-def get_upstream_index_sha(repo: git.Repo) -> Optional[str]:
+def get_upstream_index_sha(repo: "git.Repo") -> Optional[str]:
     upstream_commit = get_relevant_upstream_commit(repo)
 
     if upstream_commit and upstream_commit != repo.head.commit:
 
         return upstream_commit.hexsha
 
 
-def get_uncommitted_changes(repo: Optional[git.Repo]) -> Optional[UncommittedChanges]:
+def get_uncommitted_changes(repo: Optional["git.Repo"]) -> Optional[UncommittedChanges]:
     if not repo.is_dirty():
         return
 
     head_index_diff = get_diff(repo, repo.head.name)
 
     upstream_sha = get_upstream_index_sha(repo)
```

### Comparing `neptune_client-1.3.0/src/neptune/internal/utils/hashing.py` & `neptune_client-1.3.1/src/neptune/internal/utils/hashing.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/internal/utils/images.py` & `neptune_client-1.3.1/src/neptune/internal/utils/images.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/internal/utils/iteration.py` & `neptune_client-1.3.1/src/neptune/internal/utils/iteration.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/internal/utils/json_file_splitter.py` & `neptune_client-1.3.1/src/neptune/internal/utils/json_file_splitter.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/internal/utils/limits.py` & `neptune_client-1.3.1/src/neptune/internal/utils/limits.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/internal/utils/logger.py` & `neptune_client-1.3.1/src/neptune/internal/utils/logger.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/internal/utils/paths.py` & `neptune_client-1.3.1/src/neptune/internal/utils/paths.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/internal/utils/ping_background_job.py` & `neptune_client-1.3.1/src/neptune/internal/utils/ping_background_job.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/internal/utils/process_killer.py` & `neptune_client-1.3.1/src/neptune/internal/utils/process_killer.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/internal/utils/run_state.py` & `neptune_client-1.3.1/src/neptune/internal/utils/run_state.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/internal/utils/runningmode.py` & `neptune_client-1.3.1/src/neptune/internal/utils/runningmode.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/internal/utils/s3.py` & `neptune_client-1.3.1/src/neptune/internal/utils/s3.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/internal/utils/source_code.py` & `neptune_client-1.3.1/src/neptune/internal/utils/source_code.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/internal/utils/sync_offset_file.py` & `neptune_client-1.3.1/src/neptune/internal/utils/sync_offset_file.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/internal/utils/traceback_job.py` & `neptune_client-1.3.1/src/neptune/internal/utils/traceback_job.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/internal/utils/uncaught_exception_handler.py` & `neptune_client-1.3.1/src/neptune/internal/utils/uncaught_exception_handler.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/internal/value_to_attribute_visitor.py` & `neptune_client-1.3.1/src/neptune/internal/value_to_attribute_visitor.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/internal/websockets/__init__.py` & `neptune_client-1.3.1/src/neptune/internal/websockets/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/internal/websockets/websocket_signals_background_job.py` & `neptune_client-1.3.1/src/neptune/internal/websockets/websocket_signals_background_job.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/internal/websockets/websockets_factory.py` & `neptune_client-1.3.1/src/neptune/internal/websockets/websockets_factory.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/legacy/__init__.py` & `neptune_client-1.3.1/src/neptune/legacy/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/legacy/api_exceptions.py` & `neptune_client-1.3.1/src/neptune/legacy/api_exceptions.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/legacy/backend.py` & `neptune_client-1.3.1/src/neptune/legacy/backend.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/legacy/checkpoint.py` & `neptune_client-1.3.1/src/neptune/legacy/checkpoint.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/legacy/constants.py` & `neptune_client-1.3.1/src/neptune/legacy/constants.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/legacy/envs.py` & `neptune_client-1.3.1/src/neptune/legacy/envs.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/legacy/exceptions.py` & `neptune_client-1.3.1/src/neptune/legacy/exceptions.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/legacy/experiments.py` & `neptune_client-1.3.1/src/neptune/legacy/experiments.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/legacy/git_info.py` & `neptune_client-1.3.1/src/neptune/legacy/git_info.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/legacy/internal/__init__.py` & `neptune_client-1.3.1/src/neptune/legacy/internal/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/legacy/internal/abort.py` & `neptune_client-1.3.1/src/neptune/legacy/internal/abort.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/legacy/internal/api_clients/__init__.py` & `neptune_client-1.3.1/src/neptune/legacy/internal/api_clients/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/legacy/internal/api_clients/backend_factory.py` & `neptune_client-1.3.1/src/neptune/legacy/internal/api_clients/backend_factory.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/legacy/internal/api_clients/client_config.py` & `neptune_client-1.3.1/src/neptune/legacy/internal/api_clients/client_config.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/legacy/internal/api_clients/credentials.py` & `neptune_client-1.3.1/src/neptune/legacy/internal/api_clients/credentials.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/legacy/internal/api_clients/hosted_api_clients/__init__.py` & `neptune_client-1.3.1/src/neptune/legacy/internal/api_clients/hosted_api_clients/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/legacy/internal/api_clients/hosted_api_clients/hosted_alpha_leaderboard_api_client.py` & `neptune_client-1.3.1/src/neptune/legacy/internal/api_clients/hosted_api_clients/hosted_alpha_leaderboard_api_client.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/legacy/internal/api_clients/hosted_api_clients/hosted_backend_api_client.py` & `neptune_client-1.3.1/src/neptune/legacy/internal/api_clients/hosted_api_clients/hosted_backend_api_client.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/legacy/internal/api_clients/hosted_api_clients/mixins.py` & `neptune_client-1.3.1/src/neptune/legacy/internal/api_clients/hosted_api_clients/mixins.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/legacy/internal/api_clients/hosted_api_clients/utils.py` & `neptune_client-1.3.1/src/neptune/legacy/internal/api_clients/hosted_api_clients/utils.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/legacy/internal/api_clients/offline_backend.py` & `neptune_client-1.3.1/src/neptune/legacy/internal/api_clients/offline_backend.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/legacy/internal/backends/__init__.py` & `neptune_client-1.3.1/src/neptune/legacy/internal/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/legacy/internal/backends/hosted_neptune_backend.py` & `neptune_client-1.3.1/src/neptune/legacy/internal/backends/hosted_neptune_backend.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/legacy/internal/channels/__init__.py` & `neptune_client-1.3.1/src/neptune/legacy/internal/channels/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/legacy/internal/channels/channels.py` & `neptune_client-1.3.1/src/neptune/legacy/internal/channels/channels.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/legacy/internal/channels/channels_values_sender.py` & `neptune_client-1.3.1/src/neptune/legacy/internal/channels/channels_values_sender.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/legacy/internal/execution/__init__.py` & `neptune_client-1.3.1/src/neptune/legacy/internal/execution/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/legacy/internal/execution/execution_context.py` & `neptune_client-1.3.1/src/neptune/legacy/internal/execution/execution_context.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/legacy/internal/experiments/__init__.py` & `neptune_client-1.3.1/src/neptune/legacy/internal/experiments/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/legacy/internal/notebooks/__init__.py` & `neptune_client-1.3.1/src/neptune/legacy/internal/notebooks/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/legacy/internal/notebooks/comm.py` & `neptune_client-1.3.1/src/neptune/legacy/internal/notebooks/comm.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/legacy/internal/notebooks/notebooks.py` & `neptune_client-1.3.1/src/neptune/legacy/internal/notebooks/notebooks.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/legacy/internal/streams/__init__.py` & `neptune_client-1.3.1/src/neptune/legacy/internal/streams/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/legacy/internal/streams/channel_writer.py` & `neptune_client-1.3.1/src/neptune/legacy/internal/streams/channel_writer.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/legacy/internal/streams/stdstream_uploader.py` & `neptune_client-1.3.1/src/neptune/legacy/internal/streams/stdstream_uploader.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/legacy/internal/threads/__init__.py` & `neptune_client-1.3.1/src/neptune/legacy/internal/threads/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/legacy/internal/threads/aborting_thread.py` & `neptune_client-1.3.1/src/neptune/legacy/internal/threads/aborting_thread.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/legacy/internal/threads/hardware_metric_reporting_thread.py` & `neptune_client-1.3.1/src/neptune/legacy/internal/threads/hardware_metric_reporting_thread.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/legacy/internal/threads/neptune_thread.py` & `neptune_client-1.3.1/src/neptune/legacy/internal/threads/neptune_thread.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/legacy/internal/threads/ping_thread.py` & `neptune_client-1.3.1/src/neptune/legacy/internal/threads/ping_thread.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/legacy/internal/utils/__init__.py` & `neptune_client-1.3.1/src/neptune/legacy/internal/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/legacy/internal/utils/alpha_integration.py` & `neptune_client-1.3.1/src/neptune/legacy/internal/utils/alpha_integration.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/legacy/internal/utils/deprecation.py` & `neptune_client-1.3.1/src/neptune/legacy/internal/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/legacy/internal/utils/http.py` & `neptune_client-1.3.1/src/neptune/legacy/internal/utils/http.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/legacy/internal/utils/http_utils.py` & `neptune_client-1.3.1/src/neptune/legacy/internal/utils/http_utils.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/legacy/internal/utils/image.py` & `neptune_client-1.3.1/src/neptune/legacy/internal/utils/image.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/legacy/internal/utils/source_code.py` & `neptune_client-1.3.1/src/neptune/legacy/internal/utils/source_code.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/legacy/internal/websockets/__init__.py` & `neptune_client-1.3.1/src/neptune/legacy/internal/websockets/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/legacy/internal/websockets/message.py` & `neptune_client-1.3.1/src/neptune/legacy/internal/websockets/message.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/legacy/internal/websockets/reconnecting_websocket_factory.py` & `neptune_client-1.3.1/src/neptune/legacy/internal/websockets/reconnecting_websocket_factory.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/legacy/internal/websockets/websocket_message_processor.py` & `neptune_client-1.3.1/src/neptune/legacy/internal/websockets/websocket_message_processor.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/legacy/model.py` & `neptune_client-1.3.1/src/neptune/legacy/model.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/legacy/notebook.py` & `neptune_client-1.3.1/src/neptune/legacy/notebook.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/legacy/oauth.py` & `neptune_client-1.3.1/src/neptune/legacy/oauth.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/legacy/patterns.py` & `neptune_client-1.3.1/src/neptune/legacy/patterns.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/legacy/projects.py` & `neptune_client-1.3.1/src/neptune/legacy/projects.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/legacy/sessions.py` & `neptune_client-1.3.1/src/neptune/legacy/sessions.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/legacy/utils.py` & `neptune_client-1.3.1/src/neptune/legacy/utils.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/logging/__init__.py` & `neptune_client-1.3.1/src/neptune/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/logging/logger.py` & `neptune_client-1.3.1/src/neptune/logging/logger.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/management/__init__.py` & `neptune_client-1.3.1/src/neptune/management/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/management/exceptions.py` & `neptune_client-1.3.1/src/neptune/management/exceptions.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/management/internal/__init__.py` & `neptune_client-1.3.1/src/neptune/management/internal/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/management/internal/api.py` & `neptune_client-1.3.1/src/neptune/management/internal/api.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/management/internal/dto.py` & `neptune_client-1.3.1/src/neptune/management/internal/dto.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/management/internal/types.py` & `neptune_client-1.3.1/src/neptune/management/internal/types.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/management/internal/utils.py` & `neptune_client-1.3.1/src/neptune/management/internal/utils.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/metadata_containers/__init__.py` & `neptune_client-1.3.1/src/neptune/metadata_containers/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/metadata_containers/abstract.py` & `neptune_client-1.3.1/src/neptune/metadata_containers/abstract.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/metadata_containers/metadata_container.py` & `neptune_client-1.3.1/src/neptune/metadata_containers/metadata_container.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/metadata_containers/metadata_containers_table.py` & `neptune_client-1.3.1/src/neptune/metadata_containers/metadata_containers_table.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/metadata_containers/model.py` & `neptune_client-1.3.1/src/neptune/metadata_containers/model.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/metadata_containers/model_version.py` & `neptune_client-1.3.1/src/neptune/metadata_containers/model_version.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/metadata_containers/project.py` & `neptune_client-1.3.1/src/neptune/metadata_containers/project.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/metadata_containers/run.py` & `neptune_client-1.3.1/src/neptune/metadata_containers/run.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/new/__init__.py` & `neptune_client-1.3.1/src/neptune/new/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/new/_compatibility.py` & `neptune_client-1.3.1/src/neptune/new/_compatibility.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/new/constants.py` & `neptune_client-1.3.1/src/neptune/new/constants.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/new/envs.py` & `neptune_client-1.3.1/src/neptune/new/envs.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/new/exceptions.py` & `neptune_client-1.3.1/src/neptune/new/exceptions.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/new/handler.py` & `neptune_client-1.3.1/src/neptune/new/handler.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/new/project.py` & `neptune_client-1.3.1/src/neptune/new/project.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/new/run.py` & `neptune_client-1.3.1/src/neptune/new/run.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/new/runs_table.py` & `neptune_client-1.3.1/src/neptune/new/runs_table.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/new/utils.py` & `neptune_client-1.3.1/src/neptune/new/utils.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/new/version.py` & `neptune_client-1.3.1/src/neptune/new/version.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/types/__init__.py` & `neptune_client-1.3.1/src/neptune/types/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/types/atoms/__init__.py` & `neptune_client-1.3.1/src/neptune/types/atoms/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/types/atoms/artifact.py` & `neptune_client-1.3.1/src/neptune/types/atoms/artifact.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/types/atoms/atom.py` & `neptune_client-1.3.1/src/neptune/types/atoms/atom.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/types/atoms/boolean.py` & `neptune_client-1.3.1/src/neptune/types/atoms/boolean.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/types/atoms/datetime.py` & `neptune_client-1.3.1/src/neptune/types/atoms/datetime.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/types/atoms/file.py` & `neptune_client-1.3.1/src/neptune/types/atoms/file.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/types/atoms/float.py` & `neptune_client-1.3.1/src/neptune/types/atoms/float.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/types/atoms/git_ref.py` & `neptune_client-1.3.1/src/neptune/types/atoms/git_ref.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/types/atoms/integer.py` & `neptune_client-1.3.1/src/neptune/types/atoms/integer.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/types/atoms/string.py` & `neptune_client-1.3.1/src/neptune/types/atoms/string.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/types/file_set.py` & `neptune_client-1.3.1/src/neptune/types/file_set.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/types/mode.py` & `neptune_client-1.3.1/src/neptune/types/mode.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/types/model_version_stage.py` & `neptune_client-1.3.1/src/neptune/types/model_version_stage.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/types/namespace.py` & `neptune_client-1.3.1/src/neptune/types/namespace.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/types/series/__init__.py` & `neptune_client-1.3.1/src/neptune/types/series/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/types/series/file_series.py` & `neptune_client-1.3.1/src/neptune/types/series/file_series.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/types/series/float_series.py` & `neptune_client-1.3.1/src/neptune/types/series/float_series.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/types/series/series.py` & `neptune_client-1.3.1/src/neptune/types/series/series.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/types/series/series_value.py` & `neptune_client-1.3.1/src/neptune/types/series/series_value.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/types/series/string_series.py` & `neptune_client-1.3.1/src/neptune/types/series/string_series.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/types/sets/__init__.py` & `neptune_client-1.3.1/src/neptune/types/sets/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/types/sets/set.py` & `neptune_client-1.3.1/src/neptune/types/sets/set.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/types/sets/string_set.py` & `neptune_client-1.3.1/src/neptune/types/sets/string_set.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/types/type_casting.py` & `neptune_client-1.3.1/src/neptune/types/type_casting.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/types/value.py` & `neptune_client-1.3.1/src/neptune/types/value.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/types/value_copy.py` & `neptune_client-1.3.1/src/neptune/types/value_copy.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/types/value_visitor.py` & `neptune_client-1.3.1/src/neptune/types/value_visitor.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/typing.py` & `neptune_client-1.3.1/src/neptune/typing.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/utils.py` & `neptune_client-1.3.1/src/neptune/utils.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/vendor/lib_programname.py` & `neptune_client-1.3.1/src/neptune/vendor/lib_programname.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/vendor/pynvml.py` & `neptune_client-1.3.1/src/neptune/vendor/pynvml.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/src/neptune/version.py` & `neptune_client-1.3.1/src/neptune/version.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.3.0/PKG-INFO` & `neptune_client-1.3.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neptune-client
-Version: 1.3.0
+Version: 1.3.1
 Summary: Neptune Client
 Home-page: https://neptune.ai/
 License: Apache-2.0
 Keywords: MLOps,ML Experiment Tracking,ML Model Registry,ML Model Store,ML Metadata Store
 Author: neptune.ai
 Author-email: contact@neptune.ai
 Requires-Python: >=3.7,<4.0
@@ -130,22 +130,22 @@
 * Automate and standardize as your modeling team grows.
 * Collaborate on models and results with your team and across the org.
 * Use hosted, deploy on-premises, or in a private cloud. Integrate with any MLOps stack.
 &nbsp;
 
 &nbsp;
 <div align="center">
-    <a href="https://youtu.be/L2CAYip0DmI">
+    <a href="https://www.youtube.com/watch?v=bQzgnqM5J6U">
       <img border="0" alt="neptune.ai explainer video" src="https://raw.githubusercontent.com/neptune-ai/neptune-client/assets/readme/github-explainer-video.png" width="600">
     </a>
 </div>
 &nbsp;
 
 &nbsp;
-<a href="https://app.neptune.ai/showcase/example-project-tensorflow-keras/experiments?split=tbl&dash=charts&viewId=eccd5adf-42b3-497e-9cc2-9fa2655429b3"><b>Play with a live neptune.ai app →</b></a>
+<a href="https://app.neptune.ai/o/showcase/org/onboarding-project/runs/table?viewId=98f66b32-2279-4b73-8210-863021c440ac&product_tour_id=444083"><b>Play with a live neptune.ai app →</b></a>
 &nbsp;
 
 &nbsp;
 ## Getting started
 
 **Step 1:** Create a **[free account](https://neptune.ai/register)**
 
@@ -181,59 +181,59 @@
 * <a href="https://docs.neptune.ai/logging/what_you_can_log/"><b>Any metadata type:</b></a> metrics, parameters, dataset and model versions, images, interactive plots, videos, hardware (GPU, CPU, memory), code state.
 
 * <a href="https://docs.neptune.ai/usage/pipelines/"><b>From anywhere in your ML pipeline:</b></a> multinode pipelines, distributed computing, log during or after execution, log offline, and sync when you are back online.
 &nbsp;
 
 &nbsp;
 <div align="center">
-      <img border="0" alt="all metadata metrics" src="https://raw.githubusercontent.com/neptune-ai/neptune-client/assets/readme/all-metadata-metrics.gif" width="600">
+      <img border="0" alt="all metadata metrics" src="https://neptune.ai/wp-content/uploads/2023/06/log_metrics.gif" width="600">
     </a>
 </div>
 &nbsp;
 
 &nbsp;
 
 **Organize experiments**
 
 Organize logs in a fully customizable nested structure. Display model metadata in user-defined dashboard templates.
 
-* <a href="https://app.neptune.ai/o/showcase/org/example-project-tensorflow-keras/experiments?split=tbl&dash=charts&viewId=4a21e7e9-abab-4f9f-8723-41f5ae4f71e8&product_tour_id=314370"><b>Nested metadata structure:</b></a> flexible API lets you customize the metadata logging structure however you want. Talk to a dictionary at the code level. See the folder structure in the app. Organize nested parameter configs or the results on k-fold validation splits the way they should be.
+* <a href="https://app.neptune.ai/o/showcase/org/onboarding-project/runs/table?viewId=98f66b32-2279-4b73-8210-863021c440ac&product_tour_id=444083"><b>Nested metadata structure:</b></a> flexible API lets you customize the metadata logging structure however you want. Talk to a dictionary at the code level. See the folder structure in the app. Organize nested parameter configs or the results on k-fold validation splits the way they should be.
 
-* <a href="https://app.neptune.ai/o/showcase/org/example-project-tensorflow-keras/experiments?split=tbl&dash=charts&viewId=4a21e7e9-abab-4f9f-8723-41f5ae4f71e8&product_tour_id=314370"><b>Custom dashboards:</b></a> combine different metadata types in one view. Define it for one run. Use anywhere. Look at GPU, memory consumption, and load times to debug training speed. See learning curves, image predictions, and confusion matrix to debug model quality.
+* <a href="https://app.neptune.ai/o/showcase/org/onboarding-project/runs/table?viewId=98f66b32-2279-4b73-8210-863021c440ac&product_tour_id=444083"><b>Custom dashboards:</b></a> combine different metadata types in one view. Define it for one run. Use anywhere. Look at GPU, memory consumption, and load times to debug training speed. See learning curves, image predictions, and confusion matrix to debug model quality.
 
-* <a href="https://app.neptune.ai/o/showcase/org/example-project-tensorflow-keras/experiments?split=tbl&dash=charts&viewId=4a21e7e9-abab-4f9f-8723-41f5ae4f71e8&product_tour_id=314370"><b>Table views:</b></a> create different views of the runs table and save them for later. You can have separate table views for debugging, comparing parameter sets, or best experiments.
+* <a href="https://app.neptune.ai/o/showcase/org/onboarding-project/runs/table?viewId=98f66b32-2279-4b73-8210-863021c440ac&product_tour_id=444083"><b>Table views:</b></a> create different views of the runs table and save them for later. You can have separate table views for debugging, comparing parameter sets, or best experiments.
 &nbsp;
 
 &nbsp;
 <div align="center">
-      <img border="0" alt="organize dashboards" src="https://raw.githubusercontent.com/neptune-ai/neptune-client/assets/readme/organize-dashboards.gif" width="600">
+      <img border="0" alt="organize dashboards" src="https://neptune.ai/wp-content/uploads/2023/06/organize_custom_dashboards.gif" width="600">
     </a>
 </div>
 &nbsp;
 
 &nbsp;
 
 **Compare results**
 
 Visualize training live in the neptune.ai web app. See how different parameters and configs affect the results. Optimize models quicker.
 
-* <a href="https://app.neptune.ai/o/showcase/org/example-project-tensorflow-keras/experiments?split=tbl&dash=charts&viewId=4a21e7e9-abab-4f9f-8723-41f5ae4f71e8&product_tour_id=314370"><b>Compare:</b></a> learning curves, parameters, images, datasets.
+* <a href="https://app.neptune.ai/o/showcase/org/onboarding-project/runs/table?viewId=98f66b32-2279-4b73-8210-863021c440ac&product_tour_id=444083"><b>Compare:</b></a> learning curves, parameters, images, datasets.
 
-* <a href="https://app.neptune.ai/o/showcase/org/example-project-tensorflow-keras/experiments?split=tbl&dash=charts&viewId=4a21e7e9-abab-4f9f-8723-41f5ae4f71e8&product_tour_id=314370"><b>Search, sort, and filter:</b></a> experiments by any field you logged. Use our query language to filter runs based on parameter values, metrics, execution times, or anything else.
+* <a href="https://app.neptune.ai/o/showcase/org/onboarding-project/runs/table?viewId=98f66b32-2279-4b73-8210-863021c440ac&product_tour_id=444083"><b>Search, sort, and filter:</b></a> experiments by any field you logged. Use our query language to filter runs based on parameter values, metrics, execution times, or anything else.
 
-* <a href="https://app.neptune.ai/o/showcase/org/example-project-tensorflow-keras/experiments?split=tbl&dash=charts&viewId=4a21e7e9-abab-4f9f-8723-41f5ae4f71e8&product_tour_id=314370"><b>Visualize and display:</b></a> runs table, interactive display, folder structure, dashboards.
+* <a href="https://app.neptune.ai/o/showcase/org/onboarding-project/runs/table?viewId=98f66b32-2279-4b73-8210-863021c440ac&product_tour_id=444083"><b>Visualize and display:</b></a> runs table, interactive display, folder structure, dashboards.
 
-* <a href="https://app.neptune.ai/o/showcase/org/example-project-tensorflow-keras/experiments?split=tbl&dash=charts&viewId=4a21e7e9-abab-4f9f-8723-41f5ae4f71e8&product_tour_id=314370"><b>Monitor live:</b></a> hardware consumption metrics, GPU, CPU, memory.
+* <a href="https://app.neptune.ai/o/showcase/org/onboarding-project/runs/table?viewId=98f66b32-2279-4b73-8210-863021c440ac&product_tour_id=444083"><b>Monitor live:</b></a> hardware consumption metrics, GPU, CPU, memory.
 
-* <a href="https://app.neptune.ai/o/showcase/org/example-project-tensorflow-keras/experiments?split=tbl&dash=charts&viewId=4a21e7e9-abab-4f9f-8723-41f5ae4f71e8&product_tour_id=314370"><b>Group by:</b></a> dataset versions, parameters.
+* <a href="https://app.neptune.ai/o/showcase/org/onboarding-project/runs/table?viewId=98f66b32-2279-4b73-8210-863021c440ac&product_tour_id=444083"><b>Group by:</b></a> dataset versions, parameters.
 &nbsp;
 
 &nbsp;
 <div align="center">
-      <img border="0" alt="compare, search, filter" src="https://raw.githubusercontent.com/neptune-ai/neptune-client/assets/readme/compare-search-filter.gif" width="600">
+      <img border="0" alt="compare, search, filter" src="https://neptune.ai/wp-content/uploads/2023/06/organize_search_sort_filter.gif" width="600">
     </a>
 </div>
 &nbsp;
 
 &nbsp;
 
 **Register models**
@@ -245,37 +245,37 @@
 * <a href="https://docs.neptune.ai/model_registry/managing_stage/"><b>Review and change stages:</b></a> look at the validation, test metrics and other model metadata. You can move models between None/Staging/Production/Archived.
 
 * <a href="https://docs.neptune.ai/model_registry/overview/"><b>Access and share models:</b></a> every model and model version is accessible via the neptune.ai web app or through the API.
 &nbsp;
 
 &nbsp;
 <div align="center">
-      <img border="0" alt="register stages" src="https://raw.githubusercontent.com/neptune-ai/neptune-client/assets/readme/register-stages.gif" width="600">
+      <img border="0" alt="register models" src="https://neptune.ai/wp-content/uploads/2023/06/register_models.gif" width="600">
     </a>
 </div>
 &nbsp;
 
 &nbsp;
 
 **Share results**
 
 Have a single place where your team can see the results and access all models and experiments.
 
 * <a href="https://docs.neptune.ai/about/collaboration/"><b>Send a link:</b></a> share every chart, dashboard, table view, or anything else you see in the neptune.ai app by copying and sending persistent URLs.
 
 * <a href="https://docs.neptune.ai/usage/querying_metadata/"><b>Query API:</b></a> access all model metadata via neptune.ai API. Whatever you logged, you can query in a similar way.
 
-* <a href="https://neptune.ai/pricing"><b>Manage users and projects:</b></a> create different projects, add users to them, and grant different permissions levels.
+* <a href="https://docs.neptune.ai/management/"><b>Manage users and projects:</b></a> create different projects, add users to them, and grant different permissions levels.
 
 * <a href="https://neptune.ai/pricing"><b>Add your entire org:</b></a> get unlimited users on every paid plan. So you can invite your entire organization, including product managers and subject matter experts at no extra cost.
 &nbsp;
 
 &nbsp;
 <div align="center">
-      <img border="0" alt="share persistent link" src="https://raw.githubusercontent.com/neptune-ai/neptune-client/assets/readme/share-persistent-link.gif" width="600">
+      <img border="0" alt="share persistent link" src="https://neptune.ai/wp-content/uploads/2023/06/share_send_link.gif" width="600">
     </a>
 </div>
 &nbsp;
 
 &nbsp;
 ## Integrate with any MLOps stack
 neptune.ai integrates with <a href="https://docs.neptune.ai/integrations/"><b>25+ frameworks:</b></a> PyTorch, PyTorch Lightning, TensorFlow/Keras, LightGBM, scikit-learn, XGBoost, Optuna, Kedro, 🤗 Transformers, fastai, Prophet, and more.
```

