# Comparing `tmp/linkml_runtime-1.5.3.tar.gz` & `tmp/linkml_runtime-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linkml_runtime-1.5.3.tar", max compression
+gzip compressed data, was "linkml_runtime-1.5.4.tar", max compression
```

## Comparing `linkml_runtime-1.5.3.tar` & `linkml_runtime-1.5.4.tar`

### file list

```diff
@@ -1,142 +1,146 @@
--rw-r--r--   0        0        0     7048 2023-05-13 02:39:28.116564 linkml_runtime-1.5.3/LICENSE
--rw-r--r--   0        0        0     1996 2023-05-13 02:39:28.116564 linkml_runtime-1.5.3/README.md
--rw-r--r--   0        0        0     1179 2023-05-13 02:39:28.116564 linkml_runtime-1.5.3/linkml_runtime/__init__.py
--rw-r--r--   0        0        0      426 2023-05-13 02:39:28.116564 linkml_runtime-1.5.3/linkml_runtime/dumpers/__init__.py
--rw-r--r--   0        0        0     1264 2023-05-13 02:39:28.116564 linkml_runtime-1.5.3/linkml_runtime/dumpers/csv_dumper.py
--rw-r--r--   0        0        0      973 2023-05-13 02:39:28.116564 linkml_runtime-1.5.3/linkml_runtime/dumpers/dumper_root.py
--rw-r--r--   0        0        0     4377 2023-05-13 02:39:28.116564 linkml_runtime-1.5.3/linkml_runtime/dumpers/json_dumper.py
--rw-r--r--   0        0        0     4023 2023-05-13 02:39:28.116564 linkml_runtime-1.5.3/linkml_runtime/dumpers/rdf_dumper.py
--rw-r--r--   0        0        0     7169 2023-05-13 02:39:28.116564 linkml_runtime-1.5.3/linkml_runtime/dumpers/rdflib_dumper.py
--rw-r--r--   0        0        0      901 2023-05-13 02:39:28.116564 linkml_runtime-1.5.3/linkml_runtime/dumpers/yaml_dumper.py
--rw-r--r--   0        0        0        0 2023-05-13 02:39:28.116564 linkml_runtime-1.5.3/linkml_runtime/index/__init__.py
--rw-r--r--   0        0        0     8875 2023-05-13 02:39:28.116564 linkml_runtime-1.5.3/linkml_runtime/index/object_index.py
--rw-r--r--   0        0        0      119 2023-05-13 02:39:28.116564 linkml_runtime-1.5.3/linkml_runtime/linkml_model/README.md
--rw-r--r--   0        0        0      738 2023-05-13 02:39:28.116564 linkml_runtime-1.5.3/linkml_runtime/linkml_model/__init__.py
--rw-r--r--   0        0        0     3240 2023-05-13 02:39:28.116564 linkml_runtime-1.5.3/linkml_runtime/linkml_model/annotations.py
--rw-r--r--   0        0        0     3333 2023-05-13 02:39:28.116564 linkml_runtime-1.5.3/linkml_runtime/linkml_model/extensions.py
--rw-r--r--   0        0        0      114 2023-05-13 02:39:28.116564 linkml_runtime-1.5.3/linkml_runtime/linkml_model/graphql/README.md
--rw-r--r--   0        0        0    30306 2023-05-13 02:39:28.116564 linkml_runtime-1.5.3/linkml_runtime/linkml_model/graphql/meta.graphql
--rw-r--r--   0        0        0      111 2023-05-13 02:39:28.116564 linkml_runtime-1.5.3/linkml_runtime/linkml_model/json/README.md
--rw-r--r--   0        0        0    11169 2023-05-13 02:39:28.116564 linkml_runtime-1.5.3/linkml_runtime/linkml_model/json/annotations.json
--rw-r--r--   0        0        0     9306 2023-05-13 02:39:28.116564 linkml_runtime-1.5.3/linkml_runtime/linkml_model/json/extensions.json
--rw-r--r--   0        0        0    12109 2023-05-13 02:39:28.116564 linkml_runtime-1.5.3/linkml_runtime/linkml_model/json/mappings.json
--rw-r--r--   0        0        0   222072 2023-05-13 02:39:28.116564 linkml_runtime-1.5.3/linkml_runtime/linkml_model/json/meta.json
--rw-r--r--   0        0        0     6442 2023-05-13 02:39:28.116564 linkml_runtime-1.5.3/linkml_runtime/linkml_model/json/types.json
--rw-r--r--   0        0        0    22401 2023-05-13 02:39:28.116564 linkml_runtime-1.5.3/linkml_runtime/linkml_model/json/units.json
--rw-r--r--   0        0        0    14834 2023-05-13 02:39:28.116564 linkml_runtime-1.5.3/linkml_runtime/linkml_model/json/validation.json
--rw-r--r--   0        0        0      113 2023-05-13 02:39:28.116564 linkml_runtime-1.5.3/linkml_runtime/linkml_model/jsonld/README.md
--rw-r--r--   0        0        0      648 2023-05-13 02:39:28.116564 linkml_runtime-1.5.3/linkml_runtime/linkml_model/jsonld/annotations.context.jsonld
--rw-r--r--   0        0        0      648 2023-05-13 02:39:28.116564 linkml_runtime-1.5.3/linkml_runtime/linkml_model/jsonld/annotations.model.context.jsonld
--rw-r--r--   0        0        0     7019 2023-05-13 02:39:28.116564 linkml_runtime-1.5.3/linkml_runtime/linkml_model/jsonld/context.jsonld
--rw-r--r--   0        0        0      587 2023-05-13 02:39:28.116564 linkml_runtime-1.5.3/linkml_runtime/linkml_model/jsonld/extensions.context.jsonld
--rw-r--r--   0        0        0      587 2023-05-13 02:39:28.116564 linkml_runtime-1.5.3/linkml_runtime/linkml_model/jsonld/extensions.model.context.jsonld
--rw-r--r--   0        0        0     1615 2023-05-13 02:39:28.116564 linkml_runtime-1.5.3/linkml_runtime/linkml_model/jsonld/mappings.context.jsonld
--rw-r--r--   0        0        0     1615 2023-05-13 02:39:28.116564 linkml_runtime-1.5.3/linkml_runtime/linkml_model/jsonld/mappings.model.context.jsonld
--rw-r--r--   0        0        0    13814 2023-05-13 02:39:28.116564 linkml_runtime-1.5.3/linkml_runtime/linkml_model/jsonld/meta.context.jsonld
--rw-r--r--   0        0        0    14266 2023-05-13 02:39:28.116564 linkml_runtime-1.5.3/linkml_runtime/linkml_model/jsonld/meta.model.context.jsonld
--rw-r--r--   0        0        0      610 2023-05-13 02:39:28.116564 linkml_runtime-1.5.3/linkml_runtime/linkml_model/jsonld/types.context.jsonld
--rw-r--r--   0        0        0      610 2023-05-13 02:39:28.116564 linkml_runtime-1.5.3/linkml_runtime/linkml_model/jsonld/types.model.context.jsonld
--rw-r--r--   0        0        0     2065 2023-05-13 02:39:28.116564 linkml_runtime-1.5.3/linkml_runtime/linkml_model/jsonld/units.context.jsonld
--rw-r--r--   0        0        0     2065 2023-05-13 02:39:28.116564 linkml_runtime-1.5.3/linkml_runtime/linkml_model/jsonld/units.model.context.jsonld
--rw-r--r--   0        0        0     1910 2023-05-13 02:39:28.116564 linkml_runtime-1.5.3/linkml_runtime/linkml_model/jsonld/validation.context.jsonld
--rw-r--r--   0        0        0     1910 2023-05-13 02:39:28.116564 linkml_runtime-1.5.3/linkml_runtime/linkml_model/jsonld/validation.model.context.jsonld
--rw-r--r--   0        0        0      117 2023-05-13 02:39:28.116564 linkml_runtime-1.5.3/linkml_runtime/linkml_model/jsonschema/README.md
--rw-r--r--   0        0        0     4196 2023-05-13 02:39:28.116564 linkml_runtime-1.5.3/linkml_runtime/linkml_model/jsonschema/annotations.schema.json
--rw-r--r--   0        0        0     1984 2023-05-13 02:39:28.116564 linkml_runtime-1.5.3/linkml_runtime/linkml_model/jsonschema/extensions.schema.json
--rw-r--r--   0        0        0      297 2023-05-13 02:39:28.116564 linkml_runtime-1.5.3/linkml_runtime/linkml_model/jsonschema/mappings.schema.json
--rw-r--r--   0        0        0   353208 2023-05-13 02:39:28.120564 linkml_runtime-1.5.3/linkml_runtime/linkml_model/jsonschema/meta.schema.json
--rw-r--r--   0        0        0      291 2023-05-13 02:39:28.120564 linkml_runtime-1.5.3/linkml_runtime/linkml_model/jsonschema/types.schema.json
--rw-r--r--   0        0        0     5621 2023-05-13 02:39:28.120564 linkml_runtime-1.5.3/linkml_runtime/linkml_model/jsonschema/units.schema.json
--rw-r--r--   0        0        0     2291 2023-05-13 02:39:28.120564 linkml_runtime-1.5.3/linkml_runtime/linkml_model/jsonschema/validation.schema.json
--rw-r--r--   0        0        0     7126 2023-05-13 02:39:28.120564 linkml_runtime-1.5.3/linkml_runtime/linkml_model/linkml_files.py
--rw-r--r--   0        0        0     1821 2023-05-13 02:39:28.120564 linkml_runtime-1.5.3/linkml_runtime/linkml_model/mappings.py
--rw-r--r--   0        0        0   249036 2023-05-13 02:39:28.120564 linkml_runtime-1.5.3/linkml_runtime/linkml_model/meta.py
--rw-r--r--   0        0        0      112 2023-05-13 02:39:28.120564 linkml_runtime-1.5.3/linkml_runtime/linkml_model/model/README.md
--rw-r--r--   0        0        0      118 2023-05-13 02:39:28.120564 linkml_runtime-1.5.3/linkml_runtime/linkml_model/model/docs/credits.md
--rw-r--r--   0        0        0      141 2023-05-13 02:39:28.120564 linkml_runtime-1.5.3/linkml_runtime/linkml_model/model/docs/home.md
--rw-r--r--   0        0        0        5 2023-05-13 02:39:28.120564 linkml_runtime-1.5.3/linkml_runtime/linkml_model/model/import_map.json
--rw-r--r--   0        0        0      119 2023-05-13 02:39:28.120564 linkml_runtime-1.5.3/linkml_runtime/linkml_model/model/schema/README.md
--rw-r--r--   0        0        0      833 2023-05-13 02:39:28.120564 linkml_runtime-1.5.3/linkml_runtime/linkml_model/model/schema/annotations.yaml
--rw-r--r--   0        0        0     1057 2023-05-13 02:39:28.120564 linkml_runtime-1.5.3/linkml_runtime/linkml_model/model/schema/extensions.yaml
--rw-r--r--   0        0        0     2755 2023-05-13 02:39:28.120564 linkml_runtime-1.5.3/linkml_runtime/linkml_model/model/schema/mappings.yaml
--rw-r--r--   0        0        0    89120 2023-05-13 02:39:28.120564 linkml_runtime-1.5.3/linkml_runtime/linkml_model/model/schema/meta.yaml
--rw-r--r--   0        0        0     3880 2023-05-13 02:39:28.120564 linkml_runtime-1.5.3/linkml_runtime/linkml_model/model/schema/types.yaml
--rw-r--r--   0        0        0     2776 2023-05-13 02:39:28.120564 linkml_runtime-1.5.3/linkml_runtime/linkml_model/model/schema/units.yaml
--rw-r--r--   0        0        0     2953 2023-05-13 02:39:28.120564 linkml_runtime-1.5.3/linkml_runtime/linkml_model/model/schema/validation.yaml
--rw-r--r--   0        0        0      110 2023-05-13 02:39:28.120564 linkml_runtime-1.5.3/linkml_runtime/linkml_model/owl/README.md
--rw-r--r--   0        0        0   192274 2023-05-13 02:39:28.120564 linkml_runtime-1.5.3/linkml_runtime/linkml_model/owl/meta.owl.ttl
--rw-r--r--   0        0        0      110 2023-05-13 02:39:28.120564 linkml_runtime-1.5.3/linkml_runtime/linkml_model/rdf/README.md
--rw-r--r--   0        0        0    13054 2023-05-13 02:39:28.120564 linkml_runtime-1.5.3/linkml_runtime/linkml_model/rdf/annotations.model.ttl
--rw-r--r--   0        0        0    13054 2023-05-13 02:39:28.120564 linkml_runtime-1.5.3/linkml_runtime/linkml_model/rdf/annotations.ttl
--rw-r--r--   0        0        0    10932 2023-05-13 02:39:28.120564 linkml_runtime-1.5.3/linkml_runtime/linkml_model/rdf/extensions.model.ttl
--rw-r--r--   0        0        0    10932 2023-05-13 02:39:28.120564 linkml_runtime-1.5.3/linkml_runtime/linkml_model/rdf/extensions.ttl
--rw-r--r--   0        0        0    13825 2023-05-13 02:39:28.120564 linkml_runtime-1.5.3/linkml_runtime/linkml_model/rdf/mappings.model.ttl
--rw-r--r--   0        0        0    13825 2023-05-13 02:39:28.120564 linkml_runtime-1.5.3/linkml_runtime/linkml_model/rdf/mappings.ttl
--rw-r--r--   0        0        0   207795 2023-05-13 02:39:28.124564 linkml_runtime-1.5.3/linkml_runtime/linkml_model/rdf/meta.model.ttl
--rw-r--r--   0        0        0   207795 2023-05-13 02:39:28.124564 linkml_runtime-1.5.3/linkml_runtime/linkml_model/rdf/meta.ttl
--rw-r--r--   0        0        0     7565 2023-05-13 02:39:28.124564 linkml_runtime-1.5.3/linkml_runtime/linkml_model/rdf/types.model.ttl
--rw-r--r--   0        0        0     7565 2023-05-13 02:39:28.124564 linkml_runtime-1.5.3/linkml_runtime/linkml_model/rdf/types.ttl
--rw-r--r--   0        0        0    25276 2023-05-13 02:39:28.124564 linkml_runtime-1.5.3/linkml_runtime/linkml_model/rdf/units.model.ttl
--rw-r--r--   0        0        0    25276 2023-05-13 02:39:28.124564 linkml_runtime-1.5.3/linkml_runtime/linkml_model/rdf/units.ttl
--rw-r--r--   0        0        0    16810 2023-05-13 02:39:28.124564 linkml_runtime-1.5.3/linkml_runtime/linkml_model/rdf/validation.model.ttl
--rw-r--r--   0        0        0    16810 2023-05-13 02:39:28.124564 linkml_runtime-1.5.3/linkml_runtime/linkml_model/rdf/validation.ttl
--rw-r--r--   0        0        0      113 2023-05-13 02:39:28.124564 linkml_runtime-1.5.3/linkml_runtime/linkml_model/shex/README.md
--rw-r--r--   0        0        0     1261 2023-05-13 02:39:28.124564 linkml_runtime-1.5.3/linkml_runtime/linkml_model/shex/annotations.shex
--rw-r--r--   0        0        0     8918 2023-05-13 02:39:28.124564 linkml_runtime-1.5.3/linkml_runtime/linkml_model/shex/annotations.shexj
--rw-r--r--   0        0        0      821 2023-05-13 02:39:28.124564 linkml_runtime-1.5.3/linkml_runtime/linkml_model/shex/extensions.shex
--rw-r--r--   0        0        0     5303 2023-05-13 02:39:28.124564 linkml_runtime-1.5.3/linkml_runtime/linkml_model/shex/extensions.shexj
--rw-r--r--   0        0        0      424 2023-05-13 02:39:28.124564 linkml_runtime-1.5.3/linkml_runtime/linkml_model/shex/mappings.shex
--rw-r--r--   0        0        0     2568 2023-05-13 02:39:28.124564 linkml_runtime-1.5.3/linkml_runtime/linkml_model/shex/mappings.shexj
--rw-r--r--   0        0        0    37441 2023-05-13 02:39:28.124564 linkml_runtime-1.5.3/linkml_runtime/linkml_model/shex/meta.shex
--rw-r--r--   0        0        0   254576 2023-05-13 02:39:28.124564 linkml_runtime-1.5.3/linkml_runtime/linkml_model/shex/meta.shexj
--rw-r--r--   0        0        0      459 2023-05-13 02:39:28.124564 linkml_runtime-1.5.3/linkml_runtime/linkml_model/shex/types.shex
--rw-r--r--   0        0        0     2568 2023-05-13 02:39:28.124564 linkml_runtime-1.5.3/linkml_runtime/linkml_model/shex/types.shexj
--rw-r--r--   0        0        0     1682 2023-05-13 02:39:28.124564 linkml_runtime-1.5.3/linkml_runtime/linkml_model/shex/units.shex
--rw-r--r--   0        0        0    11643 2023-05-13 02:39:28.124564 linkml_runtime-1.5.3/linkml_runtime/linkml_model/shex/units.shexj
--rw-r--r--   0        0        0     1519 2023-05-13 02:39:28.124564 linkml_runtime-1.5.3/linkml_runtime/linkml_model/shex/validation.shex
--rw-r--r--   0        0        0     7343 2023-05-13 02:39:28.124564 linkml_runtime-1.5.3/linkml_runtime/linkml_model/shex/validation.shexj
--rw-r--r--   0        0        0     4599 2023-05-13 02:39:28.124564 linkml_runtime-1.5.3/linkml_runtime/linkml_model/types.py
--rw-r--r--   0        0        0     3332 2023-05-13 02:39:28.124564 linkml_runtime-1.5.3/linkml_runtime/linkml_model/units.py
--rw-r--r--   0        0        0     6897 2023-05-13 02:39:28.124564 linkml_runtime-1.5.3/linkml_runtime/linkml_model/validation.py
--rw-r--r--   0        0        0      426 2023-05-13 02:39:28.124564 linkml_runtime-1.5.3/linkml_runtime/loaders/__init__.py
--rw-r--r--   0        0        0     1533 2023-05-13 02:39:28.124564 linkml_runtime-1.5.3/linkml_runtime/loaders/context_flattener.py
--rw-r--r--   0        0        0     2000 2023-05-13 02:39:28.124564 linkml_runtime-1.5.3/linkml_runtime/loaders/csv_loader.py
--rw-r--r--   0        0        0     1394 2023-05-13 02:39:28.124564 linkml_runtime-1.5.3/linkml_runtime/loaders/json_loader.py
--rw-r--r--   0        0        0     5919 2023-05-13 02:39:28.124564 linkml_runtime-1.5.3/linkml_runtime/loaders/loader_root.py
--rw-r--r--   0        0        0     4831 2023-05-13 02:39:28.124564 linkml_runtime-1.5.3/linkml_runtime/loaders/rdf_loader.py
--rw-r--r--   0        0        0    14214 2023-05-13 02:39:28.124564 linkml_runtime-1.5.3/linkml_runtime/loaders/rdflib_loader.py
--rw-r--r--   0        0        0     1358 2023-05-13 02:39:28.124564 linkml_runtime-1.5.3/linkml_runtime/loaders/requests_ssl_patch.py
--rw-r--r--   0        0        0     1971 2023-05-13 02:39:28.124564 linkml_runtime-1.5.3/linkml_runtime/loaders/yaml_loader.py
--rw-r--r--   0        0        0    42276 2023-05-13 02:39:28.124564 linkml_runtime-1.5.3/linkml_runtime/processing/referencevalidator.py
--rw-r--r--   0        0        0    26951 2023-05-13 02:39:28.124564 linkml_runtime-1.5.3/linkml_runtime/processing/validation_datamodel.py
--rw-r--r--   0        0        0    10253 2023-05-13 02:39:28.124564 linkml_runtime-1.5.3/linkml_runtime/processing/validation_datamodel.yaml
--rw-r--r--   0        0        0        0 2023-05-13 02:39:28.124564 linkml_runtime-1.5.3/linkml_runtime/utils/__init__.py
--rw-r--r--   0        0        0      850 2023-05-13 02:39:28.124564 linkml_runtime-1.5.3/linkml_runtime/utils/comparefiles.py
--rw-r--r--   0        0        0     1972 2023-05-13 02:39:28.124564 linkml_runtime-1.5.3/linkml_runtime/utils/compile_python.py
--rw-r--r--   0        0        0     4034 2023-05-13 02:39:28.124564 linkml_runtime-1.5.3/linkml_runtime/utils/context_utils.py
--rw-r--r--   0        0        0     2389 2023-05-13 02:39:28.124564 linkml_runtime-1.5.3/linkml_runtime/utils/csvutils.py
--rw-r--r--   0        0        0      486 2023-05-13 02:39:28.124564 linkml_runtime-1.5.3/linkml_runtime/utils/curienamespace.py
--rw-r--r--   0        0        0     1325 2023-05-13 02:39:28.124564 linkml_runtime-1.5.3/linkml_runtime/utils/dataclass_extensions_376.py
--rw-r--r--   0        0        0      433 2023-05-13 02:39:28.124564 linkml_runtime-1.5.3/linkml_runtime/utils/dictutils.py
--rw-r--r--   0        0        0     2554 2023-05-13 02:39:28.124564 linkml_runtime-1.5.3/linkml_runtime/utils/distroutils.py
--rw-r--r--   0        0        0     3683 2023-05-13 02:39:28.124564 linkml_runtime-1.5.3/linkml_runtime/utils/enumerations.py
--rw-r--r--   0        0        0     6755 2023-05-13 02:39:28.124564 linkml_runtime-1.5.3/linkml_runtime/utils/eval_utils.py
--rw-r--r--   0        0        0     6594 2023-05-13 02:39:28.124564 linkml_runtime-1.5.3/linkml_runtime/utils/formatutils.py
--rw-r--r--   0        0        0     5672 2023-05-13 02:39:28.124564 linkml_runtime-1.5.3/linkml_runtime/utils/inference_utils.py
--rw-r--r--   0        0        0     1976 2023-05-13 02:39:28.124564 linkml_runtime-1.5.3/linkml_runtime/utils/introspection.py
--rw-r--r--   0        0        0    11553 2023-05-13 02:39:28.124564 linkml_runtime-1.5.3/linkml_runtime/utils/metamodelcore.py
--rw-r--r--   0        0        0    10580 2023-05-13 02:39:28.124564 linkml_runtime-1.5.3/linkml_runtime/utils/namespaces.py
--rw-r--r--   0        0        0     2870 2023-05-13 02:39:28.128564 linkml_runtime-1.5.3/linkml_runtime/utils/pattern.py
--rw-r--r--   0        0        0     6697 2023-05-13 02:39:28.128564 linkml_runtime-1.5.3/linkml_runtime/utils/permissiblevalueimpl.py
--rw-r--r--   0        0        0     4720 2023-05-13 02:39:28.128564 linkml_runtime-1.5.3/linkml_runtime/utils/ruleutils.py
--rw-r--r--   0        0        0     2287 2023-05-13 02:39:28.128564 linkml_runtime-1.5.3/linkml_runtime/utils/schema_as_dict.py
--rw-r--r--   0        0        0     9312 2023-05-13 02:39:28.128564 linkml_runtime-1.5.3/linkml_runtime/utils/schema_builder.py
--rw-r--r--   0        0        0     2815 2023-05-13 02:39:28.128564 linkml_runtime-1.5.3/linkml_runtime/utils/schemaops.py
--rw-r--r--   0        0        0    66900 2023-05-13 02:39:28.128564 linkml_runtime-1.5.3/linkml_runtime/utils/schemaview.py
--rw-r--r--   0        0        0     4327 2023-05-13 02:39:28.128564 linkml_runtime-1.5.3/linkml_runtime/utils/schemaview_cli.py
--rw-r--r--   0        0        0      368 2023-05-13 02:39:28.128564 linkml_runtime-1.5.3/linkml_runtime/utils/slot.py
--rw-r--r--   0        0        0      641 2023-05-13 02:39:28.128564 linkml_runtime-1.5.3/linkml_runtime/utils/strictness.py
--rw-r--r--   0        0        0     1405 2023-05-13 02:39:28.128564 linkml_runtime-1.5.3/linkml_runtime/utils/walker_utils.py
--rw-r--r--   0        0        0    19743 2023-05-13 02:39:28.128564 linkml_runtime-1.5.3/linkml_runtime/utils/yamlutils.py
--rw-r--r--   0        0        0     1848 2023-05-13 02:39:44.068446 linkml_runtime-1.5.3/pyproject.toml
--rw-r--r--   0        0        0     3715 1970-01-01 00:00:00.000000 linkml_runtime-1.5.3/PKG-INFO
+-rw-r--r--   0        0        0     7048 2023-06-14 23:48:52.228740 linkml_runtime-1.5.4/LICENSE
+-rw-r--r--   0        0        0     1996 2023-06-14 23:48:52.228740 linkml_runtime-1.5.4/README.md
+-rw-r--r--   0        0        0     1179 2023-06-14 23:48:52.228740 linkml_runtime-1.5.4/linkml_runtime/__init__.py
+-rw-r--r--   0        0        0      507 2023-06-14 23:48:52.228740 linkml_runtime-1.5.4/linkml_runtime/dumpers/__init__.py
+-rw-r--r--   0        0        0      176 2023-06-14 23:48:52.228740 linkml_runtime-1.5.4/linkml_runtime/dumpers/csv_dumper.py
+-rw-r--r--   0        0        0     1418 2023-06-14 23:48:52.228740 linkml_runtime-1.5.4/linkml_runtime/dumpers/delimited_file_dumper.py
+-rw-r--r--   0        0        0      973 2023-06-14 23:48:52.228740 linkml_runtime-1.5.4/linkml_runtime/dumpers/dumper_root.py
+-rw-r--r--   0        0        0     4377 2023-06-14 23:48:52.228740 linkml_runtime-1.5.4/linkml_runtime/dumpers/json_dumper.py
+-rw-r--r--   0        0        0     4023 2023-06-14 23:48:52.228740 linkml_runtime-1.5.4/linkml_runtime/dumpers/rdf_dumper.py
+-rw-r--r--   0        0        0     7169 2023-06-14 23:48:52.228740 linkml_runtime-1.5.4/linkml_runtime/dumpers/rdflib_dumper.py
+-rw-r--r--   0        0        0      177 2023-06-14 23:48:52.228740 linkml_runtime-1.5.4/linkml_runtime/dumpers/tsv_dumper.py
+-rw-r--r--   0        0        0      901 2023-06-14 23:48:52.228740 linkml_runtime-1.5.4/linkml_runtime/dumpers/yaml_dumper.py
+-rw-r--r--   0        0        0        0 2023-06-14 23:48:52.228740 linkml_runtime-1.5.4/linkml_runtime/index/__init__.py
+-rw-r--r--   0        0        0     8875 2023-06-14 23:48:52.228740 linkml_runtime-1.5.4/linkml_runtime/index/object_index.py
+-rw-r--r--   0        0        0      119 2023-06-14 23:48:52.228740 linkml_runtime-1.5.4/linkml_runtime/linkml_model/README.md
+-rw-r--r--   0        0        0      738 2023-06-14 23:48:52.228740 linkml_runtime-1.5.4/linkml_runtime/linkml_model/__init__.py
+-rw-r--r--   0        0        0     3240 2023-06-14 23:48:52.228740 linkml_runtime-1.5.4/linkml_runtime/linkml_model/annotations.py
+-rw-r--r--   0        0        0     3333 2023-06-14 23:48:52.228740 linkml_runtime-1.5.4/linkml_runtime/linkml_model/extensions.py
+-rw-r--r--   0        0        0      114 2023-06-14 23:48:52.228740 linkml_runtime-1.5.4/linkml_runtime/linkml_model/graphql/README.md
+-rw-r--r--   0        0        0    30306 2023-06-14 23:48:52.228740 linkml_runtime-1.5.4/linkml_runtime/linkml_model/graphql/meta.graphql
+-rw-r--r--   0        0        0      111 2023-06-14 23:48:52.232740 linkml_runtime-1.5.4/linkml_runtime/linkml_model/json/README.md
+-rw-r--r--   0        0        0    11169 2023-06-14 23:48:52.232740 linkml_runtime-1.5.4/linkml_runtime/linkml_model/json/annotations.json
+-rw-r--r--   0        0        0     9306 2023-06-14 23:48:52.232740 linkml_runtime-1.5.4/linkml_runtime/linkml_model/json/extensions.json
+-rw-r--r--   0        0        0    12109 2023-06-14 23:48:52.232740 linkml_runtime-1.5.4/linkml_runtime/linkml_model/json/mappings.json
+-rw-r--r--   0        0        0   222072 2023-06-14 23:48:52.232740 linkml_runtime-1.5.4/linkml_runtime/linkml_model/json/meta.json
+-rw-r--r--   0        0        0     6442 2023-06-14 23:48:52.232740 linkml_runtime-1.5.4/linkml_runtime/linkml_model/json/types.json
+-rw-r--r--   0        0        0    22401 2023-06-14 23:48:52.232740 linkml_runtime-1.5.4/linkml_runtime/linkml_model/json/units.json
+-rw-r--r--   0        0        0    14834 2023-06-14 23:48:52.232740 linkml_runtime-1.5.4/linkml_runtime/linkml_model/json/validation.json
+-rw-r--r--   0        0        0      113 2023-06-14 23:48:52.232740 linkml_runtime-1.5.4/linkml_runtime/linkml_model/jsonld/README.md
+-rw-r--r--   0        0        0      648 2023-06-14 23:48:52.232740 linkml_runtime-1.5.4/linkml_runtime/linkml_model/jsonld/annotations.context.jsonld
+-rw-r--r--   0        0        0      648 2023-06-14 23:48:52.232740 linkml_runtime-1.5.4/linkml_runtime/linkml_model/jsonld/annotations.model.context.jsonld
+-rw-r--r--   0        0        0     7019 2023-06-14 23:48:52.232740 linkml_runtime-1.5.4/linkml_runtime/linkml_model/jsonld/context.jsonld
+-rw-r--r--   0        0        0      587 2023-06-14 23:48:52.232740 linkml_runtime-1.5.4/linkml_runtime/linkml_model/jsonld/extensions.context.jsonld
+-rw-r--r--   0        0        0      587 2023-06-14 23:48:52.232740 linkml_runtime-1.5.4/linkml_runtime/linkml_model/jsonld/extensions.model.context.jsonld
+-rw-r--r--   0        0        0     1615 2023-06-14 23:48:52.232740 linkml_runtime-1.5.4/linkml_runtime/linkml_model/jsonld/mappings.context.jsonld
+-rw-r--r--   0        0        0     1615 2023-06-14 23:48:52.232740 linkml_runtime-1.5.4/linkml_runtime/linkml_model/jsonld/mappings.model.context.jsonld
+-rw-r--r--   0        0        0    13814 2023-06-14 23:48:52.232740 linkml_runtime-1.5.4/linkml_runtime/linkml_model/jsonld/meta.context.jsonld
+-rw-r--r--   0        0        0    14266 2023-06-14 23:48:52.232740 linkml_runtime-1.5.4/linkml_runtime/linkml_model/jsonld/meta.model.context.jsonld
+-rw-r--r--   0        0        0      610 2023-06-14 23:48:52.232740 linkml_runtime-1.5.4/linkml_runtime/linkml_model/jsonld/types.context.jsonld
+-rw-r--r--   0        0        0      610 2023-06-14 23:48:52.232740 linkml_runtime-1.5.4/linkml_runtime/linkml_model/jsonld/types.model.context.jsonld
+-rw-r--r--   0        0        0     2065 2023-06-14 23:48:52.232740 linkml_runtime-1.5.4/linkml_runtime/linkml_model/jsonld/units.context.jsonld
+-rw-r--r--   0        0        0     2065 2023-06-14 23:48:52.232740 linkml_runtime-1.5.4/linkml_runtime/linkml_model/jsonld/units.model.context.jsonld
+-rw-r--r--   0        0        0     1910 2023-06-14 23:48:52.232740 linkml_runtime-1.5.4/linkml_runtime/linkml_model/jsonld/validation.context.jsonld
+-rw-r--r--   0        0        0     1910 2023-06-14 23:48:52.232740 linkml_runtime-1.5.4/linkml_runtime/linkml_model/jsonld/validation.model.context.jsonld
+-rw-r--r--   0        0        0      117 2023-06-14 23:48:52.232740 linkml_runtime-1.5.4/linkml_runtime/linkml_model/jsonschema/README.md
+-rw-r--r--   0        0        0     4196 2023-06-14 23:48:52.232740 linkml_runtime-1.5.4/linkml_runtime/linkml_model/jsonschema/annotations.schema.json
+-rw-r--r--   0        0        0     1984 2023-06-14 23:48:52.232740 linkml_runtime-1.5.4/linkml_runtime/linkml_model/jsonschema/extensions.schema.json
+-rw-r--r--   0        0        0      297 2023-06-14 23:48:52.232740 linkml_runtime-1.5.4/linkml_runtime/linkml_model/jsonschema/mappings.schema.json
+-rw-r--r--   0        0        0   353208 2023-06-14 23:48:52.232740 linkml_runtime-1.5.4/linkml_runtime/linkml_model/jsonschema/meta.schema.json
+-rw-r--r--   0        0        0      291 2023-06-14 23:48:52.232740 linkml_runtime-1.5.4/linkml_runtime/linkml_model/jsonschema/types.schema.json
+-rw-r--r--   0        0        0     5621 2023-06-14 23:48:52.232740 linkml_runtime-1.5.4/linkml_runtime/linkml_model/jsonschema/units.schema.json
+-rw-r--r--   0        0        0     2291 2023-06-14 23:48:52.232740 linkml_runtime-1.5.4/linkml_runtime/linkml_model/jsonschema/validation.schema.json
+-rw-r--r--   0        0        0     7126 2023-06-14 23:48:52.232740 linkml_runtime-1.5.4/linkml_runtime/linkml_model/linkml_files.py
+-rw-r--r--   0        0        0     1821 2023-06-14 23:48:52.232740 linkml_runtime-1.5.4/linkml_runtime/linkml_model/mappings.py
+-rw-r--r--   0        0        0   249036 2023-06-14 23:48:52.236741 linkml_runtime-1.5.4/linkml_runtime/linkml_model/meta.py
+-rw-r--r--   0        0        0      112 2023-06-14 23:48:52.236741 linkml_runtime-1.5.4/linkml_runtime/linkml_model/model/README.md
+-rw-r--r--   0        0        0      118 2023-06-14 23:48:52.236741 linkml_runtime-1.5.4/linkml_runtime/linkml_model/model/docs/credits.md
+-rw-r--r--   0        0        0      141 2023-06-14 23:48:52.236741 linkml_runtime-1.5.4/linkml_runtime/linkml_model/model/docs/home.md
+-rw-r--r--   0        0        0        5 2023-06-14 23:48:52.236741 linkml_runtime-1.5.4/linkml_runtime/linkml_model/model/import_map.json
+-rw-r--r--   0        0        0      119 2023-06-14 23:48:52.236741 linkml_runtime-1.5.4/linkml_runtime/linkml_model/model/schema/README.md
+-rw-r--r--   0        0        0      833 2023-06-14 23:48:52.236741 linkml_runtime-1.5.4/linkml_runtime/linkml_model/model/schema/annotations.yaml
+-rw-r--r--   0        0        0     1057 2023-06-14 23:48:52.236741 linkml_runtime-1.5.4/linkml_runtime/linkml_model/model/schema/extensions.yaml
+-rw-r--r--   0        0        0     2755 2023-06-14 23:48:52.236741 linkml_runtime-1.5.4/linkml_runtime/linkml_model/model/schema/mappings.yaml
+-rw-r--r--   0        0        0    89120 2023-06-14 23:48:52.236741 linkml_runtime-1.5.4/linkml_runtime/linkml_model/model/schema/meta.yaml
+-rw-r--r--   0        0        0     3880 2023-06-14 23:48:52.236741 linkml_runtime-1.5.4/linkml_runtime/linkml_model/model/schema/types.yaml
+-rw-r--r--   0        0        0     2776 2023-06-14 23:48:52.236741 linkml_runtime-1.5.4/linkml_runtime/linkml_model/model/schema/units.yaml
+-rw-r--r--   0        0        0     2953 2023-06-14 23:48:52.236741 linkml_runtime-1.5.4/linkml_runtime/linkml_model/model/schema/validation.yaml
+-rw-r--r--   0        0        0      110 2023-06-14 23:48:52.236741 linkml_runtime-1.5.4/linkml_runtime/linkml_model/owl/README.md
+-rw-r--r--   0        0        0   192274 2023-06-14 23:48:52.236741 linkml_runtime-1.5.4/linkml_runtime/linkml_model/owl/meta.owl.ttl
+-rw-r--r--   0        0        0      110 2023-06-14 23:48:52.236741 linkml_runtime-1.5.4/linkml_runtime/linkml_model/rdf/README.md
+-rw-r--r--   0        0        0    13054 2023-06-14 23:48:52.236741 linkml_runtime-1.5.4/linkml_runtime/linkml_model/rdf/annotations.model.ttl
+-rw-r--r--   0        0        0    13054 2023-06-14 23:48:52.236741 linkml_runtime-1.5.4/linkml_runtime/linkml_model/rdf/annotations.ttl
+-rw-r--r--   0        0        0    10932 2023-06-14 23:48:52.236741 linkml_runtime-1.5.4/linkml_runtime/linkml_model/rdf/extensions.model.ttl
+-rw-r--r--   0        0        0    10932 2023-06-14 23:48:52.236741 linkml_runtime-1.5.4/linkml_runtime/linkml_model/rdf/extensions.ttl
+-rw-r--r--   0        0        0    13825 2023-06-14 23:48:52.236741 linkml_runtime-1.5.4/linkml_runtime/linkml_model/rdf/mappings.model.ttl
+-rw-r--r--   0        0        0    13825 2023-06-14 23:48:52.236741 linkml_runtime-1.5.4/linkml_runtime/linkml_model/rdf/mappings.ttl
+-rw-r--r--   0        0        0   207795 2023-06-14 23:48:52.236741 linkml_runtime-1.5.4/linkml_runtime/linkml_model/rdf/meta.model.ttl
+-rw-r--r--   0        0        0   207795 2023-06-14 23:48:52.240741 linkml_runtime-1.5.4/linkml_runtime/linkml_model/rdf/meta.ttl
+-rw-r--r--   0        0        0     7565 2023-06-14 23:48:52.240741 linkml_runtime-1.5.4/linkml_runtime/linkml_model/rdf/types.model.ttl
+-rw-r--r--   0        0        0     7565 2023-06-14 23:48:52.240741 linkml_runtime-1.5.4/linkml_runtime/linkml_model/rdf/types.ttl
+-rw-r--r--   0        0        0    25276 2023-06-14 23:48:52.240741 linkml_runtime-1.5.4/linkml_runtime/linkml_model/rdf/units.model.ttl
+-rw-r--r--   0        0        0    25276 2023-06-14 23:48:52.240741 linkml_runtime-1.5.4/linkml_runtime/linkml_model/rdf/units.ttl
+-rw-r--r--   0        0        0    16810 2023-06-14 23:48:52.240741 linkml_runtime-1.5.4/linkml_runtime/linkml_model/rdf/validation.model.ttl
+-rw-r--r--   0        0        0    16810 2023-06-14 23:48:52.240741 linkml_runtime-1.5.4/linkml_runtime/linkml_model/rdf/validation.ttl
+-rw-r--r--   0        0        0      113 2023-06-14 23:48:52.240741 linkml_runtime-1.5.4/linkml_runtime/linkml_model/shex/README.md
+-rw-r--r--   0        0        0     1261 2023-06-14 23:48:52.240741 linkml_runtime-1.5.4/linkml_runtime/linkml_model/shex/annotations.shex
+-rw-r--r--   0        0        0     8918 2023-06-14 23:48:52.240741 linkml_runtime-1.5.4/linkml_runtime/linkml_model/shex/annotations.shexj
+-rw-r--r--   0        0        0      821 2023-06-14 23:48:52.240741 linkml_runtime-1.5.4/linkml_runtime/linkml_model/shex/extensions.shex
+-rw-r--r--   0        0        0     5303 2023-06-14 23:48:52.240741 linkml_runtime-1.5.4/linkml_runtime/linkml_model/shex/extensions.shexj
+-rw-r--r--   0        0        0      424 2023-06-14 23:48:52.240741 linkml_runtime-1.5.4/linkml_runtime/linkml_model/shex/mappings.shex
+-rw-r--r--   0        0        0     2568 2023-06-14 23:48:52.240741 linkml_runtime-1.5.4/linkml_runtime/linkml_model/shex/mappings.shexj
+-rw-r--r--   0        0        0    37441 2023-06-14 23:48:52.240741 linkml_runtime-1.5.4/linkml_runtime/linkml_model/shex/meta.shex
+-rw-r--r--   0        0        0   254576 2023-06-14 23:48:52.240741 linkml_runtime-1.5.4/linkml_runtime/linkml_model/shex/meta.shexj
+-rw-r--r--   0        0        0      459 2023-06-14 23:48:52.240741 linkml_runtime-1.5.4/linkml_runtime/linkml_model/shex/types.shex
+-rw-r--r--   0        0        0     2568 2023-06-14 23:48:52.240741 linkml_runtime-1.5.4/linkml_runtime/linkml_model/shex/types.shexj
+-rw-r--r--   0        0        0     1682 2023-06-14 23:48:52.240741 linkml_runtime-1.5.4/linkml_runtime/linkml_model/shex/units.shex
+-rw-r--r--   0        0        0    11643 2023-06-14 23:48:52.240741 linkml_runtime-1.5.4/linkml_runtime/linkml_model/shex/units.shexj
+-rw-r--r--   0        0        0     1519 2023-06-14 23:48:52.240741 linkml_runtime-1.5.4/linkml_runtime/linkml_model/shex/validation.shex
+-rw-r--r--   0        0        0     7343 2023-06-14 23:48:52.240741 linkml_runtime-1.5.4/linkml_runtime/linkml_model/shex/validation.shexj
+-rw-r--r--   0        0        0     4599 2023-06-14 23:48:52.240741 linkml_runtime-1.5.4/linkml_runtime/linkml_model/types.py
+-rw-r--r--   0        0        0     3332 2023-06-14 23:48:52.240741 linkml_runtime-1.5.4/linkml_runtime/linkml_model/units.py
+-rw-r--r--   0        0        0     6897 2023-06-14 23:48:52.240741 linkml_runtime-1.5.4/linkml_runtime/linkml_model/validation.py
+-rw-r--r--   0        0        0      507 2023-06-14 23:48:52.240741 linkml_runtime-1.5.4/linkml_runtime/loaders/__init__.py
+-rw-r--r--   0        0        0     1533 2023-06-14 23:48:52.240741 linkml_runtime-1.5.4/linkml_runtime/loaders/context_flattener.py
+-rw-r--r--   0        0        0      179 2023-06-14 23:48:52.240741 linkml_runtime-1.5.4/linkml_runtime/loaders/csv_loader.py
+-rw-r--r--   0        0        0     2776 2023-06-14 23:48:52.240741 linkml_runtime-1.5.4/linkml_runtime/loaders/delimited_file_loader.py
+-rw-r--r--   0        0        0     1574 2023-06-14 23:48:52.240741 linkml_runtime-1.5.4/linkml_runtime/loaders/json_loader.py
+-rw-r--r--   0        0        0     6855 2023-06-14 23:48:52.240741 linkml_runtime-1.5.4/linkml_runtime/loaders/loader_root.py
+-rw-r--r--   0        0        0     4831 2023-06-14 23:48:52.240741 linkml_runtime-1.5.4/linkml_runtime/loaders/rdf_loader.py
+-rw-r--r--   0        0        0    14214 2023-06-14 23:48:52.240741 linkml_runtime-1.5.4/linkml_runtime/loaders/rdflib_loader.py
+-rw-r--r--   0        0        0     1358 2023-06-14 23:48:52.240741 linkml_runtime-1.5.4/linkml_runtime/loaders/requests_ssl_patch.py
+-rw-r--r--   0        0        0      180 2023-06-14 23:48:52.240741 linkml_runtime-1.5.4/linkml_runtime/loaders/tsv_loader.py
+-rw-r--r--   0        0        0     2223 2023-06-14 23:48:52.240741 linkml_runtime-1.5.4/linkml_runtime/loaders/yaml_loader.py
+-rw-r--r--   0        0        0    42276 2023-06-14 23:48:52.244741 linkml_runtime-1.5.4/linkml_runtime/processing/referencevalidator.py
+-rw-r--r--   0        0        0    26951 2023-06-14 23:48:52.244741 linkml_runtime-1.5.4/linkml_runtime/processing/validation_datamodel.py
+-rw-r--r--   0        0        0    10253 2023-06-14 23:48:52.244741 linkml_runtime-1.5.4/linkml_runtime/processing/validation_datamodel.yaml
+-rw-r--r--   0        0        0        0 2023-06-14 23:48:52.244741 linkml_runtime-1.5.4/linkml_runtime/utils/__init__.py
+-rw-r--r--   0        0        0      850 2023-06-14 23:48:52.244741 linkml_runtime-1.5.4/linkml_runtime/utils/comparefiles.py
+-rw-r--r--   0        0        0     1972 2023-06-14 23:48:52.244741 linkml_runtime-1.5.4/linkml_runtime/utils/compile_python.py
+-rw-r--r--   0        0        0     4034 2023-06-14 23:48:52.244741 linkml_runtime-1.5.4/linkml_runtime/utils/context_utils.py
+-rw-r--r--   0        0        0     2389 2023-06-14 23:48:52.244741 linkml_runtime-1.5.4/linkml_runtime/utils/csvutils.py
+-rw-r--r--   0        0        0      486 2023-06-14 23:48:52.244741 linkml_runtime-1.5.4/linkml_runtime/utils/curienamespace.py
+-rw-r--r--   0        0        0     1325 2023-06-14 23:48:52.244741 linkml_runtime-1.5.4/linkml_runtime/utils/dataclass_extensions_376.py
+-rw-r--r--   0        0        0      433 2023-06-14 23:48:52.244741 linkml_runtime-1.5.4/linkml_runtime/utils/dictutils.py
+-rw-r--r--   0        0        0     2554 2023-06-14 23:48:52.244741 linkml_runtime-1.5.4/linkml_runtime/utils/distroutils.py
+-rw-r--r--   0        0        0     3683 2023-06-14 23:48:52.244741 linkml_runtime-1.5.4/linkml_runtime/utils/enumerations.py
+-rw-r--r--   0        0        0     6755 2023-06-14 23:48:52.244741 linkml_runtime-1.5.4/linkml_runtime/utils/eval_utils.py
+-rw-r--r--   0        0        0     6594 2023-06-14 23:48:52.244741 linkml_runtime-1.5.4/linkml_runtime/utils/formatutils.py
+-rw-r--r--   0        0        0     5672 2023-06-14 23:48:52.244741 linkml_runtime-1.5.4/linkml_runtime/utils/inference_utils.py
+-rw-r--r--   0        0        0     1976 2023-06-14 23:48:52.244741 linkml_runtime-1.5.4/linkml_runtime/utils/introspection.py
+-rw-r--r--   0        0        0    11553 2023-06-14 23:48:52.244741 linkml_runtime-1.5.4/linkml_runtime/utils/metamodelcore.py
+-rw-r--r--   0        0        0    10580 2023-06-14 23:48:52.244741 linkml_runtime-1.5.4/linkml_runtime/utils/namespaces.py
+-rw-r--r--   0        0        0     2870 2023-06-14 23:48:52.244741 linkml_runtime-1.5.4/linkml_runtime/utils/pattern.py
+-rw-r--r--   0        0        0     6697 2023-06-14 23:48:52.244741 linkml_runtime-1.5.4/linkml_runtime/utils/permissiblevalueimpl.py
+-rw-r--r--   0        0        0     4720 2023-06-14 23:48:52.244741 linkml_runtime-1.5.4/linkml_runtime/utils/ruleutils.py
+-rw-r--r--   0        0        0     2287 2023-06-14 23:48:52.244741 linkml_runtime-1.5.4/linkml_runtime/utils/schema_as_dict.py
+-rw-r--r--   0        0        0     9312 2023-06-14 23:48:52.244741 linkml_runtime-1.5.4/linkml_runtime/utils/schema_builder.py
+-rw-r--r--   0        0        0     2815 2023-06-14 23:48:52.244741 linkml_runtime-1.5.4/linkml_runtime/utils/schemaops.py
+-rw-r--r--   0        0        0    66900 2023-06-14 23:48:52.244741 linkml_runtime-1.5.4/linkml_runtime/utils/schemaview.py
+-rw-r--r--   0        0        0     4327 2023-06-14 23:48:52.244741 linkml_runtime-1.5.4/linkml_runtime/utils/schemaview_cli.py
+-rw-r--r--   0        0        0      368 2023-06-14 23:48:52.244741 linkml_runtime-1.5.4/linkml_runtime/utils/slot.py
+-rw-r--r--   0        0        0      641 2023-06-14 23:48:52.244741 linkml_runtime-1.5.4/linkml_runtime/utils/strictness.py
+-rw-r--r--   0        0        0     1405 2023-06-14 23:48:52.244741 linkml_runtime-1.5.4/linkml_runtime/utils/walker_utils.py
+-rw-r--r--   0        0        0    19743 2023-06-14 23:48:52.244741 linkml_runtime-1.5.4/linkml_runtime/utils/yamlutils.py
+-rw-r--r--   0        0        0     1848 2023-06-14 23:49:12.821710 linkml_runtime-1.5.4/pyproject.toml
+-rw-r--r--   0        0        0     3616 1970-01-01 00:00:00.000000 linkml_runtime-1.5.4/PKG-INFO
```

### Comparing `linkml_runtime-1.5.3/LICENSE` & `linkml_runtime-1.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.3/README.md` & `linkml_runtime-1.5.4/README.md`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.3/linkml_runtime/__init__.py` & `linkml_runtime-1.5.4/linkml_runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.3/linkml_runtime/dumpers/dumper_root.py` & `linkml_runtime-1.5.4/linkml_runtime/dumpers/dumper_root.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.3/linkml_runtime/dumpers/json_dumper.py` & `linkml_runtime-1.5.4/linkml_runtime/dumpers/json_dumper.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.3/linkml_runtime/dumpers/rdf_dumper.py` & `linkml_runtime-1.5.4/linkml_runtime/dumpers/rdf_dumper.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.3/linkml_runtime/dumpers/rdflib_dumper.py` & `linkml_runtime-1.5.4/linkml_runtime/dumpers/rdflib_dumper.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.3/linkml_runtime/dumpers/yaml_dumper.py` & `linkml_runtime-1.5.4/linkml_runtime/dumpers/yaml_dumper.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.3/linkml_runtime/index/object_index.py` & `linkml_runtime-1.5.4/linkml_runtime/index/object_index.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.3/linkml_runtime/linkml_model/__init__.py` & `linkml_runtime-1.5.4/linkml_runtime/linkml_model/__init__.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.3/linkml_runtime/linkml_model/annotations.py` & `linkml_runtime-1.5.4/linkml_runtime/linkml_model/annotations.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.3/linkml_runtime/linkml_model/extensions.py` & `linkml_runtime-1.5.4/linkml_runtime/linkml_model/extensions.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.3/linkml_runtime/linkml_model/graphql/meta.graphql` & `linkml_runtime-1.5.4/linkml_runtime/linkml_model/graphql/meta.graphql`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.3/linkml_runtime/linkml_model/json/annotations.json` & `linkml_runtime-1.5.4/linkml_runtime/linkml_model/json/annotations.json`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.3/linkml_runtime/linkml_model/json/extensions.json` & `linkml_runtime-1.5.4/linkml_runtime/linkml_model/json/extensions.json`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.3/linkml_runtime/linkml_model/json/mappings.json` & `linkml_runtime-1.5.4/linkml_runtime/linkml_model/json/mappings.json`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.3/linkml_runtime/linkml_model/json/meta.json` & `linkml_runtime-1.5.4/linkml_runtime/linkml_model/json/meta.json`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.3/linkml_runtime/linkml_model/json/types.json` & `linkml_runtime-1.5.4/linkml_runtime/linkml_model/json/types.json`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.3/linkml_runtime/linkml_model/json/units.json` & `linkml_runtime-1.5.4/linkml_runtime/linkml_model/json/units.json`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.3/linkml_runtime/linkml_model/json/validation.json` & `linkml_runtime-1.5.4/linkml_runtime/linkml_model/json/validation.json`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.3/linkml_runtime/linkml_model/jsonld/annotations.context.jsonld` & `linkml_runtime-1.5.4/linkml_runtime/linkml_model/jsonld/annotations.context.jsonld`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.3/linkml_runtime/linkml_model/jsonld/annotations.model.context.jsonld` & `linkml_runtime-1.5.4/linkml_runtime/linkml_model/jsonld/annotations.model.context.jsonld`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.3/linkml_runtime/linkml_model/jsonld/context.jsonld` & `linkml_runtime-1.5.4/linkml_runtime/linkml_model/jsonld/context.jsonld`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.3/linkml_runtime/linkml_model/jsonld/extensions.context.jsonld` & `linkml_runtime-1.5.4/linkml_runtime/linkml_model/jsonld/extensions.context.jsonld`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.3/linkml_runtime/linkml_model/jsonld/extensions.model.context.jsonld` & `linkml_runtime-1.5.4/linkml_runtime/linkml_model/jsonld/extensions.model.context.jsonld`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.3/linkml_runtime/linkml_model/jsonld/mappings.context.jsonld` & `linkml_runtime-1.5.4/linkml_runtime/linkml_model/jsonld/mappings.context.jsonld`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.3/linkml_runtime/linkml_model/jsonld/mappings.model.context.jsonld` & `linkml_runtime-1.5.4/linkml_runtime/linkml_model/jsonld/mappings.model.context.jsonld`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.3/linkml_runtime/linkml_model/jsonld/meta.context.jsonld` & `linkml_runtime-1.5.4/linkml_runtime/linkml_model/jsonld/meta.context.jsonld`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.3/linkml_runtime/linkml_model/jsonld/meta.model.context.jsonld` & `linkml_runtime-1.5.4/linkml_runtime/linkml_model/jsonld/meta.model.context.jsonld`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.3/linkml_runtime/linkml_model/jsonld/types.context.jsonld` & `linkml_runtime-1.5.4/linkml_runtime/linkml_model/jsonld/types.context.jsonld`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.3/linkml_runtime/linkml_model/jsonld/types.model.context.jsonld` & `linkml_runtime-1.5.4/linkml_runtime/linkml_model/jsonld/types.model.context.jsonld`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.3/linkml_runtime/linkml_model/jsonld/units.context.jsonld` & `linkml_runtime-1.5.4/linkml_runtime/linkml_model/jsonld/units.context.jsonld`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.3/linkml_runtime/linkml_model/jsonld/units.model.context.jsonld` & `linkml_runtime-1.5.4/linkml_runtime/linkml_model/jsonld/units.model.context.jsonld`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.3/linkml_runtime/linkml_model/jsonld/validation.context.jsonld` & `linkml_runtime-1.5.4/linkml_runtime/linkml_model/jsonld/validation.context.jsonld`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.3/linkml_runtime/linkml_model/jsonld/validation.model.context.jsonld` & `linkml_runtime-1.5.4/linkml_runtime/linkml_model/jsonld/validation.model.context.jsonld`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.3/linkml_runtime/linkml_model/jsonschema/annotations.schema.json` & `linkml_runtime-1.5.4/linkml_runtime/linkml_model/jsonschema/annotations.schema.json`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.3/linkml_runtime/linkml_model/jsonschema/extensions.schema.json` & `linkml_runtime-1.5.4/linkml_runtime/linkml_model/jsonschema/extensions.schema.json`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.3/linkml_runtime/linkml_model/jsonschema/meta.schema.json` & `linkml_runtime-1.5.4/linkml_runtime/linkml_model/jsonschema/meta.schema.json`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.3/linkml_runtime/linkml_model/jsonschema/units.schema.json` & `linkml_runtime-1.5.4/linkml_runtime/linkml_model/jsonschema/units.schema.json`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.3/linkml_runtime/linkml_model/jsonschema/validation.schema.json` & `linkml_runtime-1.5.4/linkml_runtime/linkml_model/jsonschema/validation.schema.json`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.3/linkml_runtime/linkml_model/linkml_files.py` & `linkml_runtime-1.5.4/linkml_runtime/linkml_model/linkml_files.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.3/linkml_runtime/linkml_model/mappings.py` & `linkml_runtime-1.5.4/linkml_runtime/linkml_model/mappings.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.3/linkml_runtime/linkml_model/meta.py` & `linkml_runtime-1.5.4/linkml_runtime/linkml_model/meta.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.3/linkml_runtime/linkml_model/model/schema/annotations.yaml` & `linkml_runtime-1.5.4/linkml_runtime/linkml_model/model/schema/annotations.yaml`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.3/linkml_runtime/linkml_model/model/schema/extensions.yaml` & `linkml_runtime-1.5.4/linkml_runtime/linkml_model/model/schema/extensions.yaml`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.3/linkml_runtime/linkml_model/model/schema/mappings.yaml` & `linkml_runtime-1.5.4/linkml_runtime/linkml_model/model/schema/mappings.yaml`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.3/linkml_runtime/linkml_model/model/schema/meta.yaml` & `linkml_runtime-1.5.4/linkml_runtime/linkml_model/model/schema/meta.yaml`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.3/linkml_runtime/linkml_model/model/schema/types.yaml` & `linkml_runtime-1.5.4/linkml_runtime/linkml_model/model/schema/types.yaml`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.3/linkml_runtime/linkml_model/model/schema/units.yaml` & `linkml_runtime-1.5.4/linkml_runtime/linkml_model/model/schema/units.yaml`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.3/linkml_runtime/linkml_model/model/schema/validation.yaml` & `linkml_runtime-1.5.4/linkml_runtime/linkml_model/model/schema/validation.yaml`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.3/linkml_runtime/linkml_model/owl/meta.owl.ttl` & `linkml_runtime-1.5.4/linkml_runtime/linkml_model/owl/meta.owl.ttl`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.3/linkml_runtime/linkml_model/rdf/annotations.model.ttl` & `linkml_runtime-1.5.4/linkml_runtime/linkml_model/rdf/annotations.model.ttl`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.3/linkml_runtime/linkml_model/rdf/annotations.ttl` & `linkml_runtime-1.5.4/linkml_runtime/linkml_model/rdf/annotations.ttl`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.3/linkml_runtime/linkml_model/rdf/extensions.model.ttl` & `linkml_runtime-1.5.4/linkml_runtime/linkml_model/rdf/extensions.model.ttl`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.3/linkml_runtime/linkml_model/rdf/extensions.ttl` & `linkml_runtime-1.5.4/linkml_runtime/linkml_model/rdf/extensions.ttl`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.3/linkml_runtime/linkml_model/rdf/mappings.model.ttl` & `linkml_runtime-1.5.4/linkml_runtime/linkml_model/rdf/mappings.model.ttl`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.3/linkml_runtime/linkml_model/rdf/mappings.ttl` & `linkml_runtime-1.5.4/linkml_runtime/linkml_model/rdf/mappings.ttl`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.3/linkml_runtime/linkml_model/rdf/meta.model.ttl` & `linkml_runtime-1.5.4/linkml_runtime/linkml_model/rdf/meta.model.ttl`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.3/linkml_runtime/linkml_model/rdf/meta.ttl` & `linkml_runtime-1.5.4/linkml_runtime/linkml_model/rdf/meta.ttl`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.3/linkml_runtime/linkml_model/rdf/types.model.ttl` & `linkml_runtime-1.5.4/linkml_runtime/linkml_model/rdf/types.model.ttl`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.3/linkml_runtime/linkml_model/rdf/types.ttl` & `linkml_runtime-1.5.4/linkml_runtime/linkml_model/rdf/types.ttl`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.3/linkml_runtime/linkml_model/rdf/units.model.ttl` & `linkml_runtime-1.5.4/linkml_runtime/linkml_model/rdf/units.model.ttl`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.3/linkml_runtime/linkml_model/rdf/units.ttl` & `linkml_runtime-1.5.4/linkml_runtime/linkml_model/rdf/units.ttl`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.3/linkml_runtime/linkml_model/rdf/validation.model.ttl` & `linkml_runtime-1.5.4/linkml_runtime/linkml_model/rdf/validation.model.ttl`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.3/linkml_runtime/linkml_model/rdf/validation.ttl` & `linkml_runtime-1.5.4/linkml_runtime/linkml_model/rdf/validation.ttl`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.3/linkml_runtime/linkml_model/shex/annotations.shex` & `linkml_runtime-1.5.4/linkml_runtime/linkml_model/shex/annotations.shex`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.3/linkml_runtime/linkml_model/shex/annotations.shexj` & `linkml_runtime-1.5.4/linkml_runtime/linkml_model/shex/annotations.shexj`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.3/linkml_runtime/linkml_model/shex/extensions.shex` & `linkml_runtime-1.5.4/linkml_runtime/linkml_model/shex/extensions.shex`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.3/linkml_runtime/linkml_model/shex/extensions.shexj` & `linkml_runtime-1.5.4/linkml_runtime/linkml_model/shex/extensions.shexj`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.3/linkml_runtime/linkml_model/shex/mappings.shexj` & `linkml_runtime-1.5.4/linkml_runtime/linkml_model/shex/mappings.shexj`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.3/linkml_runtime/linkml_model/shex/meta.shex` & `linkml_runtime-1.5.4/linkml_runtime/linkml_model/shex/meta.shex`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.3/linkml_runtime/linkml_model/shex/meta.shexj` & `linkml_runtime-1.5.4/linkml_runtime/linkml_model/shex/meta.shexj`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.3/linkml_runtime/linkml_model/shex/types.shexj` & `linkml_runtime-1.5.4/linkml_runtime/linkml_model/shex/types.shexj`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.3/linkml_runtime/linkml_model/shex/units.shex` & `linkml_runtime-1.5.4/linkml_runtime/linkml_model/shex/units.shex`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.3/linkml_runtime/linkml_model/shex/units.shexj` & `linkml_runtime-1.5.4/linkml_runtime/linkml_model/shex/units.shexj`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.3/linkml_runtime/linkml_model/shex/validation.shex` & `linkml_runtime-1.5.4/linkml_runtime/linkml_model/shex/validation.shex`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.3/linkml_runtime/linkml_model/shex/validation.shexj` & `linkml_runtime-1.5.4/linkml_runtime/linkml_model/shex/validation.shexj`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.3/linkml_runtime/linkml_model/types.py` & `linkml_runtime-1.5.4/linkml_runtime/linkml_model/types.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.3/linkml_runtime/linkml_model/units.py` & `linkml_runtime-1.5.4/linkml_runtime/linkml_model/units.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.3/linkml_runtime/linkml_model/validation.py` & `linkml_runtime-1.5.4/linkml_runtime/linkml_model/validation.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.3/linkml_runtime/loaders/context_flattener.py` & `linkml_runtime-1.5.4/linkml_runtime/loaders/context_flattener.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.3/linkml_runtime/loaders/csv_loader.py` & `linkml_runtime-1.5.4/linkml_runtime/loaders/delimited_file_loader.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,45 +1,63 @@
+from abc import ABC, abstractmethod
 from json_flattener import unflatten_from_csv, KeyConfig, GlobalConfig, Serializer
 import json
 from typing import Type, Union, List
 from linkml_runtime.utils.yamlutils import YAMLRoot
 from pydantic import BaseModel
 
 from linkml_runtime.loaders.loader_root import Loader
 from linkml_runtime.loaders.json_loader import JSONLoader
 from linkml_runtime.linkml_model.meta import SlotDefinitionName, SchemaDefinition, ClassDefinition
 from linkml_runtime.utils.yamlutils import YAMLRoot
 from linkml_runtime.utils.schemaview import SchemaView
 from linkml_runtime.utils.csvutils import get_configmap
 
-class CSVLoader(Loader):
+class DelimitedFileLoader(Loader, ABC):
+
+    @property
+    @abstractmethod
+    def delimiter(self):
+        pass
+
+    def load_as_dict(self, 
+                     source: str,
+                     index_slot: SlotDefinitionName = None,
+                     schema: SchemaDefinition = None,
+                     schemaview: SchemaView = None,
+                     **kwargs) -> Union[dict, List[dict]]:
+        json_str = self._get_json_str_to_load(source, index_slot, schema, schemaview, **kwargs)
+        return JSONLoader().load_as_dict(json_str)
 
     def load_any(self, *args, **kwargs) -> Union[YAMLRoot, List[YAMLRoot]]:
         return self.load(*args, **kwargs)
 
-
     def loads(self, input,
               target_class: Type[Union[BaseModel, YAMLRoot]],
               index_slot: SlotDefinitionName = None,
               schema: SchemaDefinition = None,
               schemaview: SchemaView = None,
               **kwargs) -> str:
-        if schemaview is None:
-            schemaview = SchemaView(schema)
-        configmap = get_configmap(schemaview, index_slot)
-        config = GlobalConfig(key_configs=configmap)
-        objs = unflatten_from_csv(input, config=config, **kwargs)
-        return JSONLoader().loads(json.dumps({index_slot: objs}), target_class=target_class)
+        json_str = self._get_json_str_to_load(input, index_slot, schema, schemaview, **kwargs)
+        return JSONLoader().loads(json_str, target_class=target_class)
 
     def load(self, source: str,
              target_class: Type[Union[BaseModel, YAMLRoot]],
              index_slot: SlotDefinitionName = None,
              schema: SchemaDefinition = None,
              schemaview: SchemaView = None,
              **kwargs) -> str:
+        json_str = self._get_json_str_to_load(source, index_slot, schema, schemaview, **kwargs)
+        return JSONLoader().loads(json_str, target_class=target_class)
+
+    def _get_json_str_to_load(self,
+                          input,
+                          index_slot: SlotDefinitionName = None,
+                          schema: SchemaDefinition = None,
+                          schemaview: SchemaView = None,
+                          **kwargs):
         if schemaview is None:
             schemaview = SchemaView(schema)
         configmap = get_configmap(schemaview, index_slot)
-        config = GlobalConfig(key_configs=configmap)
-        print(f'Loading from {source}')
-        objs = unflatten_from_csv(source, config=config, **kwargs)
-        return JSONLoader().loads(json.dumps({index_slot: objs}), target_class=target_class)
+        config = GlobalConfig(key_configs=configmap, csv_delimiter=self.delimiter)
+        objs = unflatten_from_csv(input, config=config, **kwargs)
+        return json.dumps({index_slot: objs})
```

