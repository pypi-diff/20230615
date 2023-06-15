# Comparing `tmp/dagster-1.3.9.tar.gz` & `tmp/dagster-1.3.9rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-1.3.9.tar", last modified: Thu Jun  8 18:43:44 2023, max compression
+gzip compressed data, was "dagster-1.3.9rc0.tar", last modified: Thu Jun  8 18:21:09 2023, max compression
```

## Comparing `dagster-1.3.9.tar` & `dagster-1.3.9rc0.tar`

### file list

```diff
@@ -1,634 +1,634 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:43:44.575961 dagster-1.3.9/
--rw-r--r--   0 root         (0) root         (0)      549 2023-06-08 18:43:17.000000 dagster-1.3.9/COPYING
--rw-r--r--   0 root         (0) root         (0)    11344 2023-06-08 18:43:17.000000 dagster-1.3.9/LICENSE
--rw-r--r--   0 root         (0) root         (0)      485 2023-06-08 18:43:17.000000 dagster-1.3.9/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     8790 2023-06-08 18:43:44.575961 dagster-1.3.9/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7167 2023-06-08 18:43:17.000000 dagster-1.3.9/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:43:44.511960 dagster-1.3.9/dagster/
--rw-r--r--   0 root         (0) root         (0)    26213 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/__init__.py
--rw-r--r--   0 root         (0) root         (0)       31 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/__main__.py
--rw-r--r--   0 root         (0) root         (0)     5456 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_annotations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:43:44.511960 dagster-1.3.9/dagster/_api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)      731 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_api/get_server_id.py
--rw-r--r--   0 root         (0) root         (0)     2147 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_api/list_repositories.py
--rw-r--r--   0 root         (0) root         (0)      531 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_api/notebook_data.py
--rw-r--r--   0 root         (0) root         (0)     2882 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_api/snapshot_execution_plan.py
--rw-r--r--   0 root         (0) root         (0)     1664 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_api/snapshot_job.py
--rw-r--r--   0 root         (0) root         (0)     5479 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_api/snapshot_partition.py
--rw-r--r--   0 root         (0) root         (0)     1668 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_api/snapshot_repository.py
--rw-r--r--   0 root         (0) root         (0)     2727 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_api/snapshot_schedule.py
--rw-r--r--   0 root         (0) root         (0)     2901 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_api/snapshot_sensor.py
--rw-r--r--   0 root         (0) root         (0)      478 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_builtins.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:43:44.511960 dagster-1.3.9/dagster/_check/
--rw-r--r--   0 root         (0) root         (0)     1352 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_check/README.md
--rw-r--r--   0 root         (0) root         (0)    51637 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_check/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:43:44.515960 dagster-1.3.9/dagster/_cli/
--rw-r--r--   0 root         (0) root         (0)     1182 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)    26292 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_cli/api.py
--rw-r--r--   0 root         (0) root         (0)     8263 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_cli/asset.py
--rw-r--r--   0 root         (0) root         (0)     7730 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_cli/code_server.py
--rw-r--r--   0 root         (0) root         (0)     2300 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_cli/config_scaffolder.py
--rw-r--r--   0 root         (0) root         (0)     3540 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_cli/debug.py
--rw-r--r--   0 root         (0) root         (0)     5867 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_cli/dev.py
--rw-r--r--   0 root         (0) root         (0)     4154 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_cli/instance.py
--rw-r--r--   0 root         (0) root         (0)    29907 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_cli/job.py
--rw-r--r--   0 root         (0) root         (0)     1695 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_cli/load_handle.py
--rw-r--r--   0 root         (0) root         (0)     5852 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_cli/project.py
--rw-r--r--   0 root         (0) root         (0)     5129 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_cli/run.py
--rw-r--r--   0 root         (0) root         (0)    19958 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_cli/schedule.py
--rw-r--r--   0 root         (0) root         (0)    15707 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_cli/sensor.py
--rw-r--r--   0 root         (0) root         (0)     4259 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_cli/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:43:44.515960 dagster-1.3.9/dagster/_cli/workspace/
--rw-r--r--   0 root         (0) root         (0)      180 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_cli/workspace/__init__.py
--rw-r--r--   0 root         (0) root         (0)    28391 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_cli/workspace/cli_target.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:43:44.515960 dagster-1.3.9/dagster/_config/
--rw-r--r--   0 root         (0) root         (0)     3186 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_config/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3403 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_config/config_schema.py
--rw-r--r--   0 root         (0) root         (0)    15864 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_config/config_type.py
--rw-r--r--   0 root         (0) root         (0)    19601 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_config/errors.py
--rw-r--r--   0 root         (0) root         (0)     1783 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_config/evaluate_value_result.py
--rw-r--r--   0 root         (0) root         (0)    15269 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_config/field.py
--rw-r--r--   0 root         (0) root         (0)    16880 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_config/field_utils.py
--rw-r--r--   0 root         (0) root         (0)     9466 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_config/post_process.py
--rw-r--r--   0 root         (0) root         (0)      855 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_config/primitive_mapping.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:43:44.515960 dagster-1.3.9/dagster/_config/pythonic_config/
--rw-r--r--   0 root         (0) root         (0)    71995 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_config/pythonic_config/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1644 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_config/pythonic_config/attach_other_object_to_context.py
--rw-r--r--   0 root         (0) root         (0)     7261 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_config/pythonic_config/typing_utils.py
--rw-r--r--   0 root         (0) root         (0)      577 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_config/pythonic_config/utils.py
--rw-r--r--   0 root         (0) root         (0)    12143 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_config/snap.py
--rw-r--r--   0 root         (0) root         (0)     3267 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_config/source.py
--rw-r--r--   0 root         (0) root         (0)     3528 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_config/stack.py
--rw-r--r--   0 root         (0) root         (0)     7772 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_config/traversal_context.py
--rw-r--r--   0 root         (0) root         (0)     4167 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_config/type_printer.py
--rw-r--r--   0 root         (0) root         (0)    17162 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_config/validate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:43:44.519960 dagster-1.3.9/dagster/_core/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/__init__.py
--rw-r--r--   0 root         (0) root         (0)      994 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/assets.py
--rw-r--r--   0 root         (0) root         (0)    13645 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/code_pointer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:43:44.519960 dagster-1.3.9/dagster/_core/container_context/
--rw-r--r--   0 root         (0) root         (0)      184 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/container_context/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1277 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/container_context/config.py
--rw-r--r--   0 root         (0) root         (0)     2310 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/debug.py
--rw-r--r--   0 root         (0) root         (0)     3005 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/decorator_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:43:44.531961 dagster-1.3.9/dagster/_core/definitions/
--rw-r--r--   0 root         (0) root         (0)     7626 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/definitions/__init__.py
--rw-r--r--   0 root         (0) root         (0)    30543 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/definitions/asset_graph.py
--rw-r--r--   0 root         (0) root         (0)    10704 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/definitions/asset_graph_subset.py
--rw-r--r--   0 root         (0) root         (0)     3816 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/definitions/asset_in.py
--rw-r--r--   0 root         (0) root         (0)    37134 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/definitions/asset_layer.py
--rw-r--r--   0 root         (0) root         (0)     5685 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/definitions/asset_out.py
--rw-r--r--   0 root         (0) root         (0)    59306 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/definitions/asset_reconciliation_sensor.py
--rw-r--r--   0 root         (0) root         (0)    18474 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/definitions/asset_selection.py
--rw-r--r--   0 root         (0) root         (0)     7164 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/definitions/asset_sensor_definition.py
--rw-r--r--   0 root         (0) root         (0)    63783 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/definitions/assets.py
--rw-r--r--   0 root         (0) root         (0)    24376 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/definitions/assets_job.py
--rw-r--r--   0 root         (0) root         (0)     2806 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/definitions/auto_materialize_condition.py
--rw-r--r--   0 root         (0) root         (0)     5297 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/definitions/auto_materialize_policy.py
--rw-r--r--   0 root         (0) root         (0)    16105 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/definitions/cacheable_assets.py
--rw-r--r--   0 root         (0) root         (0)    45671 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/definitions/composition.py
--rw-r--r--   0 root         (0) root         (0)     4287 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/definitions/config.py
--rw-r--r--   0 root         (0) root         (0)    10845 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/definitions/configurable.py
--rw-r--r--   0 root         (0) root         (0)    20795 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/definitions/data_time.py
--rw-r--r--   0 root         (0) root         (0)    18695 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/definitions/data_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:43:44.531961 dagster-1.3.9/dagster/_core/definitions/decorators/
--rw-r--r--   0 root         (0) root         (0)      620 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/definitions/decorators/__init__.py
--rw-r--r--   0 root         (0) root         (0)    44389 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/definitions/decorators/asset_decorator.py
--rw-r--r--   0 root         (0) root         (0)     4915 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/definitions/decorators/config_mapping_decorator.py
--rw-r--r--   0 root         (0) root         (0)     8250 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/definitions/decorators/graph_decorator.py
--rw-r--r--   0 root         (0) root         (0)     9444 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/definitions/decorators/hook_decorator.py
--rw-r--r--   0 root         (0) root         (0)    10676 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/definitions/decorators/job_decorator.py
--rw-r--r--   0 root         (0) root         (0)    17845 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/definitions/decorators/op_decorator.py
--rw-r--r--   0 root         (0) root         (0)    14396 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/definitions/decorators/repository_decorator.py
--rw-r--r--   0 root         (0) root         (0)     8656 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/definitions/decorators/schedule_decorator.py
--rw-r--r--   0 root         (0) root         (0)    11936 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/definitions/decorators/sensor_decorator.py
--rw-r--r--   0 root         (0) root         (0)     7085 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/definitions/decorators/source_asset_decorator.py
--rw-r--r--   0 root         (0) root         (0)     5275 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/definitions/definition_config_schema.py
--rw-r--r--   0 root         (0) root         (0)    21205 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/definitions/definitions_class.py
--rw-r--r--   0 root         (0) root         (0)    39988 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/definitions/dependency.py
--rw-r--r--   0 root         (0) root         (0)    31576 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/definitions/events.py
--rw-r--r--   0 root         (0) root         (0)    21013 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/definitions/executor_definition.py
--rw-r--r--   0 root         (0) root         (0)    10548 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/definitions/external_asset_graph.py
--rw-r--r--   0 root         (0) root         (0)     8010 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/definitions/freshness_policy.py
--rw-r--r--   0 root         (0) root         (0)    16195 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/definitions/freshness_policy_sensor_definition.py
--rw-r--r--   0 root         (0) root         (0)    44740 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/definitions/graph_definition.py
--rw-r--r--   0 root         (0) root         (0)     6546 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/definitions/hook_definition.py
--rw-r--r--   0 root         (0) root         (0)     1515 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/definitions/hook_invocation.py
--rw-r--r--   0 root         (0) root         (0)     3205 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/definitions/inference.py
--rw-r--r--   0 root         (0) root         (0)    22898 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/definitions/input.py
--rw-r--r--   0 root         (0) root         (0)     5386 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/definitions/instigation_logger.py
--rw-r--r--   0 root         (0) root         (0)     2152 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/definitions/job_base.py
--rw-r--r--   0 root         (0) root         (0)    51157 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/definitions/job_definition.py
--rw-r--r--   0 root         (0) root         (0)    20308 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/definitions/load_assets_from_modules.py
--rw-r--r--   0 root         (0) root         (0)     6845 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/definitions/logger_definition.py
--rw-r--r--   0 root         (0) root         (0)      636 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/definitions/logger_invocation.py
--rw-r--r--   0 root         (0) root         (0)     8841 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/definitions/materialize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:43:44.531961 dagster-1.3.9/dagster/_core/definitions/metadata/
--rw-r--r--   0 root         (0) root         (0)    32319 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/definitions/metadata/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8557 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/definitions/metadata/table.py
--rw-r--r--   0 root         (0) root         (0)    56090 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/definitions/multi_asset_sensor_definition.py
--rw-r--r--   0 root         (0) root         (0)    20153 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/definitions/multi_dimensional_partitions.py
--rw-r--r--   0 root         (0) root         (0)       82 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/definitions/no_step_launcher.py
--rw-r--r--   0 root         (0) root         (0)    11927 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/definitions/node_container.py
--rw-r--r--   0 root         (0) root         (0)     8041 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/definitions/node_definition.py
--rw-r--r--   0 root         (0) root         (0)     2867 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/definitions/observe.py
--rw-r--r--   0 root         (0) root         (0)    22119 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/definitions/op_definition.py
--rw-r--r--   0 root         (0) root         (0)    19256 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/definitions/op_invocation.py
--rw-r--r--   0 root         (0) root         (0)     7509 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/definitions/op_selection.py
--rw-r--r--   0 root         (0) root         (0)    18908 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/definitions/output.py
--rw-r--r--   0 root         (0) root         (0)    39191 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/definitions/partition.py
--rw-r--r--   0 root         (0) root         (0)      196 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/definitions/partition_key_range.py
--rw-r--r--   0 root         (0) root         (0)    47274 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/definitions/partition_mapping.py
--rw-r--r--   0 root         (0) root         (0)     8902 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/definitions/partitioned_schedule.py
--rw-r--r--   0 root         (0) root         (0)     3779 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/definitions/policy.py
--rw-r--r--   0 root         (0) root         (0)    27231 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/definitions/reconstruct.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:43:44.531961 dagster-1.3.9/dagster/_core/definitions/repository_definition/
--rw-r--r--   0 root         (0) root         (0)      654 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/definitions/repository_definition/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6670 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/definitions/repository_definition/caching_index.py
--rw-r--r--   0 root         (0) root         (0)    18860 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/definitions/repository_definition/repository_data.py
--rw-r--r--   0 root         (0) root         (0)    17401 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/definitions/repository_definition/repository_data_builder.py
--rw-r--r--   0 root         (0) root         (0)    16917 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/definitions/repository_definition/repository_definition.py
--rw-r--r--   0 root         (0) root         (0)     1479 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/definitions/repository_definition/valid_definitions.py
--rw-r--r--   0 root         (0) root         (0)     5108 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/definitions/resolved_asset_deps.py
--rw-r--r--   0 root         (0) root         (0)     1336 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/definitions/resource_annotation.py
--rw-r--r--   0 root         (0) root         (0)    16162 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/definitions/resource_definition.py
--rw-r--r--   0 root         (0) root         (0)     5398 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/definitions/resource_invocation.py
--rw-r--r--   0 root         (0) root         (0)     7806 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/definitions/resource_requirement.py
--rw-r--r--   0 root         (0) root         (0)    24105 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/definitions/run_config.py
--rw-r--r--   0 root         (0) root         (0)     1445 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/definitions/run_config_schema.py
--rw-r--r--   0 root         (0) root         (0)    15824 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/definitions/run_request.py
--rw-r--r--   0 root         (0) root         (0)    38400 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/definitions/run_status_sensor_definition.py
--rw-r--r--   0 root         (0) root         (0)    37556 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/definitions/schedule_definition.py
--rw-r--r--   0 root         (0) root         (0)     5189 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/definitions/scoped_resources_builder.py
--rw-r--r--   0 root         (0) root         (0)    10837 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/definitions/selector.py
--rw-r--r--   0 root         (0) root         (0)    47376 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/definitions/sensor_definition.py
--rw-r--r--   0 root         (0) root         (0)    15391 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/definitions/source_asset.py
--rw-r--r--   0 root         (0) root         (0)     2298 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/definitions/step_launcher.py
--rw-r--r--   0 root         (0) root         (0)     1535 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/definitions/target.py
--rw-r--r--   0 root         (0) root         (0)      473 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/definitions/test_op_definition.py
--rw-r--r--   0 root         (0) root         (0)    12374 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/definitions/time_window_partition_mapping.py
--rw-r--r--   0 root         (0) root         (0)    78072 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/definitions/time_window_partitions.py
--rw-r--r--   0 root         (0) root         (0)    16744 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/definitions/unresolved_asset_job_definition.py
--rw-r--r--   0 root         (0) root         (0)     7992 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/definitions/utils.py
--rw-r--r--   0 root         (0) root         (0)     2930 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/definitions/version_strategy.py
--rw-r--r--   0 root         (0) root         (0)    26237 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/errors.py
--rw-r--r--   0 root         (0) root         (0)     6241 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/event_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:43:44.531961 dagster-1.3.9/dagster/_core/events/
--rw-r--r--   0 root         (0) root         (0)    64981 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/events/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7783 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/events/log.py
--rw-r--r--   0 root         (0) root         (0)     1614 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/events/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:43:44.535961 dagster-1.3.9/dagster/_core/execution/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/execution/__init__.py
--rw-r--r--   0 root         (0) root         (0)    38315 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/execution/api.py
--rw-r--r--   0 root         (0) root         (0)    36589 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/execution/asset_backfill.py
--rw-r--r--   0 root         (0) root         (0)    14710 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/execution/backfill.py
--rw-r--r--   0 root         (0) root         (0)     6487 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/execution/build_resources.py
--rw-r--r--   0 root         (0) root         (0)      224 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/execution/bulk_actions.py
--rw-r--r--   0 root         (0) root         (0)     5587 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/execution/compute_logs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:43:44.535961 dagster-1.3.9/dagster/_core/execution/context/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/execution/context/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21992 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/execution/context/compute.py
--rw-r--r--   0 root         (0) root         (0)    15991 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/execution/context/hook.py
--rw-r--r--   0 root         (0) root         (0)     9369 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/execution/context/init.py
--rw-r--r--   0 root         (0) root         (0)    26845 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/execution/context/input.py
--rw-r--r--   0 root         (0) root         (0)    27349 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/execution/context/invocation.py
--rw-r--r--   0 root         (0) root         (0)     3164 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/execution/context/logger.py
--rw-r--r--   0 root         (0) root         (0)    33974 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/execution/context/output.py
--rw-r--r--   0 root         (0) root         (0)    44193 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/execution/context/system.py
--rw-r--r--   0 root         (0) root         (0)    18501 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/execution/context_creation_job.py
--rw-r--r--   0 root         (0) root         (0)     5149 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/execution/execute_in_process.py
--rw-r--r--   0 root         (0) root         (0)     5426 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/execution/execute_in_process_result.py
--rw-r--r--   0 root         (0) root         (0)     9183 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/execution/execution_result.py
--rw-r--r--   0 root         (0) root         (0)     8544 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/execution/host_mode.py
--rw-r--r--   0 root         (0) root         (0)    14451 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/execution/job_backfill.py
--rw-r--r--   0 root         (0) root         (0)     6487 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/execution/job_execution_result.py
--rw-r--r--   0 root         (0) root         (0)      998 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/execution/memoization.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:43:44.539961 dagster-1.3.9/dagster/_core/execution/plan/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/execution/plan/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25252 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/execution/plan/active.py
--rw-r--r--   0 root         (0) root         (0)     7279 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/execution/plan/compute.py
--rw-r--r--   0 root         (0) root         (0)    12550 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/execution/plan/compute_generator.py
--rw-r--r--   0 root         (0) root         (0)    16658 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/execution/plan/execute_plan.py
--rw-r--r--   0 root         (0) root         (0)    27355 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/execution/plan/execute_step.py
--rw-r--r--   0 root         (0) root         (0)    10000 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/execution/plan/external_step.py
--rw-r--r--   0 root         (0) root         (0)     3664 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/execution/plan/handle.py
--rw-r--r--   0 root         (0) root         (0)    37831 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/execution/plan/inputs.py
--rw-r--r--   0 root         (0) root         (0)     4352 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/execution/plan/instance_concurrency_context.py
--rw-r--r--   0 root         (0) root         (0)     1159 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/execution/plan/local_external_step_main.py
--rw-r--r--   0 root         (0) root         (0)     5395 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/execution/plan/objects.py
--rw-r--r--   0 root         (0) root         (0)     7057 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/execution/plan/outputs.py
--rw-r--r--   0 root         (0) root         (0)    58041 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/execution/plan/plan.py
--rw-r--r--   0 root         (0) root         (0)      114 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/execution/plan/resume_retry.py
--rw-r--r--   0 root         (0) root         (0)    15616 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/execution/plan/state.py
--rw-r--r--   0 root         (0) root         (0)    15920 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/execution/plan/step.py
--rw-r--r--   0 root         (0) root         (0)     3796 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/execution/plan/utils.py
--rw-r--r--   0 root         (0) root         (0)     1762 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/execution/poll_compute_logs.py
--rw-r--r--   0 root         (0) root         (0)     8186 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/execution/resolve_versions.py
--rw-r--r--   0 root         (0) root         (0)    19280 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/execution/resources_init.py
--rw-r--r--   0 root         (0) root         (0)     2104 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/execution/retries.py
--rw-r--r--   0 root         (0) root         (0)     1651 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/execution/run_cancellation_thread.py
--rw-r--r--   0 root         (0) root         (0)    10329 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/execution/stats.py
--rw-r--r--   0 root         (0) root         (0)     1125 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/execution/tags.py
--rw-r--r--   0 root         (0) root         (0)     1172 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/execution/validate_run_config.py
--rw-r--r--   0 root         (0) root         (0)     1282 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/execution/watch_orphans.py
--rw-r--r--   0 root         (0) root         (0)     4233 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/execution/with_resources.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:43:44.539961 dagster-1.3.9/dagster/_core/executor/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/executor/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1265 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/executor/base.py
--rw-r--r--   0 root         (0) root         (0)     5990 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/executor/child_process_executor.py
--rw-r--r--   0 root         (0) root         (0)     3431 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/executor/in_process.py
--rw-r--r--   0 root         (0) root         (0)     1509 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/executor/init.py
--rw-r--r--   0 root         (0) root         (0)    15592 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/executor/multiprocess.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:43:44.539961 dagster-1.3.9/dagster/_core/executor/step_delegating/
--rw-r--r--   0 root         (0) root         (0)      247 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/executor/step_delegating/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15580 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/executor/step_delegating/step_delegating_executor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:43:44.539961 dagster-1.3.9/dagster/_core/executor/step_delegating/step_handler/
--rw-r--r--   0 root         (0) root         (0)      152 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/executor/step_delegating/step_handler/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3078 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/executor/step_delegating/step_handler/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:43:44.543961 dagster-1.3.9/dagster/_core/host_representation/
--rw-r--r--   0 root         (0) root         (0)     2789 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/host_representation/__init__.py
--rw-r--r--   0 root         (0) root         (0)    33518 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/host_representation/code_location.py
--rw-r--r--   0 root         (0) root         (0)    32089 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/host_representation/external.py
--rw-r--r--   0 root         (0) root         (0)    70934 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/host_representation/external_data.py
--rw-r--r--   0 root         (0) root         (0)    12517 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/host_representation/grpc_server_registry.py
--rw-r--r--   0 root         (0) root         (0)     1487 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/host_representation/grpc_server_state_subscriber.py
--rw-r--r--   0 root         (0) root         (0)     4333 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/host_representation/handle.py
--rw-r--r--   0 root         (0) root         (0)     1581 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/host_representation/historical.py
--rw-r--r--   0 root         (0) root         (0)     4850 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/host_representation/job_index.py
--rw-r--r--   0 root         (0) root         (0)    19051 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/host_representation/origin.py
--rw-r--r--   0 root         (0) root         (0)     3610 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/host_representation/represented.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:43:44.543961 dagster-1.3.9/dagster/_core/instance/
--rw-r--r--   0 root         (0) root         (0)   104144 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/instance/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12956 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/instance/config.py
--rw-r--r--   0 root         (0) root         (0)    24084 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/instance/ref.py
--rw-r--r--   0 root         (0) root         (0)     3899 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/instance_for_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:43:44.543961 dagster-1.3.9/dagster/_core/launcher/
--rw-r--r--   0 root         (0) root         (0)      297 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/launcher/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3758 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/launcher/base.py
--rw-r--r--   0 root         (0) root         (0)     6808 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/launcher/default_run_launcher.py
--rw-r--r--   0 root         (0) root         (0)     1586 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/launcher/sync_in_memory_run_launcher.py
--rw-r--r--   0 root         (0) root         (0)      473 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/libraries.py
--rw-r--r--   0 root         (0) root         (0)    17249 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/log_manager.py
--rw-r--r--   0 root         (0) root         (0)     1029 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/nux.py
--rw-r--r--   0 root         (0) root         (0)     3691 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/origin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:43:44.543961 dagster-1.3.9/dagster/_core/run_coordinator/
--rw-r--r--   0 root         (0) root         (0)      267 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/run_coordinator/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2005 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/run_coordinator/base.py
--rw-r--r--   0 root         (0) root         (0)     1922 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/run_coordinator/default_run_coordinator.py
--rw-r--r--   0 root         (0) root         (0)    11030 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/run_coordinator/queued_run_coordinator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:43:44.543961 dagster-1.3.9/dagster/_core/scheduler/
--rw-r--r--   0 root         (0) root         (0)      534 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/scheduler/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1241 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/scheduler/execution.py
--rw-r--r--   0 root         (0) root         (0)    21903 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/scheduler/instigation.py
--rw-r--r--   0 root         (0) root         (0)     9410 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/scheduler/scheduler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:43:44.543961 dagster-1.3.9/dagster/_core/secrets/
--rw-r--r--   0 root         (0) root         (0)       51 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/secrets/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1811 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/secrets/env_file.py
--rw-r--r--   0 root         (0) root         (0)      388 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/secrets/loader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:43:44.543961 dagster-1.3.9/dagster/_core/selector/
--rw-r--r--   0 root         (0) root         (0)      295 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/selector/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18247 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/selector/subset_selector.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:43:44.543961 dagster-1.3.9/dagster/_core/snap/
--rw-r--r--   0 root         (0) root         (0)     2815 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/snap/__init__.py
--rw-r--r--   0 root         (0) root         (0)      494 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/snap/config_types.py
--rw-r--r--   0 root         (0) root         (0)     3999 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/snap/dagster_types.py
--rw-r--r--   0 root         (0) root         (0)     9421 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/snap/dep_snapshot.py
--rw-r--r--   0 root         (0) root         (0)    12099 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/snap/execution_plan_snapshot.py
--rw-r--r--   0 root         (0) root         (0)    16654 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/snap/job_snapshot.py
--rw-r--r--   0 root         (0) root         (0)     4495 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/snap/mode.py
--rw-r--r--   0 root         (0) root         (0)    14452 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/snap/node.py
--rw-r--r--   0 root         (0) root         (0)     1964 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/snap/snap_to_yaml.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:43:44.551961 dagster-1.3.9/dagster/_core/storage/
--rw-r--r--   0 root         (0) root         (0)     3057 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/DEVELOPING.md
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:43:44.551961 dagster-1.3.9/dagster/_core/storage/alembic/
--rw-r--r--   0 root         (0) root         (0)     6676 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/alembic/README.md
--rw-r--r--   0 root         (0) root         (0)      687 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/alembic/env.py
--rw-r--r--   0 root         (0) root         (0)      494 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/alembic/script.py.mako
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:43:44.559961 dagster-1.3.9/dagster/_core/storage/alembic/versions/
--rw-r--r--   0 root         (0) root         (0)     3150 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/alembic/versions/001_initial_1.py
--rw-r--r--   0 root         (0) root         (0)      311 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/alembic/versions/001_initial_schedule.py
--rw-r--r--   0 root         (0) root         (0)     1485 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_postgres.py
--rw-r--r--   0 root         (0) root         (0)      598 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      972 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_postgres.py
--rw-r--r--   0 root         (0) root         (0)      972 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     2548 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/alembic/versions/004_add_snapshots_to_run_storage.py
--rw-r--r--   0 root         (0) root         (0)     1405 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/alembic/versions/005_add_asset_key_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1405 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/alembic/versions/005_add_asset_key_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1130 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/alembic/versions/006_scheduler_update_postgres.py
--rw-r--r--   0 root         (0) root         (0)      952 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/alembic/versions/007_create_run_id_idx_postgres.py
--rw-r--r--   0 root         (0) root         (0)      952 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/alembic/versions/007_create_run_id_idx_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      955 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/alembic/versions/008_add_run_tags_index_postgres.py
--rw-r--r--   0 root         (0) root         (0)      955 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/alembic/versions/008_add_run_tags_index_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1170 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/alembic/versions/009_add_partition_column_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1170 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/alembic/versions/009_add_partition_column_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1729 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1729 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1146 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1124 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_1.py
--rw-r--r--   0 root         (0) root         (0)     1142 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_2.py
--rw-r--r--   0 root         (0) root         (0)      416 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/alembic/versions/012_0_10_0_create_new_run_tables_postgres.py
--rw-r--r--   0 root         (0) root         (0)      416 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/alembic/versions/012_0_10_0_create_new_run_tables_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      434 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/alembic/versions/013_0_10_0_create_new_event_log_tables_postgres.py
--rw-r--r--   0 root         (0) root         (0)      434 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/alembic/versions/013_0_10_0_create_new_event_log_tables_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      431 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/alembic/versions/014_0_10_0_create_new_schedule_tables_postgres.py
--rw-r--r--   0 root         (0) root         (0)      431 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/alembic/versions/014_0_10_0_create_new_schedule_tables_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     3926 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_postgres.py
--rw-r--r--   0 root         (0) root         (0)     3926 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      408 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/alembic/versions/016_add_bulk_actions_table_postgres.py
--rw-r--r--   0 root         (0) root         (0)      408 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/alembic/versions/016_add_bulk_actions_table_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      935 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/alembic/versions/017_add_run_status_index_postgres.py
--rw-r--r--   0 root         (0) root         (0)      935 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/alembic/versions/017_add_run_status_index_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      325 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/alembic/versions/017_initial_mysql.py
--rw-r--r--   0 root         (0) root         (0)      420 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/alembic/versions/018_add_asset_tags_mysql.py
--rw-r--r--   0 root         (0) root         (0)      420 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/alembic/versions/018_add_asset_tags_postgres.py
--rw-r--r--   0 root         (0) root         (0)      420 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/alembic/versions/018_add_asset_tags_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1569 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1569 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      409 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/alembic/versions/020_add_column_asset_body_mysql.py
--rw-r--r--   0 root         (0) root         (0)      409 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/alembic/versions/020_add_column_asset_body_postgres.py
--rw-r--r--   0 root         (0) root         (0)      409 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/alembic/versions/020_add_column_asset_body_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1033 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/alembic/versions/021_add_column_mode_mysql.py
--rw-r--r--   0 root         (0) root         (0)     1031 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/alembic/versions/021_add_column_mode_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1033 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/alembic/versions/021_add_column_mode_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      432 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_mysql.py
--rw-r--r--   0 root         (0) root         (0)      432 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_postgres.py
--rw-r--r--   0 root         (0) root         (0)      432 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      420 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_mysql.py
--rw-r--r--   0 root         (0) root         (0)      420 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_postgres.py
--rw-r--r--   0 root         (0) root         (0)      420 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      530 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_mysql.py
--rw-r--r--   0 root         (0) root         (0)     1274 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1274 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      403 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/alembic/versions/025_add_range_index_mysql.py
--rw-r--r--   0 root         (0) root         (0)      403 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/alembic/versions/025_add_range_index_postgres.py
--rw-r--r--   0 root         (0) root         (0)      403 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/alembic/versions/025_add_range_index_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      634 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/alembic/versions/026_convert_start_end_times_format_mysql.py
--rw-r--r--   0 root         (0) root         (0)      433 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/alembic/versions/027_add_migration_table_mysql.py
--rw-r--r--   0 root         (0) root         (0)      433 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/alembic/versions/027_add_migration_table_postgres.py
--rw-r--r--   0 root         (0) root         (0)      433 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/alembic/versions/027_add_migration_table_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      409 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/alembic/versions/028_add_instigators_table_mysql.py
--rw-r--r--   0 root         (0) root         (0)      409 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/alembic/versions/028_add_instigators_table_postgres.py
--rw-r--r--   0 root         (0) root         (0)      409 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/alembic/versions/028_add_instigators_table_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      415 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_mysql.py
--rw-r--r--   0 root         (0) root         (0)      415 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_postgres.py
--rw-r--r--   0 root         (0) root         (0)      415 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1892 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/alembic/versions/030_add_columns_action_type_and_selector_id_.py
--rw-r--r--   0 root         (0) root         (0)      957 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/alembic/versions/031_add_kvs_table.py
--rw-r--r--   0 root         (0) root         (0)      498 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/alembic/versions/032_rebuild_event_indexes.py
--rw-r--r--   0 root         (0) root         (0)     1950 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/alembic/versions/033_add_asset_event_tags_table.py
--rw-r--r--   0 root         (0) root         (0)      428 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/alembic/versions/034_add_cached_status_data_column.py
--rw-r--r--   0 root         (0) root         (0)      426 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/alembic/versions/035_add_run_job_index.py
--rw-r--r--   0 root         (0) root         (0)     1536 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/alembic/versions/036_add_dynamic_partitions_table.py
--rw-r--r--   0 root         (0) root         (0)     2480 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/alembic/versions/037_d9092588866f_add_primary_key_cols.py
--rw-r--r--   0 root         (0) root         (0)     1176 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/alembic/versions/038_701913684cb4_add_postgres_pks.py
--rw-r--r--   0 root         (0) root         (0)     2062 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/alembic/versions/039_d3a4c9e87af3_add_asset_daemon_asset_evaluations_table.py
--rw-r--r--   0 root         (0) root         (0)     2358 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/alembic/versions/040_add_in_progress_step_table.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/alembic/versions/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7204 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/asset_value_loader.py
--rw-r--r--   0 root         (0) root         (0)     1215 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/base_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:43:44.559961 dagster-1.3.9/dagster/_core/storage/branching/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/branching/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4304 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/branching/branching_io_manager.py
--rw-r--r--   0 root         (0) root         (0)     8736 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/captured_log_manager.py
--rw-r--r--   0 root         (0) root         (0)    16247 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/cloud_storage_compute_log_manager.py
--rw-r--r--   0 root         (0) root         (0)     9545 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/compute_log_manager.py
--rw-r--r--   0 root         (0) root         (0)     1863 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/config.py
--rw-r--r--   0 root         (0) root         (0)      417 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/daemon_cursor.py
--rw-r--r--   0 root         (0) root         (0)    24055 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/dagster_run.py
--rw-r--r--   0 root         (0) root         (0)    11640 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/db_io_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:43:44.559961 dagster-1.3.9/dagster/_core/storage/event_log/
--rw-r--r--   0 root         (0) root         (0)      742 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/event_log/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16268 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/event_log/base.py
--rw-r--r--   0 root         (0) root         (0)     3753 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/event_log/in_memory.py
--rw-r--r--   0 root         (0) root         (0)     7273 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/event_log/migration.py
--rw-r--r--   0 root         (0) root         (0)     7911 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/event_log/polling_event_watcher.py
--rw-r--r--   0 root         (0) root         (0)     6408 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/event_log/schema.py
--rw-r--r--   0 root         (0) root         (0)   100680 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/event_log/sql_event_log.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:43:44.559961 dagster-1.3.9/dagster/_core/storage/event_log/sqlite/
--rw-r--r--   0 root         (0) root         (0)      200 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/event_log/sqlite/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:43:44.559961 dagster-1.3.9/dagster/_core/storage/event_log/sqlite/alembic/
--rw-r--r--   0 root         (0) root         (0)     1040 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/event_log/sqlite/alembic/alembic.ini
--rw-r--r--   0 root         (0) root         (0)     7526 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/event_log/sqlite/consolidated_sqlite_event_log.py
--rw-r--r--   0 root         (0) root         (0)    19093 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/event_log/sqlite/sqlite_event_log.py
--rw-r--r--   0 root         (0) root         (0)    10912 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/file_manager.py
--rw-r--r--   0 root         (0) root         (0)    13217 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/fs_io_manager.py
--rw-r--r--   0 root         (0) root         (0)     8915 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/input_manager.py
--rw-r--r--   0 root         (0) root         (0)    10638 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/io_manager.py
--rw-r--r--   0 root         (0) root         (0)    28589 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/legacy_storage.py
--rw-r--r--   0 root         (0) root         (0)    17301 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/local_compute_log_manager.py
--rw-r--r--   0 root         (0) root         (0)      876 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/mem_io_manager.py
--rw-r--r--   0 root         (0) root         (0)     4293 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/memoizable_io_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:43:44.559961 dagster-1.3.9/dagster/_core/storage/migration/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/migration/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14469 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/migration/utils.py
--rw-r--r--   0 root         (0) root         (0)     3186 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/noop_compute_log_manager.py
--rw-r--r--   0 root         (0) root         (0)     2361 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/output_manager.py
--rw-r--r--   0 root         (0) root         (0)    23189 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/partition_status_cache.py
--rw-r--r--   0 root         (0) root         (0)     2121 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/root.py
--rw-r--r--   0 root         (0) root         (0)     8509 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/root_input_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:43:44.559961 dagster-1.3.9/dagster/_core/storage/runs/
--rw-r--r--   0 root         (0) root         (0)      386 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/runs/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15454 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/runs/base.py
--rw-r--r--   0 root         (0) root         (0)     2416 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/runs/in_memory.py
--rw-r--r--   0 root         (0) root         (0)     8697 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/runs/migration.py
--rw-r--r--   0 root         (0) root         (0)     5982 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/runs/schema.py
--rw-r--r--   0 root         (0) root         (0)    46286 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/runs/sql_run_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:43:44.559961 dagster-1.3.9/dagster/_core/storage/runs/sqlite/
--rw-r--r--   0 root         (0) root         (0)       69 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/runs/sqlite/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:43:44.559961 dagster-1.3.9/dagster/_core/storage/runs/sqlite/alembic/
--rw-r--r--   0 root         (0) root         (0)     1040 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/runs/sqlite/alembic/alembic.ini
--rw-r--r--   0 root         (0) root         (0)     6818 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/runs/sqlite/sqlite_run_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:43:44.563961 dagster-1.3.9/dagster/_core/storage/schedules/
--rw-r--r--   0 root         (0) root         (0)      272 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/schedules/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6358 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/schedules/base.py
--rw-r--r--   0 root         (0) root         (0)     4133 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/schedules/migration.py
--rw-r--r--   0 root         (0) root         (0)     3710 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/schedules/schema.py
--rw-r--r--   0 root         (0) root         (0)    22626 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/schedules/sql_schedule_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:43:44.563961 dagster-1.3.9/dagster/_core/storage/schedules/sqlite/
--rw-r--r--   0 root         (0) root         (0)       84 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/schedules/sqlite/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:43:44.563961 dagster-1.3.9/dagster/_core/storage/schedules/sqlite/alembic/
--rw-r--r--   0 root         (0) root         (0)     1039 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/schedules/sqlite/alembic/alembic.ini
--rw-r--r--   0 root         (0) root         (0)     3684 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/schedules/sqlite/sqlite_schedule_storage.py
--rw-r--r--   0 root         (0) root         (0)     7210 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/sql.py
--rw-r--r--   0 root         (0) root         (0)     1391 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/sqlalchemy_compat.py
--rw-r--r--   0 root         (0) root         (0)      926 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/sqlite.py
--rw-r--r--   0 root         (0) root         (0)     4863 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/sqlite_storage.py
--rw-r--r--   0 root         (0) root         (0)     3199 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/tags.py
--rw-r--r--   0 root         (0) root         (0)     1128 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/temp_file_manager.py
--rw-r--r--   0 root         (0) root         (0)    11346 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/storage/upath_io_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:43:44.563961 dagster-1.3.9/dagster/_core/system_config/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/system_config/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13981 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/system_config/composite_descent.py
--rw-r--r--   0 root         (0) root         (0)    14855 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/system_config/objects.py
--rw-r--r--   0 root         (0) root         (0)    27932 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/telemetry.py
--rw-r--r--   0 root         (0) root         (0)     4824 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/telemetry_upload.py
--rw-r--r--   0 root         (0) root         (0)    18936 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/test_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:43:44.563961 dagster-1.3.9/dagster/_core/types/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/types/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3163 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/types/builtin_config_schemas.py
--rw-r--r--   0 root         (0) root         (0)     7298 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/types/config_schema.py
--rw-r--r--   0 root         (0) root         (0)    35761 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/types/dagster_type.py
--rw-r--r--   0 root         (0) root         (0)     3579 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/types/decorator.py
--rw-r--r--   0 root         (0) root         (0)     1846 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/types/loadable_target_origin.py
--rw-r--r--   0 root         (0) root         (0)     1027 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/types/primitive_mapping.py
--rw-r--r--   0 root         (0) root         (0)     4881 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/types/python_dict.py
--rw-r--r--   0 root         (0) root         (0)     2836 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/types/python_set.py
--rw-r--r--   0 root         (0) root         (0)     3712 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/types/python_tuple.py
--rw-r--r--   0 root         (0) root         (0)     1772 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/types/transform_typing.py
--rw-r--r--   0 root         (0) root         (0)     1438 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/utility_ops.py
--rw-r--r--   0 root         (0) root         (0)     4402 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:43:44.563961 dagster-1.3.9/dagster/_core/workspace/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/workspace/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4722 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/workspace/autodiscovery.py
--rw-r--r--   0 root         (0) root         (0)     3478 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/workspace/config_schema.py
--rw-r--r--   0 root         (0) root         (0)    28195 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/workspace/context.py
--rw-r--r--   0 root         (0) root         (0)    11881 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/workspace/load.py
--rw-r--r--   0 root         (0) root         (0)     4684 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/workspace/load_target.py
--rw-r--r--   0 root         (0) root         (0)     4099 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/workspace/permissions.py
--rw-r--r--   0 root         (0) root         (0)     1912 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_core/workspace/workspace.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:43:44.567961 dagster-1.3.9/dagster/_daemon/
--rw-r--r--   0 root         (0) root         (0)     2015 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_daemon/__init__.py
--rw-r--r--   0 root         (0) root         (0)       30 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_daemon/__main__.py
--rw-r--r--   0 root         (0) root         (0)     6416 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_daemon/asset_daemon.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:43:44.567961 dagster-1.3.9/dagster/_daemon/auto_run_reexecution/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_daemon/auto_run_reexecution/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6822 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_daemon/auto_run_reexecution/auto_run_reexecution.py
--rw-r--r--   0 root         (0) root         (0)     9123 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_daemon/auto_run_reexecution/event_log_consumer.py
--rw-r--r--   0 root         (0) root         (0)     2125 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_daemon/backfill.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:43:44.567961 dagster-1.3.9/dagster/_daemon/cli/
--rw-r--r--   0 root         (0) root         (0)     4447 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_daemon/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18221 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_daemon/controller.py
--rw-r--r--   0 root         (0) root         (0)    10611 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_daemon/daemon.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:43:44.567961 dagster-1.3.9/dagster/_daemon/monitoring/
--rw-r--r--   0 root         (0) root         (0)      320 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_daemon/monitoring/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1792 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_daemon/monitoring/concurrency.py
--rw-r--r--   0 root         (0) root         (0)    10036 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_daemon/monitoring/run_monitoring.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:43:44.567961 dagster-1.3.9/dagster/_daemon/run_coordinator/
--rw-r--r--   0 root         (0) root         (0)      100 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_daemon/run_coordinator/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16326 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_daemon/run_coordinator/queued_run_coordinator_daemon.py
--rw-r--r--   0 root         (0) root         (0)    39892 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_daemon/sensor.py
--rw-r--r--   0 root         (0) root         (0)     2860 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_daemon/types.py
--rw-r--r--   0 root         (0) root         (0)     6639 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_daemon/workspace.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:43:44.567961 dagster-1.3.9/dagster/_experimental/
--rw-r--r--   0 root         (0) root         (0)      300 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_experimental/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:43:44.567961 dagster-1.3.9/dagster/_generate/
--rw-r--r--   0 root         (0) root         (0)      253 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_generate/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2720 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_generate/download.py
--rw-r--r--   0 root         (0) root         (0)     4805 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_generate/generate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:43:44.507960 dagster-1.3.9/dagster/_generate/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:43:44.567961 dagster-1.3.9/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:43:44.567961 dagster-1.3.9/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/
--rw-r--r--   0 root         (0) root         (0)      175 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/assets.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:43:44.567961 dagster-1.3.9/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/test_assets.py.tmpl
--rw-r--r--   0 root         (0) root         (0)      137 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/pyproject.toml.tmpl
--rw-r--r--   0 root         (0) root         (0)       43 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/setup.cfg.tmpl
--rw-r--r--   0 root         (0) root         (0)      285 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/setup.py.tmpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:43:44.567961 dagster-1.3.9/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/
--rw-r--r--   0 root         (0) root         (0)     1753 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:43:44.567961 dagster-1.3.9/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:43:44.567961 dagster-1.3.9/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/
--rw-r--r--   0 root         (0) root         (0)       40 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/__init__.py.tmpl
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/assets.py
--rw-r--r--   0 root         (0) root         (0)      164 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/repository.py.tmpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:43:44.567961 dagster-1.3.9/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/test_assets.py.tmpl
--rw-r--r--   0 root         (0) root         (0)       80 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       34 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/setup.cfg.tmpl
--rw-r--r--   0 root         (0) root         (0)      267 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/setup.py.tmpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:43:44.571961 dagster-1.3.9/dagster/_grpc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:43:44.571961 dagster-1.3.9/dagster/_grpc/__generated__/
--rw-r--r--   0 root         (0) root         (0)      178 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_grpc/__generated__/__init__.py
--rw-r--r--   0 root         (0) root         (0)    29251 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_grpc/__generated__/api_pb2.py
--rw-r--r--   0 root         (0) root         (0)    39700 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_grpc/__generated__/api_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     2051 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_grpc/__init__.py
--rw-r--r--   0 root         (0) root         (0)       89 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_grpc/__main__.py
--rw-r--r--   0 root         (0) root         (0)    18451 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_grpc/client.py
--rw-r--r--   0 root         (0) root         (0)     4202 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_grpc/compile.py
--rw-r--r--   0 root         (0) root         (0)    21967 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_grpc/impl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:43:44.571961 dagster-1.3.9/dagster/_grpc/protos/
--rw-r--r--   0 root         (0) root         (0)     5551 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_grpc/protos/api.proto
--rw-r--r--   0 root         (0) root         (0)    12415 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_grpc/proxy_server.py
--rw-r--r--   0 root         (0) root         (0)    51532 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_grpc/server.py
--rw-r--r--   0 root         (0) root         (0)     5301 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_grpc/server_watcher.py
--rw-r--r--   0 root         (0) root         (0)    26559 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_grpc/types.py
--rw-r--r--   0 root         (0) root         (0)     2323 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_grpc/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:43:44.571961 dagster-1.3.9/dagster/_legacy/
--rw-r--r--   0 root         (0) root         (0)      222 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_legacy/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:43:44.571961 dagster-1.3.9/dagster/_loggers/
--rw-r--r--   0 root         (0) root         (0)     3781 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_loggers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3269 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_module_alias_map.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:43:44.571961 dagster-1.3.9/dagster/_scheduler/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_scheduler/__init__.py
--rw-r--r--   0 root         (0) root         (0)    34396 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_scheduler/scheduler.py
--rw-r--r--   0 root         (0) root         (0)     1361 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_scheduler/stale.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:43:44.571961 dagster-1.3.9/dagster/_serdes/
--rw-r--r--   0 root         (0) root         (0)      629 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_serdes/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8004 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_serdes/config_class.py
--rw-r--r--   0 root         (0) root         (0)      142 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_serdes/errors.py
--rw-r--r--   0 root         (0) root         (0)     7467 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_serdes/ipc.py
--rw-r--r--   0 root         (0) root         (0)    37613 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_serdes/serdes.py
--rw-r--r--   0 root         (0) root         (0)      674 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_serdes/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:43:44.571961 dagster-1.3.9/dagster/_seven/
--rw-r--r--   0 root         (0) root         (0)     5496 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_seven/__init__.py
--rw-r--r--   0 root         (0) root         (0)      553 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_seven/abc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:43:44.571961 dagster-1.3.9/dagster/_seven/compat/
--rw-r--r--   0 root         (0) root         (0)      105 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_seven/compat/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1160 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_seven/compat/pendulum.py
--rw-r--r--   0 root         (0) root         (0)      383 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_seven/json.py
--rw-r--r--   0 root         (0) root         (0)      354 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_seven/temp_dir.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:43:44.575961 dagster-1.3.9/dagster/_utils/
--rw-r--r--   0 root         (0) root         (0)    23319 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8732 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_utils/alert.py
--rw-r--r--   0 root         (0) root         (0)     6965 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_utils/backcompat.py
--rw-r--r--   0 root         (0) root         (0)     2250 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_utils/backoff.py
--rw-r--r--   0 root         (0) root         (0)     4116 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_utils/cached_method.py
--rw-r--r--   0 root         (0) root         (0)    25123 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_utils/caching_instance_queryer.py
--rw-r--r--   0 root         (0) root         (0)     3813 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_utils/concurrency.py
--rw-r--r--   0 root         (0) root         (0)     2563 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_utils/dagster_type.py
--rw-r--r--   0 root         (0) root         (0)      799 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_utils/env.py
--rw-r--r--   0 root         (0) root         (0)     4094 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_utils/error.py
--rw-r--r--   0 root         (0) root         (0)     1264 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_utils/external.py
--rw-r--r--   0 root         (0) root         (0)      883 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_utils/forked_pdb.py
--rw-r--r--   0 root         (0) root         (0)     2344 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_utils/hosted_user_process.py
--rw-r--r--   0 root         (0) root         (0)     2796 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_utils/indenting_printer.py
--rw-r--r--   0 root         (0) root         (0)      344 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_utils/internal_init.py
--rw-r--r--   0 root         (0) root         (0)     3227 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_utils/interrupts.py
--rw-r--r--   0 root         (0) root         (0)     9113 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_utils/log.py
--rw-r--r--   0 root         (0) root         (0)     2313 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_utils/merger.py
--rw-r--r--   0 root         (0) root         (0)     1507 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_utils/net.py
--rw-r--r--   0 root         (0) root         (0)      208 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_utils/partitions.py
--rw-r--r--   0 root         (0) root         (0)    12340 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_utils/schedules.py
--rw-r--r--   0 root         (0) root         (0)     3289 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_utils/tags.py
--rw-r--r--   0 root         (0) root         (0)     1820 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_utils/temp_file.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:43:44.575961 dagster-1.3.9/dagster/_utils/test/
--rw-r--r--   0 root         (0) root         (0)    12640 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_utils/test/__init__.py
--rw-r--r--   0 root         (0) root         (0)      119 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_utils/test/hello_world_defs.py
--rw-r--r--   0 root         (0) root         (0)      214 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_utils/test/hello_world_repository.py
--rw-r--r--   0 root         (0) root         (0)     8622 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_utils/test/mysql_instance.py
--rw-r--r--   0 root         (0) root         (0)      256 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_utils/test/named_hello_world_repository.py
--rw-r--r--   0 root         (0) root         (0)     9330 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_utils/test/postgres_instance.py
--rw-r--r--   0 root         (0) root         (0)    28864 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_utils/test/schedule_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:43:44.575961 dagster-1.3.9/dagster/_utils/test/toys/
--rw-r--r--   0 root         (0) root         (0)       83 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_utils/test/toys/__init__.py
--rw-r--r--   0 root         (0) root         (0)       84 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_utils/test/toys/single_repository.py
--rw-r--r--   0 root         (0) root         (0)     2004 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_utils/timing.py
--rw-r--r--   0 root         (0) root         (0)      170 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_utils/types.py
--rw-r--r--   0 root         (0) root         (0)     3334 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_utils/typing_api.py
--rw-r--r--   0 root         (0) root         (0)     4915 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/_utils/yaml_utils.py
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/py.typed
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-08 18:43:17.000000 dagster-1.3.9/dagster/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:43:44.511960 dagster-1.3.9/dagster.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8790 2023-06-08 18:43:44.000000 dagster-1.3.9/dagster.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    25431 2023-06-08 18:43:44.000000 dagster-1.3.9/dagster.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 18:43:44.000000 dagster-1.3.9/dagster.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       86 2023-06-08 18:43:44.000000 dagster-1.3.9/dagster.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)     1443 2023-06-08 18:43:44.000000 dagster-1.3.9/dagster.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-08 18:43:44.000000 dagster-1.3.9/dagster.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      154 2023-06-08 18:43:44.579961 dagster-1.3.9/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     6820 2023-06-08 18:43:17.000000 dagster-1.3.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:21:09.092564 dagster-1.3.9rc0/
+-rw-r--r--   0 root         (0) root         (0)      549 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/COPYING
+-rw-r--r--   0 root         (0) root         (0)    11344 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      485 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     8793 2023-06-08 18:21:09.092564 dagster-1.3.9rc0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7167 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:21:09.024563 dagster-1.3.9rc0/dagster/
+-rw-r--r--   0 root         (0) root         (0)    26213 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       31 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     5456 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_annotations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:21:09.024563 dagster-1.3.9rc0/dagster/_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      731 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_api/get_server_id.py
+-rw-r--r--   0 root         (0) root         (0)     2147 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_api/list_repositories.py
+-rw-r--r--   0 root         (0) root         (0)      531 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_api/notebook_data.py
+-rw-r--r--   0 root         (0) root         (0)     2882 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_api/snapshot_execution_plan.py
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_api/snapshot_job.py
+-rw-r--r--   0 root         (0) root         (0)     5479 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_api/snapshot_partition.py
+-rw-r--r--   0 root         (0) root         (0)     1668 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_api/snapshot_repository.py
+-rw-r--r--   0 root         (0) root         (0)     2727 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_api/snapshot_schedule.py
+-rw-r--r--   0 root         (0) root         (0)     2901 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_api/snapshot_sensor.py
+-rw-r--r--   0 root         (0) root         (0)      478 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_builtins.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:21:09.024563 dagster-1.3.9rc0/dagster/_check/
+-rw-r--r--   0 root         (0) root         (0)     1352 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_check/README.md
+-rw-r--r--   0 root         (0) root         (0)    51637 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_check/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:21:09.028563 dagster-1.3.9rc0/dagster/_cli/
+-rw-r--r--   0 root         (0) root         (0)     1182 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    26292 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_cli/api.py
+-rw-r--r--   0 root         (0) root         (0)     8263 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_cli/asset.py
+-rw-r--r--   0 root         (0) root         (0)     7730 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_cli/code_server.py
+-rw-r--r--   0 root         (0) root         (0)     2300 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_cli/config_scaffolder.py
+-rw-r--r--   0 root         (0) root         (0)     3540 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_cli/debug.py
+-rw-r--r--   0 root         (0) root         (0)     5867 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_cli/dev.py
+-rw-r--r--   0 root         (0) root         (0)     4154 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_cli/instance.py
+-rw-r--r--   0 root         (0) root         (0)    29907 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_cli/job.py
+-rw-r--r--   0 root         (0) root         (0)     1695 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_cli/load_handle.py
+-rw-r--r--   0 root         (0) root         (0)     5852 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_cli/project.py
+-rw-r--r--   0 root         (0) root         (0)     5129 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_cli/run.py
+-rw-r--r--   0 root         (0) root         (0)    19958 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_cli/schedule.py
+-rw-r--r--   0 root         (0) root         (0)    15707 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_cli/sensor.py
+-rw-r--r--   0 root         (0) root         (0)     4259 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_cli/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:21:09.028563 dagster-1.3.9rc0/dagster/_cli/workspace/
+-rw-r--r--   0 root         (0) root         (0)      180 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_cli/workspace/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    28391 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_cli/workspace/cli_target.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:21:09.028563 dagster-1.3.9rc0/dagster/_config/
+-rw-r--r--   0 root         (0) root         (0)     3186 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3403 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_config/config_schema.py
+-rw-r--r--   0 root         (0) root         (0)    15864 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_config/config_type.py
+-rw-r--r--   0 root         (0) root         (0)    19601 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_config/errors.py
+-rw-r--r--   0 root         (0) root         (0)     1783 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_config/evaluate_value_result.py
+-rw-r--r--   0 root         (0) root         (0)    15269 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_config/field.py
+-rw-r--r--   0 root         (0) root         (0)    16880 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_config/field_utils.py
+-rw-r--r--   0 root         (0) root         (0)     9466 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_config/post_process.py
+-rw-r--r--   0 root         (0) root         (0)      855 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_config/primitive_mapping.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:21:09.028563 dagster-1.3.9rc0/dagster/_config/pythonic_config/
+-rw-r--r--   0 root         (0) root         (0)    71995 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_config/pythonic_config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1644 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_config/pythonic_config/attach_other_object_to_context.py
+-rw-r--r--   0 root         (0) root         (0)     7261 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_config/pythonic_config/typing_utils.py
+-rw-r--r--   0 root         (0) root         (0)      577 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_config/pythonic_config/utils.py
+-rw-r--r--   0 root         (0) root         (0)    12143 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_config/snap.py
+-rw-r--r--   0 root         (0) root         (0)     3267 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_config/source.py
+-rw-r--r--   0 root         (0) root         (0)     3528 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_config/stack.py
+-rw-r--r--   0 root         (0) root         (0)     7772 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_config/traversal_context.py
+-rw-r--r--   0 root         (0) root         (0)     4167 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_config/type_printer.py
+-rw-r--r--   0 root         (0) root         (0)    17162 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_config/validate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:21:09.032563 dagster-1.3.9rc0/dagster/_core/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      994 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/assets.py
+-rw-r--r--   0 root         (0) root         (0)    13645 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/code_pointer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:21:09.032563 dagster-1.3.9rc0/dagster/_core/container_context/
+-rw-r--r--   0 root         (0) root         (0)      184 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/container_context/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1277 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/container_context/config.py
+-rw-r--r--   0 root         (0) root         (0)     2310 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/debug.py
+-rw-r--r--   0 root         (0) root         (0)     3005 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/decorator_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:21:09.040563 dagster-1.3.9rc0/dagster/_core/definitions/
+-rw-r--r--   0 root         (0) root         (0)     7626 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/definitions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    30543 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/definitions/asset_graph.py
+-rw-r--r--   0 root         (0) root         (0)    10704 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/definitions/asset_graph_subset.py
+-rw-r--r--   0 root         (0) root         (0)     3816 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/definitions/asset_in.py
+-rw-r--r--   0 root         (0) root         (0)    37134 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/definitions/asset_layer.py
+-rw-r--r--   0 root         (0) root         (0)     5685 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/definitions/asset_out.py
+-rw-r--r--   0 root         (0) root         (0)    59306 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/definitions/asset_reconciliation_sensor.py
+-rw-r--r--   0 root         (0) root         (0)    18474 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/definitions/asset_selection.py
+-rw-r--r--   0 root         (0) root         (0)     7164 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/definitions/asset_sensor_definition.py
+-rw-r--r--   0 root         (0) root         (0)    63783 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/definitions/assets.py
+-rw-r--r--   0 root         (0) root         (0)    24376 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/definitions/assets_job.py
+-rw-r--r--   0 root         (0) root         (0)     2806 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/definitions/auto_materialize_condition.py
+-rw-r--r--   0 root         (0) root         (0)     5297 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/definitions/auto_materialize_policy.py
+-rw-r--r--   0 root         (0) root         (0)    16105 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/definitions/cacheable_assets.py
+-rw-r--r--   0 root         (0) root         (0)    45671 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/definitions/composition.py
+-rw-r--r--   0 root         (0) root         (0)     4287 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/definitions/config.py
+-rw-r--r--   0 root         (0) root         (0)    10845 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/definitions/configurable.py
+-rw-r--r--   0 root         (0) root         (0)    20795 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/definitions/data_time.py
+-rw-r--r--   0 root         (0) root         (0)    18695 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/definitions/data_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:21:09.044564 dagster-1.3.9rc0/dagster/_core/definitions/decorators/
+-rw-r--r--   0 root         (0) root         (0)      620 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/definitions/decorators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    44389 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/definitions/decorators/asset_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     4915 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/definitions/decorators/config_mapping_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     8250 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/definitions/decorators/graph_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     9444 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/definitions/decorators/hook_decorator.py
+-rw-r--r--   0 root         (0) root         (0)    10676 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/definitions/decorators/job_decorator.py
+-rw-r--r--   0 root         (0) root         (0)    17845 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/definitions/decorators/op_decorator.py
+-rw-r--r--   0 root         (0) root         (0)    14396 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/definitions/decorators/repository_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     8656 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/definitions/decorators/schedule_decorator.py
+-rw-r--r--   0 root         (0) root         (0)    11936 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/definitions/decorators/sensor_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     7085 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/definitions/decorators/source_asset_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     5275 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/definitions/definition_config_schema.py
+-rw-r--r--   0 root         (0) root         (0)    21205 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/definitions/definitions_class.py
+-rw-r--r--   0 root         (0) root         (0)    39988 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/definitions/dependency.py
+-rw-r--r--   0 root         (0) root         (0)    31576 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/definitions/events.py
+-rw-r--r--   0 root         (0) root         (0)    21013 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/definitions/executor_definition.py
+-rw-r--r--   0 root         (0) root         (0)    10548 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/definitions/external_asset_graph.py
+-rw-r--r--   0 root         (0) root         (0)     8010 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/definitions/freshness_policy.py
+-rw-r--r--   0 root         (0) root         (0)    16195 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/definitions/freshness_policy_sensor_definition.py
+-rw-r--r--   0 root         (0) root         (0)    44740 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/definitions/graph_definition.py
+-rw-r--r--   0 root         (0) root         (0)     6546 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/definitions/hook_definition.py
+-rw-r--r--   0 root         (0) root         (0)     1515 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/definitions/hook_invocation.py
+-rw-r--r--   0 root         (0) root         (0)     3205 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/definitions/inference.py
+-rw-r--r--   0 root         (0) root         (0)    22898 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/definitions/input.py
+-rw-r--r--   0 root         (0) root         (0)     5386 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/definitions/instigation_logger.py
+-rw-r--r--   0 root         (0) root         (0)     2152 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/definitions/job_base.py
+-rw-r--r--   0 root         (0) root         (0)    51157 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/definitions/job_definition.py
+-rw-r--r--   0 root         (0) root         (0)    20308 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/definitions/load_assets_from_modules.py
+-rw-r--r--   0 root         (0) root         (0)     6845 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/definitions/logger_definition.py
+-rw-r--r--   0 root         (0) root         (0)      636 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/definitions/logger_invocation.py
+-rw-r--r--   0 root         (0) root         (0)     8841 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/definitions/materialize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:21:09.044564 dagster-1.3.9rc0/dagster/_core/definitions/metadata/
+-rw-r--r--   0 root         (0) root         (0)    32319 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/definitions/metadata/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8557 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/definitions/metadata/table.py
+-rw-r--r--   0 root         (0) root         (0)    56090 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/definitions/multi_asset_sensor_definition.py
+-rw-r--r--   0 root         (0) root         (0)    20153 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/definitions/multi_dimensional_partitions.py
+-rw-r--r--   0 root         (0) root         (0)       82 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/definitions/no_step_launcher.py
+-rw-r--r--   0 root         (0) root         (0)    11927 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/definitions/node_container.py
+-rw-r--r--   0 root         (0) root         (0)     8041 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/definitions/node_definition.py
+-rw-r--r--   0 root         (0) root         (0)     2867 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/definitions/observe.py
+-rw-r--r--   0 root         (0) root         (0)    22119 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/definitions/op_definition.py
+-rw-r--r--   0 root         (0) root         (0)    19256 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/definitions/op_invocation.py
+-rw-r--r--   0 root         (0) root         (0)     7509 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/definitions/op_selection.py
+-rw-r--r--   0 root         (0) root         (0)    18908 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/definitions/output.py
+-rw-r--r--   0 root         (0) root         (0)    39191 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/definitions/partition.py
+-rw-r--r--   0 root         (0) root         (0)      196 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/definitions/partition_key_range.py
+-rw-r--r--   0 root         (0) root         (0)    47274 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/definitions/partition_mapping.py
+-rw-r--r--   0 root         (0) root         (0)     8902 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/definitions/partitioned_schedule.py
+-rw-r--r--   0 root         (0) root         (0)     3779 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/definitions/policy.py
+-rw-r--r--   0 root         (0) root         (0)    27231 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/definitions/reconstruct.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:21:09.044564 dagster-1.3.9rc0/dagster/_core/definitions/repository_definition/
+-rw-r--r--   0 root         (0) root         (0)      654 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/definitions/repository_definition/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6670 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/definitions/repository_definition/caching_index.py
+-rw-r--r--   0 root         (0) root         (0)    18860 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/definitions/repository_definition/repository_data.py
+-rw-r--r--   0 root         (0) root         (0)    17401 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/definitions/repository_definition/repository_data_builder.py
+-rw-r--r--   0 root         (0) root         (0)    16917 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/definitions/repository_definition/repository_definition.py
+-rw-r--r--   0 root         (0) root         (0)     1479 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/definitions/repository_definition/valid_definitions.py
+-rw-r--r--   0 root         (0) root         (0)     5108 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/definitions/resolved_asset_deps.py
+-rw-r--r--   0 root         (0) root         (0)     1336 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/definitions/resource_annotation.py
+-rw-r--r--   0 root         (0) root         (0)    16162 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/definitions/resource_definition.py
+-rw-r--r--   0 root         (0) root         (0)     5398 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/definitions/resource_invocation.py
+-rw-r--r--   0 root         (0) root         (0)     7806 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/definitions/resource_requirement.py
+-rw-r--r--   0 root         (0) root         (0)    24105 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/definitions/run_config.py
+-rw-r--r--   0 root         (0) root         (0)     1445 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/definitions/run_config_schema.py
+-rw-r--r--   0 root         (0) root         (0)    15824 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/definitions/run_request.py
+-rw-r--r--   0 root         (0) root         (0)    38400 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/definitions/run_status_sensor_definition.py
+-rw-r--r--   0 root         (0) root         (0)    37556 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/definitions/schedule_definition.py
+-rw-r--r--   0 root         (0) root         (0)     5189 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/definitions/scoped_resources_builder.py
+-rw-r--r--   0 root         (0) root         (0)    10837 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/definitions/selector.py
+-rw-r--r--   0 root         (0) root         (0)    47376 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/definitions/sensor_definition.py
+-rw-r--r--   0 root         (0) root         (0)    15391 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/definitions/source_asset.py
+-rw-r--r--   0 root         (0) root         (0)     2298 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/definitions/step_launcher.py
+-rw-r--r--   0 root         (0) root         (0)     1535 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/definitions/target.py
+-rw-r--r--   0 root         (0) root         (0)      473 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/definitions/test_op_definition.py
+-rw-r--r--   0 root         (0) root         (0)    12374 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/definitions/time_window_partition_mapping.py
+-rw-r--r--   0 root         (0) root         (0)    78072 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/definitions/time_window_partitions.py
+-rw-r--r--   0 root         (0) root         (0)    16744 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/definitions/unresolved_asset_job_definition.py
+-rw-r--r--   0 root         (0) root         (0)     7992 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/definitions/utils.py
+-rw-r--r--   0 root         (0) root         (0)     2930 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/definitions/version_strategy.py
+-rw-r--r--   0 root         (0) root         (0)    26237 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/errors.py
+-rw-r--r--   0 root         (0) root         (0)     6241 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/event_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:21:09.044564 dagster-1.3.9rc0/dagster/_core/events/
+-rw-r--r--   0 root         (0) root         (0)    64981 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/events/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7783 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/events/log.py
+-rw-r--r--   0 root         (0) root         (0)     1614 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/events/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:21:09.048564 dagster-1.3.9rc0/dagster/_core/execution/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/execution/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    38315 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/execution/api.py
+-rw-r--r--   0 root         (0) root         (0)    36589 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/execution/asset_backfill.py
+-rw-r--r--   0 root         (0) root         (0)    14710 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/execution/backfill.py
+-rw-r--r--   0 root         (0) root         (0)     6487 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/execution/build_resources.py
+-rw-r--r--   0 root         (0) root         (0)      224 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/execution/bulk_actions.py
+-rw-r--r--   0 root         (0) root         (0)     5587 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/execution/compute_logs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:21:09.048564 dagster-1.3.9rc0/dagster/_core/execution/context/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/execution/context/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21992 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/execution/context/compute.py
+-rw-r--r--   0 root         (0) root         (0)    15991 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/execution/context/hook.py
+-rw-r--r--   0 root         (0) root         (0)     9369 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/execution/context/init.py
+-rw-r--r--   0 root         (0) root         (0)    26845 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/execution/context/input.py
+-rw-r--r--   0 root         (0) root         (0)    27349 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/execution/context/invocation.py
+-rw-r--r--   0 root         (0) root         (0)     3164 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/execution/context/logger.py
+-rw-r--r--   0 root         (0) root         (0)    33974 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/execution/context/output.py
+-rw-r--r--   0 root         (0) root         (0)    44193 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/execution/context/system.py
+-rw-r--r--   0 root         (0) root         (0)    18501 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/execution/context_creation_job.py
+-rw-r--r--   0 root         (0) root         (0)     5149 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/execution/execute_in_process.py
+-rw-r--r--   0 root         (0) root         (0)     5426 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/execution/execute_in_process_result.py
+-rw-r--r--   0 root         (0) root         (0)     9183 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/execution/execution_result.py
+-rw-r--r--   0 root         (0) root         (0)     8544 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/execution/host_mode.py
+-rw-r--r--   0 root         (0) root         (0)    14451 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/execution/job_backfill.py
+-rw-r--r--   0 root         (0) root         (0)     6487 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/execution/job_execution_result.py
+-rw-r--r--   0 root         (0) root         (0)      998 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/execution/memoization.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:21:09.052564 dagster-1.3.9rc0/dagster/_core/execution/plan/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/execution/plan/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25252 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/execution/plan/active.py
+-rw-r--r--   0 root         (0) root         (0)     7279 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/execution/plan/compute.py
+-rw-r--r--   0 root         (0) root         (0)    12550 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/execution/plan/compute_generator.py
+-rw-r--r--   0 root         (0) root         (0)    16658 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/execution/plan/execute_plan.py
+-rw-r--r--   0 root         (0) root         (0)    27355 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/execution/plan/execute_step.py
+-rw-r--r--   0 root         (0) root         (0)    10000 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/execution/plan/external_step.py
+-rw-r--r--   0 root         (0) root         (0)     3664 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/execution/plan/handle.py
+-rw-r--r--   0 root         (0) root         (0)    37831 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/execution/plan/inputs.py
+-rw-r--r--   0 root         (0) root         (0)     4352 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/execution/plan/instance_concurrency_context.py
+-rw-r--r--   0 root         (0) root         (0)     1159 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/execution/plan/local_external_step_main.py
+-rw-r--r--   0 root         (0) root         (0)     5395 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/execution/plan/objects.py
+-rw-r--r--   0 root         (0) root         (0)     7057 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/execution/plan/outputs.py
+-rw-r--r--   0 root         (0) root         (0)    58041 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/execution/plan/plan.py
+-rw-r--r--   0 root         (0) root         (0)      114 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/execution/plan/resume_retry.py
+-rw-r--r--   0 root         (0) root         (0)    15616 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/execution/plan/state.py
+-rw-r--r--   0 root         (0) root         (0)    15920 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/execution/plan/step.py
+-rw-r--r--   0 root         (0) root         (0)     3796 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/execution/plan/utils.py
+-rw-r--r--   0 root         (0) root         (0)     1762 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/execution/poll_compute_logs.py
+-rw-r--r--   0 root         (0) root         (0)     8186 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/execution/resolve_versions.py
+-rw-r--r--   0 root         (0) root         (0)    19280 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/execution/resources_init.py
+-rw-r--r--   0 root         (0) root         (0)     2104 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/execution/retries.py
+-rw-r--r--   0 root         (0) root         (0)     1651 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/execution/run_cancellation_thread.py
+-rw-r--r--   0 root         (0) root         (0)    10329 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/execution/stats.py
+-rw-r--r--   0 root         (0) root         (0)     1125 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/execution/tags.py
+-rw-r--r--   0 root         (0) root         (0)     1172 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/execution/validate_run_config.py
+-rw-r--r--   0 root         (0) root         (0)     1282 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/execution/watch_orphans.py
+-rw-r--r--   0 root         (0) root         (0)     4233 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/execution/with_resources.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:21:09.052564 dagster-1.3.9rc0/dagster/_core/executor/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/executor/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1265 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/executor/base.py
+-rw-r--r--   0 root         (0) root         (0)     5990 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/executor/child_process_executor.py
+-rw-r--r--   0 root         (0) root         (0)     3431 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/executor/in_process.py
+-rw-r--r--   0 root         (0) root         (0)     1509 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/executor/init.py
+-rw-r--r--   0 root         (0) root         (0)    15592 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/executor/multiprocess.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:21:09.052564 dagster-1.3.9rc0/dagster/_core/executor/step_delegating/
+-rw-r--r--   0 root         (0) root         (0)      247 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/executor/step_delegating/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15580 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/executor/step_delegating/step_delegating_executor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:21:09.052564 dagster-1.3.9rc0/dagster/_core/executor/step_delegating/step_handler/
+-rw-r--r--   0 root         (0) root         (0)      152 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/executor/step_delegating/step_handler/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3078 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/executor/step_delegating/step_handler/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:21:09.052564 dagster-1.3.9rc0/dagster/_core/host_representation/
+-rw-r--r--   0 root         (0) root         (0)     2789 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/host_representation/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    33518 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/host_representation/code_location.py
+-rw-r--r--   0 root         (0) root         (0)    32089 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/host_representation/external.py
+-rw-r--r--   0 root         (0) root         (0)    70934 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/host_representation/external_data.py
+-rw-r--r--   0 root         (0) root         (0)    12517 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/host_representation/grpc_server_registry.py
+-rw-r--r--   0 root         (0) root         (0)     1487 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/host_representation/grpc_server_state_subscriber.py
+-rw-r--r--   0 root         (0) root         (0)     4333 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/host_representation/handle.py
+-rw-r--r--   0 root         (0) root         (0)     1581 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/host_representation/historical.py
+-rw-r--r--   0 root         (0) root         (0)     4850 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/host_representation/job_index.py
+-rw-r--r--   0 root         (0) root         (0)    19051 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/host_representation/origin.py
+-rw-r--r--   0 root         (0) root         (0)     3610 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/host_representation/represented.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:21:09.052564 dagster-1.3.9rc0/dagster/_core/instance/
+-rw-r--r--   0 root         (0) root         (0)   104144 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/instance/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12956 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/instance/config.py
+-rw-r--r--   0 root         (0) root         (0)    24084 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/instance/ref.py
+-rw-r--r--   0 root         (0) root         (0)     3899 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/instance_for_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:21:09.056564 dagster-1.3.9rc0/dagster/_core/launcher/
+-rw-r--r--   0 root         (0) root         (0)      297 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/launcher/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3758 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/launcher/base.py
+-rw-r--r--   0 root         (0) root         (0)     6808 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/launcher/default_run_launcher.py
+-rw-r--r--   0 root         (0) root         (0)     1586 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/launcher/sync_in_memory_run_launcher.py
+-rw-r--r--   0 root         (0) root         (0)      473 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/libraries.py
+-rw-r--r--   0 root         (0) root         (0)    17249 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/log_manager.py
+-rw-r--r--   0 root         (0) root         (0)     1029 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/nux.py
+-rw-r--r--   0 root         (0) root         (0)     3691 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/origin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:21:09.056564 dagster-1.3.9rc0/dagster/_core/run_coordinator/
+-rw-r--r--   0 root         (0) root         (0)      267 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/run_coordinator/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2005 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/run_coordinator/base.py
+-rw-r--r--   0 root         (0) root         (0)     1922 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/run_coordinator/default_run_coordinator.py
+-rw-r--r--   0 root         (0) root         (0)    11030 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/run_coordinator/queued_run_coordinator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:21:09.056564 dagster-1.3.9rc0/dagster/_core/scheduler/
+-rw-r--r--   0 root         (0) root         (0)      534 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/scheduler/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1241 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/scheduler/execution.py
+-rw-r--r--   0 root         (0) root         (0)    21903 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/scheduler/instigation.py
+-rw-r--r--   0 root         (0) root         (0)     9410 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/scheduler/scheduler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:21:09.056564 dagster-1.3.9rc0/dagster/_core/secrets/
+-rw-r--r--   0 root         (0) root         (0)       51 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/secrets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1811 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/secrets/env_file.py
+-rw-r--r--   0 root         (0) root         (0)      388 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/secrets/loader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:21:09.056564 dagster-1.3.9rc0/dagster/_core/selector/
+-rw-r--r--   0 root         (0) root         (0)      295 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/selector/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18247 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/selector/subset_selector.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:21:09.056564 dagster-1.3.9rc0/dagster/_core/snap/
+-rw-r--r--   0 root         (0) root         (0)     2815 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/snap/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      494 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/snap/config_types.py
+-rw-r--r--   0 root         (0) root         (0)     3999 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/snap/dagster_types.py
+-rw-r--r--   0 root         (0) root         (0)     9421 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/snap/dep_snapshot.py
+-rw-r--r--   0 root         (0) root         (0)    12099 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/snap/execution_plan_snapshot.py
+-rw-r--r--   0 root         (0) root         (0)    16654 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/snap/job_snapshot.py
+-rw-r--r--   0 root         (0) root         (0)     4495 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/snap/mode.py
+-rw-r--r--   0 root         (0) root         (0)    14452 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/snap/node.py
+-rw-r--r--   0 root         (0) root         (0)     1964 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/snap/snap_to_yaml.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:21:09.060564 dagster-1.3.9rc0/dagster/_core/storage/
+-rw-r--r--   0 root         (0) root         (0)     3057 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/DEVELOPING.md
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:21:09.060564 dagster-1.3.9rc0/dagster/_core/storage/alembic/
+-rw-r--r--   0 root         (0) root         (0)     6676 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/alembic/README.md
+-rw-r--r--   0 root         (0) root         (0)      687 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/alembic/env.py
+-rw-r--r--   0 root         (0) root         (0)      494 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/alembic/script.py.mako
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:21:09.072564 dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/
+-rw-r--r--   0 root         (0) root         (0)     3150 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/001_initial_1.py
+-rw-r--r--   0 root         (0) root         (0)      311 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/001_initial_schedule.py
+-rw-r--r--   0 root         (0) root         (0)     1485 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      598 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      972 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      972 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     2548 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/004_add_snapshots_to_run_storage.py
+-rw-r--r--   0 root         (0) root         (0)     1405 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/005_add_asset_key_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1405 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/005_add_asset_key_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1130 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/006_scheduler_update_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      952 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/007_create_run_id_idx_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      952 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/007_create_run_id_idx_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      955 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/008_add_run_tags_index_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      955 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/008_add_run_tags_index_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1170 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/009_add_partition_column_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1170 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/009_add_partition_column_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1729 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1729 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1146 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1124 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_1.py
+-rw-r--r--   0 root         (0) root         (0)     1142 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_2.py
+-rw-r--r--   0 root         (0) root         (0)      416 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/012_0_10_0_create_new_run_tables_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      416 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/012_0_10_0_create_new_run_tables_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      434 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/013_0_10_0_create_new_event_log_tables_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      434 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/013_0_10_0_create_new_event_log_tables_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      431 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/014_0_10_0_create_new_schedule_tables_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      431 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/014_0_10_0_create_new_schedule_tables_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     3926 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     3926 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      408 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/016_add_bulk_actions_table_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      408 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/016_add_bulk_actions_table_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      935 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/017_add_run_status_index_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      935 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/017_add_run_status_index_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      325 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/017_initial_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      420 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/018_add_asset_tags_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      420 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/018_add_asset_tags_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      420 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/018_add_asset_tags_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1569 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1569 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      409 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/020_add_column_asset_body_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      409 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/020_add_column_asset_body_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      409 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/020_add_column_asset_body_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1033 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/021_add_column_mode_mysql.py
+-rw-r--r--   0 root         (0) root         (0)     1031 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/021_add_column_mode_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1033 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/021_add_column_mode_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      432 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      432 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      432 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      420 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      420 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      420 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      530 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_mysql.py
+-rw-r--r--   0 root         (0) root         (0)     1274 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1274 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      403 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/025_add_range_index_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      403 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/025_add_range_index_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      403 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/025_add_range_index_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      634 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/026_convert_start_end_times_format_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      433 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/027_add_migration_table_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      433 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/027_add_migration_table_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      433 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/027_add_migration_table_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      409 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/028_add_instigators_table_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      409 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/028_add_instigators_table_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      409 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/028_add_instigators_table_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      415 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      415 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      415 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1892 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/030_add_columns_action_type_and_selector_id_.py
+-rw-r--r--   0 root         (0) root         (0)      957 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/031_add_kvs_table.py
+-rw-r--r--   0 root         (0) root         (0)      498 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/032_rebuild_event_indexes.py
+-rw-r--r--   0 root         (0) root         (0)     1950 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/033_add_asset_event_tags_table.py
+-rw-r--r--   0 root         (0) root         (0)      428 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/034_add_cached_status_data_column.py
+-rw-r--r--   0 root         (0) root         (0)      426 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/035_add_run_job_index.py
+-rw-r--r--   0 root         (0) root         (0)     1536 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/036_add_dynamic_partitions_table.py
+-rw-r--r--   0 root         (0) root         (0)     2480 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/037_d9092588866f_add_primary_key_cols.py
+-rw-r--r--   0 root         (0) root         (0)     1176 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/038_701913684cb4_add_postgres_pks.py
+-rw-r--r--   0 root         (0) root         (0)     2062 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/039_d3a4c9e87af3_add_asset_daemon_asset_evaluations_table.py
+-rw-r--r--   0 root         (0) root         (0)     2358 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/040_add_in_progress_step_table.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7204 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/asset_value_loader.py
+-rw-r--r--   0 root         (0) root         (0)     1215 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/base_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:21:09.072564 dagster-1.3.9rc0/dagster/_core/storage/branching/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/branching/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4304 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/branching/branching_io_manager.py
+-rw-r--r--   0 root         (0) root         (0)     8736 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/captured_log_manager.py
+-rw-r--r--   0 root         (0) root         (0)    16247 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/cloud_storage_compute_log_manager.py
+-rw-r--r--   0 root         (0) root         (0)     9545 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/compute_log_manager.py
+-rw-r--r--   0 root         (0) root         (0)     1863 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/config.py
+-rw-r--r--   0 root         (0) root         (0)      417 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/daemon_cursor.py
+-rw-r--r--   0 root         (0) root         (0)    24055 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/dagster_run.py
+-rw-r--r--   0 root         (0) root         (0)    11640 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/db_io_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:21:09.072564 dagster-1.3.9rc0/dagster/_core/storage/event_log/
+-rw-r--r--   0 root         (0) root         (0)      742 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/event_log/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16268 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/event_log/base.py
+-rw-r--r--   0 root         (0) root         (0)     3753 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/event_log/in_memory.py
+-rw-r--r--   0 root         (0) root         (0)     7273 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/event_log/migration.py
+-rw-r--r--   0 root         (0) root         (0)     7911 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/event_log/polling_event_watcher.py
+-rw-r--r--   0 root         (0) root         (0)     6408 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/event_log/schema.py
+-rw-r--r--   0 root         (0) root         (0)   100680 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/event_log/sql_event_log.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:21:09.076564 dagster-1.3.9rc0/dagster/_core/storage/event_log/sqlite/
+-rw-r--r--   0 root         (0) root         (0)      200 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/event_log/sqlite/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:21:09.076564 dagster-1.3.9rc0/dagster/_core/storage/event_log/sqlite/alembic/
+-rw-r--r--   0 root         (0) root         (0)     1040 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/event_log/sqlite/alembic/alembic.ini
+-rw-r--r--   0 root         (0) root         (0)     7526 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/event_log/sqlite/consolidated_sqlite_event_log.py
+-rw-r--r--   0 root         (0) root         (0)    19093 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/event_log/sqlite/sqlite_event_log.py
+-rw-r--r--   0 root         (0) root         (0)    10912 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/file_manager.py
+-rw-r--r--   0 root         (0) root         (0)    13217 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/fs_io_manager.py
+-rw-r--r--   0 root         (0) root         (0)     8915 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/input_manager.py
+-rw-r--r--   0 root         (0) root         (0)    10638 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/io_manager.py
+-rw-r--r--   0 root         (0) root         (0)    28589 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/legacy_storage.py
+-rw-r--r--   0 root         (0) root         (0)    17301 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/local_compute_log_manager.py
+-rw-r--r--   0 root         (0) root         (0)      876 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/mem_io_manager.py
+-rw-r--r--   0 root         (0) root         (0)     4293 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/memoizable_io_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:21:09.076564 dagster-1.3.9rc0/dagster/_core/storage/migration/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/migration/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14469 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/migration/utils.py
+-rw-r--r--   0 root         (0) root         (0)     3186 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/noop_compute_log_manager.py
+-rw-r--r--   0 root         (0) root         (0)     2361 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/output_manager.py
+-rw-r--r--   0 root         (0) root         (0)    23189 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/partition_status_cache.py
+-rw-r--r--   0 root         (0) root         (0)     2121 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/root.py
+-rw-r--r--   0 root         (0) root         (0)     8509 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/root_input_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:21:09.076564 dagster-1.3.9rc0/dagster/_core/storage/runs/
+-rw-r--r--   0 root         (0) root         (0)      386 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/runs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15454 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/runs/base.py
+-rw-r--r--   0 root         (0) root         (0)     2416 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/runs/in_memory.py
+-rw-r--r--   0 root         (0) root         (0)     8697 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/runs/migration.py
+-rw-r--r--   0 root         (0) root         (0)     5982 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/runs/schema.py
+-rw-r--r--   0 root         (0) root         (0)    46286 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/runs/sql_run_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:21:09.076564 dagster-1.3.9rc0/dagster/_core/storage/runs/sqlite/
+-rw-r--r--   0 root         (0) root         (0)       69 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/runs/sqlite/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:21:09.076564 dagster-1.3.9rc0/dagster/_core/storage/runs/sqlite/alembic/
+-rw-r--r--   0 root         (0) root         (0)     1040 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/runs/sqlite/alembic/alembic.ini
+-rw-r--r--   0 root         (0) root         (0)     6818 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/runs/sqlite/sqlite_run_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:21:09.076564 dagster-1.3.9rc0/dagster/_core/storage/schedules/
+-rw-r--r--   0 root         (0) root         (0)      272 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/schedules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6358 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/schedules/base.py
+-rw-r--r--   0 root         (0) root         (0)     4133 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/schedules/migration.py
+-rw-r--r--   0 root         (0) root         (0)     3710 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/schedules/schema.py
+-rw-r--r--   0 root         (0) root         (0)    22626 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/schedules/sql_schedule_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:21:09.076564 dagster-1.3.9rc0/dagster/_core/storage/schedules/sqlite/
+-rw-r--r--   0 root         (0) root         (0)       84 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/schedules/sqlite/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:21:09.076564 dagster-1.3.9rc0/dagster/_core/storage/schedules/sqlite/alembic/
+-rw-r--r--   0 root         (0) root         (0)     1039 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/schedules/sqlite/alembic/alembic.ini
+-rw-r--r--   0 root         (0) root         (0)     3684 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/schedules/sqlite/sqlite_schedule_storage.py
+-rw-r--r--   0 root         (0) root         (0)     7210 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/sql.py
+-rw-r--r--   0 root         (0) root         (0)     1391 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/sqlalchemy_compat.py
+-rw-r--r--   0 root         (0) root         (0)      926 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     4863 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/sqlite_storage.py
+-rw-r--r--   0 root         (0) root         (0)     3199 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/tags.py
+-rw-r--r--   0 root         (0) root         (0)     1128 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/temp_file_manager.py
+-rw-r--r--   0 root         (0) root         (0)    11346 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/storage/upath_io_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:21:09.076564 dagster-1.3.9rc0/dagster/_core/system_config/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/system_config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13981 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/system_config/composite_descent.py
+-rw-r--r--   0 root         (0) root         (0)    14855 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/system_config/objects.py
+-rw-r--r--   0 root         (0) root         (0)    27932 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/telemetry.py
+-rw-r--r--   0 root         (0) root         (0)     4824 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/telemetry_upload.py
+-rw-r--r--   0 root         (0) root         (0)    18936 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:21:09.080564 dagster-1.3.9rc0/dagster/_core/types/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/types/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3163 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/types/builtin_config_schemas.py
+-rw-r--r--   0 root         (0) root         (0)     7298 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/types/config_schema.py
+-rw-r--r--   0 root         (0) root         (0)    35761 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/types/dagster_type.py
+-rw-r--r--   0 root         (0) root         (0)     3579 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/types/decorator.py
+-rw-r--r--   0 root         (0) root         (0)     1846 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/types/loadable_target_origin.py
+-rw-r--r--   0 root         (0) root         (0)     1027 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/types/primitive_mapping.py
+-rw-r--r--   0 root         (0) root         (0)     4881 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/types/python_dict.py
+-rw-r--r--   0 root         (0) root         (0)     2836 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/types/python_set.py
+-rw-r--r--   0 root         (0) root         (0)     3712 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/types/python_tuple.py
+-rw-r--r--   0 root         (0) root         (0)     1772 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/types/transform_typing.py
+-rw-r--r--   0 root         (0) root         (0)     1438 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/utility_ops.py
+-rw-r--r--   0 root         (0) root         (0)     4402 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:21:09.080564 dagster-1.3.9rc0/dagster/_core/workspace/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/workspace/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4722 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/workspace/autodiscovery.py
+-rw-r--r--   0 root         (0) root         (0)     3478 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/workspace/config_schema.py
+-rw-r--r--   0 root         (0) root         (0)    28195 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/workspace/context.py
+-rw-r--r--   0 root         (0) root         (0)    11881 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/workspace/load.py
+-rw-r--r--   0 root         (0) root         (0)     4684 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/workspace/load_target.py
+-rw-r--r--   0 root         (0) root         (0)     4099 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/workspace/permissions.py
+-rw-r--r--   0 root         (0) root         (0)     1912 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_core/workspace/workspace.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:21:09.080564 dagster-1.3.9rc0/dagster/_daemon/
+-rw-r--r--   0 root         (0) root         (0)     2015 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_daemon/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       30 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_daemon/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     6416 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_daemon/asset_daemon.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:21:09.080564 dagster-1.3.9rc0/dagster/_daemon/auto_run_reexecution/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_daemon/auto_run_reexecution/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6822 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_daemon/auto_run_reexecution/auto_run_reexecution.py
+-rw-r--r--   0 root         (0) root         (0)     9123 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_daemon/auto_run_reexecution/event_log_consumer.py
+-rw-r--r--   0 root         (0) root         (0)     2125 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_daemon/backfill.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:21:09.080564 dagster-1.3.9rc0/dagster/_daemon/cli/
+-rw-r--r--   0 root         (0) root         (0)     4447 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_daemon/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18221 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_daemon/controller.py
+-rw-r--r--   0 root         (0) root         (0)    10611 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_daemon/daemon.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:21:09.080564 dagster-1.3.9rc0/dagster/_daemon/monitoring/
+-rw-r--r--   0 root         (0) root         (0)      320 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_daemon/monitoring/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1792 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_daemon/monitoring/concurrency.py
+-rw-r--r--   0 root         (0) root         (0)    10036 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_daemon/monitoring/run_monitoring.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:21:09.080564 dagster-1.3.9rc0/dagster/_daemon/run_coordinator/
+-rw-r--r--   0 root         (0) root         (0)      100 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_daemon/run_coordinator/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16326 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_daemon/run_coordinator/queued_run_coordinator_daemon.py
+-rw-r--r--   0 root         (0) root         (0)    39892 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_daemon/sensor.py
+-rw-r--r--   0 root         (0) root         (0)     2860 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_daemon/types.py
+-rw-r--r--   0 root         (0) root         (0)     6639 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_daemon/workspace.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:21:09.080564 dagster-1.3.9rc0/dagster/_experimental/
+-rw-r--r--   0 root         (0) root         (0)      300 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_experimental/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:21:09.080564 dagster-1.3.9rc0/dagster/_generate/
+-rw-r--r--   0 root         (0) root         (0)      253 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_generate/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2720 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_generate/download.py
+-rw-r--r--   0 root         (0) root         (0)     4805 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_generate/generate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:21:09.020563 dagster-1.3.9rc0/dagster/_generate/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:21:09.080564 dagster-1.3.9rc0/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:21:09.080564 dagster-1.3.9rc0/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/
+-rw-r--r--   0 root         (0) root         (0)      175 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/assets.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:21:09.080564 dagster-1.3.9rc0/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/test_assets.py.tmpl
+-rw-r--r--   0 root         (0) root         (0)      137 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/pyproject.toml.tmpl
+-rw-r--r--   0 root         (0) root         (0)       43 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/setup.cfg.tmpl
+-rw-r--r--   0 root         (0) root         (0)      285 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/setup.py.tmpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:21:09.084564 dagster-1.3.9rc0/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/
+-rw-r--r--   0 root         (0) root         (0)     1753 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:21:09.084564 dagster-1.3.9rc0/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:21:09.084564 dagster-1.3.9rc0/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/
+-rw-r--r--   0 root         (0) root         (0)       40 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/__init__.py.tmpl
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/assets.py
+-rw-r--r--   0 root         (0) root         (0)      164 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/repository.py.tmpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:21:09.084564 dagster-1.3.9rc0/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/test_assets.py.tmpl
+-rw-r--r--   0 root         (0) root         (0)       80 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       34 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/setup.cfg.tmpl
+-rw-r--r--   0 root         (0) root         (0)      267 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/setup.py.tmpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:21:09.084564 dagster-1.3.9rc0/dagster/_grpc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:21:09.084564 dagster-1.3.9rc0/dagster/_grpc/__generated__/
+-rw-r--r--   0 root         (0) root         (0)      178 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_grpc/__generated__/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    29251 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_grpc/__generated__/api_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    39700 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_grpc/__generated__/api_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     2051 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_grpc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       89 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_grpc/__main__.py
+-rw-r--r--   0 root         (0) root         (0)    18451 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_grpc/client.py
+-rw-r--r--   0 root         (0) root         (0)     4202 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_grpc/compile.py
+-rw-r--r--   0 root         (0) root         (0)    21967 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_grpc/impl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:21:09.084564 dagster-1.3.9rc0/dagster/_grpc/protos/
+-rw-r--r--   0 root         (0) root         (0)     5551 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_grpc/protos/api.proto
+-rw-r--r--   0 root         (0) root         (0)    12415 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_grpc/proxy_server.py
+-rw-r--r--   0 root         (0) root         (0)    51532 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_grpc/server.py
+-rw-r--r--   0 root         (0) root         (0)     5301 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_grpc/server_watcher.py
+-rw-r--r--   0 root         (0) root         (0)    26559 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_grpc/types.py
+-rw-r--r--   0 root         (0) root         (0)     2323 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_grpc/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:21:09.084564 dagster-1.3.9rc0/dagster/_legacy/
+-rw-r--r--   0 root         (0) root         (0)      222 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_legacy/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:21:09.084564 dagster-1.3.9rc0/dagster/_loggers/
+-rw-r--r--   0 root         (0) root         (0)     3781 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_loggers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3269 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_module_alias_map.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:21:09.088564 dagster-1.3.9rc0/dagster/_scheduler/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_scheduler/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    34396 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_scheduler/scheduler.py
+-rw-r--r--   0 root         (0) root         (0)     1361 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_scheduler/stale.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:21:09.088564 dagster-1.3.9rc0/dagster/_serdes/
+-rw-r--r--   0 root         (0) root         (0)      629 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_serdes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8004 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_serdes/config_class.py
+-rw-r--r--   0 root         (0) root         (0)      142 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_serdes/errors.py
+-rw-r--r--   0 root         (0) root         (0)     7467 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_serdes/ipc.py
+-rw-r--r--   0 root         (0) root         (0)    37613 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_serdes/serdes.py
+-rw-r--r--   0 root         (0) root         (0)      674 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_serdes/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:21:09.088564 dagster-1.3.9rc0/dagster/_seven/
+-rw-r--r--   0 root         (0) root         (0)     5496 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_seven/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      553 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_seven/abc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:21:09.088564 dagster-1.3.9rc0/dagster/_seven/compat/
+-rw-r--r--   0 root         (0) root         (0)      105 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_seven/compat/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1160 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_seven/compat/pendulum.py
+-rw-r--r--   0 root         (0) root         (0)      383 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_seven/json.py
+-rw-r--r--   0 root         (0) root         (0)      354 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_seven/temp_dir.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:21:09.088564 dagster-1.3.9rc0/dagster/_utils/
+-rw-r--r--   0 root         (0) root         (0)    23319 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8732 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_utils/alert.py
+-rw-r--r--   0 root         (0) root         (0)     6965 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_utils/backcompat.py
+-rw-r--r--   0 root         (0) root         (0)     2250 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_utils/backoff.py
+-rw-r--r--   0 root         (0) root         (0)     4116 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_utils/cached_method.py
+-rw-r--r--   0 root         (0) root         (0)    25123 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_utils/caching_instance_queryer.py
+-rw-r--r--   0 root         (0) root         (0)     3813 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_utils/concurrency.py
+-rw-r--r--   0 root         (0) root         (0)     2563 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_utils/dagster_type.py
+-rw-r--r--   0 root         (0) root         (0)      799 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_utils/env.py
+-rw-r--r--   0 root         (0) root         (0)     4094 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_utils/error.py
+-rw-r--r--   0 root         (0) root         (0)     1264 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_utils/external.py
+-rw-r--r--   0 root         (0) root         (0)      883 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_utils/forked_pdb.py
+-rw-r--r--   0 root         (0) root         (0)     2344 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_utils/hosted_user_process.py
+-rw-r--r--   0 root         (0) root         (0)     2796 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_utils/indenting_printer.py
+-rw-r--r--   0 root         (0) root         (0)      344 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_utils/internal_init.py
+-rw-r--r--   0 root         (0) root         (0)     3227 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_utils/interrupts.py
+-rw-r--r--   0 root         (0) root         (0)     9113 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_utils/log.py
+-rw-r--r--   0 root         (0) root         (0)     2313 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_utils/merger.py
+-rw-r--r--   0 root         (0) root         (0)     1507 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_utils/net.py
+-rw-r--r--   0 root         (0) root         (0)      208 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_utils/partitions.py
+-rw-r--r--   0 root         (0) root         (0)    12340 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_utils/schedules.py
+-rw-r--r--   0 root         (0) root         (0)     3289 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_utils/tags.py
+-rw-r--r--   0 root         (0) root         (0)     1820 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_utils/temp_file.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:21:09.092564 dagster-1.3.9rc0/dagster/_utils/test/
+-rw-r--r--   0 root         (0) root         (0)    12640 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_utils/test/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      119 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_utils/test/hello_world_defs.py
+-rw-r--r--   0 root         (0) root         (0)      214 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_utils/test/hello_world_repository.py
+-rw-r--r--   0 root         (0) root         (0)     8622 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_utils/test/mysql_instance.py
+-rw-r--r--   0 root         (0) root         (0)      256 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_utils/test/named_hello_world_repository.py
+-rw-r--r--   0 root         (0) root         (0)     9330 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_utils/test/postgres_instance.py
+-rw-r--r--   0 root         (0) root         (0)    28864 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_utils/test/schedule_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:21:09.092564 dagster-1.3.9rc0/dagster/_utils/test/toys/
+-rw-r--r--   0 root         (0) root         (0)       83 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_utils/test/toys/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       84 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_utils/test/toys/single_repository.py
+-rw-r--r--   0 root         (0) root         (0)     2004 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_utils/timing.py
+-rw-r--r--   0 root         (0) root         (0)      170 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_utils/types.py
+-rw-r--r--   0 root         (0) root         (0)     3334 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_utils/typing_api.py
+-rw-r--r--   0 root         (0) root         (0)     4915 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/_utils/yaml_utils.py
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/py.typed
+-rw-r--r--   0 root         (0) root         (0)       25 2023-06-08 18:20:45.000000 dagster-1.3.9rc0/dagster/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:21:09.024563 dagster-1.3.9rc0/dagster.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8793 2023-06-08 18:21:08.000000 dagster-1.3.9rc0/dagster.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    25431 2023-06-08 18:21:08.000000 dagster-1.3.9rc0/dagster.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 18:21:08.000000 dagster-1.3.9rc0/dagster.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       86 2023-06-08 18:21:08.000000 dagster-1.3.9rc0/dagster.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)     1443 2023-06-08 18:21:08.000000 dagster-1.3.9rc0/dagster.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-08 18:21:08.000000 dagster-1.3.9rc0/dagster.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      154 2023-06-08 18:21:09.092564 dagster-1.3.9rc0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     6820 2023-06-08 18:20:46.000000 dagster-1.3.9rc0/setup.py
```

### Comparing `dagster-1.3.9/COPYING` & `dagster-1.3.9rc0/COPYING`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/LICENSE` & `dagster-1.3.9rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/PKG-INFO` & `dagster-1.3.9rc0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster
-Version: 1.3.9
+Version: 1.3.9rc0
 Summary: The data orchestration platform built for productivity.
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Project-URL: Homepage, https://dagster.io
 Project-URL: GitHub, https://github.com/dagster-io/dagster
 Project-URL: Changelog, https://github.com/dagster-io/dagster/releases
```

