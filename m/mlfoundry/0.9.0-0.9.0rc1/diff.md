# Comparing `tmp/mlfoundry-0.9.0.tar.gz` & `tmp/mlfoundry-0.9.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlfoundry-0.9.0.tar", max compression
+gzip compressed data, was "mlfoundry-0.9.0rc1.tar", max compression
```

## Comparing `mlfoundry-0.9.0.tar` & `mlfoundry-0.9.0rc1.tar`

### file list

```diff
@@ -1,114 +1,114 @@
--rw-r--r--   0        0        0     3158 2023-06-15 16:37:12.026879 mlfoundry-0.9.0/README.md
--rw-r--r--   0        0        0      991 2023-06-15 16:37:12.038879 mlfoundry-0.9.0/mlfoundry/__init__.py
--rw-r--r--   0        0        0     1211 2023-06-15 16:37:12.038879 mlfoundry-0.9.0/mlfoundry/__main__.py
--rw-r--r--   0        0        0     3713 2023-06-15 16:37:12.038879 mlfoundry-0.9.0/mlfoundry/amplitude.py
--rw-r--r--   0        0        0        0 2023-06-15 16:37:12.038879 mlfoundry-0.9.0/mlfoundry/artifact/__init__.py
--rw-r--r--   0        0        0    20613 2023-06-15 16:37:12.038879 mlfoundry-0.9.0/mlfoundry/artifact/truefoundry_artifact_repo.py
--rw-r--r--   0        0        0        0 2023-06-15 16:37:12.038879 mlfoundry-0.9.0/mlfoundry/background/__init__.py
--rw-r--r--   0        0        0      287 2023-06-15 16:37:12.038879 mlfoundry-0.9.0/mlfoundry/background/events.py
--rw-r--r--   0        0        0     3032 2023-06-15 16:37:12.038879 mlfoundry-0.9.0/mlfoundry/background/interface.py
--rw-r--r--   0        0        0     4016 2023-06-15 16:37:12.038879 mlfoundry-0.9.0/mlfoundry/background/sender.py
--rw-r--r--   0        0        0     8756 2023-06-15 16:37:12.038879 mlfoundry-0.9.0/mlfoundry/background/system_metrics.py
--rw-r--r--   0        0        0     4028 2023-06-15 16:37:12.038879 mlfoundry-0.9.0/mlfoundry/background/utils.py
--rw-r--r--   0        0        0        0 2023-06-15 16:37:12.042879 mlfoundry-0.9.0/mlfoundry/cli/__init__.py
--rw-r--r--   0        0        0      918 2023-06-15 16:37:12.042879 mlfoundry-0.9.0/mlfoundry/cli/cli_interface.py
--rw-r--r--   0        0        0      100 2023-06-15 16:37:12.042879 mlfoundry-0.9.0/mlfoundry/cli/commands/__init__.py
--rw-r--r--   0        0        0      731 2023-06-15 16:37:12.042879 mlfoundry-0.9.0/mlfoundry/cli/commands/download.py
--rw-r--r--   0        0        0      739 2023-06-15 16:37:12.042879 mlfoundry-0.9.0/mlfoundry/cli/commands/login.py
--rw-r--r--   0        0        0     2724 2023-06-15 16:37:12.042879 mlfoundry-0.9.0/mlfoundry/constants.py
--rw-r--r--   0        0        0      103 2023-06-15 16:37:12.042879 mlfoundry-0.9.0/mlfoundry/dataset/__init__.py
--rw-r--r--   0        0        0     7854 2023-06-15 16:37:12.042879 mlfoundry-0.9.0/mlfoundry/dataset/dataset.py
--rw-r--r--   0        0        0     2255 2023-06-15 16:37:12.042879 mlfoundry-0.9.0/mlfoundry/dataset/schema.py
--rw-r--r--   0        0        0    13138 2023-06-15 16:37:12.042879 mlfoundry-0.9.0/mlfoundry/dataset/serde.py
--rw-r--r--   0        0        0     2028 2023-06-15 16:37:12.042879 mlfoundry-0.9.0/mlfoundry/dataset/serde_utils.py
--rw-r--r--   0        0        0     2078 2023-06-15 16:37:12.042879 mlfoundry-0.9.0/mlfoundry/dataset/stats.py
--rw-r--r--   0        0        0     1903 2023-06-15 16:37:12.042879 mlfoundry-0.9.0/mlfoundry/dataset/types.py
--rw-r--r--   0        0        0     2588 2023-06-15 16:37:12.042879 mlfoundry-0.9.0/mlfoundry/dataset/validation.py
--rw-r--r--   0        0        0       69 2023-06-15 16:37:12.042879 mlfoundry-0.9.0/mlfoundry/dataset/whylogs_types/__init__.py
--rw-r--r--   0        0        0     4025 2023-06-15 16:37:12.042879 mlfoundry-0.9.0/mlfoundry/dataset/whylogs_types/summary.py
--rw-r--r--   0        0        0     1392 2023-06-15 16:37:12.042879 mlfoundry-0.9.0/mlfoundry/enums.py
--rw-r--r--   0        0        0      383 2023-06-15 16:37:12.042879 mlfoundry-0.9.0/mlfoundry/env_vars.py
--rw-r--r--   0        0        0      365 2023-06-15 16:37:12.042879 mlfoundry-0.9.0/mlfoundry/exceptions.py
--rw-r--r--   0        0        0     2037 2023-06-15 16:37:12.042879 mlfoundry-0.9.0/mlfoundry/frameworks/__init__.py
--rw-r--r--   0        0        0      301 2023-06-15 16:37:12.042879 mlfoundry-0.9.0/mlfoundry/frameworks/base_registry.py
--rw-r--r--   0        0        0      718 2023-06-15 16:37:12.042879 mlfoundry-0.9.0/mlfoundry/frameworks/fastai_registry.py
--rw-r--r--   0        0        0      892 2023-06-15 16:37:12.042879 mlfoundry-0.9.0/mlfoundry/frameworks/gluon_registry.py
--rw-r--r--   0        0        0      700 2023-06-15 16:37:12.042879 mlfoundry-0.9.0/mlfoundry/frameworks/h2o_registry.py
--rw-r--r--   0        0        0      712 2023-06-15 16:37:12.042879 mlfoundry-0.9.0/mlfoundry/frameworks/keras_registry.py
--rw-r--r--   0        0        0      730 2023-06-15 16:37:12.042879 mlfoundry-0.9.0/mlfoundry/frameworks/lightgbm_registry.py
--rw-r--r--   0        0        0      706 2023-06-15 16:37:12.042879 mlfoundry-0.9.0/mlfoundry/frameworks/onnx_registry.py
--rw-r--r--   0        0        0      775 2023-06-15 16:37:12.042879 mlfoundry-0.9.0/mlfoundry/frameworks/paddle_registry.py
--rw-r--r--   0        0        0      744 2023-06-15 16:37:12.042879 mlfoundry-0.9.0/mlfoundry/frameworks/pytorch_registry.py
--rw-r--r--   0        0        0      724 2023-06-15 16:37:12.042879 mlfoundry-0.9.0/mlfoundry/frameworks/sklearn_registry.py
--rw-r--r--   0        0        0      712 2023-06-15 16:37:12.042879 mlfoundry-0.9.0/mlfoundry/frameworks/spacy_registry.py
--rw-r--r--   0        0        0      748 2023-06-15 16:37:12.042879 mlfoundry-0.9.0/mlfoundry/frameworks/statsmodel_registry.py
--rw-r--r--   0        0        0     3077 2023-06-15 16:37:12.042879 mlfoundry-0.9.0/mlfoundry/frameworks/tensorflow_registry.py
--rw-r--r--   0        0        0      774 2023-06-15 16:37:12.042879 mlfoundry-0.9.0/mlfoundry/frameworks/transformers_registry.py
--rw-r--r--   0        0        0      724 2023-06-15 16:37:12.042879 mlfoundry-0.9.0/mlfoundry/frameworks/xgboost_registry.py
--rw-r--r--   0        0        0     2349 2023-06-15 16:37:12.042879 mlfoundry-0.9.0/mlfoundry/git_info.py
--rw-r--r--   0        0        0        0 2023-06-15 16:37:12.042879 mlfoundry-0.9.0/mlfoundry/integrations/__init__.py
--rw-r--r--   0        0        0    15423 2023-06-15 16:37:12.042879 mlfoundry-0.9.0/mlfoundry/integrations/lightning.py
--rw-r--r--   0        0        0    22410 2023-06-15 16:37:12.042879 mlfoundry-0.9.0/mlfoundry/integrations/transformers.py
--rw-r--r--   0        0        0     1785 2023-06-15 16:37:12.042879 mlfoundry-0.9.0/mlfoundry/internal_namespace.py
--rw-r--r--   0        0        0      571 2023-06-15 16:37:12.042879 mlfoundry-0.9.0/mlfoundry/log_types/__init__.py
--rw-r--r--   0        0        0     7978 2023-06-15 16:37:12.042879 mlfoundry-0.9.0/mlfoundry/log_types/artifacts/artifact.py
--rw-r--r--   0        0        0     1019 2023-06-15 16:37:12.042879 mlfoundry-0.9.0/mlfoundry/log_types/artifacts/constants.py
--rw-r--r--   0        0        0     3072 2023-06-15 16:37:12.042879 mlfoundry-0.9.0/mlfoundry/log_types/artifacts/general_artifact.py
--rw-r--r--   0        0        0    15275 2023-06-15 16:37:12.042879 mlfoundry-0.9.0/mlfoundry/log_types/artifacts/model.py
--rw-r--r--   0        0        0     5983 2023-06-15 16:37:12.042879 mlfoundry-0.9.0/mlfoundry/log_types/artifacts/utils.py
--rw-r--r--   0        0        0     1281 2023-06-15 16:37:12.042879 mlfoundry-0.9.0/mlfoundry/log_types/dataset_artifact.py
--rw-r--r--   0        0        0      222 2023-06-15 16:37:12.042879 mlfoundry-0.9.0/mlfoundry/log_types/dataset_schema.py
--rw-r--r--   0        0        0      318 2023-06-15 16:37:12.042879 mlfoundry-0.9.0/mlfoundry/log_types/dataset_stats.py
--rw-r--r--   0        0        0       50 2023-06-15 16:37:12.042879 mlfoundry-0.9.0/mlfoundry/log_types/image/__init__.py
--rw-r--r--   0        0        0      255 2023-06-15 16:37:12.042879 mlfoundry-0.9.0/mlfoundry/log_types/image/constants.py
--rw-r--r--   0        0        0    11446 2023-06-15 16:37:12.042879 mlfoundry-0.9.0/mlfoundry/log_types/image/image.py
--rw-r--r--   0        0        0     2767 2023-06-15 16:37:12.042879 mlfoundry-0.9.0/mlfoundry/log_types/image/image_normalizer.py
--rw-r--r--   0        0        0     1566 2023-06-15 16:37:12.042879 mlfoundry-0.9.0/mlfoundry/log_types/image/types.py
--rw-r--r--   0        0        0      271 2023-06-15 16:37:12.042879 mlfoundry-0.9.0/mlfoundry/log_types/model_artifact.py
--rw-r--r--   0        0        0     7125 2023-06-15 16:37:12.042879 mlfoundry-0.9.0/mlfoundry/log_types/plot.py
--rw-r--r--   0        0        0     2486 2023-06-15 16:37:12.042879 mlfoundry-0.9.0/mlfoundry/log_types/pydantic_base.py
--rw-r--r--   0        0        0     1332 2023-06-15 16:37:12.042879 mlfoundry-0.9.0/mlfoundry/log_types/utils.py
--rw-r--r--   0        0        0      453 2023-06-15 16:37:12.042879 mlfoundry-0.9.0/mlfoundry/logger.py
--rw-r--r--   0        0        0     9286 2023-06-15 16:37:12.042879 mlfoundry-0.9.0/mlfoundry/login.py
--rw-r--r--   0        0        0        0 2023-06-15 16:37:12.042879 mlfoundry-0.9.0/mlfoundry/metrics/__init__.py
--rw-r--r--   0        0        0     1065 2023-06-15 16:37:12.042879 mlfoundry-0.9.0/mlfoundry/metrics/v1/__init__.py
--rw-r--r--   0        0        0     2080 2023-06-15 16:37:12.042879 mlfoundry-0.9.0/mlfoundry/metrics/v1/base_metrics.py
--rw-r--r--   0        0        0     6852 2023-06-15 16:37:12.042879 mlfoundry-0.9.0/mlfoundry/metrics/v1/binary_classification_metrics.py
--rw-r--r--   0        0        0     6736 2023-06-15 16:37:12.042879 mlfoundry-0.9.0/mlfoundry/metrics/v1/multiclass_classification_metrics.py
--rw-r--r--   0        0        0     4419 2023-06-15 16:37:12.042879 mlfoundry-0.9.0/mlfoundry/metrics/v1/regression_metrics.py
--rw-r--r--   0        0        0     3976 2023-06-15 16:37:12.042879 mlfoundry-0.9.0/mlfoundry/metrics/v1/timeseries_metrics.py
--rw-r--r--   0        0        0     1026 2023-06-15 16:37:12.042879 mlfoundry-0.9.0/mlfoundry/metrics/v2/__init__.py
--rw-r--r--   0        0        0     1898 2023-06-15 16:37:12.042879 mlfoundry-0.9.0/mlfoundry/metrics/v2/base_metrics.py
--rw-r--r--   0        0        0      566 2023-06-15 16:37:12.042879 mlfoundry-0.9.0/mlfoundry/metrics/v2/custom_metric_types.py
--rw-r--r--   0        0        0     6192 2023-06-15 16:37:12.042879 mlfoundry-0.9.0/mlfoundry/metrics/v2/multiclass_classification_metrics.py
--rw-r--r--   0        0        0     2718 2023-06-15 16:37:12.042879 mlfoundry-0.9.0/mlfoundry/metrics/v2/regression_metrics.py
--rw-r--r--   0        0        0     2251 2023-06-15 16:37:12.042879 mlfoundry-0.9.0/mlfoundry/metrics/v2/timeseries_metrics.py
--rw-r--r--   0        0        0      295 2023-06-15 16:37:12.042879 mlfoundry-0.9.0/mlfoundry/metrics/v2/utils.py
--rw-r--r--   0        0        0    44335 2023-06-15 16:37:12.042879 mlfoundry-0.9.0/mlfoundry/mlfoundry_api.py
--rw-r--r--   0        0        0    46400 2023-06-15 16:37:12.042879 mlfoundry-0.9.0/mlfoundry/mlfoundry_run.py
--rw-r--r--   0        0        0        0 2023-06-15 16:37:12.042879 mlfoundry-0.9.0/mlfoundry/monitoring/__init__.py
--rw-r--r--   0        0        0     1994 2023-06-15 16:37:12.042879 mlfoundry-0.9.0/mlfoundry/monitoring/entities.py
--rw-r--r--   0        0        0       63 2023-06-15 16:37:12.042879 mlfoundry-0.9.0/mlfoundry/monitoring/store/__init__.py
--rw-r--r--   0        0        0     6630 2023-06-15 16:37:12.042879 mlfoundry-0.9.0/mlfoundry/monitoring/store/client.py
--rw-r--r--   0        0        0      169 2023-06-15 16:37:12.042879 mlfoundry-0.9.0/mlfoundry/monitoring/store/constants.py
--rw-r--r--   0        0        0      336 2023-06-15 16:37:12.042879 mlfoundry-0.9.0/mlfoundry/monitoring/store/repositories/__init__.py
--rw-r--r--   0        0        0     1351 2023-06-15 16:37:12.042879 mlfoundry-0.9.0/mlfoundry/monitoring/store/repositories/dto.py
--rw-r--r--   0        0        0     6529 2023-06-15 16:37:12.042879 mlfoundry-0.9.0/mlfoundry/monitoring/store/repositories/rest_monitoring_store.py
--rw-r--r--   0        0        0     2178 2023-06-15 16:37:12.042879 mlfoundry-0.9.0/mlfoundry/monitoring/store/worker.py
--rw-r--r--   0        0        0     4304 2023-06-15 16:37:12.042879 mlfoundry-0.9.0/mlfoundry/run_utils.py
--rw-r--r--   0        0        0      492 2023-06-15 16:37:12.042879 mlfoundry-0.9.0/mlfoundry/schema.py
--rw-r--r--   0        0        0    10048 2023-06-15 16:37:12.042879 mlfoundry-0.9.0/mlfoundry/session.py
--rw-r--r--   0        0        0        0 2023-06-15 16:37:12.042879 mlfoundry-0.9.0/mlfoundry/tracking/__init__.py
--rw-r--r--   0        0        0     2766 2023-06-15 16:37:12.046879 mlfoundry-0.9.0/mlfoundry/tracking/auth_service.py
--rw-r--r--   0        0        0     2629 2023-06-15 16:37:12.046879 mlfoundry-0.9.0/mlfoundry/tracking/entities.py
--rw-r--r--   0        0        0     1175 2023-06-15 16:37:12.046879 mlfoundry-0.9.0/mlfoundry/tracking/servicefoundry_service.py
--rw-r--r--   0        0        0     4308 2023-06-15 16:37:12.046879 mlfoundry-0.9.0/mlfoundry/tracking/truefoundry_rest_store.py
--rw-r--r--   0        0        0        0 2023-06-15 16:37:12.046879 mlfoundry-0.9.0/mlfoundry/vendor/__init__.py
--rw-r--r--   0        0        0        0 2023-06-15 16:37:12.046879 mlfoundry-0.9.0/mlfoundry/vendor/pynvml/__init__.py
--rw-r--r--   0        0        0    56147 2023-06-15 16:37:12.046879 mlfoundry-0.9.0/mlfoundry/vendor/pynvml/pynvml.py
--rw-r--r--   0        0        0      253 2023-06-15 16:37:12.046879 mlfoundry-0.9.0/mlfoundry/version.py
--rw-r--r--   0        0        0        0 2023-06-15 16:37:12.046879 mlfoundry-0.9.0/mlfoundry/webapp/__init__.py
--rw-r--r--   0        0        0       38 2023-06-15 16:37:12.046879 mlfoundry-0.9.0/mlfoundry/webapp/inputs.py
--rw-r--r--   0        0        0       39 2023-06-15 16:37:12.046879 mlfoundry-0.9.0/mlfoundry/webapp/outputs.py
--rw-r--r--   0        0        0     3548 2023-06-15 16:37:25.210944 mlfoundry-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     4925 1970-01-01 00:00:00.000000 mlfoundry-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     3158 2023-06-09 11:01:51.323648 mlfoundry-0.9.0rc1/README.md
+-rw-r--r--   0        0        0      991 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/__init__.py
+-rw-r--r--   0        0        0     1211 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/__main__.py
+-rw-r--r--   0        0        0     3713 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/amplitude.py
+-rw-r--r--   0        0        0        0 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/artifact/__init__.py
+-rw-r--r--   0        0        0    20613 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/artifact/truefoundry_artifact_repo.py
+-rw-r--r--   0        0        0        0 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/background/__init__.py
+-rw-r--r--   0        0        0      287 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/background/events.py
+-rw-r--r--   0        0        0     3032 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/background/interface.py
+-rw-r--r--   0        0        0     4016 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/background/sender.py
+-rw-r--r--   0        0        0     8756 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/background/system_metrics.py
+-rw-r--r--   0        0        0     4028 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/background/utils.py
+-rw-r--r--   0        0        0        0 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/cli/__init__.py
+-rw-r--r--   0        0        0      918 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/cli/cli_interface.py
+-rw-r--r--   0        0        0      100 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/cli/commands/__init__.py
+-rw-r--r--   0        0        0      731 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/cli/commands/download.py
+-rw-r--r--   0        0        0      739 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/cli/commands/login.py
+-rw-r--r--   0        0        0     2724 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/constants.py
+-rw-r--r--   0        0        0      103 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/dataset/__init__.py
+-rw-r--r--   0        0        0     7854 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/dataset/dataset.py
+-rw-r--r--   0        0        0     2255 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/dataset/schema.py
+-rw-r--r--   0        0        0    13138 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/dataset/serde.py
+-rw-r--r--   0        0        0     2028 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/dataset/serde_utils.py
+-rw-r--r--   0        0        0     2078 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/dataset/stats.py
+-rw-r--r--   0        0        0     1903 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/dataset/types.py
+-rw-r--r--   0        0        0     2588 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/dataset/validation.py
+-rw-r--r--   0        0        0       69 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/dataset/whylogs_types/__init__.py
+-rw-r--r--   0        0        0     4025 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/dataset/whylogs_types/summary.py
+-rw-r--r--   0        0        0     1392 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/enums.py
+-rw-r--r--   0        0        0      383 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/env_vars.py
+-rw-r--r--   0        0        0      365 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/exceptions.py
+-rw-r--r--   0        0        0     2037 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/frameworks/__init__.py
+-rw-r--r--   0        0        0      301 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/frameworks/base_registry.py
+-rw-r--r--   0        0        0      718 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/frameworks/fastai_registry.py
+-rw-r--r--   0        0        0      892 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/frameworks/gluon_registry.py
+-rw-r--r--   0        0        0      700 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/frameworks/h2o_registry.py
+-rw-r--r--   0        0        0      712 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/frameworks/keras_registry.py
+-rw-r--r--   0        0        0      730 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/frameworks/lightgbm_registry.py
+-rw-r--r--   0        0        0      706 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/frameworks/onnx_registry.py
+-rw-r--r--   0        0        0      775 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/frameworks/paddle_registry.py
+-rw-r--r--   0        0        0      744 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/frameworks/pytorch_registry.py
+-rw-r--r--   0        0        0      724 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/frameworks/sklearn_registry.py
+-rw-r--r--   0        0        0      712 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/frameworks/spacy_registry.py
+-rw-r--r--   0        0        0      748 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/frameworks/statsmodel_registry.py
+-rw-r--r--   0        0        0     3077 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/frameworks/tensorflow_registry.py
+-rw-r--r--   0        0        0      774 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/frameworks/transformers_registry.py
+-rw-r--r--   0        0        0      724 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/frameworks/xgboost_registry.py
+-rw-r--r--   0        0        0     2349 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/git_info.py
+-rw-r--r--   0        0        0        0 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/integrations/__init__.py
+-rw-r--r--   0        0        0    15423 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/integrations/lightning.py
+-rw-r--r--   0        0        0    22410 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/integrations/transformers.py
+-rw-r--r--   0        0        0     1785 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/internal_namespace.py
+-rw-r--r--   0        0        0      571 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/log_types/__init__.py
+-rw-r--r--   0        0        0     7978 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/log_types/artifacts/artifact.py
+-rw-r--r--   0        0        0     1019 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/log_types/artifacts/constants.py
+-rw-r--r--   0        0        0     3072 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/log_types/artifacts/general_artifact.py
+-rw-r--r--   0        0        0    15275 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/log_types/artifacts/model.py
+-rw-r--r--   0        0        0     5983 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/log_types/artifacts/utils.py
+-rw-r--r--   0        0        0     1281 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/log_types/dataset_artifact.py
+-rw-r--r--   0        0        0      222 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/log_types/dataset_schema.py
+-rw-r--r--   0        0        0      318 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/log_types/dataset_stats.py
+-rw-r--r--   0        0        0       50 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/log_types/image/__init__.py
+-rw-r--r--   0        0        0      255 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/log_types/image/constants.py
+-rw-r--r--   0        0        0    11446 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/log_types/image/image.py
+-rw-r--r--   0        0        0     2767 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/log_types/image/image_normalizer.py
+-rw-r--r--   0        0        0     1566 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/log_types/image/types.py
+-rw-r--r--   0        0        0      271 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/log_types/model_artifact.py
+-rw-r--r--   0        0        0     7125 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/log_types/plot.py
+-rw-r--r--   0        0        0     2486 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/log_types/pydantic_base.py
+-rw-r--r--   0        0        0     1332 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/log_types/utils.py
+-rw-r--r--   0        0        0      453 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/logger.py
+-rw-r--r--   0        0        0     9286 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/login.py
+-rw-r--r--   0        0        0        0 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/metrics/__init__.py
+-rw-r--r--   0        0        0     1065 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/metrics/v1/__init__.py
+-rw-r--r--   0        0        0     2080 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/metrics/v1/base_metrics.py
+-rw-r--r--   0        0        0     6852 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/metrics/v1/binary_classification_metrics.py
+-rw-r--r--   0        0        0     6736 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/metrics/v1/multiclass_classification_metrics.py
+-rw-r--r--   0        0        0     4419 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/metrics/v1/regression_metrics.py
+-rw-r--r--   0        0        0     3976 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/metrics/v1/timeseries_metrics.py
+-rw-r--r--   0        0        0     1026 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/metrics/v2/__init__.py
+-rw-r--r--   0        0        0     1898 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/metrics/v2/base_metrics.py
+-rw-r--r--   0        0        0      566 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/metrics/v2/custom_metric_types.py
+-rw-r--r--   0        0        0     6192 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/metrics/v2/multiclass_classification_metrics.py
+-rw-r--r--   0        0        0     2718 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/metrics/v2/regression_metrics.py
+-rw-r--r--   0        0        0     2251 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/metrics/v2/timeseries_metrics.py
+-rw-r--r--   0        0        0      295 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/metrics/v2/utils.py
+-rw-r--r--   0        0        0    44772 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/mlfoundry_api.py
+-rw-r--r--   0        0        0    46176 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/mlfoundry_run.py
+-rw-r--r--   0        0        0        0 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/monitoring/__init__.py
+-rw-r--r--   0        0        0     1994 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/monitoring/entities.py
+-rw-r--r--   0        0        0       63 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/monitoring/store/__init__.py
+-rw-r--r--   0        0        0     6630 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/monitoring/store/client.py
+-rw-r--r--   0        0        0      169 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/monitoring/store/constants.py
+-rw-r--r--   0        0        0      336 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/monitoring/store/repositories/__init__.py
+-rw-r--r--   0        0        0     1351 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/monitoring/store/repositories/dto.py
+-rw-r--r--   0        0        0     6529 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/monitoring/store/repositories/rest_monitoring_store.py
+-rw-r--r--   0        0        0     2178 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/monitoring/store/worker.py
+-rw-r--r--   0        0        0     4304 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/run_utils.py
+-rw-r--r--   0        0        0      492 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/schema.py
+-rw-r--r--   0        0        0    10031 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/session.py
+-rw-r--r--   0        0        0        0 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/tracking/__init__.py
+-rw-r--r--   0        0        0     2766 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/tracking/auth_service.py
+-rw-r--r--   0        0        0     2629 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/tracking/entities.py
+-rw-r--r--   0        0        0     1175 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/tracking/servicefoundry_service.py
+-rw-r--r--   0        0        0     4308 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/tracking/truefoundry_rest_store.py
+-rw-r--r--   0        0        0        0 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/vendor/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/vendor/pynvml/__init__.py
+-rw-r--r--   0        0        0    56147 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/vendor/pynvml/pynvml.py
+-rw-r--r--   0        0        0      253 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/version.py
+-rw-r--r--   0        0        0        0 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/webapp/__init__.py
+-rw-r--r--   0        0        0       38 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/webapp/inputs.py
+-rw-r--r--   0        0        0       39 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/webapp/outputs.py
+-rw-r--r--   0        0        0     3551 2023-06-09 11:02:10.840067 mlfoundry-0.9.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     4928 1970-01-01 00:00:00.000000 mlfoundry-0.9.0rc1/PKG-INFO
```

### Comparing `mlfoundry-0.9.0/README.md` & `mlfoundry-0.9.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0/mlfoundry/__init__.py` & `mlfoundry-0.9.0rc1/mlfoundry/__init__.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0/mlfoundry/__main__.py` & `mlfoundry-0.9.0rc1/mlfoundry/__main__.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0/mlfoundry/amplitude.py` & `mlfoundry-0.9.0rc1/mlfoundry/amplitude.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0/mlfoundry/artifact/truefoundry_artifact_repo.py` & `mlfoundry-0.9.0rc1/mlfoundry/artifact/truefoundry_artifact_repo.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0/mlfoundry/background/interface.py` & `mlfoundry-0.9.0rc1/mlfoundry/background/interface.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0/mlfoundry/background/sender.py` & `mlfoundry-0.9.0rc1/mlfoundry/background/sender.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0/mlfoundry/background/system_metrics.py` & `mlfoundry-0.9.0rc1/mlfoundry/background/system_metrics.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0/mlfoundry/background/utils.py` & `mlfoundry-0.9.0rc1/mlfoundry/background/utils.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0/mlfoundry/cli/cli_interface.py` & `mlfoundry-0.9.0rc1/mlfoundry/cli/cli_interface.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0/mlfoundry/cli/commands/download.py` & `mlfoundry-0.9.0rc1/mlfoundry/cli/commands/download.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0/mlfoundry/cli/commands/login.py` & `mlfoundry-0.9.0rc1/mlfoundry/cli/commands/login.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0/mlfoundry/constants.py` & `mlfoundry-0.9.0rc1/mlfoundry/constants.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0/mlfoundry/dataset/dataset.py` & `mlfoundry-0.9.0rc1/mlfoundry/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0/mlfoundry/dataset/schema.py` & `mlfoundry-0.9.0rc1/mlfoundry/dataset/schema.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0/mlfoundry/dataset/serde.py` & `mlfoundry-0.9.0rc1/mlfoundry/dataset/serde.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0/mlfoundry/dataset/serde_utils.py` & `mlfoundry-0.9.0rc1/mlfoundry/dataset/serde_utils.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0/mlfoundry/dataset/stats.py` & `mlfoundry-0.9.0rc1/mlfoundry/dataset/stats.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0/mlfoundry/dataset/types.py` & `mlfoundry-0.9.0rc1/mlfoundry/dataset/types.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0/mlfoundry/dataset/validation.py` & `mlfoundry-0.9.0rc1/mlfoundry/dataset/validation.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0/mlfoundry/dataset/whylogs_types/summary.py` & `mlfoundry-0.9.0rc1/mlfoundry/dataset/whylogs_types/summary.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0/mlfoundry/enums.py` & `mlfoundry-0.9.0rc1/mlfoundry/enums.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0/mlfoundry/frameworks/__init__.py` & `mlfoundry-0.9.0rc1/mlfoundry/frameworks/__init__.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0/mlfoundry/frameworks/fastai_registry.py` & `mlfoundry-0.9.0rc1/mlfoundry/frameworks/fastai_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0/mlfoundry/frameworks/gluon_registry.py` & `mlfoundry-0.9.0rc1/mlfoundry/frameworks/gluon_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0/mlfoundry/frameworks/h2o_registry.py` & `mlfoundry-0.9.0rc1/mlfoundry/frameworks/h2o_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0/mlfoundry/frameworks/keras_registry.py` & `mlfoundry-0.9.0rc1/mlfoundry/frameworks/keras_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0/mlfoundry/frameworks/lightgbm_registry.py` & `mlfoundry-0.9.0rc1/mlfoundry/frameworks/lightgbm_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0/mlfoundry/frameworks/onnx_registry.py` & `mlfoundry-0.9.0rc1/mlfoundry/frameworks/onnx_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0/mlfoundry/frameworks/paddle_registry.py` & `mlfoundry-0.9.0rc1/mlfoundry/frameworks/paddle_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0/mlfoundry/frameworks/pytorch_registry.py` & `mlfoundry-0.9.0rc1/mlfoundry/frameworks/pytorch_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0/mlfoundry/frameworks/sklearn_registry.py` & `mlfoundry-0.9.0rc1/mlfoundry/frameworks/sklearn_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0/mlfoundry/frameworks/spacy_registry.py` & `mlfoundry-0.9.0rc1/mlfoundry/frameworks/spacy_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0/mlfoundry/frameworks/statsmodel_registry.py` & `mlfoundry-0.9.0rc1/mlfoundry/frameworks/statsmodel_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0/mlfoundry/frameworks/tensorflow_registry.py` & `mlfoundry-0.9.0rc1/mlfoundry/frameworks/tensorflow_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0/mlfoundry/frameworks/transformers_registry.py` & `mlfoundry-0.9.0rc1/mlfoundry/frameworks/transformers_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0/mlfoundry/frameworks/xgboost_registry.py` & `mlfoundry-0.9.0rc1/mlfoundry/frameworks/xgboost_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0/mlfoundry/git_info.py` & `mlfoundry-0.9.0rc1/mlfoundry/git_info.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0/mlfoundry/integrations/lightning.py` & `mlfoundry-0.9.0rc1/mlfoundry/integrations/lightning.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0/mlfoundry/integrations/transformers.py` & `mlfoundry-0.9.0rc1/mlfoundry/integrations/transformers.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0/mlfoundry/internal_namespace.py` & `mlfoundry-0.9.0rc1/mlfoundry/internal_namespace.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0/mlfoundry/log_types/__init__.py` & `mlfoundry-0.9.0rc1/mlfoundry/log_types/__init__.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0/mlfoundry/log_types/artifacts/artifact.py` & `mlfoundry-0.9.0rc1/mlfoundry/log_types/artifacts/artifact.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0/mlfoundry/log_types/artifacts/constants.py` & `mlfoundry-0.9.0rc1/mlfoundry/log_types/artifacts/constants.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0/mlfoundry/log_types/artifacts/general_artifact.py` & `mlfoundry-0.9.0rc1/mlfoundry/log_types/artifacts/general_artifact.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0/mlfoundry/log_types/artifacts/model.py` & `mlfoundry-0.9.0rc1/mlfoundry/log_types/artifacts/model.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0/mlfoundry/log_types/artifacts/utils.py` & `mlfoundry-0.9.0rc1/mlfoundry/log_types/artifacts/utils.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0/mlfoundry/log_types/dataset_artifact.py` & `mlfoundry-0.9.0rc1/mlfoundry/log_types/dataset_artifact.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0/mlfoundry/log_types/image/image.py` & `mlfoundry-0.9.0rc1/mlfoundry/log_types/image/image.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0/mlfoundry/log_types/image/image_normalizer.py` & `mlfoundry-0.9.0rc1/mlfoundry/log_types/image/image_normalizer.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0/mlfoundry/log_types/image/types.py` & `mlfoundry-0.9.0rc1/mlfoundry/log_types/image/types.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0/mlfoundry/log_types/plot.py` & `mlfoundry-0.9.0rc1/mlfoundry/log_types/plot.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0/mlfoundry/log_types/pydantic_base.py` & `mlfoundry-0.9.0rc1/mlfoundry/log_types/pydantic_base.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0/mlfoundry/log_types/utils.py` & `mlfoundry-0.9.0rc1/mlfoundry/log_types/utils.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0/mlfoundry/login.py` & `mlfoundry-0.9.0rc1/mlfoundry/login.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0/mlfoundry/metrics/v1/__init__.py` & `mlfoundry-0.9.0rc1/mlfoundry/metrics/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0/mlfoundry/metrics/v1/base_metrics.py` & `mlfoundry-0.9.0rc1/mlfoundry/metrics/v1/base_metrics.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0/mlfoundry/metrics/v1/binary_classification_metrics.py` & `mlfoundry-0.9.0rc1/mlfoundry/metrics/v1/binary_classification_metrics.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0/mlfoundry/metrics/v1/multiclass_classification_metrics.py` & `mlfoundry-0.9.0rc1/mlfoundry/metrics/v1/multiclass_classification_metrics.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0/mlfoundry/metrics/v1/regression_metrics.py` & `mlfoundry-0.9.0rc1/mlfoundry/metrics/v1/regression_metrics.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0/mlfoundry/metrics/v1/timeseries_metrics.py` & `mlfoundry-0.9.0rc1/mlfoundry/metrics/v1/timeseries_metrics.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0/mlfoundry/metrics/v2/__init__.py` & `mlfoundry-0.9.0rc1/mlfoundry/metrics/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0/mlfoundry/metrics/v2/base_metrics.py` & `mlfoundry-0.9.0rc1/mlfoundry/metrics/v2/base_metrics.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0/mlfoundry/metrics/v2/custom_metric_types.py` & `mlfoundry-0.9.0rc1/mlfoundry/metrics/v2/custom_metric_types.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0/mlfoundry/metrics/v2/multiclass_classification_metrics.py` & `mlfoundry-0.9.0rc1/mlfoundry/metrics/v2/multiclass_classification_metrics.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0/mlfoundry/metrics/v2/regression_metrics.py` & `mlfoundry-0.9.0rc1/mlfoundry/metrics/v2/regression_metrics.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0/mlfoundry/metrics/v2/timeseries_metrics.py` & `mlfoundry-0.9.0rc1/mlfoundry/metrics/v2/timeseries_metrics.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0/mlfoundry/mlfoundry_api.py` & `mlfoundry-0.9.0rc1/mlfoundry/mlfoundry_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,14 +76,20 @@
     ### Get client
     ```python
     import mlfoundry
 
     client = mlfoundry.get_client()
     ```
     """
+    # TODO (chiragjn): Will potentially need to make MlFoundry (and possibly MlFoundryRun) a Singleton instance.
+    #                  Since this sets the tracking URI in global namespace, if someone were to call
+    #                  get_client again with different tracking uri, the ongoing run's data will start getting
+    #                  pushed to another datastore. Or we should not allow passing in tracking URI and just have
+    #                  fixed online and offline clients
+
     user_id = amplitude.NO_USER
 
     session = None
 
     # NOTE: hack to run tests
     if os.getenv(TRACKING_HOST_GLOBAL, "").startswith("file:"):
         tracking_uri = os.getenv(TRACKING_HOST_GLOBAL)
@@ -312,17 +318,15 @@
         else:
             tags = {}
 
         tags.update(_get_internal_env_vars_values())
         run = self.mlflow_client.create_run(ml_repo_id, name=run_name, tags=tags)
         mlf_run_id = run.info.run_id
 
-        mlf_run = MlFoundryRun(
-            experiment_id=ml_repo_id, run_id=mlf_run_id, auto_end=True, **kwargs
-        )
+        mlf_run = MlFoundryRun(ml_repo_id, mlf_run_id, **kwargs)
         # TODO(Rizwan): Revisit this once run lifecycle is formalised
         mlf_run._add_git_info()
         mlf_run._add_python_mlf_version()
         logger.info(f"Run {run.info.fqn!r} has started.")
         return mlf_run
 
     def get_run(self, run_id: str) -> MlFoundryRun:
```

### Comparing `mlfoundry-0.9.0/mlfoundry/mlfoundry_run.py` & `mlfoundry-0.9.0rc1/mlfoundry/mlfoundry_run.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,41 +53,38 @@
 
     VALID_PARAM_AND_METRIC_NAMES = re.compile(r"^[A-Za-z0-9_\-\. /]+$")
 
     def __init__(
         self,
         experiment_id: str,
         run_id: str,
-        auto_end: bool = False,
         **kwargs,
     ):
         """__init__.
 
         Args:
             experiment_id (str): experiment_id
             run_id (str): run_id