### Comparing `linkml_runtime-1.5.3/linkml_runtime/loaders/json_loader.py` & `linkml_runtime-1.5.4/linkml_runtime/loaders/json_loader.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,24 +6,31 @@
 
 from linkml_runtime.loaders.loader_root import Loader
 from linkml_runtime.utils.yamlutils import YAMLRoot
 from pydantic import BaseModel
 
 class JSONLoader(Loader):
 
-    def load_any(self, source: Union[str, dict, TextIO], target_class: Type[Union[BaseModel, YAMLRoot]], *, base_dir: Optional[str] = None,
-             metadata: Optional[FileInfo] = None, **_) -> Union[BaseModel, YAMLRoot, List[BaseModel], List[YAMLRoot]]:
-        def loader(data: Union[str, dict], _: FileInfo) -> Optional[Dict]:
-            data_as_dict = json.loads(data) if isinstance(data, str) else data
-            if isinstance(data_as_dict, list):
-                return self.json_clean(data_as_dict)
+    def load_as_dict(self, 
+                     source: Union[str, dict, TextIO], 
+                     *, 
+                     base_dir: Optional[str] = None,
+                     metadata: Optional[FileInfo] = None) -> Union[dict, List[dict]]:
+        data = self._read_source(source, base_dir=base_dir, metadata=metadata, accept_header="application/ld+json, application/json, text/json")
+        data_as_dict = json.loads(data) if isinstance(data, str) else data
+        return self.json_clean(data_as_dict)
+
+    def load_any(self, 
+                 source: Union[str, dict, TextIO], 
+                 target_class: Type[Union[BaseModel, YAMLRoot]], 
+                 *, 
+                 base_dir: Optional[str] = None,
+                 metadata: Optional[FileInfo] = None, 
+                 **_) -> Union[BaseModel, YAMLRoot, List[BaseModel], List[YAMLRoot]]:
+        data_as_dict = self.load_as_dict(source, base_dir=base_dir, metadata=metadata)
+
+        if isinstance(data_as_dict, dict):
             typ = data_as_dict.pop('@type', None)
             if typ and typ != target_class.__name__:
                 logging.warning(f"Warning: input type mismatch. Expected: {target_class.__name__}, Actual: {typ}")
