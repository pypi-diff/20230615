# Comparing `tmp/nodestream-0.1.0.tar.gz` & `tmp/nodestream-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nodestream-0.1.0.tar", max compression
+gzip compressed data, was "nodestream-0.2.0.tar", max compression
```

## Comparing `nodestream-0.1.0.tar` & `nodestream-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,122 @@
--rw-r--r--   0        0        0        0 2023-01-25 16:02:05.032491 nodestream-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-01-25 16:02:05.032446 nodestream-0.1.0/nodestream/__init__.py
--rw-r--r--   0        0        0      279 2023-01-25 16:02:21.169322 nodestream-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      514 1970-01-01 00:00:00.000000 nodestream-0.1.0/setup.py
--rw-r--r--   0        0        0      298 1970-01-01 00:00:00.000000 nodestream-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    32335 2023-05-18 13:51:44.150322 nodestream-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1629 2023-06-05 20:55:40.249844 nodestream-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-05-18 13:51:44.151306 nodestream-0.2.0/nodestream/__init__.py
+-rw-r--r--   0        0        0      321 2023-06-06 14:48:12.777929 nodestream-0.2.0/nodestream/argument_resolvers/__init__.py
+-rw-r--r--   0        0        0      440 2023-06-06 14:48:12.778117 nodestream-0.2.0/nodestream/argument_resolvers/argument_resolver.py
+-rw-r--r--   0        0        0      600 2023-06-06 14:48:12.778550 nodestream-0.2.0/nodestream/argument_resolvers/environment_variable_resolver.py
+-rw-r--r--   0        0        0      689 2023-06-06 14:48:12.778951 nodestream-0.2.0/nodestream/argument_resolvers/include_file_resolver.py
+-rw-r--r--   0        0        0      262 2023-06-08 00:32:08.908151 nodestream-0.2.0/nodestream/audits/__init__.py
+-rw-r--r--   0        0        0      695 2023-06-08 00:37:19.628414 nodestream-0.2.0/nodestream/audits/audit.py
+-rw-r--r--   0        0        0      375 2023-06-08 00:27:12.187711 nodestream-0.2.0/nodestream/audits/audit_printer.py
+-rw-r--r--   0        0        0     1635 2023-06-08 14:38:42.505682 nodestream-0.2.0/nodestream/audits/audit_referencial_integrity.py
+-rw-r--r--   0        0        0     1516 2023-06-08 14:22:33.346618 nodestream-0.2.0/nodestream/audits/audit_ttls.py
+-rw-r--r--   0        0        0      109 2023-05-29 23:36:36.044355 nodestream-0.2.0/nodestream/cli/__init__.py
+-rw-r--r--   0        0        0      924 2023-06-08 00:35:45.179471 nodestream-0.2.0/nodestream/cli/application.py
+-rw-r--r--   0        0        0      250 2023-06-05 20:55:40.270364 nodestream-0.2.0/nodestream/cli/commands/__init__.py
+-rw-r--r--   0        0        0      482 2023-06-08 00:34:18.198907 nodestream-0.2.0/nodestream/cli/commands/audit_command.py
+-rw-r--r--   0        0        0      268 2023-06-08 00:35:30.685238 nodestream-0.2.0/nodestream/cli/commands/audit_refs.py
+-rw-r--r--   0        0        0      204 2023-06-08 00:34:41.019749 nodestream-0.2.0/nodestream/cli/commands/audit_ttls.py
+-rw-r--r--   0        0        0     1090 2023-06-05 20:55:40.270526 nodestream-0.2.0/nodestream/cli/commands/new.py
+-rw-r--r--   0        0        0     1108 2023-06-08 00:13:08.470729 nodestream-0.2.0/nodestream/cli/commands/nodestream_command.py
+-rw-r--r--   0        0        0     1213 2023-06-07 19:09:40.099387 nodestream-0.2.0/nodestream/cli/commands/print_schema.py
+-rw-r--r--   0        0        0      893 2023-06-05 20:55:40.270803 nodestream-0.2.0/nodestream/cli/commands/remove.py
+-rw-r--r--   0        0        0     1087 2023-06-06 14:48:12.780185 nodestream-0.2.0/nodestream/cli/commands/run.py
+-rw-r--r--   0        0        0     1342 2023-06-05 20:55:40.271104 nodestream-0.2.0/nodestream/cli/commands/scaffold.py
+-rw-r--r--   0        0        0      508 2023-06-06 14:48:12.780577 nodestream-0.2.0/nodestream/cli/commands/shared_options.py
+-rw-r--r--   0        0        0      596 2023-06-05 20:55:40.271384 nodestream-0.2.0/nodestream/cli/commands/show.py
+-rw-r--r--   0        0        0      986 2023-06-08 00:02:45.190774 nodestream-0.2.0/nodestream/cli/operations/__init__.py
+-rw-r--r--   0        0        0      988 2023-06-05 20:55:40.271830 nodestream-0.2.0/nodestream/cli/operations/add_pipeline_to_project.py
+-rw-r--r--   0        0        0      438 2023-06-05 20:55:40.271946 nodestream-0.2.0/nodestream/cli/operations/commit_project_to_disk.py
+-rw-r--r--   0        0        0     2153 2023-06-05 20:55:40.272099 nodestream-0.2.0/nodestream/cli/operations/generate_pipeline_scaffold.py
+-rw-r--r--   0        0        0     1434 2023-06-05 20:55:40.272303 nodestream-0.2.0/nodestream/cli/operations/generate_project.py
+-rw-r--r--   0        0        0     2317 2023-06-05 20:55:40.272481 nodestream-0.2.0/nodestream/cli/operations/generate_python_scaffold.py
+-rw-r--r--   0        0        0      370 2023-06-05 20:55:40.272873 nodestream-0.2.0/nodestream/cli/operations/initialize_logger.py
+-rw-r--r--   0        0        0      339 2023-06-05 20:55:40.273047 nodestream-0.2.0/nodestream/cli/operations/initialize_project.py
+-rw-r--r--   0        0        0      384 2023-06-05 20:55:40.273394 nodestream-0.2.0/nodestream/cli/operations/operation.py
+-rw-r--r--   0        0        0     1208 2023-06-07 19:09:40.100607 nodestream-0.2.0/nodestream/cli/operations/print_project_schema.py
+-rw-r--r--   0        0        0      533 2023-06-05 20:55:40.273559 nodestream-0.2.0/nodestream/cli/operations/remove_pipeline_from_project.py
+-rw-r--r--   0        0        0     1137 2023-06-08 00:31:31.712160 nodestream-0.2.0/nodestream/cli/operations/run_audit.py
+-rw-r--r--   0        0        0     2337 2023-06-05 20:55:40.273891 nodestream-0.2.0/nodestream/cli/operations/run_pipeline.py
+-rw-r--r--   0        0        0     2399 2023-06-05 20:55:40.274048 nodestream-0.2.0/nodestream/cli/operations/show_pipelines.py
+-rw-r--r--   0        0        0      329 2023-06-07 19:09:40.100995 nodestream-0.2.0/nodestream/cli/schema_printers/__init__.py
+-rw-r--r--   0        0        0     5717 2023-06-07 19:09:40.101284 nodestream-0.2.0/nodestream/cli/schema_printers/graphql_schema_printer.py
+-rw-r--r--   0        0        0      272 2023-06-07 19:09:40.101737 nodestream-0.2.0/nodestream/cli/schema_printers/plain_text_schema_printer.py
+-rw-r--r--   0        0        0      634 2023-06-07 19:09:40.102022 nodestream-0.2.0/nodestream/cli/schema_printers/schema_printer.py
+-rw-r--r--   0        0        0      165 2023-05-19 19:07:54.211393 nodestream-0.2.0/nodestream/databases/__init__.py
+-rw-r--r--   0        0        0     2958 2023-06-06 14:48:12.780980 nodestream-0.2.0/nodestream/databases/debounced_ingest_strategy.py
+-rw-r--r--   0        0        0      166 2023-05-23 15:05:18.008404 nodestream-0.2.0/nodestream/databases/neo4j/__init__.py
+-rw-r--r--   0        0        0     2673 2023-06-06 17:09:46.058615 nodestream-0.2.0/nodestream/databases/neo4j/index_query_builder.py
+-rw-r--r--   0        0        0     8831 2023-06-06 14:48:12.781801 nodestream-0.2.0/nodestream/databases/neo4j/ingest_query_builder.py
+-rw-r--r--   0        0        0     1034 2023-05-23 15:05:18.009754 nodestream-0.2.0/nodestream/databases/neo4j/query.py
+-rw-r--r--   0        0        0     3934 2023-06-06 14:48:12.782196 nodestream-0.2.0/nodestream/databases/neo4j/query_executor.py
+-rw-r--r--   0        0        0     2793 2023-05-25 20:54:40.568938 nodestream-0.2.0/nodestream/databases/operation_debouncer.py
+-rw-r--r--   0        0        0     2060 2023-06-06 14:48:12.782584 nodestream-0.2.0/nodestream/databases/query_executor.py
+-rw-r--r--   0        0        0     1661 2023-06-06 14:48:12.783036 nodestream-0.2.0/nodestream/databases/writer.py
+-rw-r--r--   0        0        0     2547 2023-06-06 14:48:12.783447 nodestream-0.2.0/nodestream/exceptions.py
+-rw-r--r--   0        0        0       63 2023-05-24 19:45:31.927731 nodestream-0.2.0/nodestream/extractors/__init__.py
+-rw-r--r--   0        0        0     2641 2023-06-06 17:09:46.059395 nodestream-0.2.0/nodestream/extractors/files.py
+-rw-r--r--   0        0        0        0 2023-05-18 13:51:44.153895 nodestream-0.2.0/nodestream/extractors/stores/__init__.py
+-rw-r--r--   0        0        0      130 2023-06-05 20:55:40.275076 nodestream-0.2.0/nodestream/extractors/stores/aws/__init__.py
+-rw-r--r--   0        0        0     4568 2023-05-24 18:15:07.882841 nodestream-0.2.0/nodestream/extractors/stores/aws/athena_extractor.py
+-rw-r--r--   0        0        0     2498 2023-05-19 21:00:08.060042 nodestream-0.2.0/nodestream/extractors/stores/aws/credential_utils.py
+-rw-r--r--   0        0        0     2162 2023-06-05 20:55:40.275409 nodestream-0.2.0/nodestream/extractors/stores/aws/s3_extractor.py
+-rw-r--r--   0        0        0      231 2023-05-29 23:36:36.048603 nodestream-0.2.0/nodestream/extractors/streams/__init__.py
+-rw-r--r--   0        0        0     2850 2023-06-06 17:09:46.060022 nodestream-0.2.0/nodestream/extractors/streams/extractor.py
+-rw-r--r--   0        0        0     1550 2023-06-05 20:55:40.276295 nodestream-0.2.0/nodestream/extractors/streams/kafka.py
+-rw-r--r--   0        0        0      617 2023-06-06 14:48:12.783869 nodestream-0.2.0/nodestream/extractors/ttls.py
+-rw-r--r--   0        0        0      630 2023-06-06 14:48:12.784290 nodestream-0.2.0/nodestream/interpreting/__init__.py
+-rw-r--r--   0        0        0     1367 2023-06-06 14:48:12.784779 nodestream-0.2.0/nodestream/interpreting/extract_variables_interpretation.py
+-rw-r--r--   0        0        0      823 2023-06-06 14:48:12.785215 nodestream-0.2.0/nodestream/interpreting/interpretation.py
+-rw-r--r--   0        0        0     4603 2023-06-06 14:48:12.785766 nodestream-0.2.0/nodestream/interpreting/interpreter.py
+-rw-r--r--   0        0        0     1236 2023-06-06 14:48:12.786283 nodestream-0.2.0/nodestream/interpreting/properties_interpretation.py
+-rw-r--r--   0        0        0     1826 2023-06-06 14:48:12.786677 nodestream-0.2.0/nodestream/interpreting/record_decomposers.py
+-rw-r--r--   0        0        0     9831 2023-06-08 14:26:36.774221 nodestream-0.2.0/nodestream/interpreting/relationship_interpretation.py
+-rw-r--r--   0        0        0     4412 2023-06-06 14:48:12.787449 nodestream-0.2.0/nodestream/interpreting/source_node_interpretation.py
+-rw-r--r--   0        0        0     1915 2023-06-06 14:48:12.787601 nodestream-0.2.0/nodestream/interpreting/switch_interpretation.py
+-rw-r--r--   0        0        0      486 2023-05-23 15:05:18.012902 nodestream-0.2.0/nodestream/logging.py
+-rw-r--r--   0        0        0     1541 2023-06-07 19:09:40.102805 nodestream-0.2.0/nodestream/model/__init__.py
+-rw-r--r--   0        0        0     3300 2023-06-06 14:48:12.788476 nodestream-0.2.0/nodestream/model/desired_ingest.py
+-rw-r--r--   0        0        0     6242 2023-06-06 14:48:12.788918 nodestream-0.2.0/nodestream/model/graph_objects.py
+-rw-r--r--   0        0        0     1337 2023-06-08 14:35:15.964089 nodestream-0.2.0/nodestream/model/indexes.py
+-rw-r--r--   0        0        0     2668 2023-06-06 14:48:12.789751 nodestream-0.2.0/nodestream/model/ingest_strategy.py
+-rw-r--r--   0        0        0      873 2023-05-18 13:51:44.156142 nodestream-0.2.0/nodestream/model/ingestion_hooks.py
+-rw-r--r--   0        0        0     1226 2023-06-06 14:48:12.790109 nodestream-0.2.0/nodestream/model/interpreter_context.py
+-rw-r--r--   0        0        0      282 2023-05-19 19:07:54.215627 nodestream-0.2.0/nodestream/model/match_strategy.py
+-rw-r--r--   0        0        0    13791 2023-06-07 19:09:40.103762 nodestream-0.2.0/nodestream/model/schema.py
+-rw-r--r--   0        0        0      794 2023-06-08 00:32:09.016719 nodestream-0.2.0/nodestream/model/ttl.py
+-rw-r--r--   0        0        0      327 2023-05-29 23:36:36.050183 nodestream-0.2.0/nodestream/normalizers/__init__.py
+-rw-r--r--   0        0        0      240 2023-05-30 15:58:51.571325 nodestream-0.2.0/nodestream/normalizers/lowercase_strings.py
+-rw-r--r--   0        0        0     1482 2023-06-07 22:45:15.385531 nodestream-0.2.0/nodestream/normalizers/normalizer.py
+-rw-r--r--   0        0        0      249 2023-05-30 15:58:51.571776 nodestream-0.2.0/nodestream/normalizers/remove_trailing_dots.py
+-rw-r--r--   0        0        0      236 2023-05-30 15:58:51.572307 nodestream-0.2.0/nodestream/normalizers/trim_whitespace.py
+-rw-r--r--   0        0        0      866 2023-06-06 14:48:12.791862 nodestream-0.2.0/nodestream/pipeline/__init__.py
+-rw-r--r--   0        0        0     1641 2023-06-06 14:48:12.792250 nodestream-0.2.0/nodestream/pipeline/class_loader.py
+-rw-r--r--   0        0        0     1150 2023-05-24 23:18:33.740527 nodestream-0.2.0/nodestream/pipeline/extractors.py
+-rw-r--r--   0        0        0     2774 2023-06-06 14:48:12.792635 nodestream-0.2.0/nodestream/pipeline/filters.py
+-rw-r--r--   0        0        0       22 2023-05-19 19:07:54.216776 nodestream-0.2.0/nodestream/pipeline/flush.py
+-rw-r--r--   0        0        0      415 2023-05-31 17:06:52.911049 nodestream-0.2.0/nodestream/pipeline/meta.py
+-rw-r--r--   0        0        0      985 2023-06-07 19:09:40.104346 nodestream-0.2.0/nodestream/pipeline/pipeline.py
+-rw-r--r--   0        0        0     2908 2023-06-07 19:09:40.105095 nodestream-0.2.0/nodestream/pipeline/pipeline_file_loader.py
+-rw-r--r--   0        0        0      706 2023-05-25 15:29:43.396280 nodestream-0.2.0/nodestream/pipeline/step.py
+-rw-r--r--   0        0        0     1036 2023-06-06 17:12:22.610218 nodestream-0.2.0/nodestream/pipeline/transformers.py
+-rw-r--r--   0        0        0     1797 2023-05-24 22:50:05.012870 nodestream-0.2.0/nodestream/pipeline/writers.py
+-rw-r--r--   0        0        0      351 2023-05-18 13:51:44.158173 nodestream-0.2.0/nodestream/project/__init__.py
+-rw-r--r--   0        0        0     2219 2023-06-07 19:09:40.105974 nodestream-0.2.0/nodestream/project/pipeline_definition.py
+-rw-r--r--   0        0        0     1170 2023-05-29 23:36:36.051060 nodestream-0.2.0/nodestream/project/pipeline_progress_reporter.py
+-rw-r--r--   0        0        0     2554 2023-06-07 19:09:40.106585 nodestream-0.2.0/nodestream/project/pipeline_scope.py
+-rw-r--r--   0        0        0     3754 2023-06-08 14:14:09.012485 nodestream-0.2.0/nodestream/project/project.py
+-rw-r--r--   0        0        0      736 2023-05-31 17:06:52.911695 nodestream-0.2.0/nodestream/project/run_request.py
+-rw-r--r--   0        0        0     1460 2023-05-30 15:58:51.572815 nodestream-0.2.0/nodestream/subclass_registry.py
+-rw-r--r--   0        0        0       78 2023-06-06 17:15:51.421169 nodestream-0.2.0/nodestream/transformers/__init__.py
+-rw-r--r--   0        0        0      464 2023-06-06 17:15:30.987309 nodestream-0.2.0/nodestream/transformers/value_projection.py
+-rw-r--r--   0        0        0      566 2023-05-29 23:36:36.052195 nodestream-0.2.0/nodestream/utilities.py
+-rw-r--r--   0        0        0      734 2023-05-25 02:48:03.113484 nodestream-0.2.0/nodestream/value_providers/__init__.py
+-rw-r--r--   0        0        0     1729 2023-06-06 17:09:46.061093 nodestream-0.2.0/nodestream/value_providers/jmespath_value_provider.py
+-rw-r--r--   0        0        0     1099 2023-06-06 17:09:46.061833 nodestream-0.2.0/nodestream/value_providers/jq_value_provder.py
+-rw-r--r--   0        0        0     1250 2023-06-06 14:48:12.795058 nodestream-0.2.0/nodestream/value_providers/mapping_value_provider.py
+-rw-r--r--   0        0        0      591 2023-05-18 13:51:44.159528 nodestream-0.2.0/nodestream/value_providers/static_value_provider.py
+-rw-r--r--   0        0        0     1262 2023-06-06 14:48:12.795541 nodestream-0.2.0/nodestream/value_providers/string_format_value_provider.py
+-rw-r--r--   0        0        0     2205 2023-06-06 14:48:12.797030 nodestream-0.2.0/nodestream/value_providers/value_provider.py
+-rw-r--r--   0        0        0      957 2023-05-18 13:51:44.159795 nodestream-0.2.0/nodestream/value_providers/variable_value_provider.py
+-rw-r--r--   0        0        0     1696 2023-06-07 21:56:49.102433 nodestream-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3071 1970-01-01 00:00:00.000000 nodestream-0.2.0/PKG-INFO
```