-            auto_end (bool): If to end the run at garbage collection or process end (atexit)
         """
+
         self._experiment_id = str(experiment_id)
-        self._run_id = run_id
-        self._auto_end = auto_end
         # TODO (chiragjn): mlflow_client be a protected/private member
         self.mlflow_client = MlflowClient()
         self._project_name = self.mlflow_client.get_experiment(self._experiment_id).name
+        self._run_id = run_id
         self._run_info: Optional[RunInfo] = None
 
         from mlfoundry.dataset import TabularDatasetDriver
 
         self._dataset_module: TabularDatasetDriver = TabularDatasetDriver(
             mlflow_client=self.mlflow_client, run_id=run_id
         )
 
         self._terminate_called = False
-        if self._auto_end:
-            ACTIVE_RUNS.add_run(self)
+        ACTIVE_RUNS.add_run(self)
         print(f"Link to the dashboard for the run: {self.dashboard_link}")
 
     def _get_run_info(self) -> RunInfo:
         if self._run_info is not None:
             return self._run_info
 
         self._run_info = self.mlflow_client.get_run(self.run_id).info
@@ -109,18 +106,14 @@
     def status(self) -> str:
         return self.mlflow_client.get_run(self.run_id).info.status
 
     @property
     def ml_repo(self) -> str:
         return self._project_name
 
-    @property
-    def auto_end(self) -> bool:
-        return self._auto_end
-
     def __repr__(self) -> str:
         return f"<{type(self).__name__} at 0x{id(self):x}: run={self.fqn!r}>"
 
     def __enter__(self):
         return self
 
     def _terminate_run_if_running(self, termination_status: RunStatus):
@@ -151,16 +144,16 @@
         print(f"Finished run: {self.fqn!r}, Dashboard: {self.dashboard_link}")
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         status = RunStatus.FINISHED if exc_type is None else RunStatus.FAILED
         self._terminate_run_if_running(status)
 
     def __del__(self):
-        if self.auto_end:
-            self._terminate_run_if_running(RunStatus.FINISHED)
+        # TODO (chiragjn): Should this be marked as FINISHED or KILLED?
+        self._terminate_run_if_running(RunStatus.FINISHED)
 
     @property
     def dashboard_link(self) -> str:
         """Get Mlfoundry dashboard link for a `run`"""
 
         base_url = "{uri.scheme}://{uri.netloc}/".format(
             uri=urlsplit(mlflow.get_tracking_uri())
```

### Comparing `mlfoundry-0.9.0/mlfoundry/monitoring/entities.py` & `mlfoundry-0.9.0rc1/mlfoundry/monitoring/entities.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0/mlfoundry/monitoring/store/client.py` & `mlfoundry-0.9.0rc1/mlfoundry/monitoring/store/client.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0/mlfoundry/monitoring/store/repositories/dto.py` & `mlfoundry-0.9.0rc1/mlfoundry/monitoring/store/repositories/dto.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0/mlfoundry/monitoring/store/repositories/rest_monitoring_store.py` & `mlfoundry-0.9.0rc1/mlfoundry/monitoring/store/repositories/rest_monitoring_store.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0/mlfoundry/monitoring/store/worker.py` & `mlfoundry-0.9.0rc1/mlfoundry/monitoring/store/worker.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0/mlfoundry/run_utils.py` & `mlfoundry-0.9.0rc1/mlfoundry/run_utils.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0/mlfoundry/session.py` & `mlfoundry-0.9.0rc1/mlfoundry/session.py`

 * *Files 1% similar despite different names*

```diff
@@ -162,15 +162,15 @@
             if run.run_id in self._active_runs:
                 del self._active_runs[run.run_id]
 
     def close_active_runs(self):
         with SESSION_LOCK:
             for run_ref in list(self._active_runs.values()):
                 run = run_ref()
-                if run and run.auto_end:
+                if run:
                     run.end()
             self._active_runs.clear()
 
 
 ACTIVE_RUNS = ActiveRuns()
 atexit.register(ACTIVE_RUNS.close_active_runs)
```

### Comparing `mlfoundry-0.9.0/mlfoundry/tracking/auth_service.py` & `mlfoundry-0.9.0rc1/mlfoundry/tracking/auth_service.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0/mlfoundry/tracking/entities.py` & `mlfoundry-0.9.0rc1/mlfoundry/tracking/entities.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0/mlfoundry/tracking/servicefoundry_service.py` & `mlfoundry-0.9.0rc1/mlfoundry/tracking/servicefoundry_service.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0/mlfoundry/tracking/truefoundry_rest_store.py` & `mlfoundry-0.9.0rc1/mlfoundry/tracking/truefoundry_rest_store.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0/mlfoundry/vendor/pynvml/pynvml.py` & `mlfoundry-0.9.0rc1/mlfoundry/vendor/pynvml/pynvml.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.9.0/pyproject.toml` & `mlfoundry-0.9.0rc1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mlfoundry"
-version = "0.9.0" # do not change, auto-generated by poetry-dynamic-versioning
+version = "0.9.0rc1" # do not change, auto-generated by poetry-dynamic-versioning
 description = "Truefoundry's Experiment Tracking, Model Registry and Model Monitoring Library"
 authors = ["Abhishek Choudhary <abhichoudhary06@gmail.com>"]
 homepage = "https://github.com/truefoundry/mlfoundry"
 repository = "https://github.com/truefoundry/mlfoundry"
 readme = "README.md"
 packages = [
     { include = "mlfoundry" },
```

### Comparing `mlfoundry-0.9.0/PKG-INFO` & `mlfoundry-0.9.0rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlfoundry
-Version: 0.9.0
+Version: 0.9.0rc1
 Summary: Truefoundry's Experiment Tracking, Model Registry and Model Monitoring Library
 Home-page: https://github.com/truefoundry/mlfoundry
 Author: Abhishek Choudhary
 Author-email: abhichoudhary06@gmail.com
 Requires-Python: >=3.7,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