-            return self.json_clean(data_as_dict)
 
-        if not metadata:
-            metadata = FileInfo()
-        if base_dir and not metadata.base_path:
-            metadata.base_path = base_dir
-        return self.load_source(source, loader, target_class,
-                                accept_header="application/ld+json, application/json, text/json", metadata=metadata)
+        return self._construct_target_class(data_as_dict, target_class)
```

### Comparing `linkml_runtime-1.5.3/linkml_runtime/loaders/loader_root.py` & `linkml_runtime-1.5.4/linkml_runtime/loaders/loader_root.py`

 * *Files 12% similar despite different names*

```diff
@@ -48,42 +48,18 @@
         :param target_class: Destination class
         :param accept_header: Accept header to use if doing a request
         :param metadata: Metadata about the source.  Filled in as we go along
 
         :return: Instance of the target class if loader worked
         """
 
-        # Makes coding easier down the line if we've got this, even if it is strictly internal
-        if metadata is None:
-            metadata = FileInfo()
-        if not isinstance(source, dict):
-            data = hbread(source, metadata, metadata.base_path, accept_header)
-        else:
-            data = source
+        data = self._read_source(source, metadata=metadata, base_dir=metadata.base_path, accept_header=accept_header)
         data_as_dict = loader(data, metadata)
+        return self._construct_target_class(data_as_dict, target_class=target_class)
 
-        if data_as_dict:
-            if isinstance(data_as_dict, list):
-               if issubclass(target_class, YAMLRoot):
-                   return [target_class(**as_dict(x)) for x in data_as_dict]
-               elif issubclass(target_class, BaseModel):
-                   return [target_class.parse_obj(**as_dict(x)) for x in data_as_dict]
-               else:
-                   raise ValueError(f'Cannot load list of {target_class}')
-            elif isinstance(data_as_dict, dict):
-                if issubclass(target_class, BaseModel):
-                    return target_class.parse_obj(data_as_dict)
-                else:
-                    return target_class(**data_as_dict)
-            elif isinstance(data_as_dict, JsonObj):
-                return [target_class(**as_dict(x)) for x in data_as_dict]
-            else:
-                raise ValueError(f'Unexpected type {data_as_dict}')
-        else:
-            return None
 
     def load(self, *args, **kwargs) -> Union[BaseModel, YAMLRoot]:
         """
         Load source as an instance of target_class
 
         :param source: source file/text/url to load
         :param target_class: destination class