### Comparing `dagster-1.3.9/README.md` & `dagster-1.3.9rc0/README.md`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/__init__.py` & `dagster-1.3.9rc0/dagster/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_annotations.py` & `dagster-1.3.9rc0/dagster/_annotations.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_api/get_server_id.py` & `dagster-1.3.9rc0/dagster/_api/get_server_id.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_api/list_repositories.py` & `dagster-1.3.9rc0/dagster/_api/list_repositories.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_api/notebook_data.py` & `dagster-1.3.9rc0/dagster/_api/notebook_data.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_api/snapshot_execution_plan.py` & `dagster-1.3.9rc0/dagster/_api/snapshot_execution_plan.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_api/snapshot_job.py` & `dagster-1.3.9rc0/dagster/_api/snapshot_job.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_api/snapshot_partition.py` & `dagster-1.3.9rc0/dagster/_api/snapshot_partition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_api/snapshot_repository.py` & `dagster-1.3.9rc0/dagster/_api/snapshot_repository.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_api/snapshot_schedule.py` & `dagster-1.3.9rc0/dagster/_api/snapshot_schedule.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_api/snapshot_sensor.py` & `dagster-1.3.9rc0/dagster/_api/snapshot_sensor.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_check/README.md` & `dagster-1.3.9rc0/dagster/_check/README.md`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_check/__init__.py` & `dagster-1.3.9rc0/dagster/_check/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_cli/__init__.py` & `dagster-1.3.9rc0/dagster/_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_cli/api.py` & `dagster-1.3.9rc0/dagster/_cli/api.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_cli/asset.py` & `dagster-1.3.9rc0/dagster/_cli/asset.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_cli/code_server.py` & `dagster-1.3.9rc0/dagster/_cli/code_server.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_cli/config_scaffolder.py` & `dagster-1.3.9rc0/dagster/_cli/config_scaffolder.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_cli/debug.py` & `dagster-1.3.9rc0/dagster/_cli/debug.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_cli/dev.py` & `dagster-1.3.9rc0/dagster/_cli/dev.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_cli/instance.py` & `dagster-1.3.9rc0/dagster/_cli/instance.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_cli/job.py` & `dagster-1.3.9rc0/dagster/_cli/job.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_cli/load_handle.py` & `dagster-1.3.9rc0/dagster/_cli/load_handle.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_cli/project.py` & `dagster-1.3.9rc0/dagster/_cli/project.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_cli/run.py` & `dagster-1.3.9rc0/dagster/_cli/run.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_cli/schedule.py` & `dagster-1.3.9rc0/dagster/_cli/schedule.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_cli/sensor.py` & `dagster-1.3.9rc0/dagster/_cli/sensor.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_cli/utils.py` & `dagster-1.3.9rc0/dagster/_cli/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_cli/workspace/cli_target.py` & `dagster-1.3.9rc0/dagster/_cli/workspace/cli_target.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_config/__init__.py` & `dagster-1.3.9rc0/dagster/_config/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_config/config_schema.py` & `dagster-1.3.9rc0/dagster/_config/config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_config/config_type.py` & `dagster-1.3.9rc0/dagster/_config/config_type.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_config/errors.py` & `dagster-1.3.9rc0/dagster/_config/errors.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_config/evaluate_value_result.py` & `dagster-1.3.9rc0/dagster/_config/evaluate_value_result.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_config/field.py` & `dagster-1.3.9rc0/dagster/_config/field.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_config/field_utils.py` & `dagster-1.3.9rc0/dagster/_config/field_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_config/post_process.py` & `dagster-1.3.9rc0/dagster/_config/post_process.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_config/primitive_mapping.py` & `dagster-1.3.9rc0/dagster/_config/primitive_mapping.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_config/pythonic_config/__init__.py` & `dagster-1.3.9rc0/dagster/_config/pythonic_config/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_config/pythonic_config/attach_other_object_to_context.py` & `dagster-1.3.9rc0/dagster/_config/pythonic_config/attach_other_object_to_context.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_config/pythonic_config/typing_utils.py` & `dagster-1.3.9rc0/dagster/_config/pythonic_config/typing_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_config/pythonic_config/utils.py` & `dagster-1.3.9rc0/dagster/_config/pythonic_config/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_config/snap.py` & `dagster-1.3.9rc0/dagster/_config/snap.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_config/source.py` & `dagster-1.3.9rc0/dagster/_config/source.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_config/stack.py` & `dagster-1.3.9rc0/dagster/_config/stack.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_config/traversal_context.py` & `dagster-1.3.9rc0/dagster/_config/traversal_context.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_config/type_printer.py` & `dagster-1.3.9rc0/dagster/_config/type_printer.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_config/validate.py` & `dagster-1.3.9rc0/dagster/_config/validate.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/assets.py` & `dagster-1.3.9rc0/dagster/_core/assets.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/code_pointer.py` & `dagster-1.3.9rc0/dagster/_core/code_pointer.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/container_context/config.py` & `dagster-1.3.9rc0/dagster/_core/container_context/config.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/debug.py` & `dagster-1.3.9rc0/dagster/_core/debug.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/decorator_utils.py` & `dagster-1.3.9rc0/dagster/_core/decorator_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/definitions/__init__.py` & `dagster-1.3.9rc0/dagster/_core/definitions/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/definitions/asset_graph.py` & `dagster-1.3.9rc0/dagster/_core/definitions/asset_graph.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/definitions/asset_graph_subset.py` & `dagster-1.3.9rc0/dagster/_core/definitions/asset_graph_subset.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/definitions/asset_in.py` & `dagster-1.3.9rc0/dagster/_core/definitions/asset_in.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/definitions/asset_layer.py` & `dagster-1.3.9rc0/dagster/_core/definitions/asset_layer.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/definitions/asset_out.py` & `dagster-1.3.9rc0/dagster/_core/definitions/asset_out.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/definitions/asset_reconciliation_sensor.py` & `dagster-1.3.9rc0/dagster/_core/definitions/asset_reconciliation_sensor.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/definitions/asset_selection.py` & `dagster-1.3.9rc0/dagster/_core/definitions/asset_selection.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/definitions/asset_sensor_definition.py` & `dagster-1.3.9rc0/dagster/_core/definitions/asset_sensor_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/definitions/assets.py` & `dagster-1.3.9rc0/dagster/_core/definitions/assets.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/definitions/assets_job.py` & `dagster-1.3.9rc0/dagster/_core/definitions/assets_job.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/definitions/auto_materialize_condition.py` & `dagster-1.3.9rc0/dagster/_core/definitions/auto_materialize_condition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/definitions/auto_materialize_policy.py` & `dagster-1.3.9rc0/dagster/_core/definitions/auto_materialize_policy.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/definitions/cacheable_assets.py` & `dagster-1.3.9rc0/dagster/_core/definitions/cacheable_assets.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/definitions/composition.py` & `dagster-1.3.9rc0/dagster/_core/definitions/composition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/definitions/config.py` & `dagster-1.3.9rc0/dagster/_core/definitions/config.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/definitions/configurable.py` & `dagster-1.3.9rc0/dagster/_core/definitions/configurable.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/definitions/data_time.py` & `dagster-1.3.9rc0/dagster/_core/definitions/data_time.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/definitions/data_version.py` & `dagster-1.3.9rc0/dagster/_core/definitions/data_version.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/definitions/decorators/__init__.py` & `dagster-1.3.9rc0/dagster/_core/definitions/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/definitions/decorators/asset_decorator.py` & `dagster-1.3.9rc0/dagster/_core/definitions/decorators/asset_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/definitions/decorators/config_mapping_decorator.py` & `dagster-1.3.9rc0/dagster/_core/definitions/decorators/config_mapping_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/definitions/decorators/graph_decorator.py` & `dagster-1.3.9rc0/dagster/_core/definitions/decorators/graph_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/definitions/decorators/hook_decorator.py` & `dagster-1.3.9rc0/dagster/_core/definitions/decorators/hook_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/definitions/decorators/job_decorator.py` & `dagster-1.3.9rc0/dagster/_core/definitions/decorators/job_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/definitions/decorators/op_decorator.py` & `dagster-1.3.9rc0/dagster/_core/definitions/decorators/op_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/definitions/decorators/repository_decorator.py` & `dagster-1.3.9rc0/dagster/_core/definitions/decorators/repository_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/definitions/decorators/schedule_decorator.py` & `dagster-1.3.9rc0/dagster/_core/definitions/decorators/schedule_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/definitions/decorators/sensor_decorator.py` & `dagster-1.3.9rc0/dagster/_core/definitions/decorators/sensor_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/definitions/decorators/source_asset_decorator.py` & `dagster-1.3.9rc0/dagster/_core/definitions/decorators/source_asset_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/definitions/definition_config_schema.py` & `dagster-1.3.9rc0/dagster/_core/definitions/definition_config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/definitions/definitions_class.py` & `dagster-1.3.9rc0/dagster/_core/definitions/definitions_class.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/definitions/dependency.py` & `dagster-1.3.9rc0/dagster/_core/definitions/dependency.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/definitions/events.py` & `dagster-1.3.9rc0/dagster/_core/definitions/events.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/definitions/executor_definition.py` & `dagster-1.3.9rc0/dagster/_core/definitions/executor_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/definitions/external_asset_graph.py` & `dagster-1.3.9rc0/dagster/_core/definitions/external_asset_graph.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/definitions/freshness_policy.py` & `dagster-1.3.9rc0/dagster/_core/definitions/freshness_policy.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/definitions/freshness_policy_sensor_definition.py` & `dagster-1.3.9rc0/dagster/_core/definitions/freshness_policy_sensor_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/definitions/graph_definition.py` & `dagster-1.3.9rc0/dagster/_core/definitions/graph_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/definitions/hook_definition.py` & `dagster-1.3.9rc0/dagster/_core/definitions/hook_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/definitions/hook_invocation.py` & `dagster-1.3.9rc0/dagster/_core/definitions/hook_invocation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/definitions/inference.py` & `dagster-1.3.9rc0/dagster/_core/definitions/inference.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/definitions/input.py` & `dagster-1.3.9rc0/dagster/_core/definitions/input.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/definitions/instigation_logger.py` & `dagster-1.3.9rc0/dagster/_core/definitions/instigation_logger.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/definitions/job_base.py` & `dagster-1.3.9rc0/dagster/_core/definitions/job_base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/definitions/job_definition.py` & `dagster-1.3.9rc0/dagster/_core/definitions/job_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/definitions/load_assets_from_modules.py` & `dagster-1.3.9rc0/dagster/_core/definitions/load_assets_from_modules.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/definitions/logger_definition.py` & `dagster-1.3.9rc0/dagster/_core/definitions/logger_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/definitions/logger_invocation.py` & `dagster-1.3.9rc0/dagster/_core/definitions/logger_invocation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/definitions/materialize.py` & `dagster-1.3.9rc0/dagster/_core/definitions/materialize.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/definitions/metadata/__init__.py` & `dagster-1.3.9rc0/dagster/_core/definitions/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/definitions/metadata/table.py` & `dagster-1.3.9rc0/dagster/_core/definitions/metadata/table.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/definitions/multi_asset_sensor_definition.py` & `dagster-1.3.9rc0/dagster/_core/definitions/multi_asset_sensor_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/definitions/multi_dimensional_partitions.py` & `dagster-1.3.9rc0/dagster/_core/definitions/multi_dimensional_partitions.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/definitions/node_container.py` & `dagster-1.3.9rc0/dagster/_core/definitions/node_container.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/definitions/node_definition.py` & `dagster-1.3.9rc0/dagster/_core/definitions/node_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/definitions/observe.py` & `dagster-1.3.9rc0/dagster/_core/definitions/observe.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/definitions/op_definition.py` & `dagster-1.3.9rc0/dagster/_core/definitions/op_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/definitions/op_invocation.py` & `dagster-1.3.9rc0/dagster/_core/definitions/op_invocation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/definitions/op_selection.py` & `dagster-1.3.9rc0/dagster/_core/definitions/op_selection.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/definitions/output.py` & `dagster-1.3.9rc0/dagster/_core/definitions/output.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/definitions/partition.py` & `dagster-1.3.9rc0/dagster/_core/definitions/partition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/definitions/partition_mapping.py` & `dagster-1.3.9rc0/dagster/_core/definitions/partition_mapping.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/definitions/partitioned_schedule.py` & `dagster-1.3.9rc0/dagster/_core/definitions/partitioned_schedule.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/definitions/policy.py` & `dagster-1.3.9rc0/dagster/_core/definitions/policy.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/definitions/reconstruct.py` & `dagster-1.3.9rc0/dagster/_core/definitions/reconstruct.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/definitions/repository_definition/__init__.py` & `dagster-1.3.9rc0/dagster/_core/definitions/repository_definition/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/definitions/repository_definition/caching_index.py` & `dagster-1.3.9rc0/dagster/_core/definitions/repository_definition/caching_index.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/definitions/repository_definition/repository_data.py` & `dagster-1.3.9rc0/dagster/_core/definitions/repository_definition/repository_data.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/definitions/repository_definition/repository_data_builder.py` & `dagster-1.3.9rc0/dagster/_core/definitions/repository_definition/repository_data_builder.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/definitions/repository_definition/repository_definition.py` & `dagster-1.3.9rc0/dagster/_core/definitions/repository_definition/repository_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/definitions/repository_definition/valid_definitions.py` & `dagster-1.3.9rc0/dagster/_core/definitions/repository_definition/valid_definitions.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/definitions/resolved_asset_deps.py` & `dagster-1.3.9rc0/dagster/_core/definitions/resolved_asset_deps.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/definitions/resource_annotation.py` & `dagster-1.3.9rc0/dagster/_core/definitions/resource_annotation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/definitions/resource_definition.py` & `dagster-1.3.9rc0/dagster/_core/definitions/resource_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/definitions/resource_invocation.py` & `dagster-1.3.9rc0/dagster/_core/definitions/resource_invocation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/definitions/resource_requirement.py` & `dagster-1.3.9rc0/dagster/_core/definitions/resource_requirement.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/definitions/run_config.py` & `dagster-1.3.9rc0/dagster/_core/definitions/run_config.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/definitions/run_config_schema.py` & `dagster-1.3.9rc0/dagster/_core/definitions/run_config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/definitions/run_request.py` & `dagster-1.3.9rc0/dagster/_core/definitions/run_request.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/definitions/run_status_sensor_definition.py` & `dagster-1.3.9rc0/dagster/_core/definitions/run_status_sensor_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/definitions/schedule_definition.py` & `dagster-1.3.9rc0/dagster/_core/definitions/schedule_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/definitions/scoped_resources_builder.py` & `dagster-1.3.9rc0/dagster/_core/definitions/scoped_resources_builder.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/definitions/selector.py` & `dagster-1.3.9rc0/dagster/_core/definitions/selector.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/definitions/sensor_definition.py` & `dagster-1.3.9rc0/dagster/_core/definitions/sensor_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/definitions/source_asset.py` & `dagster-1.3.9rc0/dagster/_core/definitions/source_asset.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/definitions/step_launcher.py` & `dagster-1.3.9rc0/dagster/_core/definitions/step_launcher.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/definitions/target.py` & `dagster-1.3.9rc0/dagster/_core/definitions/target.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/definitions/time_window_partition_mapping.py` & `dagster-1.3.9rc0/dagster/_core/definitions/time_window_partition_mapping.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/definitions/time_window_partitions.py` & `dagster-1.3.9rc0/dagster/_core/definitions/time_window_partitions.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/definitions/unresolved_asset_job_definition.py` & `dagster-1.3.9rc0/dagster/_core/definitions/unresolved_asset_job_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/definitions/utils.py` & `dagster-1.3.9rc0/dagster/_core/definitions/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/definitions/version_strategy.py` & `dagster-1.3.9rc0/dagster/_core/definitions/version_strategy.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/errors.py` & `dagster-1.3.9rc0/dagster/_core/errors.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/event_api.py` & `dagster-1.3.9rc0/dagster/_core/event_api.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/events/__init__.py` & `dagster-1.3.9rc0/dagster/_core/events/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/events/log.py` & `dagster-1.3.9rc0/dagster/_core/events/log.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/events/utils.py` & `dagster-1.3.9rc0/dagster/_core/events/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/execution/api.py` & `dagster-1.3.9rc0/dagster/_core/execution/api.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/execution/asset_backfill.py` & `dagster-1.3.9rc0/dagster/_core/execution/asset_backfill.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/execution/backfill.py` & `dagster-1.3.9rc0/dagster/_core/execution/backfill.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/execution/build_resources.py` & `dagster-1.3.9rc0/dagster/_core/execution/build_resources.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/execution/compute_logs.py` & `dagster-1.3.9rc0/dagster/_core/execution/compute_logs.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/execution/context/compute.py` & `dagster-1.3.9rc0/dagster/_core/execution/context/compute.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/execution/context/hook.py` & `dagster-1.3.9rc0/dagster/_core/execution/context/hook.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/execution/context/init.py` & `dagster-1.3.9rc0/dagster/_core/execution/context/init.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/execution/context/input.py` & `dagster-1.3.9rc0/dagster/_core/execution/context/input.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/execution/context/invocation.py` & `dagster-1.3.9rc0/dagster/_core/execution/context/invocation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/execution/context/logger.py` & `dagster-1.3.9rc0/dagster/_core/execution/context/logger.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/execution/context/output.py` & `dagster-1.3.9rc0/dagster/_core/execution/context/output.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/execution/context/system.py` & `dagster-1.3.9rc0/dagster/_core/execution/context/system.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/execution/context_creation_job.py` & `dagster-1.3.9rc0/dagster/_core/execution/context_creation_job.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/execution/execute_in_process.py` & `dagster-1.3.9rc0/dagster/_core/execution/execute_in_process.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/execution/execute_in_process_result.py` & `dagster-1.3.9rc0/dagster/_core/execution/execute_in_process_result.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/execution/execution_result.py` & `dagster-1.3.9rc0/dagster/_core/execution/execution_result.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/execution/host_mode.py` & `dagster-1.3.9rc0/dagster/_core/execution/host_mode.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/execution/job_backfill.py` & `dagster-1.3.9rc0/dagster/_core/execution/job_backfill.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/execution/job_execution_result.py` & `dagster-1.3.9rc0/dagster/_core/execution/job_execution_result.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/execution/memoization.py` & `dagster-1.3.9rc0/dagster/_core/execution/memoization.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/execution/plan/active.py` & `dagster-1.3.9rc0/dagster/_core/execution/plan/active.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/execution/plan/compute.py` & `dagster-1.3.9rc0/dagster/_core/execution/plan/compute.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/execution/plan/compute_generator.py` & `dagster-1.3.9rc0/dagster/_core/execution/plan/compute_generator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/execution/plan/execute_plan.py` & `dagster-1.3.9rc0/dagster/_core/execution/plan/execute_plan.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/execution/plan/execute_step.py` & `dagster-1.3.9rc0/dagster/_core/execution/plan/execute_step.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/execution/plan/external_step.py` & `dagster-1.3.9rc0/dagster/_core/execution/plan/external_step.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/execution/plan/handle.py` & `dagster-1.3.9rc0/dagster/_core/execution/plan/handle.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/execution/plan/inputs.py` & `dagster-1.3.9rc0/dagster/_core/execution/plan/inputs.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/execution/plan/instance_concurrency_context.py` & `dagster-1.3.9rc0/dagster/_core/execution/plan/instance_concurrency_context.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/execution/plan/local_external_step_main.py` & `dagster-1.3.9rc0/dagster/_core/execution/plan/local_external_step_main.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/execution/plan/objects.py` & `dagster-1.3.9rc0/dagster/_core/execution/plan/objects.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/execution/plan/outputs.py` & `dagster-1.3.9rc0/dagster/_core/execution/plan/outputs.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/execution/plan/plan.py` & `dagster-1.3.9rc0/dagster/_core/execution/plan/plan.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/execution/plan/state.py` & `dagster-1.3.9rc0/dagster/_core/execution/plan/state.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/execution/plan/step.py` & `dagster-1.3.9rc0/dagster/_core/execution/plan/step.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/execution/plan/utils.py` & `dagster-1.3.9rc0/dagster/_core/execution/plan/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/execution/poll_compute_logs.py` & `dagster-1.3.9rc0/dagster/_core/execution/poll_compute_logs.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/execution/resolve_versions.py` & `dagster-1.3.9rc0/dagster/_core/execution/resolve_versions.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/execution/resources_init.py` & `dagster-1.3.9rc0/dagster/_core/execution/resources_init.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/execution/retries.py` & `dagster-1.3.9rc0/dagster/_core/execution/retries.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/execution/run_cancellation_thread.py` & `dagster-1.3.9rc0/dagster/_core/execution/run_cancellation_thread.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/execution/stats.py` & `dagster-1.3.9rc0/dagster/_core/execution/stats.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/execution/tags.py` & `dagster-1.3.9rc0/dagster/_core/execution/tags.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/execution/validate_run_config.py` & `dagster-1.3.9rc0/dagster/_core/execution/validate_run_config.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/execution/watch_orphans.py` & `dagster-1.3.9rc0/dagster/_core/execution/watch_orphans.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/execution/with_resources.py` & `dagster-1.3.9rc0/dagster/_core/execution/with_resources.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/executor/base.py` & `dagster-1.3.9rc0/dagster/_core/executor/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/executor/child_process_executor.py` & `dagster-1.3.9rc0/dagster/_core/executor/child_process_executor.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/executor/in_process.py` & `dagster-1.3.9rc0/dagster/_core/executor/in_process.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/executor/init.py` & `dagster-1.3.9rc0/dagster/_core/executor/init.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/executor/multiprocess.py` & `dagster-1.3.9rc0/dagster/_core/executor/multiprocess.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/executor/step_delegating/step_delegating_executor.py` & `dagster-1.3.9rc0/dagster/_core/executor/step_delegating/step_delegating_executor.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/executor/step_delegating/step_handler/base.py` & `dagster-1.3.9rc0/dagster/_core/executor/step_delegating/step_handler/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/host_representation/__init__.py` & `dagster-1.3.9rc0/dagster/_core/host_representation/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/host_representation/code_location.py` & `dagster-1.3.9rc0/dagster/_core/host_representation/code_location.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/host_representation/external.py` & `dagster-1.3.9rc0/dagster/_core/host_representation/external.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/host_representation/external_data.py` & `dagster-1.3.9rc0/dagster/_core/host_representation/external_data.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/host_representation/grpc_server_registry.py` & `dagster-1.3.9rc0/dagster/_core/host_representation/grpc_server_registry.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/host_representation/grpc_server_state_subscriber.py` & `dagster-1.3.9rc0/dagster/_core/host_representation/grpc_server_state_subscriber.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/host_representation/handle.py` & `dagster-1.3.9rc0/dagster/_core/host_representation/handle.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/host_representation/historical.py` & `dagster-1.3.9rc0/dagster/_core/host_representation/historical.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/host_representation/job_index.py` & `dagster-1.3.9rc0/dagster/_core/host_representation/job_index.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/host_representation/origin.py` & `dagster-1.3.9rc0/dagster/_core/host_representation/origin.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/host_representation/represented.py` & `dagster-1.3.9rc0/dagster/_core/host_representation/represented.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/instance/__init__.py` & `dagster-1.3.9rc0/dagster/_core/instance/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/instance/config.py` & `dagster-1.3.9rc0/dagster/_core/instance/config.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/instance/ref.py` & `dagster-1.3.9rc0/dagster/_core/instance/ref.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/instance_for_test.py` & `dagster-1.3.9rc0/dagster/_core/instance_for_test.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/launcher/base.py` & `dagster-1.3.9rc0/dagster/_core/launcher/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/launcher/default_run_launcher.py` & `dagster-1.3.9rc0/dagster/_core/launcher/default_run_launcher.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/launcher/sync_in_memory_run_launcher.py` & `dagster-1.3.9rc0/dagster/_core/launcher/sync_in_memory_run_launcher.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/log_manager.py` & `dagster-1.3.9rc0/dagster/_core/log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/nux.py` & `dagster-1.3.9rc0/dagster/_core/nux.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/origin.py` & `dagster-1.3.9rc0/dagster/_core/origin.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/run_coordinator/base.py` & `dagster-1.3.9rc0/dagster/_core/run_coordinator/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/run_coordinator/default_run_coordinator.py` & `dagster-1.3.9rc0/dagster/_core/run_coordinator/default_run_coordinator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/run_coordinator/queued_run_coordinator.py` & `dagster-1.3.9rc0/dagster/_core/run_coordinator/queued_run_coordinator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/scheduler/__init__.py` & `dagster-1.3.9rc0/dagster/_core/scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/scheduler/execution.py` & `dagster-1.3.9rc0/dagster/_core/scheduler/execution.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/scheduler/instigation.py` & `dagster-1.3.9rc0/dagster/_core/scheduler/instigation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/scheduler/scheduler.py` & `dagster-1.3.9rc0/dagster/_core/scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/secrets/env_file.py` & `dagster-1.3.9rc0/dagster/_core/secrets/env_file.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/selector/subset_selector.py` & `dagster-1.3.9rc0/dagster/_core/selector/subset_selector.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/snap/__init__.py` & `dagster-1.3.9rc0/dagster/_core/snap/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/snap/dagster_types.py` & `dagster-1.3.9rc0/dagster/_core/snap/dagster_types.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/snap/dep_snapshot.py` & `dagster-1.3.9rc0/dagster/_core/snap/dep_snapshot.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/snap/execution_plan_snapshot.py` & `dagster-1.3.9rc0/dagster/_core/snap/execution_plan_snapshot.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/snap/job_snapshot.py` & `dagster-1.3.9rc0/dagster/_core/snap/job_snapshot.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/snap/mode.py` & `dagster-1.3.9rc0/dagster/_core/snap/mode.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/snap/node.py` & `dagster-1.3.9rc0/dagster/_core/snap/node.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/snap/snap_to_yaml.py` & `dagster-1.3.9rc0/dagster/_core/snap/snap_to_yaml.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/storage/DEVELOPING.md` & `dagster-1.3.9rc0/dagster/_core/storage/DEVELOPING.md`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/storage/alembic/README.md` & `dagster-1.3.9rc0/dagster/_core/storage/alembic/README.md`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/storage/alembic/env.py` & `dagster-1.3.9rc0/dagster/_core/storage/alembic/env.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/storage/alembic/versions/001_initial_1.py` & `dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/001_initial_1.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_postgres.py` & `dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_sqlite.py` & `dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_postgres.py` & `dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_sqlite.py` & `dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/storage/alembic/versions/004_add_snapshots_to_run_storage.py` & `dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/004_add_snapshots_to_run_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/storage/alembic/versions/005_add_asset_key_postgres.py` & `dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/005_add_asset_key_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/storage/alembic/versions/005_add_asset_key_sqlite.py` & `dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/005_add_asset_key_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/storage/alembic/versions/006_scheduler_update_postgres.py` & `dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/006_scheduler_update_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/storage/alembic/versions/007_create_run_id_idx_postgres.py` & `dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/007_create_run_id_idx_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/storage/alembic/versions/007_create_run_id_idx_sqlite.py` & `dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/007_create_run_id_idx_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/storage/alembic/versions/008_add_run_tags_index_postgres.py` & `dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/008_add_run_tags_index_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/storage/alembic/versions/008_add_run_tags_index_sqlite.py` & `dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/008_add_run_tags_index_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/storage/alembic/versions/009_add_partition_column_postgres.py` & `dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/009_add_partition_column_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/storage/alembic/versions/009_add_partition_column_sqlite.py` & `dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/009_add_partition_column_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_postgres.py` & `dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_sqlite.py` & `dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_postgres.py` & `dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_1.py` & `dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_1.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_2.py` & `dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_2.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_postgres.py` & `dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_sqlite.py` & `dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/storage/alembic/versions/017_add_run_status_index_postgres.py` & `dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/017_add_run_status_index_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/storage/alembic/versions/017_add_run_status_index_sqlite.py` & `dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/017_add_run_status_index_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_postgres.py` & `dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_sqlite.py` & `dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/storage/alembic/versions/021_add_column_mode_mysql.py` & `dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/021_add_column_mode_mysql.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/storage/alembic/versions/021_add_column_mode_postgres.py` & `dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/021_add_column_mode_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/storage/alembic/versions/021_add_column_mode_sqlite.py` & `dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/021_add_column_mode_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_mysql.py` & `dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_mysql.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_postgres.py` & `dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_sqlite.py` & `dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/storage/alembic/versions/026_convert_start_end_times_format_mysql.py` & `dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/026_convert_start_end_times_format_mysql.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/storage/alembic/versions/030_add_columns_action_type_and_selector_id_.py` & `dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/030_add_columns_action_type_and_selector_id_.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/storage/alembic/versions/031_add_kvs_table.py` & `dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/031_add_kvs_table.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/storage/alembic/versions/033_add_asset_event_tags_table.py` & `dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/033_add_asset_event_tags_table.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/storage/alembic/versions/036_add_dynamic_partitions_table.py` & `dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/036_add_dynamic_partitions_table.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/storage/alembic/versions/037_d9092588866f_add_primary_key_cols.py` & `dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/037_d9092588866f_add_primary_key_cols.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/storage/alembic/versions/038_701913684cb4_add_postgres_pks.py` & `dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/038_701913684cb4_add_postgres_pks.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/storage/alembic/versions/039_d3a4c9e87af3_add_asset_daemon_asset_evaluations_table.py` & `dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/039_d3a4c9e87af3_add_asset_daemon_asset_evaluations_table.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/storage/alembic/versions/040_add_in_progress_step_table.py` & `dagster-1.3.9rc0/dagster/_core/storage/alembic/versions/040_add_in_progress_step_table.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/storage/asset_value_loader.py` & `dagster-1.3.9rc0/dagster/_core/storage/asset_value_loader.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/storage/base_storage.py` & `dagster-1.3.9rc0/dagster/_core/storage/base_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/storage/branching/branching_io_manager.py` & `dagster-1.3.9rc0/dagster/_core/storage/branching/branching_io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/storage/captured_log_manager.py` & `dagster-1.3.9rc0/dagster/_core/storage/captured_log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/storage/cloud_storage_compute_log_manager.py` & `dagster-1.3.9rc0/dagster/_core/storage/cloud_storage_compute_log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/storage/compute_log_manager.py` & `dagster-1.3.9rc0/dagster/_core/storage/compute_log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/storage/config.py` & `dagster-1.3.9rc0/dagster/_core/storage/config.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/storage/dagster_run.py` & `dagster-1.3.9rc0/dagster/_core/storage/dagster_run.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/storage/db_io_manager.py` & `dagster-1.3.9rc0/dagster/_core/storage/db_io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/storage/event_log/__init__.py` & `dagster-1.3.9rc0/dagster/_core/storage/event_log/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/storage/event_log/base.py` & `dagster-1.3.9rc0/dagster/_core/storage/event_log/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/storage/event_log/in_memory.py` & `dagster-1.3.9rc0/dagster/_core/storage/event_log/in_memory.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/storage/event_log/migration.py` & `dagster-1.3.9rc0/dagster/_core/storage/event_log/migration.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/storage/event_log/polling_event_watcher.py` & `dagster-1.3.9rc0/dagster/_core/storage/event_log/polling_event_watcher.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/storage/event_log/schema.py` & `dagster-1.3.9rc0/dagster/_core/storage/event_log/schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/storage/event_log/sql_event_log.py` & `dagster-1.3.9rc0/dagster/_core/storage/event_log/sql_event_log.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/storage/event_log/sqlite/alembic/alembic.ini` & `dagster-1.3.9rc0/dagster/_core/storage/event_log/sqlite/alembic/alembic.ini`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/storage/event_log/sqlite/consolidated_sqlite_event_log.py` & `dagster-1.3.9rc0/dagster/_core/storage/event_log/sqlite/consolidated_sqlite_event_log.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/storage/event_log/sqlite/sqlite_event_log.py` & `dagster-1.3.9rc0/dagster/_core/storage/event_log/sqlite/sqlite_event_log.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/storage/file_manager.py` & `dagster-1.3.9rc0/dagster/_core/storage/file_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/storage/fs_io_manager.py` & `dagster-1.3.9rc0/dagster/_core/storage/fs_io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/storage/input_manager.py` & `dagster-1.3.9rc0/dagster/_core/storage/input_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/storage/io_manager.py` & `dagster-1.3.9rc0/dagster/_core/storage/io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/storage/legacy_storage.py` & `dagster-1.3.9rc0/dagster/_core/storage/legacy_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/storage/local_compute_log_manager.py` & `dagster-1.3.9rc0/dagster/_core/storage/local_compute_log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/storage/mem_io_manager.py` & `dagster-1.3.9rc0/dagster/_core/storage/mem_io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/storage/memoizable_io_manager.py` & `dagster-1.3.9rc0/dagster/_core/storage/memoizable_io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/storage/migration/utils.py` & `dagster-1.3.9rc0/dagster/_core/storage/migration/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/storage/noop_compute_log_manager.py` & `dagster-1.3.9rc0/dagster/_core/storage/noop_compute_log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/storage/output_manager.py` & `dagster-1.3.9rc0/dagster/_core/storage/output_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/storage/partition_status_cache.py` & `dagster-1.3.9rc0/dagster/_core/storage/partition_status_cache.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/storage/root.py` & `dagster-1.3.9rc0/dagster/_core/storage/root.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/storage/root_input_manager.py` & `dagster-1.3.9rc0/dagster/_core/storage/root_input_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/storage/runs/base.py` & `dagster-1.3.9rc0/dagster/_core/storage/runs/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/storage/runs/in_memory.py` & `dagster-1.3.9rc0/dagster/_core/storage/runs/in_memory.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/storage/runs/migration.py` & `dagster-1.3.9rc0/dagster/_core/storage/runs/migration.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/storage/runs/schema.py` & `dagster-1.3.9rc0/dagster/_core/storage/runs/schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/storage/runs/sql_run_storage.py` & `dagster-1.3.9rc0/dagster/_core/storage/runs/sql_run_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/storage/runs/sqlite/alembic/alembic.ini` & `dagster-1.3.9rc0/dagster/_core/storage/runs/sqlite/alembic/alembic.ini`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/storage/runs/sqlite/sqlite_run_storage.py` & `dagster-1.3.9rc0/dagster/_core/storage/runs/sqlite/sqlite_run_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/storage/schedules/base.py` & `dagster-1.3.9rc0/dagster/_core/storage/schedules/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/storage/schedules/migration.py` & `dagster-1.3.9rc0/dagster/_core/storage/schedules/migration.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/storage/schedules/schema.py` & `dagster-1.3.9rc0/dagster/_core/storage/schedules/schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/storage/schedules/sql_schedule_storage.py` & `dagster-1.3.9rc0/dagster/_core/storage/schedules/sql_schedule_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/storage/schedules/sqlite/alembic/alembic.ini` & `dagster-1.3.9rc0/dagster/_core/storage/schedules/sqlite/alembic/alembic.ini`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/storage/schedules/sqlite/sqlite_schedule_storage.py` & `dagster-1.3.9rc0/dagster/_core/storage/schedules/sqlite/sqlite_schedule_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/storage/sql.py` & `dagster-1.3.9rc0/dagster/_core/storage/sql.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/storage/sqlalchemy_compat.py` & `dagster-1.3.9rc0/dagster/_core/storage/sqlalchemy_compat.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/storage/sqlite.py` & `dagster-1.3.9rc0/dagster/_core/storage/sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/storage/sqlite_storage.py` & `dagster-1.3.9rc0/dagster/_core/storage/sqlite_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/storage/tags.py` & `dagster-1.3.9rc0/dagster/_core/storage/tags.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/storage/temp_file_manager.py` & `dagster-1.3.9rc0/dagster/_core/storage/temp_file_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/storage/upath_io_manager.py` & `dagster-1.3.9rc0/dagster/_core/storage/upath_io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/system_config/composite_descent.py` & `dagster-1.3.9rc0/dagster/_core/system_config/composite_descent.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/system_config/objects.py` & `dagster-1.3.9rc0/dagster/_core/system_config/objects.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/telemetry.py` & `dagster-1.3.9rc0/dagster/_core/telemetry.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/telemetry_upload.py` & `dagster-1.3.9rc0/dagster/_core/telemetry_upload.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/test_utils.py` & `dagster-1.3.9rc0/dagster/_core/test_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/types/builtin_config_schemas.py` & `dagster-1.3.9rc0/dagster/_core/types/builtin_config_schemas.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/types/config_schema.py` & `dagster-1.3.9rc0/dagster/_core/types/config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/types/dagster_type.py` & `dagster-1.3.9rc0/dagster/_core/types/dagster_type.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/types/decorator.py` & `dagster-1.3.9rc0/dagster/_core/types/decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/types/loadable_target_origin.py` & `dagster-1.3.9rc0/dagster/_core/types/loadable_target_origin.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/types/primitive_mapping.py` & `dagster-1.3.9rc0/dagster/_core/types/primitive_mapping.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/types/python_dict.py` & `dagster-1.3.9rc0/dagster/_core/types/python_dict.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/types/python_set.py` & `dagster-1.3.9rc0/dagster/_core/types/python_set.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/types/python_tuple.py` & `dagster-1.3.9rc0/dagster/_core/types/python_tuple.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/types/transform_typing.py` & `dagster-1.3.9rc0/dagster/_core/types/transform_typing.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/utility_ops.py` & `dagster-1.3.9rc0/dagster/_core/utility_ops.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/utils.py` & `dagster-1.3.9rc0/dagster/_core/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/workspace/autodiscovery.py` & `dagster-1.3.9rc0/dagster/_core/workspace/autodiscovery.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/workspace/config_schema.py` & `dagster-1.3.9rc0/dagster/_core/workspace/config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/workspace/context.py` & `dagster-1.3.9rc0/dagster/_core/workspace/context.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/workspace/load.py` & `dagster-1.3.9rc0/dagster/_core/workspace/load.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/workspace/load_target.py` & `dagster-1.3.9rc0/dagster/_core/workspace/load_target.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/workspace/permissions.py` & `dagster-1.3.9rc0/dagster/_core/workspace/permissions.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_core/workspace/workspace.py` & `dagster-1.3.9rc0/dagster/_core/workspace/workspace.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_daemon/__init__.py` & `dagster-1.3.9rc0/dagster/_daemon/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_daemon/asset_daemon.py` & `dagster-1.3.9rc0/dagster/_daemon/asset_daemon.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_daemon/auto_run_reexecution/auto_run_reexecution.py` & `dagster-1.3.9rc0/dagster/_daemon/auto_run_reexecution/auto_run_reexecution.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_daemon/auto_run_reexecution/event_log_consumer.py` & `dagster-1.3.9rc0/dagster/_daemon/auto_run_reexecution/event_log_consumer.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_daemon/backfill.py` & `dagster-1.3.9rc0/dagster/_daemon/backfill.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_daemon/cli/__init__.py` & `dagster-1.3.9rc0/dagster/_daemon/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_daemon/controller.py` & `dagster-1.3.9rc0/dagster/_daemon/controller.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_daemon/daemon.py` & `dagster-1.3.9rc0/dagster/_daemon/daemon.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_daemon/monitoring/concurrency.py` & `dagster-1.3.9rc0/dagster/_daemon/monitoring/concurrency.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_daemon/monitoring/run_monitoring.py` & `dagster-1.3.9rc0/dagster/_daemon/monitoring/run_monitoring.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_daemon/run_coordinator/queued_run_coordinator_daemon.py` & `dagster-1.3.9rc0/dagster/_daemon/run_coordinator/queued_run_coordinator_daemon.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_daemon/sensor.py` & `dagster-1.3.9rc0/dagster/_daemon/sensor.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_daemon/types.py` & `dagster-1.3.9rc0/dagster/_daemon/types.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_daemon/workspace.py` & `dagster-1.3.9rc0/dagster/_daemon/workspace.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_generate/download.py` & `dagster-1.3.9rc0/dagster/_generate/download.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_generate/generate.py` & `dagster-1.3.9rc0/dagster/_generate/generate.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/README.md` & `dagster-1.3.9rc0/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/README.md`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_grpc/__generated__/api_pb2.py` & `dagster-1.3.9rc0/dagster/_grpc/__generated__/api_pb2.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_grpc/__generated__/api_pb2_grpc.py` & `dagster-1.3.9rc0/dagster/_grpc/__generated__/api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_grpc/__init__.py` & `dagster-1.3.9rc0/dagster/_grpc/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_grpc/client.py` & `dagster-1.3.9rc0/dagster/_grpc/client.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_grpc/compile.py` & `dagster-1.3.9rc0/dagster/_grpc/compile.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_grpc/impl.py` & `dagster-1.3.9rc0/dagster/_grpc/impl.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_grpc/protos/api.proto` & `dagster-1.3.9rc0/dagster/_grpc/protos/api.proto`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_grpc/proxy_server.py` & `dagster-1.3.9rc0/dagster/_grpc/proxy_server.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_grpc/server.py` & `dagster-1.3.9rc0/dagster/_grpc/server.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_grpc/server_watcher.py` & `dagster-1.3.9rc0/dagster/_grpc/server_watcher.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_grpc/types.py` & `dagster-1.3.9rc0/dagster/_grpc/types.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_grpc/utils.py` & `dagster-1.3.9rc0/dagster/_grpc/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_loggers/__init__.py` & `dagster-1.3.9rc0/dagster/_loggers/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_module_alias_map.py` & `dagster-1.3.9rc0/dagster/_module_alias_map.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_scheduler/scheduler.py` & `dagster-1.3.9rc0/dagster/_scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_scheduler/stale.py` & `dagster-1.3.9rc0/dagster/_scheduler/stale.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_serdes/__init__.py` & `dagster-1.3.9rc0/dagster/_serdes/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_serdes/config_class.py` & `dagster-1.3.9rc0/dagster/_serdes/config_class.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_serdes/ipc.py` & `dagster-1.3.9rc0/dagster/_serdes/ipc.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_serdes/serdes.py` & `dagster-1.3.9rc0/dagster/_serdes/serdes.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_serdes/utils.py` & `dagster-1.3.9rc0/dagster/_serdes/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_seven/__init__.py` & `dagster-1.3.9rc0/dagster/_seven/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_seven/abc.py` & `dagster-1.3.9rc0/dagster/_seven/abc.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_seven/compat/pendulum.py` & `dagster-1.3.9rc0/dagster/_seven/compat/pendulum.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_utils/__init__.py` & `dagster-1.3.9rc0/dagster/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_utils/alert.py` & `dagster-1.3.9rc0/dagster/_utils/alert.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_utils/backcompat.py` & `dagster-1.3.9rc0/dagster/_utils/backcompat.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_utils/backoff.py` & `dagster-1.3.9rc0/dagster/_utils/backoff.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_utils/cached_method.py` & `dagster-1.3.9rc0/dagster/_utils/cached_method.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_utils/caching_instance_queryer.py` & `dagster-1.3.9rc0/dagster/_utils/caching_instance_queryer.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_utils/concurrency.py` & `dagster-1.3.9rc0/dagster/_utils/concurrency.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_utils/dagster_type.py` & `dagster-1.3.9rc0/dagster/_utils/dagster_type.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_utils/env.py` & `dagster-1.3.9rc0/dagster/_utils/env.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_utils/error.py` & `dagster-1.3.9rc0/dagster/_utils/error.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_utils/external.py` & `dagster-1.3.9rc0/dagster/_utils/external.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_utils/forked_pdb.py` & `dagster-1.3.9rc0/dagster/_utils/forked_pdb.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_utils/hosted_user_process.py` & `dagster-1.3.9rc0/dagster/_utils/hosted_user_process.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_utils/indenting_printer.py` & `dagster-1.3.9rc0/dagster/_utils/indenting_printer.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_utils/interrupts.py` & `dagster-1.3.9rc0/dagster/_utils/interrupts.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_utils/log.py` & `dagster-1.3.9rc0/dagster/_utils/log.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_utils/merger.py` & `dagster-1.3.9rc0/dagster/_utils/merger.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_utils/net.py` & `dagster-1.3.9rc0/dagster/_utils/net.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_utils/schedules.py` & `dagster-1.3.9rc0/dagster/_utils/schedules.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_utils/tags.py` & `dagster-1.3.9rc0/dagster/_utils/tags.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_utils/temp_file.py` & `dagster-1.3.9rc0/dagster/_utils/temp_file.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_utils/test/__init__.py` & `dagster-1.3.9rc0/dagster/_utils/test/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_utils/test/mysql_instance.py` & `dagster-1.3.9rc0/dagster/_utils/test/mysql_instance.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_utils/test/postgres_instance.py` & `dagster-1.3.9rc0/dagster/_utils/test/postgres_instance.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_utils/test/schedule_storage.py` & `dagster-1.3.9rc0/dagster/_utils/test/schedule_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_utils/timing.py` & `dagster-1.3.9rc0/dagster/_utils/timing.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_utils/typing_api.py` & `dagster-1.3.9rc0/dagster/_utils/typing_api.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster/_utils/yaml_utils.py` & `dagster-1.3.9rc0/dagster/_utils/yaml_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster.egg-info/PKG-INFO` & `dagster-1.3.9rc0/dagster.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster
-Version: 1.3.9
+Version: 1.3.9rc0
 Summary: The data orchestration platform built for productivity.
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Project-URL: Homepage, https://dagster.io
 Project-URL: GitHub, https://github.com/dagster-io/dagster
 Project-URL: Changelog, https://github.com/dagster-io/dagster/releases
```

### Comparing `dagster-1.3.9/dagster.egg-info/SOURCES.txt` & `dagster-1.3.9rc0/dagster.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/dagster.egg-info/requires.txt` & `dagster-1.3.9rc0/dagster.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `dagster-1.3.9/setup.py` & `dagster-1.3.9rc0/setup.py`

 * *Files identical despite different names*