@@ -93,14 +69,17 @@
         :return: instance of target_class
         """
         results = self.load_any(*args, **kwargs)
         if isinstance(results, BaseModel) or isinstance(results, YAMLRoot):
             return results
         else:
             raise ValueError(f'Result is not an instance of BaseModel or YAMLRoot: {type(results)}')
+    
+    def load_as_dict(self, *args, **kwargs) -> Union[dict, List[dict]]:
+        raise NotImplementedError()
 
     @abstractmethod
     def load_any(self, source: Union[str, dict, TextIO], target_class: Type[Union[BaseModel, YAMLRoot]], *, base_dir: Optional[str] = None,
              metadata: Optional[FileInfo] = None, **_) -> Union[BaseModel, YAMLRoot, List[BaseModel], List[YAMLRoot]]:
         """
         Load source as an instance of target_class, or list of instances of target_class
 
@@ -130,7 +109,48 @@
         :param source: source
         :param target_class: destination class
         :param metadata: metadata about the source
         :param _: extensions
         :return: instance of taarget_class
         """
         return self.load(source, target_class, metadata=metadata)
+
+    def _construct_target_class(self, 
+                                data_as_dict: Union[dict, List[dict]],
+                                target_class: Union[Type[YAMLRoot], Type[BaseModel]]) -> Optional[Union[BaseModel, YAMLRoot, List[BaseModel], List[YAMLRoot]]]:
+        if data_as_dict:
+            if isinstance(data_as_dict, list):
+               if issubclass(target_class, YAMLRoot):
+                   return [target_class(**as_dict(x)) for x in data_as_dict]
+               elif issubclass(target_class, BaseModel):
+                   return [target_class.parse_obj(**as_dict(x)) for x in data_as_dict]
+               else:
+                   raise ValueError(f'Cannot load list of {target_class}')
+            elif isinstance(data_as_dict, dict):
+                if issubclass(target_class, BaseModel):
+                    return target_class.parse_obj(data_as_dict)
+                else:
+                    return target_class(**data_as_dict)
+            elif isinstance(data_as_dict, JsonObj):
+                return [target_class(**as_dict(x)) for x in data_as_dict]
+            else:
+                raise ValueError(f'Unexpected type {data_as_dict}')
+        else:
+            return None
+
+    def _read_source(self,
+                     source: Union[str, dict, TextIO], 
+                     *, 
+                     base_dir: Optional[str] = None, 
+                     metadata: Optional[FileInfo] = None, 
+                     accept_header: Optional[str] = "text/plain, application/yaml;q=0.9") -> Union[dict, str]:
+        if metadata is None:
+            metadata = FileInfo()
+        if base_dir and not metadata.base_path:
+            metadata.base_path = base_dir
+
+        if not isinstance(source, dict):
+            data = hbread(source, metadata, metadata.base_path, accept_header)
+        else:
+            data = source
+
+        return data
```

### Comparing `linkml_runtime-1.5.3/linkml_runtime/loaders/rdf_loader.py` & `linkml_runtime-1.5.4/linkml_runtime/loaders/rdf_loader.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.3/linkml_runtime/loaders/rdflib_loader.py` & `linkml_runtime-1.5.4/linkml_runtime/loaders/rdflib_loader.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.3/linkml_runtime/loaders/requests_ssl_patch.py` & `linkml_runtime-1.5.4/linkml_runtime/loaders/requests_ssl_patch.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.3/linkml_runtime/loaders/yaml_loader.py` & `linkml_runtime-1.5.4/linkml_runtime/loaders/yaml_loader.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,34 +10,39 @@
 from pydantic import BaseModel
 
 class YAMLLoader(Loader):
     """
     A Loader that is capable of instantiating LinkML data objects from a YAML file
     """
 
+    def load_as_dict(self, 
+                     source: Union[str, dict, TextIO], 
+                     *, 
+                     base_dir: Optional[str] = None,
+                     metadata: Optional[FileInfo] = None) -> Union[dict, List[dict]]:
+        if metadata is None:
+            metadata = FileInfo()
+        if base_dir and not metadata.base_path:
+            metadata.base_path = base_dir
+        data = self._read_source(source, base_dir=base_dir, metadata=metadata, accept_header="text/yaml, application/yaml;q=0.9")
+        if isinstance(data, str):
+            data = StringIO(data)
+            if metadata and metadata.source_file:
+                data.name = os.path.relpath(metadata.source_file, metadata.base_path)
+            return yaml.load(data, DupCheckYamlLoader)
+        else:
+            return data
+
     def load_any(self,
                  source: Union[str, dict, TextIO],
                  target_class: Union[Type[YAMLRoot],Type[BaseModel]],
                  *, base_dir: Optional[str] = None,
                  metadata: Optional[FileInfo] = None, **_) -> Union[YAMLRoot, List[YAMLRoot]]:
-        def loader(data: Union[str, dict], source_file: FileInfo) -> Optional[Dict]:
-            if isinstance(data, str):
-                data = StringIO(data)
-                if source_file and source_file.source_file:
-                    data.name = os.path.relpath(source_file.source_file, source_file.base_path)
-                return yaml.load(data, DupCheckYamlLoader)
-            else:
-                return data
-
-        if not metadata:
-            metadata = FileInfo()
-        if base_dir and not metadata.base_path:
-            metadata.base_path = base_dir
-        return self.load_source(source, loader, target_class, accept_header="text/yaml, application/yaml;q=0.9",
-                                metadata=metadata)
+        data_as_dict = self.load_as_dict(source, base_dir=base_dir, metadata=metadata)
+        return self._construct_target_class(data_as_dict, target_class)
 
     def loads_any(self, source: str, target_class: Type[Union[BaseModel, YAMLRoot]], *, metadata: Optional[FileInfo] = None, **_) -> Union[BaseModel, YAMLRoot, List[BaseModel], List[YAMLRoot]]:
         """
         Load source as a string
         @param source: source
         @param target_class: destination class
         @param metadata: metadata about the source
```

### Comparing `linkml_runtime-1.5.3/linkml_runtime/processing/referencevalidator.py` & `linkml_runtime-1.5.4/linkml_runtime/processing/referencevalidator.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.3/linkml_runtime/processing/validation_datamodel.py` & `linkml_runtime-1.5.4/linkml_runtime/processing/validation_datamodel.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.3/linkml_runtime/processing/validation_datamodel.yaml` & `linkml_runtime-1.5.4/linkml_runtime/processing/validation_datamodel.yaml`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.3/linkml_runtime/utils/comparefiles.py` & `linkml_runtime-1.5.4/linkml_runtime/utils/comparefiles.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.3/linkml_runtime/utils/compile_python.py` & `linkml_runtime-1.5.4/linkml_runtime/utils/compile_python.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.3/linkml_runtime/utils/context_utils.py` & `linkml_runtime-1.5.4/linkml_runtime/utils/context_utils.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.3/linkml_runtime/utils/csvutils.py` & `linkml_runtime-1.5.4/linkml_runtime/utils/csvutils.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.3/linkml_runtime/utils/dataclass_extensions_376.py` & `linkml_runtime-1.5.4/linkml_runtime/utils/dataclass_extensions_376.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.3/linkml_runtime/utils/distroutils.py` & `linkml_runtime-1.5.4/linkml_runtime/utils/distroutils.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.3/linkml_runtime/utils/enumerations.py` & `linkml_runtime-1.5.4/linkml_runtime/utils/enumerations.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.3/linkml_runtime/utils/eval_utils.py` & `linkml_runtime-1.5.4/linkml_runtime/utils/eval_utils.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.3/linkml_runtime/utils/formatutils.py` & `linkml_runtime-1.5.4/linkml_runtime/utils/formatutils.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.3/linkml_runtime/utils/inference_utils.py` & `linkml_runtime-1.5.4/linkml_runtime/utils/inference_utils.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.3/linkml_runtime/utils/introspection.py` & `linkml_runtime-1.5.4/linkml_runtime/utils/introspection.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.3/linkml_runtime/utils/metamodelcore.py` & `linkml_runtime-1.5.4/linkml_runtime/utils/metamodelcore.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.3/linkml_runtime/utils/namespaces.py` & `linkml_runtime-1.5.4/linkml_runtime/utils/namespaces.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.3/linkml_runtime/utils/pattern.py` & `linkml_runtime-1.5.4/linkml_runtime/utils/pattern.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.3/linkml_runtime/utils/permissiblevalueimpl.py` & `linkml_runtime-1.5.4/linkml_runtime/utils/permissiblevalueimpl.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.3/linkml_runtime/utils/ruleutils.py` & `linkml_runtime-1.5.4/linkml_runtime/utils/ruleutils.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.3/linkml_runtime/utils/schema_as_dict.py` & `linkml_runtime-1.5.4/linkml_runtime/utils/schema_as_dict.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.3/linkml_runtime/utils/schema_builder.py` & `linkml_runtime-1.5.4/linkml_runtime/utils/schema_builder.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.3/linkml_runtime/utils/schemaops.py` & `linkml_runtime-1.5.4/linkml_runtime/utils/schemaops.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.3/linkml_runtime/utils/schemaview.py` & `linkml_runtime-1.5.4/linkml_runtime/utils/schemaview.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.3/linkml_runtime/utils/schemaview_cli.py` & `linkml_runtime-1.5.4/linkml_runtime/utils/schemaview_cli.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.3/linkml_runtime/utils/strictness.py` & `linkml_runtime-1.5.4/linkml_runtime/utils/strictness.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.3/linkml_runtime/utils/walker_utils.py` & `linkml_runtime-1.5.4/linkml_runtime/utils/walker_utils.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.3/linkml_runtime/utils/yamlutils.py` & `linkml_runtime-1.5.4/linkml_runtime/utils/yamlutils.py`

 * *Files identical despite different names*

### Comparing `linkml_runtime-1.5.3/pyproject.toml` & `linkml_runtime-1.5.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "linkml-runtime"
-version = "v1.5.3"
+version = "v1.5.4"
 description = "Runtime environment for LinkML, the Linked open data modeling language"
 authors = [
     "Chris Mungall <cjmungall@lbl.gov>",
     "Harold Solbrig <solbrig@jhu.edu>",
     "Sierra Moxon <smoxon@lbl.gov>",
     "Bill Duncan <wdduncan@gmail.com>",
     "Harshad Hegde <hhegde@lbl.gov>"
```

### Comparing `linkml_runtime-1.5.3/PKG-INFO` & `linkml_runtime-1.5.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linkml-runtime
-Version: 1.5.3
+Version: 1.5.4
 Summary: Runtime environment for LinkML, the Linked open data modeling language
 Home-page: https://github.com/linkml/linkml-runtime
 Keywords: linkml,metamodel,schema visualization,rdf,owl,yaml
 Author: Chris Mungall
 Author-email: cjmungall@lbl.gov
 Requires-Python: >=3.7.6,<4.0.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,23 +15,21 @@
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: click
 Requires-Dist: curies (>=0.5.4)
 Requires-Dist: deprecated
 Requires-Dist: hbreader
 Requires-Dist: json-flattener (>=0.1.9)
-Requires-Dist: jsonasobj2 (>=1.0.4,<2.0.0)
+Requires-Dist: jsonasobj2 (>=1.0.4,<2.dev0)
 Requires-Dist: jsonschema (>=3.2.0)
 Requires-Dist: prefixcommons (>=0.1.12)
 Requires-Dist: prefixmaps (>=0.1.4)
 Requires-Dist: pydantic (>=1.10.2,<2.0.0)
 Requires-Dist: pyyaml
 Requires-Dist: rdflib (>=6.0.0)
 Requires-Dist: requests
```

