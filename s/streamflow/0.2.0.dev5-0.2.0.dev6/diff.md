# Comparing `tmp/streamflow-0.2.0.dev5.tar.gz` & `tmp/streamflow-0.2.0.dev6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamflow-0.2.0.dev5.tar", last modified: Sat May  6 16:06:51 2023, max compression
+gzip compressed data, was "streamflow-0.2.0.dev6.tar", last modified: Thu Jun 15 00:43:44 2023, max compression
```

## Comparing `streamflow-0.2.0.dev5.tar` & `streamflow-0.2.0.dev6.tar`

### file list

```diff
@@ -1,175 +1,180 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:06:51.756713 streamflow-0.2.0.dev5/
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11551 2023-05-06 16:06:51.756713 streamflow-0.2.0.dev5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10236 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/bandit-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:06:51.708713 streamflow-0.2.0.dev5/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/lint-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/report-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 16:06:51.756713 streamflow-0.2.0.dev5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:06:51.712713 streamflow-0.2.0.dev5/streamflow/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:06:51.716713 streamflow-0.2.0.dev5/streamflow/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/config/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:06:51.700713 streamflow-0.2.0.dev5/streamflow/config/schemas/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:06:51.716713 streamflow-0.2.0.dev5/streamflow/config/schemas/v1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    13177 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/config/schemas/v1.0/config_schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/config/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:06:51.720713 streamflow-0.2.0.dev5/streamflow/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4460 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/core/asyncache.py
--rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/core/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/core/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     9163 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/core/deployment.py
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/core/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     6787 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/core/persistence.py
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/core/provenance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/core/recovery.py
--rw-r--r--   0 runner    (1001) docker     (123)     7754 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/core/scheduling.py
--rw-r--r--   0 runner    (1001) docker     (123)     7963 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/core/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    24035 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/core/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:06:51.724713 streamflow-0.2.0.dev5/streamflow/cwl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/cwl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:06:51.728713 streamflow-0.2.0.dev5/streamflow/cwl/antlr/
--rw-r--r--   0 runner    (1001) docker     (123)    51958 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/cwl/antlr/ECMAScriptLexer.py
--rw-r--r--   0 runner    (1001) docker     (123)    33090 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/cwl/antlr/ECMAScriptListener.py
--rw-r--r--   0 runner    (1001) docker     (123)   228628 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/cwl/antlr/ECMAScriptParser.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/cwl/antlr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/cwl/combinator.py
--rw-r--r--   0 runner    (1001) docker     (123)    52552 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/cwl/command.py
--rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/cwl/expression.py
--rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/cwl/hardware.py
--rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/cwl/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    49536 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/cwl/processor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:06:51.728713 streamflow-0.2.0.dev5/streamflow/cwl/requirement/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/cwl/requirement/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:06:51.728713 streamflow-0.2.0.dev5/streamflow/cwl/requirement/docker/
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/cwl/requirement/docker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15297 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/cwl/requirement/docker/docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/cwl/requirement/docker/kubernetes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:06:51.728713 streamflow-0.2.0.dev5/streamflow/cwl/requirement/docker/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)    13724 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/cwl/requirement/docker/schemas/docker.json
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/cwl/requirement/docker/schemas/kubernetes.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/cwl/requirement/docker/schemas/kubernetes.json
--rw-r--r--   0 runner    (1001) docker     (123)     9243 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/cwl/requirement/docker/schemas/singularity.json
--rw-r--r--   0 runner    (1001) docker     (123)     9715 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/cwl/requirement/docker/singularity.py
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/cwl/requirement/docker/translator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/cwl/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)    22258 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/cwl/step.py
--rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/cwl/token.py
--rw-r--r--   0 runner    (1001) docker     (123)    12464 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/cwl/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)   113743 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/cwl/translator.py
--rw-r--r--   0 runner    (1001) docker     (123)    40610 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/cwl/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:06:51.732713 streamflow-0.2.0.dev5/streamflow/data/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16753 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/data/data_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    15070 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/data/remotepath.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:06:51.732713 streamflow-0.2.0.dev5/streamflow/data/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/data/schemas/data_manager.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:06:51.736713 streamflow-0.2.0.dev5/streamflow/deployment/
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/deployment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36140 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/deployment/aiotarstream.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:06:51.736713 streamflow-0.2.0.dev5/streamflow/deployment/connector/
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/deployment/connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14800 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/deployment/connector/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    53904 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/deployment/connector/container.py
--rw-r--r--   0 runner    (1001) docker     (123)    44082 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/deployment/connector/kubernetes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/deployment/connector/local.py
--rw-r--r--   0 runner    (1001) docker     (123)    15373 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/deployment/connector/occam.py
--rw-r--r--   0 runner    (1001) docker     (123)    22133 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/deployment/connector/queue_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:06:51.740713 streamflow-0.2.0.dev5/streamflow/deployment/connector/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/deployment/connector/schemas/docker-compose.json
--rw-r--r--   0 runner    (1001) docker     (123)    14544 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/deployment/connector/schemas/docker.json
--rw-r--r--   0 runner    (1001) docker     (123)     6491 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/deployment/connector/schemas/helm3.json
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/deployment/connector/schemas/kubernetes.json
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/deployment/connector/schemas/local.json
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/deployment/connector/schemas/occam.json
--rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/deployment/connector/schemas/queue_manager.json
--rw-r--r--   0 runner    (1001) docker     (123)    10049 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/deployment/connector/schemas/singularity.json
--rw-r--r--   0 runner    (1001) docker     (123)     5023 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/deployment/connector/schemas/ssh.json
--rw-r--r--   0 runner    (1001) docker     (123)    25573 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/deployment/connector/ssh.py
--rw-r--r--   0 runner    (1001) docker     (123)     9853 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/deployment/deployment_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:06:51.740713 streamflow-0.2.0.dev5/streamflow/deployment/filter/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/deployment/filter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:06:51.740713 streamflow-0.2.0.dev5/streamflow/deployment/filter/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/deployment/filter/schemas/shuffle.json
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/deployment/filter/shuffle.py
--rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/deployment/future.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:06:51.740713 streamflow-0.2.0.dev5/streamflow/deployment/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/deployment/schemas/deployment_manager.json
--rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/deployment/stream.py
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/deployment/template.py
--rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/deployment/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/deployment/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:06:51.744713 streamflow-0.2.0.dev5/streamflow/ext/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3670 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/ext/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     9342 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/ext/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/log_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     9859 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     6838 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:06:51.744713 streamflow-0.2.0.dev5/streamflow/persistence/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/persistence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/persistence/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/persistence/loading_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:06:51.744713 streamflow-0.2.0.dev5/streamflow/persistence/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/persistence/schemas/sqlite.json
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/persistence/schemas/sqlite.sql
--rw-r--r--   0 runner    (1001) docker     (123)    18997 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/persistence/sqlite.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:06:51.744713 streamflow-0.2.0.dev5/streamflow/provenance/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/provenance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    64182 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/provenance/run_crate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:06:51.748713 streamflow-0.2.0.dev5/streamflow/recovery/
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/recovery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/recovery/checkpoint_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    11361 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/recovery/failure_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/recovery/recovery.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:06:51.748713 streamflow-0.2.0.dev5/streamflow/recovery/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/recovery/schemas/default_checkpoint_manager.json
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/recovery/schemas/default_failure_manager.json
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/recovery/schemas/dummy_checkpoint_manager.json
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/recovery/schemas/dummy_failure_manager.json
--rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/report.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:06:51.748713 streamflow-0.2.0.dev5/streamflow/scheduling/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/scheduling/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:06:51.748713 streamflow-0.2.0.dev5/streamflow/scheduling/policy/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/scheduling/policy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/scheduling/policy/data_locality.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:06:51.752713 streamflow-0.2.0.dev5/streamflow/scheduling/policy/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/scheduling/policy/schemas/data_locality.json
--rw-r--r--   0 runner    (1001) docker     (123)    16672 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/scheduling/scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:06:51.752713 streamflow-0.2.0.dev5/streamflow/scheduling/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/scheduling/schemas/scheduler.json
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:06:51.752713 streamflow-0.2.0.dev5/streamflow/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8471 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/workflow/combinator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6399 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/workflow/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/workflow/port.py
--rw-r--r--   0 runner    (1001) docker     (123)    62216 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/workflow/step.py
--rw-r--r--   0 runner    (1001) docker     (123)     4839 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/workflow/token.py
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/workflow/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/streamflow/workflow/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:06:51.712713 streamflow-0.2.0.dev5/streamflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11551 2023-05-06 16:06:51.000000 streamflow-0.2.0.dev5/streamflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-05-06 16:06:51.000000 streamflow-0.2.0.dev5/streamflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 16:06:51.000000 streamflow-0.2.0.dev5/streamflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-06 16:06:51.000000 streamflow-0.2.0.dev5/streamflow.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-05-06 16:06:51.000000 streamflow-0.2.0.dev5/streamflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-06 16:06:51.000000 streamflow-0.2.0.dev5/streamflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 16:06:51.000000 streamflow-0.2.0.dev5/streamflow.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/test-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:06:51.756713 streamflow-0.2.0.dev5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     8288 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/tests/test_cwl_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)    24802 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/tests/test_cwl_persistence.py
--rw-r--r--   0 runner    (1001) docker     (123)    10836 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/tests/test_persistence.py
--rw-r--r--   0 runner    (1001) docker     (123)     7568 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/tests/test_remotepath.py
--rw-r--r--   0 runner    (1001) docker     (123)    16712 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/tests/test_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7541 2023-05-06 16:06:41.000000 streamflow-0.2.0.dev5/tests/test_transfer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:43:44.574962 streamflow-0.2.0.dev6/
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11551 2023-06-15 00:43:44.574962 streamflow-0.2.0.dev6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10236 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/bandit-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:43:44.554962 streamflow-0.2.0.dev6/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/lint-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/report-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 00:43:44.574962 streamflow-0.2.0.dev6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:43:44.554962 streamflow-0.2.0.dev6/streamflow/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:43:44.558962 streamflow-0.2.0.dev6/streamflow/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/config/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:43:44.550962 streamflow-0.2.0.dev6/streamflow/config/schemas/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:43:44.558962 streamflow-0.2.0.dev6/streamflow/config/schemas/v1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    13177 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/config/schemas/v1.0/config_schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/config/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:43:44.558962 streamflow-0.2.0.dev6/streamflow/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4460 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/core/asyncache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/core/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/core/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9163 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/core/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/core/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7071 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/core/persistence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/core/provenance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/core/recovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7754 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/core/scheduling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8455 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24153 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/core/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:43:44.562962 streamflow-0.2.0.dev6/streamflow/cwl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/cwl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:43:44.562962 streamflow-0.2.0.dev6/streamflow/cwl/antlr/
+-rw-r--r--   0 runner    (1001) docker     (123)    52296 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/cwl/antlr/ECMAScriptLexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33065 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/cwl/antlr/ECMAScriptListener.py
+-rw-r--r--   0 runner    (1001) docker     (123)   228650 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/cwl/antlr/ECMAScriptParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/cwl/antlr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/cwl/combinator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52552 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/cwl/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/cwl/expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/cwl/hardware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/cwl/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49556 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/cwl/processor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:43:44.562962 streamflow-0.2.0.dev6/streamflow/cwl/requirement/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/cwl/requirement/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:43:44.562962 streamflow-0.2.0.dev6/streamflow/cwl/requirement/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/cwl/requirement/docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15297 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/cwl/requirement/docker/docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/cwl/requirement/docker/kubernetes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:43:44.562962 streamflow-0.2.0.dev6/streamflow/cwl/requirement/docker/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)    13724 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/cwl/requirement/docker/schemas/docker.json
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/cwl/requirement/docker/schemas/kubernetes.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/cwl/requirement/docker/schemas/kubernetes.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9243 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/cwl/requirement/docker/schemas/singularity.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9715 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/cwl/requirement/docker/singularity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/cwl/requirement/docker/translator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/cwl/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23150 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/cwl/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/cwl/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12751 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/cwl/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)   113743 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/cwl/translator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40610 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/cwl/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:43:44.562962 streamflow-0.2.0.dev6/streamflow/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16753 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/data/data_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15070 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/data/remotepath.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:43:44.562962 streamflow-0.2.0.dev6/streamflow/data/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/data/schemas/data_manager.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:43:44.566962 streamflow-0.2.0.dev6/streamflow/deployment/
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/deployment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36140 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/deployment/aiotarstream.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:43:44.566962 streamflow-0.2.0.dev6/streamflow/deployment/connector/
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/deployment/connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14253 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/deployment/connector/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52606 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/deployment/connector/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43726 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/deployment/connector/kubernetes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/deployment/connector/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15378 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/deployment/connector/occam.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43252 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/deployment/connector/queue_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:43:44.566962 streamflow-0.2.0.dev6/streamflow/deployment/connector/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/deployment/connector/schemas/docker-compose.json
+-rw-r--r--   0 runner    (1001) docker     (123)    14544 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/deployment/connector/schemas/docker.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5486 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/deployment/connector/schemas/flux.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6491 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/deployment/connector/schemas/helm3.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/deployment/connector/schemas/kubernetes.json
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/deployment/connector/schemas/local.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/deployment/connector/schemas/occam.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/deployment/connector/schemas/pbs.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/deployment/connector/schemas/queue_manager.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10049 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/deployment/connector/schemas/singularity.json
+-rw-r--r--   0 runner    (1001) docker     (123)    21318 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/deployment/connector/schemas/slurm.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5023 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/deployment/connector/schemas/ssh.json
+-rw-r--r--   0 runner    (1001) docker     (123)    25573 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/deployment/connector/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9853 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/deployment/deployment_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:43:44.566962 streamflow-0.2.0.dev6/streamflow/deployment/filter/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/deployment/filter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:43:44.566962 streamflow-0.2.0.dev6/streamflow/deployment/filter/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/deployment/filter/schemas/shuffle.json
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/deployment/filter/shuffle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/deployment/future.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:43:44.566962 streamflow-0.2.0.dev6/streamflow/deployment/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/deployment/schemas/deployment_manager.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/deployment/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/deployment/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/deployment/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/deployment/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:43:44.570962 streamflow-0.2.0.dev6/streamflow/ext/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3670 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/ext/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12778 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/ext/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/log_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10158 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7243 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:43:44.570962 streamflow-0.2.0.dev6/streamflow/persistence/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/persistence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/persistence/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/persistence/loading_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:43:44.570962 streamflow-0.2.0.dev6/streamflow/persistence/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/persistence/schemas/sqlite.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/persistence/schemas/sqlite.sql
+-rw-r--r--   0 runner    (1001) docker     (123)    19823 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/persistence/sqlite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:43:44.570962 streamflow-0.2.0.dev6/streamflow/provenance/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/provenance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64182 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/provenance/run_crate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:43:44.570962 streamflow-0.2.0.dev6/streamflow/recovery/
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/recovery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/recovery/checkpoint_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11361 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/recovery/failure_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/recovery/recovery.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:43:44.570962 streamflow-0.2.0.dev6/streamflow/recovery/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/recovery/schemas/default_checkpoint_manager.json
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/recovery/schemas/default_failure_manager.json
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/recovery/schemas/dummy_checkpoint_manager.json
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/recovery/schemas/dummy_failure_manager.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/report.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:43:44.570962 streamflow-0.2.0.dev6/streamflow/scheduling/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/scheduling/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:43:44.570962 streamflow-0.2.0.dev6/streamflow/scheduling/policy/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/scheduling/policy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/scheduling/policy/data_locality.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:43:44.570962 streamflow-0.2.0.dev6/streamflow/scheduling/policy/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/scheduling/policy/schemas/data_locality.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16672 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/scheduling/scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:43:44.570962 streamflow-0.2.0.dev6/streamflow/scheduling/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/scheduling/schemas/scheduler.json
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:43:44.574962 streamflow-0.2.0.dev6/streamflow/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8428 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/workflow/combinator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6399 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/workflow/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/workflow/port.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66334 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/workflow/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4849 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/workflow/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/workflow/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/streamflow/workflow/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:43:44.558962 streamflow-0.2.0.dev6/streamflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11551 2023-06-15 00:43:44.000000 streamflow-0.2.0.dev6/streamflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-06-15 00:43:44.000000 streamflow-0.2.0.dev6/streamflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 00:43:44.000000 streamflow-0.2.0.dev6/streamflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-15 00:43:44.000000 streamflow-0.2.0.dev6/streamflow.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-06-15 00:43:44.000000 streamflow-0.2.0.dev6/streamflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-15 00:43:44.000000 streamflow-0.2.0.dev6/streamflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 00:43:44.000000 streamflow-0.2.0.dev6/streamflow.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:43:44.574962 streamflow-0.2.0.dev6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     8288 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/tests/test_cwl_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24808 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/tests/test_cwl_persistence.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13743 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/tests/test_cwl_provenance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10836 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/tests/test_persistence.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20695 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/tests/test_provenance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7568 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/tests/test_remotepath.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16712 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/tests/test_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7541 2023-06-15 00:43:34.000000 streamflow-0.2.0.dev6/tests/test_transfer.py
```

### Comparing `streamflow-0.2.0.dev5/LICENSE` & `streamflow-0.2.0.dev6/LICENSE`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev5/PKG-INFO` & `streamflow-0.2.0.dev6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamflow
-Version: 0.2.0.dev5
+Version: 0.2.0.dev6
 Summary: StreamFlow framework
 Author-email: Iacopo Colonnelli <iacopo.colonnelli@unito.it>
 License: LGPL-3.0-or-later
 Project-URL: Homepage, https://streamflow.di.unito.it
 Project-URL: Package, https://pypi.org/project/streamflow
 Project-URL: Repository, https://github.com/alpha-unito/streamflow
 Project-URL: Docker, https://hub.docker.com/r/alphaunito/streamflow
```

### Comparing `streamflow-0.2.0.dev5/README.md` & `streamflow-0.2.0.dev6/README.md`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev5/pyproject.toml` & `streamflow-0.2.0.dev6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev5/streamflow/config/config.py` & `streamflow-0.2.0.dev6/streamflow/config/config.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev5/streamflow/config/schemas/v1.0/config_schema.json` & `streamflow-0.2.0.dev6/streamflow/config/schemas/v1.0/config_schema.json`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev5/streamflow/config/validator.py` & `streamflow-0.2.0.dev6/streamflow/config/validator.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev5/streamflow/core/asyncache.py` & `streamflow-0.2.0.dev6/streamflow/core/asyncache.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev5/streamflow/core/config.py` & `streamflow-0.2.0.dev6/streamflow/core/config.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev5/streamflow/core/context.py` & `streamflow-0.2.0.dev6/streamflow/core/context.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev5/streamflow/core/data.py` & `streamflow-0.2.0.dev6/streamflow/core/data.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev5/streamflow/core/deployment.py` & `streamflow-0.2.0.dev6/streamflow/core/deployment.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev5/streamflow/core/exception.py` & `streamflow-0.2.0.dev6/streamflow/core/exception.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev5/streamflow/core/persistence.py` & `streamflow-0.2.0.dev6/streamflow/core/persistence.py`

 * *Files 2% similar despite different names*

```diff
@@ -152,14 +152,26 @@
         ...
 
     @abstractmethod
     async def close(self):
         ...
 
     @abstractmethod
+    async def get_dependees(
+        self, token_id: int
+    ) -> MutableSequence[MutableMapping[str, Any]]:
+        ...
+
+    @abstractmethod
+    async def get_dependers(
+        self, token_id: int
+    ) -> MutableSequence[MutableMapping[str, Any]]:
+        ...
+
+    @abstractmethod
     async def get_command(self, command_id: int) -> MutableMapping[str, Any]:
         ...
 
     @abstractmethod
     async def get_commands_by_step(
         self, step_id: int
     ) -> MutableSequence[MutableMapping[str, Any]]:
```

### Comparing `streamflow-0.2.0.dev5/streamflow/core/provenance.py` & `streamflow-0.2.0.dev6/streamflow/core/provenance.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev5/streamflow/core/recovery.py` & `streamflow-0.2.0.dev6/streamflow/core/recovery.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev5/streamflow/core/scheduling.py` & `streamflow-0.2.0.dev6/streamflow/core/scheduling.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev5/streamflow/core/utils.py` & `streamflow-0.2.0.dev6/streamflow/core/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -155,14 +155,32 @@
         return posixpath.join(dst, os.path.basename(src))
     # Otherwise
     else:
         # Keep current dst
         return dst
 
 
+def get_option(
+    name: str,
+    value: Any,
+) -> str:
+    if len(name) > 1:
+        name = f"-{name} "
+    if isinstance(value, bool):
+        return f"-{name} " if value else ""
+    elif isinstance(value, str) or isinstance(value, int):
+        return f'-{name} "{value}" '
+    elif isinstance(value, MutableSequence):
+        return "".join([f'-{name} "{item}" ' for item in value])
+    elif value is None:
+        return ""
+    else:
+        raise TypeError("Unsupported value type")
+
+
 async def get_remote_to_remote_write_command(
     src_connector: Connector,
     src_location: Location,
     src: str,
     dst_connector: Connector,
     dst_locations: MutableSequence[Location],
     dst: str,
```

### Comparing `streamflow-0.2.0.dev5/streamflow/core/workflow.py` & `streamflow-0.2.0.dev6/streamflow/core/workflow.py`

 * *Files 0% similar despite different names*

```diff
@@ -521,14 +521,16 @@
     ) -> Token:
         value = json.loads(row["value"])
         if isinstance(value, MutableMapping) and "token" in value:
             value = await loading_context.load_token(context, value["token"])
         return cls(tag=row["tag"], value=value)
 
     async def _save_value(self, context: StreamFlowContext):
+        if isinstance(self.value, Token) and not self.value.persistent_id:
+            await self.value.save(context)
         return (
             {"token": self.value.persistent_id}
             if isinstance(self.value, Token)
             else self.value
         )
 
     async def get_weight(self, context: StreamFlowContext):
```

### Comparing `streamflow-0.2.0.dev5/streamflow/cwl/antlr/ECMAScriptLexer.py` & `streamflow-0.2.0.dev6/streamflow/cwl/antlr/ECMAScriptLexer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-# Generated from ECMAScript.g4 by ANTLR 4.12.0
-import sys
-
+# Generated from ECMAScript.g4 by ANTLR 4.13.0
 from antlr4 import *
-
+from io import StringIO
+import sys
 if sys.version_info[1] > 5:
     from typing import TextIO
 else:
     from typing.io import TextIO
 
 
 def serializedATN():
@@ -103,15 +102,15 @@
         0,231,0,233,0,235,0,237,0,239,0,241,0,243,0,245,0,247,0,249,0,251,
         0,253,0,255,0,257,0,259,0,261,0,1,0,19,3,0,10,10,13,13,8232,8233,
         2,0,88,88,120,120,4,0,9,9,11,12,32,32,160,160,4,0,10,10,13,13,34,
         34,92,92,4,0,10,10,13,13,39,39,92,92,9,0,34,34,39,39,92,92,98,98,
         102,102,110,110,114,114,116,116,118,118,12,0,10,10,13,13,34,34,39,
         39,48,57,92,92,98,98,102,102,110,110,114,114,116,118,120,120,2,0,
         117,117,120,120,1,0,48,57,3,0,48,57,65,70,97,102,1,0,48,55,1,0,49,
-        57,2,0,69,69,101,101,2,0,43,43,45,45,650,0,36,36,65,90,95,95,97,
+        57,2,0,69,69,101,101,2,0,43,43,45,45,661,0,36,36,65,90,95,95,97,
         122,170,170,181,181,186,186,192,214,216,246,248,705,710,721,736,
         740,748,748,750,750,880,884,886,887,890,893,895,895,902,902,904,
         906,908,908,910,929,931,1013,1015,1153,1162,1327,1329,1366,1369,
         1369,1376,1416,1488,1514,1519,1522,1568,1610,1646,1647,1649,1747,
         1749,1749,1765,1766,1774,1775,1786,1788,1791,1791,1808,1808,1810,
         1839,1869,1957,1969,1969,1994,2026,2036,2037,2042,2042,2048,2069,
         2074,2074,2084,2084,2088,2088,2112,2136,2144,2154,2160,2183,2185,
@@ -181,196 +180,200 @@
         68115,68117,68119,68121,68149,68192,68220,68224,68252,68288,68295,
         68297,68324,68352,68405,68416,68437,68448,68466,68480,68497,68608,
         68680,68736,68786,68800,68850,68864,68899,69248,69289,69296,69297,
         69376,69404,69415,69415,69424,69445,69488,69505,69552,69572,69600,
         69622,69635,69687,69745,69746,69749,69749,69763,69807,69840,69864,
         69891,69926,69956,69956,69959,69959,69968,70002,70006,70006,70019,
         70066,70081,70084,70106,70106,70108,70108,70144,70161,70163,70187,
-        70272,70278,70280,70280,70282,70285,70287,70301,70303,70312,70320,
-        70366,70405,70412,70415,70416,70419,70440,70442,70448,70450,70451,
-        70453,70457,70461,70461,70480,70480,70493,70497,70656,70708,70727,
-        70730,70751,70753,70784,70831,70852,70853,70855,70855,71040,71086,
-        71128,71131,71168,71215,71236,71236,71296,71338,71352,71352,71424,
-        71450,71488,71494,71680,71723,71840,71903,71935,71942,71945,71945,
-        71948,71955,71957,71958,71960,71983,71999,71999,72001,72001,72096,
-        72103,72106,72144,72161,72161,72163,72163,72192,72192,72203,72242,
-        72250,72250,72272,72272,72284,72329,72349,72349,72368,72440,72704,
-        72712,72714,72750,72768,72768,72818,72847,72960,72966,72968,72969,
-        72971,73008,73030,73030,73056,73061,73063,73064,73066,73097,73112,
-        73112,73440,73458,73648,73648,73728,74649,74880,75075,77712,77808,
-        77824,78894,82944,83526,92160,92728,92736,92766,92784,92862,92880,
-        92909,92928,92975,92992,92995,93027,93047,93053,93071,93760,93823,
-        93952,94026,94032,94032,94099,94111,94176,94177,94179,94179,94208,
-        100343,100352,101589,101632,101640,110576,110579,110581,110587,110589,
-        110590,110592,110882,110928,110930,110948,110951,110960,111355,113664,
-        113770,113776,113788,113792,113800,113808,113817,119808,119892,119894,
-        119964,119966,119967,119970,119970,119973,119974,119977,119980,119982,
-        119993,119995,119995,119997,120003,120005,120069,120071,120074,120077,
-        120084,120086,120092,120094,120121,120123,120126,120128,120132,120134,
-        120134,120138,120144,120146,120485,120488,120512,120514,120538,120540,
-        120570,120572,120596,120598,120628,120630,120654,120656,120686,120688,
-        120712,120714,120744,120746,120770,120772,120779,122624,122654,123136,
-        123180,123191,123197,123214,123214,123536,123565,123584,123627,124896,
-        124902,124904,124907,124909,124910,124912,124926,124928,125124,125184,
-        125251,125259,125259,126464,126467,126469,126495,126497,126498,126500,
-        126500,126503,126503,126505,126514,126516,126519,126521,126521,126523,
-        126523,126530,126530,126535,126535,126537,126537,126539,126539,126541,
-        126543,126545,126546,126548,126548,126551,126551,126553,126553,126555,
-        126555,126557,126557,126559,126559,126561,126562,126564,126564,126567,
-        126570,126572,126578,126580,126583,126585,126588,126590,126590,126592,
-        126601,126603,126619,126625,126627,126629,126633,126635,126651,131072,
-        173791,173824,177976,177984,178205,178208,183969,183984,191456,194560,
-        195101,196608,201546,396,0,48,57,95,95,768,879,1155,1159,1425,1469,
-        1471,1471,1473,1474,1476,1477,1479,1479,1552,1562,1611,1641,1648,
-        1648,1750,1756,1759,1764,1767,1768,1770,1773,1776,1785,1809,1809,
-        1840,1866,1958,1968,1984,1993,2027,2035,2045,2045,2070,2073,2075,
-        2083,2085,2087,2089,2093,2137,2139,2200,2207,2250,2273,2275,2306,
-        2362,2362,2364,2364,2369,2376,2381,2381,2385,2391,2402,2403,2406,
-        2415,2433,2433,2492,2492,2497,2500,2509,2509,2530,2531,2534,2543,
-        2558,2558,2561,2562,2620,2620,2625,2626,2631,2632,2635,2637,2641,
-        2641,2662,2673,2677,2677,2689,2690,2748,2748,2753,2757,2759,2760,
-        2765,2765,2786,2787,2790,2799,2810,2815,2817,2817,2876,2876,2879,
-        2879,2881,2884,2893,2893,2901,2902,2914,2915,2918,2927,2946,2946,
-        3008,3008,3021,3021,3046,3055,3072,3072,3076,3076,3132,3132,3134,
-        3136,3142,3144,3146,3149,3157,3158,3170,3171,3174,3183,3201,3201,
-        3260,3260,3263,3263,3270,3270,3276,3277,3298,3299,3302,3311,3328,
-        3329,3387,3388,3393,3396,3405,3405,3426,3427,3430,3439,3457,3457,
-        3530,3530,3538,3540,3542,3542,3558,3567,3633,3633,3636,3642,3655,
-        3662,3664,3673,3761,3761,3764,3772,3784,3789,3792,3801,3864,3865,
-        3872,3881,3893,3893,3895,3895,3897,3897,3953,3966,3968,3972,3974,
-        3975,3981,3991,3993,4028,4038,4038,4141,4144,4146,4151,4153,4154,
-        4157,4158,4160,4169,4184,4185,4190,4192,4209,4212,4226,4226,4229,
-        4230,4237,4237,4240,4249,4253,4253,4957,4959,5906,5908,5938,5939,
-        5970,5971,6002,6003,6068,6069,6071,6077,6086,6086,6089,6099,6109,
-        6109,6112,6121,6155,6157,6159,6169,6277,6278,6313,6313,6432,6434,
-        6439,6440,6450,6450,6457,6459,6470,6479,6608,6617,6679,6680,6683,
-        6683,6742,6742,6744,6750,6752,6752,6754,6754,6757,6764,6771,6780,
-        6783,6793,6800,6809,6832,6845,6847,6862,6912,6915,6964,6964,6966,
-        6970,6972,6972,6978,6978,6992,7001,7019,7027,7040,7041,7074,7077,
-        7080,7081,7083,7085,7088,7097,7142,7142,7144,7145,7149,7149,7151,
-        7153,7212,7219,7222,7223,7232,7241,7248,7257,7376,7378,7380,7392,
-        7394,7400,7405,7405,7412,7412,7416,7417,7616,7679,8255,8256,8276,
-        8276,8400,8412,8417,8417,8421,8432,11503,11505,11647,11647,11744,
-        11775,12330,12333,12441,12442,42528,42537,42607,42607,42612,42621,
-        42654,42655,42736,42737,43010,43010,43014,43014,43019,43019,43045,
-        43046,43052,43052,43204,43205,43216,43225,43232,43249,43263,43273,
-        43302,43309,43335,43345,43392,43394,43443,43443,43446,43449,43452,
-        43453,43472,43481,43493,43493,43504,43513,43561,43566,43569,43570,
-        43573,43574,43587,43587,43596,43596,43600,43609,43644,43644,43696,
-        43696,43698,43700,43703,43704,43710,43711,43713,43713,43756,43757,
-        43766,43766,44005,44005,44008,44008,44013,44013,44016,44025,64286,
-        64286,65024,65039,65056,65071,65075,65076,65101,65103,65296,65305,
-        65343,65343,66045,66045,66272,66272,66422,66426,66720,66729,68097,
-        68099,68101,68102,68108,68111,68152,68154,68159,68159,68325,68326,
-        68900,68903,68912,68921,69291,69292,69446,69456,69506,69509,69633,
-        69633,69688,69702,69734,69744,69747,69748,69759,69761,69811,69814,
-        69817,69818,69826,69826,69872,69881,69888,69890,69927,69931,69933,
-        69940,69942,69951,70003,70003,70016,70017,70070,70078,70089,70092,
-        70095,70105,70191,70193,70196,70196,70198,70199,70206,70206,70367,
-        70367,70371,70378,70384,70393,70400,70401,70459,70460,70464,70464,
-        70502,70508,70512,70516,70712,70719,70722,70724,70726,70726,70736,
-        70745,70750,70750,70835,70840,70842,70842,70847,70848,70850,70851,
-        70864,70873,71090,71093,71100,71101,71103,71104,71132,71133,71219,
-        71226,71229,71229,71231,71232,71248,71257,71339,71339,71341,71341,
-        71344,71349,71351,71351,71360,71369,71453,71455,71458,71461,71463,
-        71467,71472,71481,71727,71735,71737,71738,71904,71913,71995,71996,
-        71998,71998,72003,72003,72016,72025,72148,72151,72154,72155,72160,
-        72160,72193,72202,72243,72248,72251,72254,72263,72263,72273,72278,
-        72281,72283,72330,72342,72344,72345,72752,72758,72760,72765,72767,
-        72767,72784,72793,72850,72871,72874,72880,72882,72883,72885,72886,
-        73009,73014,73018,73018,73020,73021,73023,73029,73031,73031,73040,
-        73049,73104,73105,73109,73109,73111,73111,73120,73129,73459,73460,
-        92768,92777,92864,92873,92912,92916,92976,92982,93008,93017,94031,
-        94031,94095,94098,94180,94180,113821,113822,118528,118573,118576,
-        118598,119143,119145,119163,119170,119173,119179,119210,119213,119362,
-        119364,120782,120831,121344,121398,121403,121452,121461,121461,121476,
-        121476,121499,121503,121505,121519,122880,122886,122888,122904,122907,
-        122913,122915,122916,122918,122922,123184,123190,123200,123209,123566,
-        123566,123628,123641,125136,125142,125252,125258,125264,125273,130032,
-        130041,917760,917999,6,0,10,10,13,13,42,42,47,47,91,92,8232,8233,
-        5,0,10,10,13,13,47,47,91,92,8232,8233,4,0,10,10,13,13,92,93,8232,
-        8233,941,0,1,1,0,0,0,0,3,1,0,0,0,0,5,1,0,0,0,0,7,1,0,0,0,0,9,1,0,
-        0,0,0,11,1,0,0,0,0,13,1,0,0,0,0,15,1,0,0,0,0,17,1,0,0,0,0,19,1,0,
-        0,0,0,21,1,0,0,0,0,23,1,0,0,0,0,25,1,0,0,0,0,27,1,0,0,0,0,29,1,0,
-        0,0,0,31,1,0,0,0,0,33,1,0,0,0,0,35,1,0,0,0,0,37,1,0,0,0,0,39,1,0,
-        0,0,0,41,1,0,0,0,0,43,1,0,0,0,0,45,1,0,0,0,0,47,1,0,0,0,0,49,1,0,
-        0,0,0,51,1,0,0,0,0,53,1,0,0,0,0,55,1,0,0,0,0,57,1,0,0,0,0,59,1,0,
-        0,0,0,61,1,0,0,0,0,63,1,0,0,0,0,65,1,0,0,0,0,67,1,0,0,0,0,69,1,0,
-        0,0,0,71,1,0,0,0,0,73,1,0,0,0,0,75,1,0,0,0,0,77,1,0,0,0,0,79,1,0,
-        0,0,0,81,1,0,0,0,0,83,1,0,0,0,0,85,1,0,0,0,0,87,1,0,0,0,0,89,1,0,
-        0,0,0,91,1,0,0,0,0,93,1,0,0,0,0,95,1,0,0,0,0,97,1,0,0,0,0,99,1,0,
-        0,0,0,101,1,0,0,0,0,103,1,0,0,0,0,105,1,0,0,0,0,107,1,0,0,0,0,109,
-        1,0,0,0,0,111,1,0,0,0,0,113,1,0,0,0,0,115,1,0,0,0,0,117,1,0,0,0,
-        0,119,1,0,0,0,0,121,1,0,0,0,0,123,1,0,0,0,0,125,1,0,0,0,0,127,1,
-        0,0,0,0,129,1,0,0,0,0,131,1,0,0,0,0,133,1,0,0,0,0,135,1,0,0,0,0,
-        137,1,0,0,0,0,139,1,0,0,0,0,141,1,0,0,0,0,143,1,0,0,0,0,145,1,0,
-        0,0,0,147,1,0,0,0,0,149,1,0,0,0,0,151,1,0,0,0,0,153,1,0,0,0,0,155,
-        1,0,0,0,0,157,1,0,0,0,0,159,1,0,0,0,0,161,1,0,0,0,0,163,1,0,0,0,
-        0,165,1,0,0,0,0,167,1,0,0,0,0,169,1,0,0,0,0,171,1,0,0,0,0,173,1,
-        0,0,0,0,175,1,0,0,0,0,177,1,0,0,0,0,179,1,0,0,0,0,181,1,0,0,0,0,
-        183,1,0,0,0,0,185,1,0,0,0,0,187,1,0,0,0,0,189,1,0,0,0,0,191,1,0,
-        0,0,0,193,1,0,0,0,0,195,1,0,0,0,0,197,1,0,0,0,0,199,1,0,0,0,0,201,
-        1,0,0,0,0,203,1,0,0,0,0,205,1,0,0,0,1,263,1,0,0,0,3,269,1,0,0,0,
-        5,273,1,0,0,0,7,275,1,0,0,0,9,277,1,0,0,0,11,279,1,0,0,0,13,281,
-        1,0,0,0,15,283,1,0,0,0,17,285,1,0,0,0,19,287,1,0,0,0,21,289,1,0,
-        0,0,23,291,1,0,0,0,25,293,1,0,0,0,27,295,1,0,0,0,29,297,1,0,0,0,
-        31,300,1,0,0,0,33,303,1,0,0,0,35,305,1,0,0,0,37,307,1,0,0,0,39,309,
-        1,0,0,0,41,311,1,0,0,0,43,313,1,0,0,0,45,315,1,0,0,0,47,317,1,0,
-        0,0,49,320,1,0,0,0,51,323,1,0,0,0,53,327,1,0,0,0,55,329,1,0,0,0,
-        57,331,1,0,0,0,59,334,1,0,0,0,61,337,1,0,0,0,63,340,1,0,0,0,65,343,
-        1,0,0,0,67,347,1,0,0,0,69,351,1,0,0,0,71,353,1,0,0,0,73,355,1,0,
-        0,0,75,357,1,0,0,0,77,360,1,0,0,0,79,363,1,0,0,0,81,366,1,0,0,0,
-        83,369,1,0,0,0,85,372,1,0,0,0,87,375,1,0,0,0,89,378,1,0,0,0,91,382,
-        1,0,0,0,93,386,1,0,0,0,95,391,1,0,0,0,97,394,1,0,0,0,99,397,1,0,
-        0,0,101,400,1,0,0,0,103,414,1,0,0,0,105,440,1,0,0,0,107,442,1,0,
-        0,0,109,449,1,0,0,0,111,456,1,0,0,0,113,462,1,0,0,0,115,465,1,0,
-        0,0,117,476,1,0,0,0,119,483,1,0,0,0,121,488,1,0,0,0,123,493,1,0,
-        0,0,125,497,1,0,0,0,127,501,1,0,0,0,129,507,1,0,0,0,131,515,1,0,
-        0,0,133,522,1,0,0,0,135,527,1,0,0,0,137,536,1,0,0,0,139,540,1,0,
-        0,0,141,547,1,0,0,0,143,553,1,0,0,0,145,562,1,0,0,0,147,571,1,0,
-        0,0,149,576,1,0,0,0,151,581,1,0,0,0,153,589,1,0,0,0,155,592,1,0,
-        0,0,157,598,1,0,0,0,159,605,1,0,0,0,161,608,1,0,0,0,163,612,1,0,
-        0,0,165,618,1,0,0,0,167,623,1,0,0,0,169,631,1,0,0,0,171,637,1,0,
-        0,0,173,643,1,0,0,0,175,650,1,0,0,0,177,657,1,0,0,0,179,669,1,0,
-        0,0,181,674,1,0,0,0,183,683,1,0,0,0,185,691,1,0,0,0,187,702,1,0,
-        0,0,189,711,1,0,0,0,191,722,1,0,0,0,193,730,1,0,0,0,195,737,1,0,
-        0,0,197,760,1,0,0,0,199,763,1,0,0,0,201,769,1,0,0,0,203,783,1,0,
-        0,0,205,794,1,0,0,0,207,800,1,0,0,0,209,806,1,0,0,0,211,812,1,0,
-        0,0,213,816,1,0,0,0,215,818,1,0,0,0,217,822,1,0,0,0,219,828,1,0,
-        0,0,221,830,1,0,0,0,223,835,1,0,0,0,225,837,1,0,0,0,227,843,1,0,
-        0,0,229,845,1,0,0,0,231,847,1,0,0,0,233,849,1,0,0,0,235,859,1,0,
-        0,0,237,861,1,0,0,0,239,873,1,0,0,0,241,879,1,0,0,0,243,881,1,0,
-        0,0,245,883,1,0,0,0,247,885,1,0,0,0,249,895,1,0,0,0,251,901,1,0,
-        0,0,253,906,1,0,0,0,255,908,1,0,0,0,257,910,1,0,0,0,259,913,1,0,
-        0,0,261,924,1,0,0,0,263,264,4,0,0,0,264,265,5,47,0,0,265,266,3,247,
-        123,0,266,267,5,47,0,0,267,268,3,249,124,0,268,2,1,0,0,0,269,270,
-        7,0,0,0,270,271,1,0,0,0,271,272,6,1,0,0,272,4,1,0,0,0,273,274,5,
-        91,0,0,274,6,1,0,0,0,275,276,5,93,0,0,276,8,1,0,0,0,277,278,5,40,
-        0,0,278,10,1,0,0,0,279,280,5,41,0,0,280,12,1,0,0,0,281,282,5,123,
-        0,0,282,14,1,0,0,0,283,284,5,125,0,0,284,16,1,0,0,0,285,286,5,59,
-        0,0,286,18,1,0,0,0,287,288,5,44,0,0,288,20,1,0,0,0,289,290,5,61,
-        0,0,290,22,1,0,0,0,291,292,5,63,0,0,292,24,1,0,0,0,293,294,5,58,
-        0,0,294,26,1,0,0,0,295,296,5,46,0,0,296,28,1,0,0,0,297,298,5,43,
-        0,0,298,299,5,43,0,0,299,30,1,0,0,0,300,301,5,45,0,0,301,302,5,45,
-        0,0,302,32,1,0,0,0,303,304,5,43,0,0,304,34,1,0,0,0,305,306,5,45,
-        0,0,306,36,1,0,0,0,307,308,5,126,0,0,308,38,1,0,0,0,309,310,5,33,
-        0,0,310,40,1,0,0,0,311,312,5,42,0,0,312,42,1,0,0,0,313,314,5,47,
-        0,0,314,44,1,0,0,0,315,316,5,37,0,0,316,46,1,0,0,0,317,318,5,62,
-        0,0,318,319,5,62,0,0,319,48,1,0,0,0,320,321,5,60,0,0,321,322,5,60,
-        0,0,322,50,1,0,0,0,323,324,5,62,0,0,324,325,5,62,0,0,325,326,5,62,
-        0,0,326,52,1,0,0,0,327,328,5,60,0,0,328,54,1,0,0,0,329,330,5,62,
-        0,0,330,56,1,0,0,0,331,332,5,60,0,0,332,333,5,61,0,0,333,58,1,0,
-        0,0,334,335,5,62,0,0,335,336,5,61,0,0,336,60,1,0,0,0,337,338,5,61,
-        0,0,338,339,5,61,0,0,339,62,1,0,0,0,340,341,5,33,0,0,341,342,5,61,
-        0,0,342,64,1,0,0,0,343,344,5,61,0,0,344,345,5,61,0,0,345,346,5,61,
-        0,0,346,66,1,0,0,0,347,348,5,33,0,0,348,349,5,61,0,0,349,350,5,61,
-        0,0,350,68,1,0,0,0,351,352,5,38,0,0,352,70,1,0,0,0,353,354,5,94,
-        0,0,354,72,1,0,0,0,355,356,5,124,0,0,356,74,1,0,0,0,357,358,5,38,
-        0,0,358,359,5,38,0,0,359,76,1,0,0,0,360,361,5,124,0,0,361,362,5,
-        124,0,0,362,78,1,0,0,0,363,364,5,42,0,0,364,365,5,61,0,0,365,80,
+        70207,70208,70272,70278,70280,70280,70282,70285,70287,70301,70303,
+        70312,70320,70366,70405,70412,70415,70416,70419,70440,70442,70448,
+        70450,70451,70453,70457,70461,70461,70480,70480,70493,70497,70656,
+        70708,70727,70730,70751,70753,70784,70831,70852,70853,70855,70855,
+        71040,71086,71128,71131,71168,71215,71236,71236,71296,71338,71352,
+        71352,71424,71450,71488,71494,71680,71723,71840,71903,71935,71942,
+        71945,71945,71948,71955,71957,71958,71960,71983,71999,71999,72001,
+        72001,72096,72103,72106,72144,72161,72161,72163,72163,72192,72192,
+        72203,72242,72250,72250,72272,72272,72284,72329,72349,72349,72368,
+        72440,72704,72712,72714,72750,72768,72768,72818,72847,72960,72966,
+        72968,72969,72971,73008,73030,73030,73056,73061,73063,73064,73066,
+        73097,73112,73112,73440,73458,73474,73474,73476,73488,73490,73523,
+        73648,73648,73728,74649,74880,75075,77712,77808,77824,78895,78913,
+        78918,82944,83526,92160,92728,92736,92766,92784,92862,92880,92909,
+        92928,92975,92992,92995,93027,93047,93053,93071,93760,93823,93952,
+        94026,94032,94032,94099,94111,94176,94177,94179,94179,94208,100343,
+        100352,101589,101632,101640,110576,110579,110581,110587,110589,110590,
+        110592,110882,110898,110898,110928,110930,110933,110933,110948,110951,
+        110960,111355,113664,113770,113776,113788,113792,113800,113808,113817,
+        119808,119892,119894,119964,119966,119967,119970,119970,119973,119974,
+        119977,119980,119982,119993,119995,119995,119997,120003,120005,120069,
+        120071,120074,120077,120084,120086,120092,120094,120121,120123,120126,
+        120128,120132,120134,120134,120138,120144,120146,120485,120488,120512,
+        120514,120538,120540,120570,120572,120596,120598,120628,120630,120654,
+        120656,120686,120688,120712,120714,120744,120746,120770,120772,120779,
+        122624,122654,122661,122666,122928,122989,123136,123180,123191,123197,
+        123214,123214,123536,123565,123584,123627,124112,124139,124896,124902,
+        124904,124907,124909,124910,124912,124926,124928,125124,125184,125251,
+        125259,125259,126464,126467,126469,126495,126497,126498,126500,126500,
+        126503,126503,126505,126514,126516,126519,126521,126521,126523,126523,
+        126530,126530,126535,126535,126537,126537,126539,126539,126541,126543,
+        126545,126546,126548,126548,126551,126551,126553,126553,126555,126555,
+        126557,126557,126559,126559,126561,126562,126564,126564,126567,126570,
+        126572,126578,126580,126583,126585,126588,126590,126590,126592,126601,
+        126603,126619,126625,126627,126629,126633,126635,126651,131072,173791,
+        173824,177977,177984,178205,178208,183969,183984,191456,194560,195101,
+        196608,201546,201552,205743,407,0,48,57,95,95,768,879,1155,1159,
+        1425,1469,1471,1471,1473,1474,1476,1477,1479,1479,1552,1562,1611,
+        1641,1648,1648,1750,1756,1759,1764,1767,1768,1770,1773,1776,1785,
+        1809,1809,1840,1866,1958,1968,1984,1993,2027,2035,2045,2045,2070,
+        2073,2075,2083,2085,2087,2089,2093,2137,2139,2200,2207,2250,2273,
+        2275,2306,2362,2362,2364,2364,2369,2376,2381,2381,2385,2391,2402,
+        2403,2406,2415,2433,2433,2492,2492,2497,2500,2509,2509,2530,2531,
+        2534,2543,2558,2558,2561,2562,2620,2620,2625,2626,2631,2632,2635,
+        2637,2641,2641,2662,2673,2677,2677,2689,2690,2748,2748,2753,2757,
+        2759,2760,2765,2765,2786,2787,2790,2799,2810,2815,2817,2817,2876,
+        2876,2879,2879,2881,2884,2893,2893,2901,2902,2914,2915,2918,2927,
+        2946,2946,3008,3008,3021,3021,3046,3055,3072,3072,3076,3076,3132,
+        3132,3134,3136,3142,3144,3146,3149,3157,3158,3170,3171,3174,3183,
+        3201,3201,3260,3260,3263,3263,3270,3270,3276,3277,3298,3299,3302,
+        3311,3328,3329,3387,3388,3393,3396,3405,3405,3426,3427,3430,3439,
+        3457,3457,3530,3530,3538,3540,3542,3542,3558,3567,3633,3633,3636,
+        3642,3655,3662,3664,3673,3761,3761,3764,3772,3784,3790,3792,3801,
+        3864,3865,3872,3881,3893,3893,3895,3895,3897,3897,3953,3966,3968,
+        3972,3974,3975,3981,3991,3993,4028,4038,4038,4141,4144,4146,4151,
+        4153,4154,4157,4158,4160,4169,4184,4185,4190,4192,4209,4212,4226,
+        4226,4229,4230,4237,4237,4240,4249,4253,4253,4957,4959,5906,5908,
+        5938,5939,5970,5971,6002,6003,6068,6069,6071,6077,6086,6086,6089,
+        6099,6109,6109,6112,6121,6155,6157,6159,6169,6277,6278,6313,6313,
+        6432,6434,6439,6440,6450,6450,6457,6459,6470,6479,6608,6617,6679,
+        6680,6683,6683,6742,6742,6744,6750,6752,6752,6754,6754,6757,6764,
+        6771,6780,6783,6793,6800,6809,6832,6845,6847,6862,6912,6915,6964,
+        6964,6966,6970,6972,6972,6978,6978,6992,7001,7019,7027,7040,7041,
+        7074,7077,7080,7081,7083,7085,7088,7097,7142,7142,7144,7145,7149,
+        7149,7151,7153,7212,7219,7222,7223,7232,7241,7248,7257,7376,7378,
+        7380,7392,7394,7400,7405,7405,7412,7412,7416,7417,7616,7679,8255,
+        8256,8276,8276,8400,8412,8417,8417,8421,8432,11503,11505,11647,11647,
+        11744,11775,12330,12333,12441,12442,42528,42537,42607,42607,42612,
+        42621,42654,42655,42736,42737,43010,43010,43014,43014,43019,43019,
+        43045,43046,43052,43052,43204,43205,43216,43225,43232,43249,43263,
+        43273,43302,43309,43335,43345,43392,43394,43443,43443,43446,43449,
+        43452,43453,43472,43481,43493,43493,43504,43513,43561,43566,43569,
+        43570,43573,43574,43587,43587,43596,43596,43600,43609,43644,43644,
+        43696,43696,43698,43700,43703,43704,43710,43711,43713,43713,43756,
+        43757,43766,43766,44005,44005,44008,44008,44013,44013,44016,44025,
+        64286,64286,65024,65039,65056,65071,65075,65076,65101,65103,65296,
+        65305,65343,65343,66045,66045,66272,66272,66422,66426,66720,66729,
+        68097,68099,68101,68102,68108,68111,68152,68154,68159,68159,68325,
+        68326,68900,68903,68912,68921,69291,69292,69373,69375,69446,69456,
+        69506,69509,69633,69633,69688,69702,69734,69744,69747,69748,69759,
+        69761,69811,69814,69817,69818,69826,69826,69872,69881,69888,69890,
+        69927,69931,69933,69940,69942,69951,70003,70003,70016,70017,70070,
+        70078,70089,70092,70095,70105,70191,70193,70196,70196,70198,70199,
+        70206,70206,70209,70209,70367,70367,70371,70378,70384,70393,70400,
+        70401,70459,70460,70464,70464,70502,70508,70512,70516,70712,70719,
+        70722,70724,70726,70726,70736,70745,70750,70750,70835,70840,70842,
+        70842,70847,70848,70850,70851,70864,70873,71090,71093,71100,71101,
+        71103,71104,71132,71133,71219,71226,71229,71229,71231,71232,71248,
+        71257,71339,71339,71341,71341,71344,71349,71351,71351,71360,71369,
+        71453,71455,71458,71461,71463,71467,71472,71481,71727,71735,71737,
+        71738,71904,71913,71995,71996,71998,71998,72003,72003,72016,72025,
+        72148,72151,72154,72155,72160,72160,72193,72202,72243,72248,72251,
+        72254,72263,72263,72273,72278,72281,72283,72330,72342,72344,72345,
+        72752,72758,72760,72765,72767,72767,72784,72793,72850,72871,72874,
+        72880,72882,72883,72885,72886,73009,73014,73018,73018,73020,73021,
+        73023,73029,73031,73031,73040,73049,73104,73105,73109,73109,73111,
+        73111,73120,73129,73459,73460,73472,73473,73526,73530,73536,73536,
+        73538,73538,73552,73561,78912,78912,78919,78933,92768,92777,92864,
+        92873,92912,92916,92976,92982,93008,93017,94031,94031,94095,94098,
+        94180,94180,113821,113822,118528,118573,118576,118598,119143,119145,
+        119163,119170,119173,119179,119210,119213,119362,119364,120782,120831,
+        121344,121398,121403,121452,121461,121461,121476,121476,121499,121503,
+        121505,121519,122880,122886,122888,122904,122907,122913,122915,122916,
+        122918,122922,123023,123023,123184,123190,123200,123209,123566,123566,
+        123628,123641,124140,124153,125136,125142,125252,125258,125264,125273,
+        130032,130041,917760,917999,6,0,10,10,13,13,42,42,47,47,91,92,8232,
+        8233,5,0,10,10,13,13,47,47,91,92,8232,8233,4,0,10,10,13,13,92,93,
+        8232,8233,941,0,1,1,0,0,0,0,3,1,0,0,0,0,5,1,0,0,0,0,7,1,0,0,0,0,
+        9,1,0,0,0,0,11,1,0,0,0,0,13,1,0,0,0,0,15,1,0,0,0,0,17,1,0,0,0,0,
+        19,1,0,0,0,0,21,1,0,0,0,0,23,1,0,0,0,0,25,1,0,0,0,0,27,1,0,0,0,0,
+        29,1,0,0,0,0,31,1,0,0,0,0,33,1,0,0,0,0,35,1,0,0,0,0,37,1,0,0,0,0,
+        39,1,0,0,0,0,41,1,0,0,0,0,43,1,0,0,0,0,45,1,0,0,0,0,47,1,0,0,0,0,
+        49,1,0,0,0,0,51,1,0,0,0,0,53,1,0,0,0,0,55,1,0,0,0,0,57,1,0,0,0,0,
+        59,1,0,0,0,0,61,1,0,0,0,0,63,1,0,0,0,0,65,1,0,0,0,0,67,1,0,0,0,0,
+        69,1,0,0,0,0,71,1,0,0,0,0,73,1,0,0,0,0,75,1,0,0,0,0,77,1,0,0,0,0,
+        79,1,0,0,0,0,81,1,0,0,0,0,83,1,0,0,0,0,85,1,0,0,0,0,87,1,0,0,0,0,
+        89,1,0,0,0,0,91,1,0,0,0,0,93,1,0,0,0,0,95,1,0,0,0,0,97,1,0,0,0,0,
+        99,1,0,0,0,0,101,1,0,0,0,0,103,1,0,0,0,0,105,1,0,0,0,0,107,1,0,0,
+        0,0,109,1,0,0,0,0,111,1,0,0,0,0,113,1,0,0,0,0,115,1,0,0,0,0,117,
+        1,0,0,0,0,119,1,0,0,0,0,121,1,0,0,0,0,123,1,0,0,0,0,125,1,0,0,0,
+        0,127,1,0,0,0,0,129,1,0,0,0,0,131,1,0,0,0,0,133,1,0,0,0,0,135,1,
+        0,0,0,0,137,1,0,0,0,0,139,1,0,0,0,0,141,1,0,0,0,0,143,1,0,0,0,0,
+        145,1,0,0,0,0,147,1,0,0,0,0,149,1,0,0,0,0,151,1,0,0,0,0,153,1,0,
+        0,0,0,155,1,0,0,0,0,157,1,0,0,0,0,159,1,0,0,0,0,161,1,0,0,0,0,163,
+        1,0,0,0,0,165,1,0,0,0,0,167,1,0,0,0,0,169,1,0,0,0,0,171,1,0,0,0,
+        0,173,1,0,0,0,0,175,1,0,0,0,0,177,1,0,0,0,0,179,1,0,0,0,0,181,1,
+        0,0,0,0,183,1,0,0,0,0,185,1,0,0,0,0,187,1,0,0,0,0,189,1,0,0,0,0,
+        191,1,0,0,0,0,193,1,0,0,0,0,195,1,0,0,0,0,197,1,0,0,0,0,199,1,0,
+        0,0,0,201,1,0,0,0,0,203,1,0,0,0,0,205,1,0,0,0,1,263,1,0,0,0,3,269,
+        1,0,0,0,5,273,1,0,0,0,7,275,1,0,0,0,9,277,1,0,0,0,11,279,1,0,0,0,
+        13,281,1,0,0,0,15,283,1,0,0,0,17,285,1,0,0,0,19,287,1,0,0,0,21,289,
+        1,0,0,0,23,291,1,0,0,0,25,293,1,0,0,0,27,295,1,0,0,0,29,297,1,0,
+        0,0,31,300,1,0,0,0,33,303,1,0,0,0,35,305,1,0,0,0,37,307,1,0,0,0,
+        39,309,1,0,0,0,41,311,1,0,0,0,43,313,1,0,0,0,45,315,1,0,0,0,47,317,
+        1,0,0,0,49,320,1,0,0,0,51,323,1,0,0,0,53,327,1,0,0,0,55,329,1,0,
+        0,0,57,331,1,0,0,0,59,334,1,0,0,0,61,337,1,0,0,0,63,340,1,0,0,0,
+        65,343,1,0,0,0,67,347,1,0,0,0,69,351,1,0,0,0,71,353,1,0,0,0,73,355,
+        1,0,0,0,75,357,1,0,0,0,77,360,1,0,0,0,79,363,1,0,0,0,81,366,1,0,
+        0,0,83,369,1,0,0,0,85,372,1,0,0,0,87,375,1,0,0,0,89,378,1,0,0,0,
+        91,382,1,0,0,0,93,386,1,0,0,0,95,391,1,0,0,0,97,394,1,0,0,0,99,397,
+        1,0,0,0,101,400,1,0,0,0,103,414,1,0,0,0,105,440,1,0,0,0,107,442,
+        1,0,0,0,109,449,1,0,0,0,111,456,1,0,0,0,113,462,1,0,0,0,115,465,
+        1,0,0,0,117,476,1,0,0,0,119,483,1,0,0,0,121,488,1,0,0,0,123,493,
+        1,0,0,0,125,497,1,0,0,0,127,501,1,0,0,0,129,507,1,0,0,0,131,515,
+        1,0,0,0,133,522,1,0,0,0,135,527,1,0,0,0,137,536,1,0,0,0,139,540,
+        1,0,0,0,141,547,1,0,0,0,143,553,1,0,0,0,145,562,1,0,0,0,147,571,
+        1,0,0,0,149,576,1,0,0,0,151,581,1,0,0,0,153,589,1,0,0,0,155,592,
+        1,0,0,0,157,598,1,0,0,0,159,605,1,0,0,0,161,608,1,0,0,0,163,612,
+        1,0,0,0,165,618,1,0,0,0,167,623,1,0,0,0,169,631,1,0,0,0,171,637,
+        1,0,0,0,173,643,1,0,0,0,175,650,1,0,0,0,177,657,1,0,0,0,179,669,
+        1,0,0,0,181,674,1,0,0,0,183,683,1,0,0,0,185,691,1,0,0,0,187,702,
+        1,0,0,0,189,711,1,0,0,0,191,722,1,0,0,0,193,730,1,0,0,0,195,737,
+        1,0,0,0,197,760,1,0,0,0,199,763,1,0,0,0,201,769,1,0,0,0,203,783,
+        1,0,0,0,205,794,1,0,0,0,207,800,1,0,0,0,209,806,1,0,0,0,211,812,
+        1,0,0,0,213,816,1,0,0,0,215,818,1,0,0,0,217,822,1,0,0,0,219,828,
+        1,0,0,0,221,830,1,0,0,0,223,835,1,0,0,0,225,837,1,0,0,0,227,843,
+        1,0,0,0,229,845,1,0,0,0,231,847,1,0,0,0,233,849,1,0,0,0,235,859,
+        1,0,0,0,237,861,1,0,0,0,239,873,1,0,0,0,241,879,1,0,0,0,243,881,
+        1,0,0,0,245,883,1,0,0,0,247,885,1,0,0,0,249,895,1,0,0,0,251,901,
+        1,0,0,0,253,906,1,0,0,0,255,908,1,0,0,0,257,910,1,0,0,0,259,913,
+        1,0,0,0,261,924,1,0,0,0,263,264,4,0,0,0,264,265,5,47,0,0,265,266,
+        3,247,123,0,266,267,5,47,0,0,267,268,3,249,124,0,268,2,1,0,0,0,269,
+        270,7,0,0,0,270,271,1,0,0,0,271,272,6,1,0,0,272,4,1,0,0,0,273,274,
+        5,91,0,0,274,6,1,0,0,0,275,276,5,93,0,0,276,8,1,0,0,0,277,278,5,
+        40,0,0,278,10,1,0,0,0,279,280,5,41,0,0,280,12,1,0,0,0,281,282,5,
+        123,0,0,282,14,1,0,0,0,283,284,5,125,0,0,284,16,1,0,0,0,285,286,
+        5,59,0,0,286,18,1,0,0,0,287,288,5,44,0,0,288,20,1,0,0,0,289,290,
+        5,61,0,0,290,22,1,0,0,0,291,292,5,63,0,0,292,24,1,0,0,0,293,294,
+        5,58,0,0,294,26,1,0,0,0,295,296,5,46,0,0,296,28,1,0,0,0,297,298,
+        5,43,0,0,298,299,5,43,0,0,299,30,1,0,0,0,300,301,5,45,0,0,301,302,
+        5,45,0,0,302,32,1,0,0,0,303,304,5,43,0,0,304,34,1,0,0,0,305,306,
+        5,45,0,0,306,36,1,0,0,0,307,308,5,126,0,0,308,38,1,0,0,0,309,310,
+        5,33,0,0,310,40,1,0,0,0,311,312,5,42,0,0,312,42,1,0,0,0,313,314,
+        5,47,0,0,314,44,1,0,0,0,315,316,5,37,0,0,316,46,1,0,0,0,317,318,
+        5,62,0,0,318,319,5,62,0,0,319,48,1,0,0,0,320,321,5,60,0,0,321,322,
+        5,60,0,0,322,50,1,0,0,0,323,324,5,62,0,0,324,325,5,62,0,0,325,326,
+        5,62,0,0,326,52,1,0,0,0,327,328,5,60,0,0,328,54,1,0,0,0,329,330,
+        5,62,0,0,330,56,1,0,0,0,331,332,5,60,0,0,332,333,5,61,0,0,333,58,
+        1,0,0,0,334,335,5,62,0,0,335,336,5,61,0,0,336,60,1,0,0,0,337,338,
+        5,61,0,0,338,339,5,61,0,0,339,62,1,0,0,0,340,341,5,33,0,0,341,342,
+        5,61,0,0,342,64,1,0,0,0,343,344,5,61,0,0,344,345,5,61,0,0,345,346,
+        5,61,0,0,346,66,1,0,0,0,347,348,5,33,0,0,348,349,5,61,0,0,349,350,
+        5,61,0,0,350,68,1,0,0,0,351,352,5,38,0,0,352,70,1,0,0,0,353,354,
+        5,94,0,0,354,72,1,0,0,0,355,356,5,124,0,0,356,74,1,0,0,0,357,358,
+        5,38,0,0,358,359,5,38,0,0,359,76,1,0,0,0,360,361,5,124,0,0,361,362,
+        5,124,0,0,362,78,1,0,0,0,363,364,5,42,0,0,364,365,5,61,0,0,365,80,
         1,0,0,0,366,367,5,47,0,0,367,368,5,61,0,0,368,82,1,0,0,0,369,370,
         5,37,0,0,370,371,5,61,0,0,371,84,1,0,0,0,372,373,5,43,0,0,373,374,
         5,61,0,0,374,86,1,0,0,0,375,376,5,45,0,0,376,377,5,61,0,0,377,88,
         1,0,0,0,378,379,5,60,0,0,379,380,5,60,0,0,380,381,5,61,0,0,381,90,
         1,0,0,0,382,383,5,62,0,0,383,384,5,62,0,0,384,385,5,61,0,0,385,92,
         1,0,0,0,386,387,5,62,0,0,387,388,5,62,0,0,388,389,5,62,0,0,389,390,
         5,61,0,0,390,94,1,0,0,0,391,392,5,38,0,0,392,393,5,61,0,0,393,96,
@@ -715,15 +718,15 @@
                   "RegularExpressionBackslashSequence", "RegularExpressionClass", 
                   "RegularExpressionClassChar" ]
 
     grammarFileName = "ECMAScript.g4"
 
     def __init__(self, input=None, output:TextIO = sys.stdout):
         super().__init__(input, output)
-        self.checkVersion("4.12.0")
+        self.checkVersion("4.13.0")
         self._interp = LexerATNSimulator(self, self.atn, self.decisionsToDFA, PredictionContextCache())
         self._actions = None
         self._predicates = None
 
 
         # A flag indicating if the lexer should operate in strict mode
         # When set to true, FutureReservedWords are tokenized, when false,
```

### Comparing `streamflow-0.2.0.dev5/streamflow/cwl/antlr/ECMAScriptListener.py` & `streamflow-0.2.0.dev6/streamflow/cwl/antlr/ECMAScriptListener.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-# Generated from ECMAScript.g4 by ANTLR 4.12.0
+# Generated from ECMAScript.g4 by ANTLR 4.13.0
 from antlr4 import *
-if __name__ is not None and "." in __name__:
+if "." in __name__:
     from .ECMAScriptParser import ECMAScriptParser
 else:
     from ECMAScriptParser import ECMAScriptParser
 
 # This class defines a complete listener for a parse tree produced by ECMAScriptParser.
 class ECMAScriptListener(ParseTreeListener):
```

### Comparing `streamflow-0.2.0.dev5/streamflow/cwl/antlr/ECMAScriptParser.py` & `streamflow-0.2.0.dev6/streamflow/cwl/antlr/ECMAScriptParser.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-# Generated from ECMAScript.g4 by ANTLR 4.12.0
+# Generated from ECMAScript.g4 by ANTLR 4.13.0
 # encoding: utf-8
-import sys
-
 from antlr4 import *
-
+from io import StringIO
+import sys
 if sys.version_info[1] > 5:
 	from typing import TextIO
 else:
 	from typing.io import TextIO
 
 def serializedATN():
     return [
@@ -471,15 +470,15 @@
     WhiteSpaces=100
     MultiLineComment=101
     SingleLineComment=102
     UnexpectedCharacter=103
 
     def __init__(self, input:TokenStream, output:TextIO = sys.stdout):
         super().__init__(input, output)
-        self.checkVersion("4.12.0")
+        self.checkVersion("4.13.0")
         self._interp = ParserATNSimulator(self, self.atn, self.decisionsToDFA, self.sharedContextCache)
         self._predicates = None
 
 
 
     def here(self, type):
         """Returns `True` iff on the current index of the parser's
```

### Comparing `streamflow-0.2.0.dev5/streamflow/cwl/combinator.py` & `streamflow-0.2.0.dev6/streamflow/cwl/combinator.py`

 * *Files 22% similar despite different names*

```diff
@@ -62,21 +62,35 @@
 
     async def combine(
         self, port_name: str, token: Token
     ) -> AsyncIterable[MutableMapping[str, Token]]:
         if not isinstance(token, IterationTerminationToken):
             async for schema in super().combine(port_name, token):
                 # If there is only one input, merge its value
+                input_token_ids = []
                 if len(self.input_names) == 1:
-                    if isinstance(outputs := schema[self.input_names[0]], ListToken):
+                    if isinstance(
+                        outputs := schema[self.input_names[0]]["token"], ListToken
+                    ):
                         outputs = outputs.value
                     else:
                         outputs = [outputs]
-                    tag = schema[self.input_names[0]].tag
+                    tag = schema[self.input_names[0]]["token"].tag
+                    input_token_ids = schema[self.input_names[0]]["input_ids"]
                 # Otherwise, merge multiple inputs in a single list
                 else:
-                    outputs = [schema[name] for name in self.input_names]
+                    outputs = [schema[name]["token"] for name in self.input_names]
+                    input_token_ids = [
+                        id
+                        for name in self.input_names
+                        for id in schema[name]["input_ids"]
+                    ]
                     tag = get_tag(outputs)
                 # Flatten if needed
                 if self.flatten:
                     outputs = _flatten_token_list(outputs)
-                yield {self.output_name: ListToken(value=outputs, tag=tag)}
+                yield {
+                    self.output_name: {
+                        "token": ListToken(value=outputs, tag=tag),
+                        "input_ids": input_token_ids,
+                    }
+                }
```

### Comparing `streamflow-0.2.0.dev5/streamflow/cwl/command.py` & `streamflow-0.2.0.dev6/streamflow/cwl/command.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev5/streamflow/cwl/expression.py` & `streamflow-0.2.0.dev6/streamflow/cwl/expression.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev5/streamflow/cwl/hardware.py` & `streamflow-0.2.0.dev6/streamflow/cwl/hardware.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev5/streamflow/cwl/main.py` & `streamflow-0.2.0.dev6/streamflow/cwl/main.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev5/streamflow/cwl/processor.py` & `streamflow-0.2.0.dev6/streamflow/cwl/processor.py`

 * *Files 1% similar despite different names*

```diff
@@ -342,15 +342,15 @@
                     token_value=token.value,
                     token_type=self.token_type,
                     enum_symbols=self.enum_symbols,
                     optional=self.optional,
                     check_file=True,
                 )
         # Return the token
-        return token
+        return token.update(token.value)
 
 
 class CWLCommandOutputProcessor(CommandOutputProcessor):
     def __init__(
         self,
         name: str,
         workflow: Workflow,
```

### Comparing `streamflow-0.2.0.dev5/streamflow/cwl/requirement/docker/docker.py` & `streamflow-0.2.0.dev6/streamflow/cwl/requirement/docker/docker.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev5/streamflow/cwl/requirement/docker/kubernetes.py` & `streamflow-0.2.0.dev6/streamflow/cwl/requirement/docker/kubernetes.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev5/streamflow/cwl/requirement/docker/schemas/docker.json` & `streamflow-0.2.0.dev6/streamflow/cwl/requirement/docker/schemas/docker.json`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev5/streamflow/cwl/requirement/docker/schemas/kubernetes.jinja2` & `streamflow-0.2.0.dev6/streamflow/cwl/requirement/docker/schemas/kubernetes.jinja2`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev5/streamflow/cwl/requirement/docker/schemas/kubernetes.json` & `streamflow-0.2.0.dev6/streamflow/cwl/requirement/docker/schemas/kubernetes.json`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev5/streamflow/cwl/requirement/docker/schemas/singularity.json` & `streamflow-0.2.0.dev6/streamflow/cwl/requirement/docker/schemas/singularity.json`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev5/streamflow/cwl/requirement/docker/singularity.py` & `streamflow-0.2.0.dev6/streamflow/cwl/requirement/docker/singularity.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev5/streamflow/cwl/requirement/docker/translator.py` & `streamflow-0.2.0.dev6/streamflow/cwl/requirement/docker/translator.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev5/streamflow/cwl/runner.py` & `streamflow-0.2.0.dev6/streamflow/cwl/runner.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev5/streamflow/cwl/step.py` & `streamflow-0.2.0.dev6/streamflow/cwl/step.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 from streamflow.log_handler import logger
 from streamflow.workflow.port import JobPort
 from streamflow.workflow.step import (
     ConditionalStep,
     InputInjectorStep,
     LoopOutputStep,
     TransferStep,
+    _get_token_ids,
 )
 from streamflow.workflow.token import IterationTerminationToken, ListToken, ObjectToken
 
 
 async def _download_file(job: Job, url: str, context: StreamFlowContext) -> str:
     connector = context.scheduler.get_connector(job.name)
     locations = context.scheduler.get_locations(job.name)
@@ -95,20 +96,32 @@
             raise WorkflowDefinitionException(
                 "Conditional 'when' must evaluate to 'true' or 'false'"
             )
 
     async def _on_true(self, inputs: MutableMapping[str, Token]):
         # Propagate output tokens
         for port_name, port in self.get_output_ports().items():
-            port.put(inputs[port_name])
+            port.put(
+                await self._persist_token(
+                    token=inputs[port_name].update(inputs[port_name].value),
+                    port=port,
+                    input_token_ids=_get_token_ids(inputs.values()),
+                )
+            )
 
     async def _on_false(self, inputs: MutableMapping[str, Token]):
         # Propagate skip tokens
         for port in self.get_skip_ports().values():
-            port.put(Token(value=None, tag=get_tag(inputs.values())))
+            port.put(
+                await self._persist_token(
+                    token=Token(value=None, tag=get_tag(inputs.values())),
+                    port=port,
+                    input_token_ids=_get_token_ids(inputs.values()),
+                )
+            )
 
     async def _save_additional_params(
         self, context: StreamFlowContext
     ) -> MutableMapping[str, Any]:
         return {
             **await super()._save_additional_params(context),
             **{
@@ -195,27 +208,39 @@
             workflow=await loading_context.load_workflow(context, row["workflow"]),
             scatter_method=params["scatter_method"],
         )
 
     async def _on_true(self, inputs: MutableMapping[str, Token]):
         # Propagate output tokens
         for port_name, port in self.get_output_ports().items():
-            port.put(inputs[port_name])
+            port.put(
+                await self._persist_token(
+                    token=inputs[port_name].update(inputs[port_name].value),
+                    port=port,
+                    input_token_ids=_get_token_ids(inputs.values()),
+                )
+            )
 
     async def _on_false(self, inputs: MutableMapping[str, Token]):
         # Get empty scatter return value
         if self.scatter_method == "nested_crossproduct":
             token_value = [
                 ListToken(value=[], tag=get_tag(inputs.values())) for _ in inputs
             ]
         else:
             token_value = []
         # Propagate skip tokens
         for port in self.get_skip_ports().values():
-            port.put(ListToken(value=token_value, tag=get_tag(inputs.values())))
+            port.put(
+                await self._persist_token(
+                    token=ListToken(value=token_value, tag=get_tag(inputs.values())),
+                    port=port,
+                    input_token_ids=_get_token_ids(inputs.values()),
+                )
+            )
 
     async def _save_additional_params(
         self, context: StreamFlowContext
     ) -> MutableMapping[str, Any]:
         return {
             **await super()._save_additional_params(context),
             **{"scatter_method": self.scatter_method},
```

### Comparing `streamflow-0.2.0.dev5/streamflow/cwl/token.py` & `streamflow-0.2.0.dev6/streamflow/cwl/token.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev5/streamflow/cwl/transformer.py` & `streamflow-0.2.0.dev6/streamflow/cwl/transformer.py`

 * *Files 3% similar despite different names*

```diff
@@ -73,15 +73,15 @@
             )
         if not self.default_port:
             raise WorkflowDefinitionException(
                 f"{self.name} step must contain a default port."
             )
         primary_token = next(iter(inputs[k] for k in inputs))
         if get_token_value(primary_token) is not None:
-            return {self.get_output_name(): primary_token}
+            return {self.get_output_name(): primary_token.update(primary_token.value)}
         else:
             if not self.default_token:
                 self.default_token = (
                     await self._get_inputs({"__default__": self.default_port})
                 )["__default__"]
             return {self.get_output_name(): self.default_token.retag(primary_token.tag)}
 
@@ -149,15 +149,15 @@
 
 
 class FirstNonNullTransformer(OneToOneTransformer):
     def _transform(self, name: str, token: Token) -> Token:
         if isinstance(token, ListToken):
             for t in token.value:
                 if get_token_value(t) is not None:
-                    return t
+                    return t.update(t.value)
             raise WorkflowExecutionException(f"All sources are null in token {name}")
         elif isinstance(token.value, Token):
             return token.update(self._transform(name, token.value))
         else:
             raise WorkflowExecutionException(f"Invalid value for token {name}")
 
     async def transform(
@@ -166,28 +166,31 @@
         return {self.get_output_name(): self._transform(*next(iter(inputs.items())))}
 
 
 class ForwardTransformer(OneToOneTransformer):
     async def transform(
         self, inputs: MutableMapping[str, Token]
     ) -> MutableMapping[str, Token]:
-        return {self.get_output_name(): next(iter(inputs.values()))}
+        token = next(iter(inputs.values()))
+        return {self.get_output_name(): token.update(token.value)}
 
 
 class ListToElementTransformer(OneToOneTransformer):
     def _transform(self, token: Token) -> Token:
         if isinstance(token, ListToken):
             if len(token.value) == 1:
-                return token.value[0]
+                return token.value[0].update(token.value[0].value)
             else:
                 return token.update(token.value)
         elif isinstance(token.value, Token):
             return token.update(self._transform(token.value))
         else:
-            return token.value
+            raise WorkflowDefinitionException(
+                f"Invalid token value: Token required, but received {type(token.value)}"
+            )
 
     async def transform(
         self, inputs: MutableMapping[str, Token]
     ) -> MutableMapping[str, Token]:
         return {self.get_output_name(): self._transform(next(iter(inputs.values())))}
 
 
@@ -202,15 +205,15 @@
                             f"Expected only one source to be non-null in token {name}"
                         )
                     ret = t
             if ret is None:
                 raise WorkflowExecutionException(
                     f"All sources are null in token {name}"
                 )
-            return ret
+            return ret.update(ret.value) if isinstance(ret, Token) else ret
         elif isinstance(token.value, Token):
             return token.update(self._transform(name, token.value))
         else:
             raise WorkflowExecutionException(f"Invalid value for token {name}")
 
     async def transform(
         self, inputs: MutableMapping[str, Token]
```

### Comparing `streamflow-0.2.0.dev5/streamflow/cwl/translator.py` & `streamflow-0.2.0.dev6/streamflow/cwl/translator.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev5/streamflow/cwl/utils.py` & `streamflow-0.2.0.dev6/streamflow/cwl/utils.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev5/streamflow/data/data_manager.py` & `streamflow-0.2.0.dev6/streamflow/data/data_manager.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev5/streamflow/data/remotepath.py` & `streamflow-0.2.0.dev6/streamflow/data/remotepath.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev5/streamflow/deployment/aiotarstream.py` & `streamflow-0.2.0.dev6/streamflow/deployment/aiotarstream.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev5/streamflow/deployment/connector/__init__.py` & `streamflow-0.2.0.dev6/streamflow/deployment/connector/__init__.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev5/streamflow/deployment/connector/base.py` & `streamflow-0.2.0.dev6/streamflow/deployment/connector/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -65,32 +65,14 @@
 
 
 class FutureAware(metaclass=FutureMeta):
     __slots__ = ()
 
 
 class BaseConnector(Connector, FutureAware):
-    @staticmethod
-    def get_option(
-        name: str,
-        value: Any,
-    ) -> str:
-        if len(name) > 1:
-            name = f"-{name} "
-        if isinstance(value, bool):
-            return f"-{name} " if value else ""
-        elif isinstance(value, str):
-            return f'-{name} "{value}" '
-        elif isinstance(value, MutableSequence):
-            return "".join([f'-{name} "{item}" ' for item in value])
-        elif value is None:
-            return ""
-        else:
-            raise TypeError("Unsupported value type")
-
     def __init__(self, deployment_name: str, config_dir: str, transferBufferSize: int):
         super().__init__(deployment_name, config_dir)
         self.transferBufferSize: int = transferBufferSize
         self.is_deployed: bool = False
 
     async def _copy_local_to_remote(
         self,
```

### Comparing `streamflow-0.2.0.dev5/streamflow/deployment/connector/container.py` & `streamflow-0.2.0.dev6/streamflow/deployment/connector/container.py`

 * *Files 19% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from cachetools import Cache, TTLCache
 
 from streamflow.core import utils
 from streamflow.core.asyncache import cachedmethod
 from streamflow.core.deployment import Connector, Location
 from streamflow.core.exception import WorkflowExecutionException
 from streamflow.core.scheduling import AvailableLocation
-from streamflow.core.utils import get_local_to_remote_destination
+from streamflow.core.utils import get_local_to_remote_destination, get_option
 from streamflow.deployment.connector.base import BaseConnector
 from streamflow.log_handler import logger
 
 
 def _check_docker_compose_installed():
     if which("docker-compose") is None:
         raise WorkflowExecutionException(
@@ -559,117 +559,106 @@
             if logger.isEnabledFor(logging.DEBUG):
                 logger.debug(f"Using Docker {await _get_docker_version()}.")
             # Pull image if it doesn't exist
             if not await _exists_docker_image(self.image):
                 await _pull_docker_image(self.image)
             # Deploy the Docker container
             for _ in range(0, self.replicas):
-                deploy_command = "".join(
-                    [
-                        "docker ",
-                        "run ",
-                        "--detach ",
-                        "--interactive ",
-                        self.get_option("add-host", self.addHost),
-                        self.get_option("blkio-weight", self.addHost),
-                        self.get_option("blkio-weight-device", self.blkioWeightDevice),
-                        self.get_option("cap-add", self.capAdd),
-                        self.get_option("cap-drop", self.capDrop),
-                        self.get_option("cgroup-parent", self.cgroupParent),
-                        self.get_option("cgroupns", self.cgroupns),
-                        self.get_option("cidfile", self.cidfile),
-                        self.get_option("cpu-period", self.cpuPeriod),
-                        self.get_option("cpu-quota", self.cpuQuota),
-                        self.get_option("cpu-rt-period", self.cpuRTPeriod),
-                        self.get_option("cpu-rt-runtime", self.cpuRTRuntime),
-                        self.get_option("cpu-shares", self.cpuShares),
-                        self.get_option("cpus", self.cpus),
-                        self.get_option("cpuset-cpus", self.cpusetCpus),
-                        self.get_option("cpuset-mems", self.cpusetMems),
-                        self.get_option("detach-keys", self.detachKeys),
-                        self.get_option("device", self.device),
-                        self.get_option("device-cgroup-rule", self.deviceCgroupRule),
-                        self.get_option("device-read-bps", self.deviceReadBps),
-                        self.get_option("device-read-iops", self.deviceReadIops),
-                        self.get_option("device-write-bps", self.deviceWriteBps),
-                        self.get_option("device-write-iops", self.deviceWriteIops),
-                        "--disable-content-trust={disableContentTrust} ".format(
-                            disableContentTrust="true"
-                            if self.disableContentTrust
-                            else "false"
-                        ),
-                        self.get_option("dns", self.dns),
-                        self.get_option("dns-option", self.dnsOptions),
-                        self.get_option("dns-search", self.dnsSearch),
-                        self.get_option("domainname", self.domainname),
-                        self.get_option("entrypoint", self.entrypoint),
-                        self.get_option("env", self.env),
-                        self.get_option("env-file", self.envFile),
-                        self.get_option("expose", self.expose),
-                        self.get_option("gpus", self.gpus),
-                        self.get_option("group-add", self.groupAdd),
-                        self.get_option("health-cmd", self.healthCmd),
-                        self.get_option("health-interval", self.healthInterval),
-                        self.get_option("health-retries", self.healthRetries),
-                        self.get_option("health-start-period", self.healthStartPeriod),
-                        self.get_option("health-timeout", self.healthTimeout),
-                        self.get_option("hostname", self.hostname),
-                        self.get_option("init", self.init),
-                        self.get_option("ip", self.ip),
-                        self.get_option("ip6", self.ip6),
-                        self.get_option("ipc", self.ipc),
-                        self.get_option("isolation", self.isolation),
-                        self.get_option("kernel-memory", self.kernelMemory),
-                        self.get_option("label", self.label),
-                        self.get_option("label-file", self.labelFile),
-                        self.get_option("link", self.link),
-                        self.get_option("link-local-ip", self.linkLocalIP),
-                        self.get_option("log-driver", self.logDriver),
-                        self.get_option("log-opt", self.logOpts),
-                        self.get_option("mac-address", self.macAddress),
-                        self.get_option("memory", self.memory),
-                        self.get_option("memory-reservation", self.memoryReservation),
-                        self.get_option("memory-swap", self.memorySwap),
-                        self.get_option("memory-swappiness", self.memorySwappiness),
-                        self.get_option("mount", self.mount),
-                        self.get_option("network", self.network),
-                        self.get_option("network-alias", self.networkAlias),
-                        self.get_option("no-healthcheck", self.noHealthcheck),
-                        self.get_option("oom-kill-disable", self.oomKillDisable),
-                        self.get_option("oom-score-adj", self.oomScoreAdj),
-                        self.get_option("pid", self.pid),
-                        self.get_option("pids-limit", self.pidsLimit),
-                        self.get_option("privileged", self.privileged),
-                        self.get_option("publish", self.publish),
-                        self.get_option("publish-all", self.publishAll),
-                        self.get_option("read-only", self.readOnly),
-                        self.get_option("restart", self.restart),
-                        self.get_option("rm", self.rm),
-                        self.get_option("runtime", self.runtime),
-                        self.get_option("security-opt", self.securityOpts),
-                        self.get_option("shm-size", self.shmSize),
-                        "--sig-proxy={sigProxy} ".format(
-                            sigProxy="true" if self.sigProxy else "false"
-                        ),
-                        self.get_option("stop-signal", self.stopSignal),
-                        self.get_option("stop-timeout", self.stopTimeout),
-                        self.get_option("storage-opt", self.storageOpts),
-                        self.get_option("sysctl", self.sysctl),
-                        self.get_option("tmpfs", self.tmpfs),
-                        self.get_option("ulimit", self.ulimit),
-                        self.get_option("user", self.user),
-                        self.get_option("userns", self.userns),
-                        self.get_option("uts", self.uts),
-                        self.get_option("volume", self.volume),
-                        self.get_option("volume-driver", self.volumeDriver),
-                        self.get_option("volumes-from", self.volumesFrom),
-                        self.get_option("workdir", self.workdir),
-                        f"{self.image} ",
-                        " ".join(self.command) if self.command else "",
-                    ]
+                deploy_command = (
+                    f"docker run --detach --interactive "
+                    f"{get_option('add-host', self.addHost)}"
+                    f"{get_option('blkio-weight', self.addHost)}"
+                    f"{get_option('blkio-weight-device', self.blkioWeightDevice)}"
+                    f"{get_option('cap-add', self.capAdd)}"
+                    f"{get_option('cap-drop', self.capDrop)}"
+                    f"{get_option('cgroup-parent', self.cgroupParent)}"
+                    f"{get_option('cgroupns', self.cgroupns)}"
+                    f"{get_option('cidfile', self.cidfile)}"
+                    f"{get_option('cpu-period', self.cpuPeriod)}"
+                    f"{get_option('cpu-quota', self.cpuQuota)}"
+                    f"{get_option('cpu-rt-period', self.cpuRTPeriod)}"
+                    f"{get_option('cpu-rt-runtime', self.cpuRTRuntime)}"
+                    f"{get_option('cpu-shares', self.cpuShares)}"
+                    f"{get_option('cpus', self.cpus)}"
+                    f"{get_option('cpuset-cpus', self.cpusetCpus)}"
+                    f"{get_option('cpuset-mems', self.cpusetMems)}"
+                    f"{get_option('detach-keys', self.detachKeys)}"
+                    f"{get_option('device', self.device)}"
+                    f"{get_option('device-cgroup-rule', self.deviceCgroupRule)}"
+                    f"{get_option('device-read-bps', self.deviceReadBps)}"
+                    f"{get_option('device-read-iops', self.deviceReadIops)}"
+                    f"{get_option('device-write-bps', self.deviceWriteBps)}"
+                    f"{get_option('device-write-iops', self.deviceWriteIops)}"
+                    f"--disable-content-trust={'true' if self.disableContentTrust else 'false'} "
+                    f"{get_option('dns', self.dns)}"
+                    f"{get_option('dns-option', self.dnsOptions)}"
+                    f"{get_option('dns-search', self.dnsSearch)}"
+                    f"{get_option('domainname', self.domainname)}"
+                    f"{get_option('entrypoint', self.entrypoint)}"
+                    f"{get_option('env', self.env)}"
+                    f"{get_option('env-file', self.envFile)}"
+                    f"{get_option('expose', self.expose)}"
+                    f"{get_option('gpus', self.gpus)}"
+                    f"{get_option('group-add', self.groupAdd)}"
+                    f"{get_option('health-cmd', self.healthCmd)}"
+                    f"{get_option('health-interval', self.healthInterval)}"
+                    f"{get_option('health-retries', self.healthRetries)}"
+                    f"{get_option('health-start-period', self.healthStartPeriod)}"
+                    f"{get_option('health-timeout', self.healthTimeout)}"
+                    f"{get_option('hostname', self.hostname)}"
+                    f"{get_option('init', self.init)}"
+                    f"{get_option('ip', self.ip)}"
+                    f"{get_option('ip6', self.ip6)}"
+                    f"{get_option('ipc', self.ipc)}"
+                    f"{get_option('isolation', self.isolation)}"
+                    f"{get_option('kernel-memory', self.kernelMemory)}"
+                    f"{get_option('label', self.label)}"
+                    f"{get_option('label-file', self.labelFile)}"
+                    f"{get_option('link', self.link)}"
+                    f"{get_option('link-local-ip', self.linkLocalIP)}"
+                    f"{get_option('log-driver', self.logDriver)}"
+                    f"{get_option('log-opt', self.logOpts)}"
+                    f"{get_option('mac-address', self.macAddress)}"
+                    f"{get_option('memory', self.memory)}"
+                    f"{get_option('memory-reservation', self.memoryReservation)}"
+                    f"{get_option('memory-swap', self.memorySwap)}"
+                    f"{get_option('memory-swappiness', self.memorySwappiness)}"
+                    f"{get_option('mount', self.mount)}"
+                    f"{get_option('network', self.network)}"
+                    f"{get_option('network-alias', self.networkAlias)}"
+                    f"{get_option('no-healthcheck', self.noHealthcheck)}"
+                    f"{get_option('oom-kill-disable', self.oomKillDisable)}"
+                    f"{get_option('oom-score-adj', self.oomScoreAdj)}"
+                    f"{get_option('pid', self.pid)}"
+                    f"{get_option('pids-limit', self.pidsLimit)}"
+                    f"{get_option('privileged', self.privileged)}"
+                    f"{get_option('publish', self.publish)}"
+                    f"{get_option('publish-all', self.publishAll)}"
+                    f"{get_option('read-only', self.readOnly)}"
+                    f"{get_option('restart', self.restart)}"
+                    f"{get_option('rm', self.rm)}"
+                    f"{get_option('runtime', self.runtime)}"
+                    f"{get_option('security-opt', self.securityOpts)}"
+                    f"{get_option('shm-size', self.shmSize)}"
+                    f"--sig-proxy={'true' if self.sigProxy else 'false'} "
+                    f"{get_option('stop-signal', self.stopSignal)}"
+                    f"{get_option('stop-timeout', self.stopTimeout)}"
+                    f"{get_option('storage-opt', self.storageOpts)}"
+                    f"{get_option('sysctl', self.sysctl)}"
+                    f"{get_option('tmpfs', self.tmpfs)}"
+                    f"{get_option('ulimit', self.ulimit)}"
+                    f"{get_option('user', self.user)}"
+                    f"{get_option('userns', self.userns)}"
+                    f"{get_option('uts', self.uts)}"
+                    f"{get_option('volume', self.volume)}"
+                    f"{get_option('volume-driver', self.volumeDriver)}"
+                    f"{get_option('volumes-from', self.volumesFrom)}"
+                    f"{get_option('workdir', self.workdir)}"
+                    f"{self.image} "
+                    f"{' '.join(self.command) if self.command else ''}"
                 )
                 if logger.isEnabledFor(logging.DEBUG):
                     logger.debug(f"EXECUTING command {deploy_command}")
                 proc = await asyncio.create_subprocess_exec(
                     *shlex.split(deploy_command),
                     stdout=asyncio.subprocess.PIPE,
                     stderr=asyncio.subprocess.PIPE,
@@ -782,32 +771,30 @@
         self.tls = tls
         self.tlscacert = tlscacert
         self.tlscert = tlscert
         self.tlskey = tlskey
         self.tlsverify = tlsverify
 
     def _get_base_command(self) -> str:
-        return "".join(
-            [
-                "docker-compose ",
-                self.get_option("file", self.files),
-                self.get_option("project-name", self.projectName),
-                self.get_option("verbose", self.verbose),
-                self.get_option("log-level", self.logLevel),
-                self.get_option("no-ansi", self.noAnsi),
-                self.get_option("host", self.host),
-                self.get_option("tls", self.tls),
-                self.get_option("tlscacert", self.tlscacert),
-                self.get_option("tlscert", self.tlscert),
-                self.get_option("tlskey", self.tlskey),
-                self.get_option("tlsverify", self.tlsverify),
-                self.get_option("skip-hostname-check", self.skipHostnameCheck),
-                self.get_option("project-directory", self.projectDirectory),
-                self.get_option("compatibility", self.compatibility),
-            ]
+        return (
+            f"docker-compose "
+            f"{get_option('file', self.files)}"
+            f"{get_option('project-name', self.projectName)}"
+            f"{get_option('verbose', self.verbose)}"
+            f"{get_option('log-level', self.logLevel)}"
+            f"{get_option('no-ansi', self.noAnsi)}"
+            f"{get_option('host', self.host)}"
+            f"{get_option('tls', self.tls)}"
+            f"{get_option('tlscacert', self.tlscacert)}"
+            f"{get_option('tlscert', self.tlscert)}"
+            f"{get_option('tlskey', self.tlskey)}"
+            f"{get_option('tlsverify', self.tlsverify)}"
+            f"{get_option('skip-hostname-check', self.skipHostnameCheck)}"
+            f"{get_option('project-directory', self.projectDirectory)}"
+            f"{get_option('compatibility', self.compatibility)}"
         )
 
     async def deploy(self, external: bool) -> None:
         if not external:
             _check_docker_installed("Docker Compose")
             version = await _get_docker_compose_version()
             if version.startswith("v"):
@@ -819,25 +806,22 @@
                     f"Docker Compose version 2.x or later is required."
                 )
             if logger.isEnabledFor(logging.DEBUG):
                 logger.debug(
                     f"Using Docker {await _get_docker_version()} "
                     f"and Docker Compose {version}."
                 )
-            deploy_command = self._get_base_command() + "".join(
-                [
-                    "up ",
-                    "--detach ",
-                    self.get_option("no-deps ", self.noDeps),
-                    self.get_option("force-recreate", self.forceRecreate),
-                    self.get_option("always-recreate-deps", self.alwaysRecreateDeps),
-                    self.get_option("no-recreate", self.noRecreate),
-                    self.get_option("no-build", self.noBuild),
-                    self.get_option("no-start", self.noStart),
-                ]
+            deploy_command = (
+                f"{self._get_base_command()} up --detach "
+                f"{get_option('no-deps ', self.noDeps)}"
+                f"{get_option('force-recreate', self.forceRecreate)}"
+                f"{get_option('always-recreate-deps', self.alwaysRecreateDeps)}"
+                f"{get_option('no-recreate', self.noRecreate)}"
+                f"{get_option('no-build', self.noBuild)}"
+                f"{get_option('no-start', self.noStart)}"
             )
             if logger.isEnabledFor(logging.DEBUG):
                 logger.debug(f"EXECUTING command {deploy_command}")
             proc = await asyncio.create_subprocess_exec(
                 *shlex.split(deploy_command),
                 stderr=asyncio.subprocess.STDOUT,
                 stdout=asyncio.subprocess.PIPE,
@@ -887,15 +871,15 @@
             __name__, os.path.join("schemas", "docker-compose.json")
         )
 
     async def undeploy(self, external: bool) -> None:
         if not external:
             undeploy_command = (
                 self._get_base_command()
-                + f"down {self.get_option('volumes', self.removeVolumes)}"
+                + f"down {get_option('volumes', self.removeVolumes)}"
             )
             if logger.isEnabledFor(logging.DEBUG):
                 logger.debug(f"EXECUTING command {undeploy_command}")
             proc = await asyncio.create_subprocess_exec(
                 *shlex.split(undeploy_command),
                 stderr=asyncio.subprocess.STDOUT,
                 stdout=asyncio.subprocess.PIPE,
@@ -1103,69 +1087,69 @@
             if logger.isEnabledFor(logging.DEBUG):
                 logger.debug(f"Using {await _get_singularity_version()}.")
             _prepare_volumes(self.bind, self.mount)
             for _ in range(0, self.replicas):
                 instance_name = utils.random_name()
                 deploy_command = (
                     f"singularity instance start "
-                    f"{self.get_option('add-caps', self.addCaps)}"
-                    f"{self.get_option('allow-setuid', self.allowSetuid)}"
-                    f"{self.get_option('apply-cgroups', self.applyCgroups)}"
-                    f"{self.get_option('bind', self.bind)}"
-                    f"{self.get_option('blkio-weight', self.blkioWeight)}"
-                    f"{self.get_option('blkio-weight-device', self.blkioWeightDevice)}"
-                    f"{self.get_option('boot', self.boot)}"
-                    f"{self.get_option('cleanenv', self.cleanenv)}"
-                    f"{self.get_option('compat', self.compat)}"
-                    f"{self.get_option('contain', self.contain)}"
-                    f"{self.get_option('containall', self.containall)}"
-                    f"{self.get_option('cpu-shares', self.cpuShares)}"
-                    f"{self.get_option('cpus', self.cpus)}"
-                    f"{self.get_option('cpuset-cpus', self.cpusetCpus)}"
-                    f"{self.get_option('cpuset-mems', self.cpusetMems)}"
-                    f"{self.get_option('disable-cache', self.disableCache)}"
-                    f"{self.get_option('docker-host', self.dockerHost)}"
-                    f"{self.get_option('dns', self.dns)}"
-                    f"{self.get_option('drop-caps', self.dropCaps)}"
-                    f"{self.get_option('env-file', self.envFile)}"
-                    f"{self.get_option('fakeroot', self.fakeroot)}"
-                    f"{self.get_option('fusemount', self.fusemount)}"
-                    f"{self.get_option('home', self.home)}"
-                    f"{self.get_option('hostname', self.hostname)}"
-                    f"{self.get_option('ipc', self.ipc)}"
-                    f"{self.get_option('keep-privs', self.keepPrivs)}"
-                    f"{self.get_option('memory', self.memory)}"
-                    f"{self.get_option('memory-reservation', self.memoryReservation)}"
-                    f"{self.get_option('memory-swap', self.memorySwap)}"
-                    f"{self.get_option('mount', self.mount)}"
-                    f"{self.get_option('net', self.net)}"
-                    f"{self.get_option('network', self.network)}"
-                    f"{self.get_option('network-args', self.networkArgs)}"
-                    f"{self.get_option('no-eval', self.noEval)}"
-                    f"{self.get_option('no-home', self.noHome)}"
-                    f"{self.get_option('no-https', self.noHttps)}"
-                    f"{self.get_option('no-init', self.noInit)}"
-                    f"{self.get_option('no-mount', self.noMount)}"
-                    f"{self.get_option('no-privs', self.noPrivs)}"
-                    f"{self.get_option('no-umask', self.noUmask)}"
-                    f"{self.get_option('nv', self.nv)}"
-                    f"{self.get_option('nvccli', self.nvccli)}"
-                    f"{self.get_option('oom-kill-disable', self.oomKillDisable)}"
-                    f"{self.get_option('overlay', self.overlay)}"
-                    f"{self.get_option('pem-path', self.pemPath)}"
-                    f"{self.get_option('pid-file', self.pidFile)}"
-                    f"{self.get_option('pids-limit', self.pidsLimit)}"
-                    f"{self.get_option('rocm', self.rocm)}"
-                    f"{self.get_option('scratch', self.scratch)}"
-                    f"{self.get_option('security', self.security)}"
-                    f"{self.get_option('userns', self.userns)}"
-                    f"{self.get_option('uts', self.uts)}"
-                    f"{self.get_option('workdir', self.workdir)}"
-                    f"{self.get_option('writable', self.writable)}"
-                    f"{self.get_option('writable-tmpfs', self.writableTmpfs)}"
+                    f"{get_option('add-caps', self.addCaps)}"
+                    f"{get_option('allow-setuid', self.allowSetuid)}"
+                    f"{get_option('apply-cgroups', self.applyCgroups)}"
+                    f"{get_option('bind', self.bind)}"
+                    f"{get_option('blkio-weight', self.blkioWeight)}"
+                    f"{get_option('blkio-weight-device', self.blkioWeightDevice)}"
+                    f"{get_option('boot', self.boot)}"
+                    f"{get_option('cleanenv', self.cleanenv)}"
+                    f"{get_option('compat', self.compat)}"
+                    f"{get_option('contain', self.contain)}"
+                    f"{get_option('containall', self.containall)}"
+                    f"{get_option('cpu-shares', self.cpuShares)}"
+                    f"{get_option('cpus', self.cpus)}"
+                    f"{get_option('cpuset-cpus', self.cpusetCpus)}"
+                    f"{get_option('cpuset-mems', self.cpusetMems)}"
+                    f"{get_option('disable-cache', self.disableCache)}"
+                    f"{get_option('docker-host', self.dockerHost)}"
+                    f"{get_option('dns', self.dns)}"
+                    f"{get_option('drop-caps', self.dropCaps)}"
+                    f"{get_option('env-file', self.envFile)}"
+                    f"{get_option('fakeroot', self.fakeroot)}"
+                    f"{get_option('fusemount', self.fusemount)}"
+                    f"{get_option('home', self.home)}"
+                    f"{get_option('hostname', self.hostname)}"
+                    f"{get_option('ipc', self.ipc)}"
+                    f"{get_option('keep-privs', self.keepPrivs)}"
+                    f"{get_option('memory', self.memory)}"
+                    f"{get_option('memory-reservation', self.memoryReservation)}"
+                    f"{get_option('memory-swap', self.memorySwap)}"
+                    f"{get_option('mount', self.mount)}"
+                    f"{get_option('net', self.net)}"
+                    f"{get_option('network', self.network)}"
+                    f"{get_option('network-args', self.networkArgs)}"
+                    f"{get_option('no-eval', self.noEval)}"
+                    f"{get_option('no-home', self.noHome)}"
+                    f"{get_option('no-https', self.noHttps)}"
+                    f"{get_option('no-init', self.noInit)}"
+                    f"{get_option('no-mount', self.noMount)}"
+                    f"{get_option('no-privs', self.noPrivs)}"
+                    f"{get_option('no-umask', self.noUmask)}"
+                    f"{get_option('nv', self.nv)}"
+                    f"{get_option('nvccli', self.nvccli)}"
+                    f"{get_option('oom-kill-disable', self.oomKillDisable)}"
+                    f"{get_option('overlay', self.overlay)}"
+                    f"{get_option('pem-path', self.pemPath)}"
+                    f"{get_option('pid-file', self.pidFile)}"
+                    f"{get_option('pids-limit', self.pidsLimit)}"
+                    f"{get_option('rocm', self.rocm)}"
+                    f"{get_option('scratch', self.scratch)}"
+                    f"{get_option('security', self.security)}"
+                    f"{get_option('userns', self.userns)}"
+                    f"{get_option('uts', self.uts)}"
+                    f"{get_option('workdir', self.workdir)}"
+                    f"{get_option('writable', self.writable)}"
+                    f"{get_option('writable-tmpfs', self.writableTmpfs)}"
                     f"{self.image} "
                     f"{instance_name} "
                     f"{' '.join(self.command) if self.command else ''}"
                 )
                 if logger.isEnabledFor(logging.DEBUG):
                     logger.debug(f"EXECUTING command {deploy_command}")
                 proc = await asyncio.create_subprocess_exec(
```

### Comparing `streamflow-0.2.0.dev5/streamflow/deployment/connector/kubernetes.py` & `streamflow-0.2.0.dev6/streamflow/deployment/connector/kubernetes.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 from streamflow.core.data import StreamWrapperContext
 from streamflow.core.deployment import Connector, Location
 from streamflow.core.exception import (
     WorkflowDefinitionException,
     WorkflowExecutionException,
 )
 from streamflow.core.scheduling import AvailableLocation
+from streamflow.core.utils import get_option
 from streamflow.deployment import aiotarstream
 from streamflow.deployment.aiotarstream import BaseStreamWrapper
 from streamflow.deployment.connector.base import BaseConnector, extract_tar_stream
 from streamflow.log_handler import logger
 
 SERVICE_NAMESPACE_FILENAME = "/var/run/secrets/kubernetes.io/serviceaccount/namespace"
 
@@ -409,26 +410,22 @@
                 effective_locations.append(location)
         return effective_locations
 
     def _get_run_command(
         self, command: str, location: Location, interactive: bool = False
     ):
         pod, container = location.name.split(":")
-        return "".join(
-            [
-                "kubectl ",
-                self.get_option("namespace", self.namespace),
-                self.get_option("kubeconfig", self.kubeconfig),
-                "exec ",
-                f"{pod} ",
-                self.get_option("i", interactive),
-                self.get_option("container", container),
-                "-- ",
-                command,
-            ]
+        return (
+            f"kubectl "
+            f"{get_option('namespace', self.namespace)}"
+            f"{get_option('kubeconfig', self.kubeconfig)}"
+            f"exec {pod} "
+            f"{get_option('i', interactive)}"
+            f"{get_option('container', container)}"
+            f"-- {command}"
         )
 
     @abstractmethod
     async def _get_running_pods(self) -> MutableSequence[Any]:
         ...
 
     def _get_stream_reader(self, location: Location, src: str) -> StreamWrapperContext:
@@ -974,25 +971,23 @@
         self.username: str | None = username
         self.yamlValues: MutableSequence[str] | None = yamlValues
         self.verify: bool = verify
         self.chartVersion: str | None = chartVersion
         self.wait: bool = wait
 
     def _get_base_command(self) -> str:
-        return "".join(
-            [
-                "helm ",
-                self.get_option("debug", self.debug),
-                self.get_option("kube-context", self.kubeContext),
-                self.get_option("kubeconfig", self.kubeconfig),
-                self.get_option("namespace", self.namespace),
-                self.get_option("registry-config", self.registryConfig),
-                self.get_option("repository-cache", self.repositoryCache),
-                self.get_option("repository-config", self.repositoryConfig),
-            ]
+        return (
+            f"helm "
+            f"{get_option('debug', self.debug)}"
+            f"{get_option('kube-context', self.kubeContext)}"
+            f"{get_option('kubeconfig', self.kubeconfig)}"
+            f"{get_option('namespace', self.namespace)}"
+            f"{get_option('registry-config', self.registryConfig)}"
+            f"{get_option('repository-cache', self.repositoryCache)}"
+            f"{get_option('repository-config', self.repositoryConfig)}"
         )
 
     async def _get_running_pods(self) -> MutableSequence[Any]:
         return await self.client.list_namespaced_pod(
             namespace=self.namespace or "default",
             label_selector=f"app.kubernetes.io/instance={self.releaseName}",
             field_selector="status.phase=Running",
@@ -1009,42 +1004,40 @@
             if not version.startswith("v3"):
                 raise WorkflowExecutionException(
                     f"Helm {version} is not compatible with Helm3Connector"
                 )
             if logger.isEnabledFor(logging.DEBUG):
                 logger.debug(f"Using Helm {version}.")
             # Deploy Helm charts
-            deploy_command = self._get_base_command() + "".join(
-                [
-                    "install ",
-                    self.get_option("atomic", self.atomic),
-                    self.get_option("ca-file", self.caFile),
-                    self.get_option("cert-file", self.certFile),
-                    self.get_option("dep-up", self.depUp),
-                    self.get_option("devel", self.devel),
-                    self.get_option("key-file", self.keyFile),
-                    self.get_option("keyring", self.keyring),
-                    self.get_option("name-template", self.nameTemplate),
-                    self.get_option("no-hooks", self.noHooks),
-                    self.get_option("password", self.password),
-                    self.get_option("render-subchart-notes", self.renderSubchartNotes),
-                    self.get_option("repo", self.repo),
-                    self.get_option("set", self.commandLineValues),
-                    self.get_option("set-file", self.fileValues),
-                    self.get_option("set-string", self.stringValues),
-                    self.get_option("skip-crds", self.skipCrds),
-                    self.get_option("timeout", self.timeout),
-                    self.get_option("username", self.username),
-                    self.get_option("values", self.yamlValues),
-                    self.get_option("verify", self.verify),
-                    self.get_option("version", self.chartVersion),
-                    self.get_option("wait", self.wait),
-                    f"{self.releaseName} ",
-                    self.chart,
-                ]
+            deploy_command = (
+                f"{self._get_base_command()} install "
+                f"{get_option('atomic', self.atomic)}"
+                f"{get_option('ca-file', self.caFile)}"
+                f"{get_option('cert-file', self.certFile)}"
+                f"{get_option('dep-up', self.depUp)}"
+                f"{get_option('devel', self.devel)}"
+                f"{get_option('key-file', self.keyFile)}"
+                f"{get_option('keyring', self.keyring)}"
+                f"{get_option('name-template', self.nameTemplate)}"
+                f"{get_option('no-hooks', self.noHooks)}"
+                f"{get_option('password', self.password)}"
+                f"{get_option('render-subchart-notes', self.renderSubchartNotes)}"
+                f"{get_option('repo', self.repo)}"
+                f"{get_option('set', self.commandLineValues)}"
+                f"{get_option('set-file', self.fileValues)}"
+                f"{get_option('set-string', self.stringValues)}"
+                f"{get_option('skip-crds', self.skipCrds)}"
+                f"{get_option('timeout', self.timeout)}"
+                f"{get_option('username', self.username)}"
+                f"{get_option('values', self.yamlValues)}"
+                f"{get_option('verify', self.verify)}"
+                f"{get_option('version', self.chartVersion)}"
+                f"{get_option('wait', self.wait)}"
+                f"{self.releaseName} "
+                f"{self.chart}"
             )
             if logger.isEnabledFor(logging.DEBUG):
                 logger.debug(f"EXECUTING {deploy_command}")
             proc = await asyncio.create_subprocess_exec(
                 *shlex.split(deploy_command),
                 stderr=asyncio.subprocess.STDOUT,
                 stdout=asyncio.subprocess.PIPE,
@@ -1060,22 +1053,20 @@
         return pkg_resources.resource_filename(
             __name__, os.path.join("schemas", "helm3.json")
         )
 
     async def undeploy(self, external: bool) -> None:
         if not external:
             # Undeploy
-            undeploy_command = self._get_base_command() + "".join(
-                [
-                    "uninstall ",
-                    self.get_option("keep-history", self.keepHistory),
-                    self.get_option("no-hooks", self.noHooks),
-                    self.get_option("timeout", self.timeout),
-                    self.releaseName,
-                ]
+            undeploy_command = (
+                f"{self._get_base_command()}  uninstall "
+                f"{get_option('keep-history', self.keepHistory)}"
+                f"{get_option('no-hooks', self.noHooks)}"
+                f"{get_option('timeout', self.timeout)}"
+                f"{self.releaseName}"
             )
             if logger.isEnabledFor(logging.DEBUG):
                 logger.debug(f"EXECUTING {undeploy_command}")
             proc = await asyncio.create_subprocess_exec(
                 *shlex.split(undeploy_command),
                 stderr=asyncio.subprocess.STDOUT,
                 stdout=asyncio.subprocess.PIPE,
```

### Comparing `streamflow-0.2.0.dev5/streamflow/deployment/connector/local.py` & `streamflow-0.2.0.dev6/streamflow/deployment/connector/local.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev5/streamflow/deployment/connector/occam.py` & `streamflow-0.2.0.dev6/streamflow/deployment/connector/occam.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 import asyncssh
 import pkg_resources
 from ruamel.yaml import YAML
 
 from streamflow.core import utils
 from streamflow.core.deployment import Location
 from streamflow.core.scheduling import AvailableLocation
+from streamflow.core.utils import get_option
 from streamflow.deployment.connector.ssh import SSHConnector
 from streamflow.log_handler import logger
 
 
 class OccamConnector(SSHConnector):
     def __init__(
         self,
@@ -270,26 +271,27 @@
                 await asyncio.gather(*scp_tasks)
             delete_command = ["rm", "-rf", temp_dir]
             await self.run(location, delete_command)
 
     async def _deploy_node(
         self, name: str, service: MutableMapping[str, Any], node: str
     ):
-        deploy_command = "".join(
-            [
-                (f"cd {service.get('workdir')} && " if "workdir" in service else ""),
-                "occam-run ",
-                self.get_option("x", service.get("x11")),
-                self.get_option("n", node),
-                self.get_option("i", service.get("stdin")),
-                self.get_option("c", service.get("jobidFile")),
-                self.get_option("s", service.get("shmSize")),
-                self.get_option("v", service.get("volumes")),
-                f"{service['image']} " " ".join(service.get("command", "")),
-            ]
+        deploy_command = (
+            f"cd {service.get('workdir')} && "
+            if "workdir" in service
+            else ""
+            f"occam-run "
+            f"{get_option('x', service.get('x11'))}"
+            f"{get_option('n', node)}"
+            f"{get_option('i', service.get('stdin'))}"
+            f"{get_option('c', service.get('jobidFile'))}"
+            f"{get_option('s', service.get('shmSize'))}"
+            f"{get_option('v', service.get('volumes'))}"
+            f"{service['image']} "
+            f"{' '.join(service.get('command', ''))}"
         )
         if logger.isEnabledFor(logging.DEBUG):
             logger.debug(f"EXECUTING {deploy_command}")
         async with self._get_ssh_client(name) as ssh_client:
             result = await ssh_client.run(deploy_command)
         output = result.stdout
         search_result = re.findall(f"({node}-[0-9]+).*", output, re.MULTILINE)
```

### Comparing `streamflow-0.2.0.dev5/streamflow/deployment/connector/queue_manager.py` & `streamflow-0.2.0.dev6/streamflow/deployment/connector/ssh.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,80 +1,281 @@
 from __future__ import annotations
 
 import asyncio
-import base64
-import json
+import contextlib
 import logging
 import os
-import shlex
-from abc import ABC, abstractmethod
-from functools import partial
+import posixpath
+import tarfile
+from pathlib import PurePosixPath
 from typing import Any, MutableMapping, MutableSequence
 
-import cachetools
+import asyncssh
 import pkg_resources
+from cachetools import Cache, LRUCache
 
 from streamflow.core import utils
 from streamflow.core.asyncache import cachedmethod
+from streamflow.core.data import StreamWrapperContext
 from streamflow.core.deployment import Connector, Location
-from streamflow.core.exception import (
-    WorkflowDefinitionException,
-    WorkflowExecutionException,
-)
-from streamflow.core.scheduling import AvailableLocation
-from streamflow.deployment.connector.ssh import SSHConnector
+from streamflow.core.exception import WorkflowExecutionException
+from streamflow.core.scheduling import AvailableLocation, Hardware
+from streamflow.deployment import aiotarstream
+from streamflow.deployment.connector.base import BaseConnector, extract_tar_stream
+from streamflow.deployment.stream import StreamReaderWrapper, StreamWriterWrapper
 from streamflow.deployment.template import CommandTemplateMap
-from streamflow.deployment.wrapper import ConnectorWrapper
 from streamflow.log_handler import logger
 
 
-class QueueManagerConnector(ConnectorWrapper, ABC):
+async def _get_disk_usage(
+    ssh_client: asyncssh.SSHClientConnection, directory: str
+) -> float:
+    if directory:
+        result = await ssh_client.run(
+            f"df {directory} | tail -n 1 | awk '{{print $2}}'",
+            stderr=asyncio.subprocess.STDOUT,
+        )
+        if result.returncode == 0:
+            return float(result.stdout.strip()) / 2**10
+        else:
+            raise WorkflowExecutionException(result.returncode)
+    else:
+        return float("inf")
+
+
+def _parse_hostname(hostname):
+    if ":" in hostname:
+        hostname, port = hostname.split(":")
+        port = int(port)
+    else:
+        port = 22
+    return hostname, port
+
+
+class SSHContext:
+    def __init__(
+        self,
+        streamflow_config_dir: str,
+        config: SSHConfig,
+        max_concurrent_sessions: int,
+    ):
+        self._streamflow_config_dir: str = streamflow_config_dir
+        self._config: SSHConfig = config
+        self._max_concurrent_sessions: int = max_concurrent_sessions
+        self._ssh_connection: asyncssh.SSHClientConnection | None = None
+        self._sessions: int = 0
+
+    async def __aenter__(self):
+        if self._ssh_connection is None:
+            self._ssh_connection = await self._get_connection(self._config)
+        self._sessions += 1
+        return self._ssh_connection
+
+    async def __aexit__(self, exc_type, exc_val, exc_tb):
+        self._sessions -= 1
+
+    async def _get_connection(
+        self, config: SSHConfig
+    ) -> asyncssh.SSHClientConnection | None:
+        if config is None:
+            return None
+        (hostname, port) = _parse_hostname(config.hostname)
+        passphrase = (
+            self._get_param_from_file(config.ssh_key_passphrase_file)
+            if config.ssh_key_passphrase_file
+            else None
+        )
+        password = (
+            self._get_param_from_file(config.password_file)
+            if config.password_file
+            else None
+        )
+        return await asyncssh.connect(
+            client_keys=config.client_keys,
+            compression_algs=None,
+            encryption_algs=[
+                "aes128-gcm@openssh.com",
+                "aes256-ctr",
+                "aes192-ctr",
+                "aes128-ctr",
+            ],
+            known_hosts=() if config.check_host_key else None,
+            host=hostname,
+            passphrase=passphrase,
+            password=password,
+            port=port,
+            tunnel=await self._get_connection(config.tunnel),
+            username=config.username,
+        )
+
+    def _get_param_from_file(self, file_path: str):
+        if not os.path.isabs(file_path):
+            file_path = os.path.join(self._streamflow_config_dir, file_path)
+        with open(file_path) as f:
+            return f.read().strip()
+
+    async def close(self):
+        if self._ssh_connection is not None:
+            self._ssh_connection.close()
+
+    def full(self) -> bool:
+        return self._sessions == self._max_concurrent_sessions
+
+
+class SSHContextManager:
+    def __init__(
+        self, condition: asyncio.Condition, contexts: MutableSequence[SSHContext]
+    ):
+        self._condition: asyncio.Condition = condition
+        self._contexts: MutableSequence[SSHContext] = contexts
+        self._selected_context: SSHContext | None = None
+
+    async def __aenter__(self):
+        async with self._condition:
+            while True:
+                for context in self._contexts:
+                    if not context.full():
+                        ssh_connection = await context.__aenter__()
+                        self._selected_context = context
+                        return ssh_connection
+                await self._condition.wait()
+
+    async def __aexit__(self, exc_type, exc_val, exc_tb):
+        async with self._condition:
+            if self._selected_context:
+                await self._selected_context.__aexit__(exc_type, exc_val, exc_tb)
+                self._condition.notify_all()
+
+
+class SSHContextFactory:
+    def __init__(
+        self,
+        streamflow_config_dir: str,
+        config: SSHConfig,
+        max_concurrent_sessions: int,
+        max_connections: int,
+    ):
+        self._condition: asyncio.Condition = asyncio.Condition()
+        self._contexts: MutableSequence[SSHContext] = [
+            SSHContext(
+                streamflow_config_dir=streamflow_config_dir,
+                config=config,
+                max_concurrent_sessions=max_concurrent_sessions,
+            )
+            for _ in range(max_connections)
+        ]
+
+    async def close(self):
+        await asyncio.gather(*(asyncio.create_task(c.close()) for c in self._contexts))
+
+    def get(self):
+        return SSHContextManager(condition=self._condition, contexts=self._contexts)
+
+
+class SSHStreamWrapperContext(StreamWrapperContext):
+    def __init__(self, src: str, ssh_context: SSHContextManager):
+        super().__init__()
+        self.src: str = src
+        self.ssh_context: SSHContextManager = ssh_context
+        self.ssh_process: asyncssh.SSHClientProcess | None = None
+        self.stream: StreamReaderWrapper | None = None
+
+    async def __aenter__(self):
+        ssh_client = await self.ssh_context.__aenter__()
+        dirname, basename = posixpath.split(self.src)
+        self.ssh_process = await (
+            await ssh_client.create_process(
+                f"tar chf - -C {dirname} {basename}",
+                stdin=asyncio.subprocess.DEVNULL,
+                encoding=None,
+            )
+        ).__aenter__()
+        self.stream = StreamReaderWrapper(self.ssh_process.stdout)
+        return self.stream
+
+    async def __aexit__(self, exc_type, exc_val, exc_tb):
+        if self.stream:
+            await self.stream.close()
+        if self.ssh_process:
+            await self.ssh_process.__aexit__(exc_type, exc_val, exc_tb)
+        await self.ssh_context.__aexit__(exc_type, exc_val, exc_tb)
+
+
+class SSHConfig:
+    def __init__(
+        self,
+        check_host_key: bool,
+        client_keys: MutableSequence[str],
+        hostname: str,
+        password_file: str | None,
+        ssh_key_passphrase_file: str | None,
+        tunnel: SSHConfig | None,
+        username: str,
+    ):
+        self.check_host_key: bool = check_host_key
+        self.client_keys: MutableSequence[str] = client_keys
+        self.hostname: str = hostname
+        self.password_file: str | None = password_file
+        self.ssh_key_passphrase_file: str | None = ssh_key_passphrase_file
+        self.tunnel: SSHConfig | None = tunnel
+        self.username: str = username
+
+
+class SSHConnector(BaseConnector):
+    @staticmethod
+    def _get_command(
+        location: Location,
+        command: MutableSequence[str],
+        environment: MutableMapping[str, str] = None,
+        workdir: str | None = None,
+        stdin: int | str | None = None,
+        stdout: int | str = asyncio.subprocess.STDOUT,
+        stderr: int | str = asyncio.subprocess.STDOUT,
+        job_name: str | None = None,
+    ):
+        command = utils.create_command(
+            command=command,
+            environment=environment,
+            workdir=workdir,
+            stdin=stdin,
+            stdout=stdout,
+            stderr=stderr,
+        )
+        if logger.isEnabledFor(logging.DEBUG):
+            logger.debug(
+                f"EXECUTING command {command} on {location}" f" for job {job_name}"
+                if job_name
+                else ""
+            )
+        return utils.encode_command(command)
+
     def __init__(
         self,
         deployment_name: str,
         config_dir: str,
-        connector: Connector,
-        hostname: str | None = None,
-        username: str | None = None,
+        nodes: MutableSequence[Any],
+        username: str,
         checkHostKey: bool = True,
         dataTransferConnection: str | MutableMapping[str, Any] | None = None,
         file: str | None = None,
-        maxConcurrentJobs: int | None = 1,
-        maxConcurrentSessions: int | None = 10,
-        maxConnections: int | None = 1,
+        maxConcurrentSessions: int = 10,
+        maxConnections: int = 1,
         passwordFile: str | None = None,
-        pollingInterval: int = 5,
         services: MutableMapping[str, str] | None = None,
+        sharedPaths: MutableSequence[str] | None = None,
         sshKey: str | None = None,
         sshKeyPassphraseFile: str | None = None,
+        tunnel: MutableMapping[str, Any] | None = None,
         transferBufferSize: int = 2**16,
     ) -> None:
-        self._inner_ssh_connector: bool = False
-        if hostname is not None:
-            if logger.isEnabledFor(logging.WARN):
-                logger.warn(
-                    "Inline SSH options are deprecated and will be removed in StreamFlow 0.3.0. "
-                    "Define a standalone SSH connector and link to it using the `connector` property."
-                )
-            self._inner_ssh_connector = True
-            connector: Connector = SSHConnector(
-                deployment_name=f"{deployment_name}-ssh",
-                config_dir=config_dir,
-                checkHostKey=checkHostKey,
-                dataTransferConnection=dataTransferConnection,
-                maxConcurrentSessions=maxConcurrentSessions,
-                maxConnections=maxConnections,
-                nodes=[hostname],
-                passwordFile=passwordFile,
-                sshKey=sshKey,
-                sshKeyPassphraseFile=sshKeyPassphraseFile,
-                transferBufferSize=transferBufferSize,
-                username=username,
-            )
-        super().__init__(deployment_name, config_dir, connector)
+        super().__init__(
+            deployment_name=deployment_name,
+            config_dir=config_dir,
+            transferBufferSize=transferBufferSize,
+        )
         services_map: MutableMapping[str, Any] = {}
         if services:
             for name, service in services.items():
                 with open(os.path.join(self.config_dir, service)) as f:
                     services_map[name] = f.read()
         if file is not None:
             if logger.isEnabledFor(logging.WARN):
@@ -87,87 +288,321 @@
                     default=f.read(), template_map=services_map
                 )
         else:
             self.template_map: CommandTemplateMap = CommandTemplateMap(
                 default="#!/bin/sh\n\n{{streamflow_command}}",
                 template_map=services_map,
             )
-        self.maxConcurrentJobs: int = maxConcurrentJobs
-        self.pollingInterval: int = pollingInterval
-        self.scheduledJobs: MutableSequence[str] = []
-        self.jobsCache: cachetools.Cache = cachetools.TTLCache(
-            maxsize=1, ttl=self.pollingInterval
-        )
-        self.jobsCacheLock: asyncio.Lock = asyncio.Lock()
-
-    async def _get_location(self):
-        locations = await self.connector.get_available_locations()
-        if len(locations) != 1:
-            raise WorkflowDefinitionException(
-                f"QueueManager connectors support only nested connectors with a single location. "
-                f"{self.connector.deployment_name} returned {len(locations)} available locations."
-            )
-        return list(locations.values())[0]
-
-    @abstractmethod
-    async def _get_output(self, job_id: str, location: Location) -> str:
-        ...
-
-    @abstractmethod
-    async def _get_returncode(self, job_id: str, location: Location) -> int:
-        ...
-
-    @abstractmethod
-    async def _get_running_jobs(self, location: Location) -> bool:
-        ...
-
-    @abstractmethod
-    async def _remove_jobs(self, location: Location) -> None:
-        ...
+        self.checkHostKey: bool = checkHostKey
+        self.passwordFile: str | None = passwordFile
+        self.maxConcurrentSessions: int = maxConcurrentSessions
+        self.maxConnections: int = maxConnections
+        self.sharedPaths: MutableSequence[str] = sharedPaths or []
+        self.sshKey: str | None = sshKey
+        self.sshKeyPassphraseFile: str | None = sshKeyPassphraseFile
+        self.ssh_context_factories: MutableMapping[str, SSHContextFactory] = {}
+        self.data_transfer_context_factories: MutableMapping[
+            str, SSHContextFactory
+        ] = {}
+        self.username: str = username
+        self.tunnel: SSHConfig | None = self._get_config(tunnel)
+        self.dataTransferConfig: SSHConfig | None = self._get_config(
+            dataTransferConnection
+        )
+        self.nodes: MutableMapping[str, SSHConfig] = {
+            n.hostname: n for n in [self._get_config(n) for n in nodes]
+        }
+        self.hardwareCache: Cache = LRUCache(maxsize=len(self.nodes))
+
+    async def _copy_local_to_remote_single(
+        self, src: str, dst: str, location: Location, read_only: bool = False
+    ):
+        async with self._get_data_transfer_client(location.name) as ssh_client:
+            async with ssh_client.create_process(
+                "tar xf - -C /",
+                stderr=asyncio.subprocess.DEVNULL,
+                stdout=asyncio.subprocess.DEVNULL,
+                encoding=None,
+            ) as proc:
+                try:
+                    async with aiotarstream.open(
+                        stream=StreamWriterWrapper(proc.stdin),
+                        format=tarfile.GNU_FORMAT,
+                        mode="w",
+                        dereference=True,
+                        copybufsize=self.transferBufferSize,
+                    ) as tar:
+                        await tar.add(src, arcname=dst)
+                except tarfile.TarError as e:
+                    raise WorkflowExecutionException(
+                        f"Error copying {src} to {dst} on location {location}: {e}"
+                    ) from e
 
-    @abstractmethod
-    async def _run_batch_command(
+    async def _copy_remote_to_local(
+        self, src: str, dst: str, location: Location, read_only: bool = False
+    ) -> None:
+        dirname, basename = posixpath.split(src)
+        async with self._get_data_transfer_client(location.name) as ssh_client:
+            async with ssh_client.create_process(
+                f"tar chf - -C {dirname} {basename}",
+                stdin=asyncio.subprocess.DEVNULL,
+                encoding=None,
+            ) as proc:
+                try:
+                    async with aiotarstream.open(
+                        stream=StreamReaderWrapper(proc.stdout),
+                        mode="r",
+                        copybufsize=self.transferBufferSize,
+                    ) as tar:
+                        await extract_tar_stream(tar, src, dst, self.transferBufferSize)
+                except tarfile.TarError as e:
+                    raise WorkflowExecutionException(
+                        f"Error copying {src} from location {location} to {dst}: {e}"
+                    ) from e
+
+    async def _copy_remote_to_remote(
         self,
-        command: str,
-        job_name: str,
-        location: Location,
-        workdir: str | None = None,
-        stdin: int | str | None = None,
-        stdout: int | str = asyncio.subprocess.STDOUT,
-        stderr: int | str = asyncio.subprocess.STDOUT,
-        timeout: int | None = None,
-    ) -> str:
-        ...
+        src: str,
+        dst: str,
+        locations: MutableSequence[Location],
+        source_location: Location,
+        source_connector: Connector | None = None,
+        read_only: bool = False,
+    ) -> None:
+        source_connector = source_connector or self
+        if source_connector == self and source_location.name in [
+            loc.name for loc in locations
+        ]:
+            if src != dst:
+                command = ["/bin/cp", "-rf", src, dst]
+                await self.run(source_location, command)
+                locations.remove(source_location)
+        write_command = " ".join(
+            await utils.get_remote_to_remote_write_command(
+                src_connector=source_connector,
+                src_location=source_location,
+                src=src,
+                dst_connector=self,
+                dst_locations=locations,
+                dst=dst,
+            )
+        )
+        if locations:
+            async with source_connector._get_stream_reader(
+                source_location, src
+            ) as reader:
+                async with contextlib.AsyncExitStack() as exit_stack:
+                    # Open a target StreamWriter for each location
+                    writer_clients = await asyncio.gather(
+                        *(
+                            asyncio.create_task(
+                                exit_stack.enter_async_context(
+                                    self._get_data_transfer_client(location.name)
+                                )
+                            )
+                            for location in locations
+                        )
+                    )
+                    async with contextlib.AsyncExitStack() as writers_stack:
+                        writers = await asyncio.gather(
+                            *(
+                                asyncio.create_task(
+                                    writers_stack.enter_async_context(
+                                        client.create_process(
+                                            write_command,
+                                            stderr=asyncio.subprocess.DEVNULL,
+                                            stdout=asyncio.subprocess.DEVNULL,
+                                            encoding=None,
+                                        )
+                                    )
+                                )
+                                for client in writer_clients
+                            )
+                        )
+                        # Multiplex the reader output to all the writers
+                        while content := await reader.read(
+                            source_connector.transferBufferSize
+                        ):
+                            for writer in writers:
+                                writer.stdin.write(content)
+                            await asyncio.gather(
+                                *(
+                                    asyncio.create_task(writer.stdin.drain())
+                                    for writer in writers
+                                )
+                            )
+
+    def _get_config(self, node: str | MutableMapping[str, Any]):
+        if node is None:
+            return None
+        elif isinstance(node, str):
+            node = {"hostname": node}
+        ssh_key = node["sshKey"] if "sshKey" in node else self.sshKey
+        return SSHConfig(
+            hostname=node["hostname"],
+            username=node["username"] if "username" in node else self.username,
+            check_host_key=node["checkHostKey"]
+            if "checkHostKey" in node
+            else self.checkHostKey,
+            client_keys=[ssh_key] if ssh_key is not None else [],
+            password_file=node["passwordFile"]
+            if "passwordFile" in node
+            else self.passwordFile,
+            ssh_key_passphrase_file=(
+                node["sshKeyPassphraseFile"]
+                if "sshKeyPassphraseFile" in node
+                else self.sshKeyPassphraseFile
+            ),
+            tunnel=(
+                self._get_config(node["tunnel"])
+                if "tunnel" in node
+                else self.tunnel
+                if hasattr(self, "tunnel")
+                else None
+            ),
+        )
+
+    def _get_data_transfer_client(self, location: str) -> SSHContextManager:
+        if self.dataTransferConfig:
+            if location not in self.data_transfer_context_factories:
+                self.data_transfer_context_factories[location] = SSHContextFactory(
+                    streamflow_config_dir=self.config_dir,
+                    config=self.dataTransferConfig,
+                    max_concurrent_sessions=self.maxConcurrentSessions,
+                    max_connections=self.maxConnections,
+                )
+            return self.data_transfer_context_factories[location].get()
+        else:
+            return self._get_ssh_client(location)
+
+    async def _get_existing_parent(self, location: str, directory: str):
+        if directory is None:
+            return None
+        async with self._get_ssh_client(location) as ssh_client:
+            while True:
+                result = await ssh_client.run(
+                    f'test -e "{directory}"',
+                    stderr=asyncio.subprocess.STDOUT,
+                )
+                if result.returncode == 0:
+                    return directory
+                elif result.returncode == 1:
+                    directory = PurePosixPath(directory).parent
+                else:
+                    raise WorkflowExecutionException(result.stdout.strip())
+
+    @cachedmethod(lambda self: self.hardwareCache)
+    async def _get_location_hardware(
+        self,
+        location: str,
+        input_directory: str,
+        output_directory: str,
+        tmp_directory: str,
+    ) -> Hardware:
+        try:
+            async with self._get_ssh_client(location) as ssh_client:
+                (
+                    cores,
+                    memory,
+                    input_directory,
+                    output_directory,
+                    tmp_directory,
+                ) = await asyncio.gather(
+                    asyncio.create_task(
+                        ssh_client.run("nproc", stderr=asyncio.subprocess.STDOUT)
+                    ),
+                    asyncio.create_task(
+                        ssh_client.run(
+                            "free | grep Mem | awk '{print $2}'",
+                            stderr=asyncio.subprocess.STDOUT,
+                        )
+                    ),
+                    asyncio.create_task(_get_disk_usage(ssh_client, input_directory)),
+                    asyncio.create_task(_get_disk_usage(ssh_client, output_directory)),
+                    asyncio.create_task(_get_disk_usage(ssh_client, tmp_directory)),
+                )
+                if cores.returncode == 0 and memory.returncode == 0:
+                    return Hardware(
+                        cores=float(cores.stdout.strip()),
+                        memory=float(memory.stdout.strip()) / 2**10,
+                        input_directory=input_directory,
+                        output_directory=output_directory,
+                        tmp_directory=tmp_directory,
+                    )
+                else:
+                    raise WorkflowExecutionException(
+                        f"Impossible to retrieve locations for {location}"
+                    )
+        except WorkflowExecutionException:
+            raise WorkflowExecutionException(
+                f"Impossible to retrieve locations for {location}"
+            )
+
+    def _get_run_command(
+        self, command: str, location: Location, interactive: bool = False
+    ):
+        return f"ssh {location.name} {command}"
+
+    def _get_ssh_client(self, location: str) -> SSHContextManager:
+        if location not in self.ssh_context_factories:
+            self.ssh_context_factories[location] = SSHContextFactory(
+                streamflow_config_dir=self.config_dir,
+                config=self.nodes[location],
+                max_concurrent_sessions=self.maxConcurrentSessions,
+                max_connections=self.maxConnections,
+            )
+        return self.ssh_context_factories[location].get()
+
+    def _get_stream_reader(self, location: Location, src: str) -> StreamWrapperContext:
+        return SSHStreamWrapperContext(
+            src=src, ssh_context=self._get_data_transfer_client(location.name)
+        )
+
+    async def deploy(self, external: bool) -> None:
+        pass
 
     async def get_available_locations(
         self,
         service: str | None = None,
         input_directory: str | None = None,
         output_directory: str | None = None,
         tmp_directory: str | None = None,
     ) -> MutableMapping[str, AvailableLocation]:
-        if service is not None and service not in self.template_map.templates:
-            raise WorkflowDefinitionException(
-                f"Invalid service {service} for deployment {self.deployment_name}."
-            )
-        hostname = (await self._get_location()).hostname
-        return {
-            hostname: AvailableLocation(
-                name=hostname,
+        locations = {}
+        for location_obj in self.nodes.values():
+            inpdir, outdir, tmpdir = await asyncio.gather(
+                asyncio.create_task(
+                    self._get_existing_parent(location_obj.hostname, input_directory)
+                ),
+                asyncio.create_task(
+                    self._get_existing_parent(location_obj.hostname, output_directory)
+                ),
+                asyncio.create_task(
+                    self._get_existing_parent(location_obj.hostname, tmp_directory)
+                ),
+            )
+            hardware = await self._get_location_hardware(
+                location=location_obj.hostname,
+                input_directory=inpdir,
+                output_directory=outdir,
+                tmp_directory=tmpdir,
+            )
+            locations[location_obj.hostname] = AvailableLocation(
+                name=location_obj.hostname,
                 deployment=self.deployment_name,
                 service=service,
-                hostname=hostname,
-                slots=self.maxConcurrentJobs,
+                hostname=location_obj.hostname,
+                hardware=hardware,
             )
-        }
+        return locations
 
     @classmethod
     def get_schema(cls) -> str:
         return pkg_resources.resource_filename(
-            __name__, os.path.join("schemas", "queue_manager.json")
+            __name__, os.path.join("schemas", "ssh.json")
         )
 
     async def run(
         self,
         location: Location,
         command: MutableSequence[str],
         environment: MutableMapping[str, str] = None,
@@ -175,451 +610,48 @@
         stdin: int | str | None = None,
         stdout: int | str = asyncio.subprocess.STDOUT,
         stderr: int | str = asyncio.subprocess.STDOUT,
         capture_output: bool = False,
         timeout: int | None = None,
         job_name: str | None = None,
     ) -> tuple[Any | None, int] | None:
-        if job_name:
-            command = utils.create_command(
-                command=command, environment=environment, workdir=workdir
-            )
-            if logger.isEnabledFor(logging.DEBUG):
-                logger.debug(
-                    "EXECUTING command {command} on {location} {job}".format(
-                        command=command,
-                        location=location,
-                        job=f"for job {job_name}" if job_name else "",
-                    )
-                )
-            command = utils.encode_command(command)
+        command = self._get_command(
+            location=location,
+            command=command,
+            environment=environment,
+            workdir=workdir,
+            stdin=stdin,
+            stdout=stdout,
+            stderr=stderr,
+            job_name=job_name,
+        )
+        if job_name is not None:
             command = self.template_map.get_command(
                 command=command,
                 template=location.service,
                 environment=environment,
                 workdir=workdir,
             )
-            job_id = await self._run_batch_command(
-                command=command,
-                job_name=job_name,
-                location=location,
-                workdir=workdir,
-                stdin=stdin,
-                stdout=stdout,
-                stderr=stderr,
-                timeout=timeout,
-            )
-            if logger.isEnabledFor(logging.INFO):
-                logger.info(f"Scheduled job {job_name} with job id {job_id}")
-            self.scheduledJobs.append(job_id)
-            async with self.jobsCacheLock:
-                self.jobsCache.clear()
-            while True:
-                async with self.jobsCacheLock:
-                    running_jobs = await self._get_running_jobs(location)
-                if job_id not in running_jobs:
-                    break
-                await asyncio.sleep(self.pollingInterval)
-            self.scheduledJobs.remove(job_id)
-            return (
-                await self._get_output(job_id, location)
-                if stdout == asyncio.subprocess.STDOUT
-                else None,
-                await self._get_returncode(job_id, location),
-            )
-        else:
-            return await super().run(
-                location=location,
-                command=command,
-                environment=environment,
-                workdir=workdir,
-                stdin=stdin,
-                stdout=stdout,
-                stderr=stderr,
-                job_name=job_name,
-                timeout=timeout,
-                capture_output=capture_output,
-            )
-
-    async def undeploy(self, external: bool) -> None:
-        await self._remove_jobs(await self._get_location())
-        self.scheduledJobs = {}
-        if self._inner_ssh_connector:
-            if logger.isEnabledFor(logging.INFO):
-                logger.warn(
-                    f"UNDEPLOYING inner SSH connector for {self.deployment_name} deployment."
-                )
-            await self.connector.undeploy(external)
-            if logger.isEnabledFor(logging.INFO):
-                logger.warn(
-                    f"COMPLETED Undeployment of inner SSH connector for {self.deployment_name} deployment."
+            command = utils.encode_command(command)
+            async with self._get_ssh_client(location.name) as ssh_client:
+                result = await asyncio.wait_for(
+                    ssh_client.run(command, stderr=asyncio.subprocess.STDOUT),
+                    timeout=timeout,
                 )
-
-
-class SlurmConnector(QueueManagerConnector):
-    async def _get_output(self, job_id: str, location: Location) -> str:
-        command = [
-            "scontrol",
-            "show",
-            "-o",
-            "job",
-            job_id,
-            "|",
-            "sed",
-            "-n",
-            "'s/^.*StdOut=\\([^[:space:]]*\\).*/\\1/p'",
-        ]
-        if logger.isEnabledFor(logging.DEBUG):
-            logger.debug(f"Running command {' '.join(command)}")
-        stdout, _ = await self.connector.run(
-            location=location,
-            command=command,
-            capture_output=True,
-        )
-        if output_path := stdout.strip():
-            stdout, _ = await self.connector.run(
-                location=location, command=["cat", output_path], capture_output=True
-            )
-            return stdout.strip()
-        else:
-            return ""
-
-    async def _get_returncode(self, job_id: str, location: Location) -> int:
-        command = [
-            "scontrol",
-            "show",
-            "-o",
-            "job",
-            job_id,
-            "|",
-            "sed",
-            "-n",
-            "'s/^.*ExitCode=\\([0-9]\\+\\):.*/\\1/p'",
-        ]
-        if logger.isEnabledFor(logging.DEBUG):
-            logger.debug(f"Running command {' '.join(command)}")
-        stdout, _ = await self.connector.run(
-            location=location,
-            command=command,
-            capture_output=True,
-        )
-        return int(stdout.strip())
-
-    @cachedmethod(
-        lambda self: self.jobsCache,
-        key=partial(cachetools.keys.hashkey, "running_jobs"),
-    )
-    async def _get_running_jobs(self, location: Location) -> MutableSequence[str]:
-        command = [
-            "squeue",
-            "-h",
-            "-j",
-            ",".join(self.scheduledJobs),
-            "-t",
-            ",".join(
-                [
-                    "PENDING",
-                    "RUNNING",
-                    "SUSPENDED",
-                    "COMPLETING",
-                    "CONFIGURING",
-                    "RESIZING",
-                    "REVOKED",
-                    "SPECIAL_EXIT",
-                ]
-            ),
-            "-O",
-            "JOBID",
-        ]
-        if logger.isEnabledFor(logging.DEBUG):
-            logger.debug(f"Running command {' '.join(command)}")
-        stdout, _ = await self.connector.run(
-            location=location,
-            command=command,
-            capture_output=True,
-        )
-        return [j.strip() for j in stdout.strip().splitlines()]
-
-    async def _remove_jobs(self, location: Location) -> None:
-        await self.connector.run(
-            location=location, command=["scancel", " ".join(self.scheduledJobs)]
-        )
-
-    async def _run_batch_command(
-        self,
-        command: str,
-        job_name: str,
-        location: Location,
-        workdir: str | None = None,
-        stdin: int | str | None = None,
-        stdout: int | str = asyncio.subprocess.STDOUT,
-        stderr: int | str = asyncio.subprocess.STDOUT,
-        timeout: int | None = None,
-    ) -> str:
-        batch_command = [
-            "echo",
-            base64.b64encode(command.encode("utf-8")).decode("utf-8"),
-            "|",
-            "base64",
-            "-d",
-            "|",
-            "sbatch",
-            "--parsable",
-        ]
-        if workdir is not None:
-            batch_command.extend(["-D", workdir])
-        if stdin is not None:
-            batch_command.extend(["-i", shlex.quote(stdin)])
-        if stdout != asyncio.subprocess.STDOUT:
-            batch_command.extend(["-o", shlex.quote(stdout)])
-        if stderr != asyncio.subprocess.STDOUT and stderr != stdout:
-            batch_command.extend(["-e", shlex.quote(stderr)])
-        if timeout:
-            batch_command.extend(["-t", utils.format_seconds_to_hhmmss(timeout)])
-        if logger.isEnabledFor(logging.DEBUG):
-            logger.debug(f"Running command {' '.join(batch_command)}")
-        stdout, returncode = await self.connector.run(
-            location=location, command=batch_command, capture_output=True
-        )
-        if returncode == 0:
-            return stdout.strip()
         else:
-            raise WorkflowExecutionException(
-                f"Error submitting job {job_name} to Slurm: {stdout.strip()}"
-            )
-
-
-class PBSConnector(QueueManagerConnector):
-    async def _get_output(self, job_id: str, location: Location) -> str:
-        result = json.loads(await self._run_qstat_command(job_id, location))
-        output_path = result["Jobs"][job_id]["Output_Path"]
-        if ":" in output_path:
-            output_path = "".join(output_path.split(":")[1:])
-        if output_path:
-            stdout, _ = await self.connector.run(
-                location=location, command=["cat", output_path], capture_output=True
-            )
-            return stdout.strip()
-        else:
-            return ""
-
-    async def _get_returncode(self, job_id: str, location: Location) -> int:
-        result = json.loads(await self._run_qstat_command(job_id, location))
-        return int(result["Jobs"][job_id]["Exit_status"])
-
-    @cachedmethod(
-        lambda self: self.jobsCache,
-        key=partial(cachetools.keys.hashkey, "running_jobs"),
-    )
-    async def _get_running_jobs(self, location: Location) -> MutableSequence[str]:
-        command = [
-            "qstat",
-            " ".join(self.scheduledJobs),
-            "-xf",
-            "-Fjson",
-        ]
-        if logger.isEnabledFor(logging.DEBUG):
-            logger.debug(f"Running command {command}")
-        stdout, _ = await self.connector.run(
-            location=location,
-            command=command,
-            capture_output=True,
-        )
-        result = json.loads(stdout.strip())
-        return [
-            j
-            for j in self.scheduledJobs
-            if j not in result["Jobs"]  # Job id has not been processed yet
-            or result["Jobs"][j]["job_state"] not in ["E", "F"]  # Job finished
-        ]
-
-    async def _remove_jobs(self, location: Location) -> None:
-        await self.connector.run(
-            location=location, command=["qdel", " ".join(self.scheduledJobs)]
-        )
-
-    async def _run_batch_command(
-        self,
-        command: str,
-        job_name: str,
-        location: Location,
-        workdir: str | None = None,
-        stdin: int | str | None = None,
-        stdout: int | str = asyncio.subprocess.STDOUT,
-        stderr: int | str = asyncio.subprocess.STDOUT,
-        timeout: int | None = None,
-    ) -> str:
-        batch_command = ["sh", "-c"]
-        if workdir is not None:
-            batch_command.extend(["cd", workdir, "&&"])
-        batch_command.extend(
-            [
-                "echo",
-                base64.b64encode(command.encode("utf-8")).decode("utf-8"),
-                "|",
-                "base64",
-                "-d",
-                "|",
-                "qsub",
-            ]
-        )
-        if stdin is not None:
-            batch_command.extend(["-i", stdin])
-        batch_command.extend(
-            [
-                "-i",
-                stdout if stdout != asyncio.subprocess.STDOUT else utils.random_name(),
-            ]
-        )
-        if stderr != asyncio.subprocess.STDOUT and stderr != stdout:
-            batch_command.extend(["-e", stderr])
-        if timeout:
-            batch_command.extend(
-                ["-l", f"walltime={utils.format_seconds_to_hhmmss(timeout)}"]
-            )
-        batch_command.append("-")
-        stdout, returncode = await self.connector.run(
-            location=location, command=batch_command, capture_output=True
-        )
-        if returncode == 0:
-            return stdout.strip()
-        else:
-            raise WorkflowExecutionException(
-                f"Error submitting job {job_name} to PBS: {stdout.strip()}"
-            )
-
-    async def _run_qstat_command(self, job_id: str, location: Location) -> str:
-        command = [
-            "qstat",
-            job_id,
-            "-xf",
-            "-Fjson",
-        ]
-        if logger.isEnabledFor(logging.DEBUG):
-            logger.debug(f"Running command {command}")
-        stdout, _ = await self.connector.run(
-            location=location,
-            command=command,
-            capture_output=True,
-        )
-        return stdout.strip()
-
-
-class FluxConnector(QueueManagerConnector):
-    async def _get_output(self, job_id: str, location: Location) -> str:
-        # This will hang if the job is not complete
-        command = [
-            "flux",
-            "job",
-            "attach",
-            job_id,
-        ]
-        if logger.isEnabledFor(logging.DEBUG):
-            logger.debug(f"Running command {' '.join(command)}")
-        stdout, _ = await self.connector.run(
-            location=location,
-            command=command,
-            capture_output=True,
-        )
-        if output_path := stdout.strip():
-            stdout, _ = await self.connector.run(
-                location=location, command=["cat", output_path], capture_output=True
-            )
-            return stdout.strip()
-        else:
-            return ""
-
-    async def _get_returncode(self, job_id: str, location: Location) -> int:
-        command = [
-            "flux",
-            "jobs",
-            "--no-header",
-            "-o",
-            "{returncode}",
-            job_id,
-        ]
-        if logger.isEnabledFor(logging.DEBUG):
-            logger.debug(f"Running command {' '.join(command)}")
-        stdout, _ = await self.connector.run(
-            location=location,
-            command=command,
-            capture_output=True,
-        )
-        return int(stdout.strip())
-
-    @cachedmethod(
-        lambda self: self.jobsCache,
-        key=partial(cachetools.keys.hashkey, "running_jobs"),
-    )
-    async def _get_running_jobs(self, location: Location) -> MutableSequence[str]:
-        # If we add the job id, the filter is ignored
-        command = [
-            "flux",
-            "jobs",
-            "--no-header",
-            "--filter=pending,running",
-            '-o "{id}"',
-        ]
-        if logger.isEnabledFor(logging.DEBUG):
-            logger.debug(f"Running command {' '.join(command)}")
-        stdout, _ = await self.connector.run(
-            location=location,
-            command=command,
-            capture_output=True,
-        )
-        # Filter down to the job ids we are interested in
-        return [
-            j.strip()
-            for j in stdout.strip().splitlines()
-            if j.strip() in self.scheduledJobs
-        ]
-
-    async def _remove_jobs(self, location: Location) -> None:
-        await self.connector.run(
-            location=location,
-            command=["flux", "job", "cancel", " ".join(self.scheduledJobs)],
-        )
+            async with self._get_ssh_client(location.name) as ssh_client:
+                result = await asyncio.wait_for(
+                    ssh_client.run(
+                        command,
+                        stderr=asyncio.subprocess.STDOUT,
+                    ),
+                    timeout=timeout,
+                )
+        return result.stdout.strip(), result.returncode if capture_output else None
 
-    async def _run_batch_command(
-        self,
-        command: str,
-        job_name: str,
-        location: Location,
-        workdir: str | None = None,
-        stdin: int | str | None = None,
-        stdout: int | str = asyncio.subprocess.STDOUT,
-        stderr: int | str = asyncio.subprocess.STDOUT,
-        timeout: int | None = None,
-    ) -> str:
-        batch_command = [
-            "echo",
-            base64.b64encode(command.encode("utf-8")).decode("utf-8"),
-            "|",
-            "base64",
-            "-d",
-            "|",
-            "flux",
-            "batch",
-            "-N",
-            "1",
-        ]
-        if workdir is not None:
-            batch_command.extend(["--cwd", workdir])
-        if stdin is not None:
-            batch_command.extend(["--input", shlex.quote(stdin)])
-        if stdout != asyncio.subprocess.STDOUT:
-            batch_command.extend(["--output", shlex.quote(stdout)])
-        if stderr != asyncio.subprocess.STDOUT and stderr != stdout:
-            batch_command.extend(["--error", shlex.quote(stderr)])
-        if timeout:
-            batch_command.extend(["-t", utils.format_seconds_to_hhmmss(timeout)])
-        if logger.isEnabledFor(logging.DEBUG):
-            logger.debug(f"Running command {' '.join(batch_command)}")
-        stdout, returncode = await self.connector.run(
-            location=location, command=batch_command, capture_output=True
-        )
-        if returncode == 0:
-            return stdout.strip()
-        else:
-            raise WorkflowExecutionException(
-                f"Error submitting job {job_name} to Flux: {stdout.strip()}"
-            )
+    async def undeploy(self, external: bool) -> None:
+        for ssh_context in self.ssh_context_factories.values():
+            await ssh_context.close()
+        self.ssh_context_factories = {}
+        for ssh_context in self.data_transfer_context_factories.values():
+            await ssh_context.close()
+        self.data_transfer_context_factories = {}
```

### Comparing `streamflow-0.2.0.dev5/streamflow/deployment/connector/schemas/docker-compose.json` & `streamflow-0.2.0.dev6/streamflow/deployment/connector/schemas/docker-compose.json`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev5/streamflow/deployment/connector/schemas/docker.json` & `streamflow-0.2.0.dev6/streamflow/deployment/connector/schemas/docker.json`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev5/streamflow/deployment/connector/schemas/helm3.json` & `streamflow-0.2.0.dev6/streamflow/deployment/connector/schemas/helm3.json`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev5/streamflow/deployment/connector/schemas/kubernetes.json` & `streamflow-0.2.0.dev6/streamflow/deployment/connector/schemas/kubernetes.json`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev5/streamflow/deployment/connector/schemas/occam.json` & `streamflow-0.2.0.dev6/streamflow/deployment/connector/schemas/occam.json`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev5/streamflow/deployment/connector/schemas/queue_manager.json` & `streamflow-0.2.0.dev6/streamflow/deployment/connector/schemas/queue_manager.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7933333333333333%*

 * *Differences: {"'properties'": "{delete: ['services']}", 'delete': "['additionalProperties']"}*

```diff
@@ -1,11 +1,10 @@
 {
     "$id": "queue_manager.json",
     "$schema": "http://json-schema.org/draft-07/schema#",
-    "additionalProperties": false,
     "properties": {
         "checkHostKey": {
             "default": true,
             "description": "(**Deprecated.** Use the `wraps` directive to wrap a standalone SSH connector.) Perform a strict validation of the host SSH keys (and return exception if key is not recognized as valid)",
             "type": "boolean"
         },
         "dataTransferConnection": {
@@ -48,23 +47,14 @@
             "type": "string"
         },
         "pollingInterval": {
             "default": 5,
             "description": "Time interval (in seconds) between consecutive termination checks",
             "type": "integer"
         },
-        "services": {
-            "patternProperties": {
-                "^[a-z][a-zA-Z0-9._-]*$": {
-                    "description": "Path to a file containing a Jinja2 template, describing how the StreamFlow command should be executed in the remote environment",
-                    "type": "string"
-                }
-            },
-            "type": "object"
-        },
         "sshKey": {
             "description": "(**Deprecated.** Use the `wraps` directive to wrap a standalone SSH connector.) Path to the SSH key needed to connect with Slurm environment",
             "type": "string"
         },
         "sshKeyPassphraseFile": {
             "description": "(**Deprecated.** Use the `wraps` directive to wrap a standalone SSH connector.) Path to a file containing the passphrase protecting the SSH key",
             "type": "string"
```

### Comparing `streamflow-0.2.0.dev5/streamflow/deployment/connector/schemas/singularity.json` & `streamflow-0.2.0.dev6/streamflow/deployment/connector/schemas/singularity.json`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev5/streamflow/deployment/connector/schemas/ssh.json` & `streamflow-0.2.0.dev6/streamflow/deployment/connector/schemas/ssh.json`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev5/streamflow/deployment/deployment_manager.py` & `streamflow-0.2.0.dev6/streamflow/deployment/deployment_manager.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev5/streamflow/deployment/filter/shuffle.py` & `streamflow-0.2.0.dev6/streamflow/deployment/filter/shuffle.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev5/streamflow/deployment/future.py` & `streamflow-0.2.0.dev6/streamflow/deployment/future.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev5/streamflow/deployment/stream.py` & `streamflow-0.2.0.dev6/streamflow/deployment/stream.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev5/streamflow/deployment/template.py` & `streamflow-0.2.0.dev6/streamflow/deployment/template.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev5/streamflow/deployment/utils.py` & `streamflow-0.2.0.dev6/streamflow/deployment/utils.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev5/streamflow/deployment/wrapper.py` & `streamflow-0.2.0.dev6/streamflow/deployment/wrapper.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev5/streamflow/ext/plugin.py` & `streamflow-0.2.0.dev6/streamflow/ext/plugin.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev5/streamflow/ext/utils.py` & `streamflow-0.2.0.dev6/streamflow/ext/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,29 +6,41 @@
 from typing import Any, MutableMapping
 
 import jsonref
 from importlib_metadata import entry_points
 
 from streamflow.core.exception import InvalidPluginException
 from streamflow.core.utils import get_class_fullname
-from streamflow.ext.plugin import StreamFlowPlugin
+from streamflow.ext.plugin import StreamFlowPlugin, extension_points
 from streamflow.log_handler import logger
 
 PLUGIN_ENTRY_POINT = "unito.streamflow.plugin"
 
 
 def _filter_by_name(classes: MutableMapping[str, Any], name: str):
     filtered_classes = {}
     for class_ in classes:
         ext_objs = [ext for ext in classes[class_] if ext["name"] == name]
         if len(ext_objs) > 0:
             filtered_classes[class_] = ext_objs
     return filtered_classes
 
 
+def _flatten_all_of(entity_schema):
+    for obj in entity_schema["allOf"]:
+        if "allOf" in obj:
+            obj["properties"] = {**_flatten_all_of(obj), **obj.get("properties", {})}
+        entity_schema["properties"] = {
+            **obj.get("properties", {}),
+            **entity_schema.get("properties", {}),
+        }
+    del entity_schema["allOf"]
+    return dict(sorted(entity_schema["properties"].items()))
+
+
 def _get_property_desc(k: str, obj: MutableMapping[str, Any]) -> str:
     property_desc = [k]
     if "type" in obj:
         property_desc[0] = f"{property_desc[0]}: {_get_type_repr(obj)}"
     elif "oneOf" in obj:
         types = [_get_type_repr(oo) for oo in obj["oneOf"] if "type" in oo]
         property_desc[0] = f"{property_desc[0]}: Union[{', '.join(types)}]"
@@ -38,22 +50,113 @@
         property_desc.append(obj["description"])
     return "\n".join(property_desc)
 
 
 def _get_type_repr(obj: MutableMapping[str, Any]) -> str | None:
     if "type" in obj:
         if obj["type"] == "object":
-            return obj.get("title", "object")
+            if "patternProperties" in obj:
+                if len(obj["patternProperties"]) > 1:
+                    types = [
+                        _get_type_repr(t) for t in obj["patternProperties"].values()
+                    ]
+                    type_ = f"Union[{', '.join(types)}]"
+                else:
+                    type_ = _get_type_repr(list(obj["patternProperties"].values())[0])
+                return f"Map[str, {type_}]"
+            else:
+                return obj.get("title", "object")
         else:
             return obj["type"]
     else:
         return None
 
 
-def list_extensions():
+def list_extensions(name: str | None, type_: str | None):
+    extensions = {}
+    max_sizes = {
+        "name": 0,
+        "class": 0,
+        "plugin": 0,
+    }
+    for ext, classes in extension_points.items():
+        if type_ is None or ext == type_:
+            for n, v in classes.items():
+                if name is None or name == n:
+                    extensions.setdefault(ext, {})[n] = {
+                        "name": n,
+                        "class": get_class_fullname(v),
+                        "plugin": "-",
+                    }
+                    for k in max_sizes:
+                        max_sizes[k] = max(max_sizes[k], len(extensions[ext][n][k]))
+    if plugins := entry_points(group=PLUGIN_ENTRY_POINT):
+        for plugin in plugins:
+            plugin_class = (plugin.load())()
+            plugin_class.register()
+            if isinstance(plugin_class, StreamFlowPlugin):
+                plugin_classes = (
+                    {k: v for k, v in plugin_class.classes_.items() if k == type_}
+                    if type_ is not None
+                    else plugin_class.classes_
+                )
+                if name is not None:
+                    plugin_classes = _filter_by_name(plugin_classes, name)
+                for ext, items in plugin_classes.items():
+                    for item in items:
+                        extensions.setdefault(ext, {})[item["name"]] = {
+                            "name": item["name"],
+                            "class": get_class_fullname(item["class"]),
+                            "plugin": plugin.name,
+                        }
+                        for k in max_sizes:
+                            max_sizes[k] = max(
+                                max_sizes[k], len(extensions[ext][item["name"]][k])
+                            )
+    format_string = (
+        "{:<"
+        + str(max(max_sizes["name"] + 2, 6))
+        + "}"
+        + "{:<"
+        + str(max(max_sizes["class"] + 2, 12))
+        + "}"
+        + "{:<"
+        + str(max(max_sizes["plugin"], 8))
+        + "}"
+    )
+    if extensions:
+        for ext, items in extensions.items():
+            if type_ is None:
+                print(
+                    f"There {'are' if len(items) > 1 else 'is'} "
+                    f"{len(items)} available extension{'s' if len(items) > 1 else ''} "
+                    f"for the `{ext}` extension point:"
+                )
+            print(format_string.format("NAME", "CLASS_NAME", "PLUGIN"))
+            for item in items.values():
+                print(
+                    format_string.format(
+                        item["name"],
+                        item["class"],
+                        item["plugin"],
+                    )
+                )
+            print("")
+    else:
+        print(
+            "There are no available StreamFlow extensions{type}{sep}{name}.".format(
+                type=f" of type `{type_}`" if type_ is not None else "",
+                sep=" and" if type_ is not None and name is not None else "",
+                name=f" with name `{name}`" if name is not None else "",
+            ),
+            file=sys.stderr,
+        )
+
+
+def list_plugins():
     if plugins := entry_points(group=PLUGIN_ENTRY_POINT):
         plugin_objs = []
         max_sizes = {
             "name": 0,
             "package": 0,
             "version": 0,
             "class": 0,
@@ -111,71 +214,104 @@
                 )
         else:
             raise InvalidPluginException(
                 "StreamFlow plugins must extend the streamflow.ext.StreamFlowPlugin class"
             )
 
 
-def show_extension(
-    plugin: str, name: str | None, type_: str | None, show_schema: bool = False
-):
+def show_extension(name: str, type_: str):
+    plugin = "-"
+    if name in extension_points[type_]:
+        class_ = extension_points[type_][name]
+    else:
+        class_ = None
+        for plugin_obj in entry_points(group=PLUGIN_ENTRY_POINT):
+            plugin_class = (plugin_obj.load())()
+            if isinstance(plugin_class, StreamFlowPlugin):
+                plugin_class.register()
+                plugin_classes = _filter_by_name(
+                    {k: v for k, v in plugin_class.classes_.items() if k == type_}, name
+                )
+                for item in plugin_classes.get(type_, []):
+                    if item["name"] == name:
+                        class_ = item["class"]
+                        plugin = plugin_obj.name
+    if class_ is not None:
+        class_name = get_class_fullname(class_)
+        entity_schema = class_.get_schema()
+        with open(entity_schema) as f:
+            entity_schema = jsonref.loads(
+                f.read(),
+                base_uri=f"file://{os.path.dirname(entity_schema)}/",
+                jsonschema=True,
+            )
+        if "allOf" in entity_schema:
+            entity_schema["properties"] = _flatten_all_of(entity_schema)
+        format_string = (
+            "{:<"
+            + str(max(len(name) + 2, 6))
+            + "}"
+            + "{:<"
+            + str(max(len(class_name) + 2, 10))
+            + "}"
+            + "{:<"
+            + str(max(len(plugin), 8))
+            + "}"
+        )
+        print(format_string.format("NAME", "CLASS_NAME", "PLUGIN"))
+        print(format_string.format(name, class_name, plugin))
+        property_descs = []
+        for k, v in entity_schema.get("properties", {}).items():
+            if k in entity_schema.get("required", []):
+                property_descs.append(_get_property_desc(k, v))
+        if property_descs:
+            print("\nREQUIRED\n")
+            print("\n---\n".join(property_descs))
+            property_descs = []
+        for k, v in entity_schema.get("properties", {}).items():
+            if k not in entity_schema.get("required", []):
+                property_descs.append(_get_property_desc(k, v))
+        if property_descs:
+            print("\nOPTIONAL\n")
+            print("\n---\n".join(property_descs))
+    else:
+        print(
+            f"No StreamFlow extension `{name}` of type `{type_}` detected.",
+            file=sys.stderr,
+        )
+
+
+def show_plugin(plugin: str):
     if plugins := entry_points(name=plugin, group=PLUGIN_ENTRY_POINT):
-        plugin = plugins[plugin]
-        plugin_class = (plugin.load())()
+        plugin_obj = plugins[plugin]
+        plugin_class = (plugin_obj.load())()
         if isinstance(plugin_class, StreamFlowPlugin):
             plugin_class.register()
-            print(f"NAME: {plugin.name}")
-            print(f"PACKAGE: {plugin.dist.name}")
-            print(f"VERSION: {plugin.dist.version}")
+            print(f"NAME: {plugin_obj.name}")
+            print(f"PACKAGE: {plugin_obj.dist.name}")
+            print(f"VERSION: {plugin_obj.dist.version}")
             print(f"CLASS_NAME: {get_class_fullname(type(plugin_class))}\n")
-            plugin_classes = plugin_class.classes_
-            if type_ is not None:
-                plugin_classes = {k: v for k, v in plugin_classes.items() if k == type_}
-                if len(plugin_classes) == 0:
-                    print(
-                        f"It does not provide any StreamFlow extension of type `{type_}`"
-                    )
-                else:
-                    if name is not None:
-                        plugin_classes = _filter_by_name(plugin_classes, name)
-                        if len(plugin_classes) == 0:
-                            print(
-                                f"It does not provide any StreamFlow extension of type `{type_}` with name `{name}`"
-                            )
-            elif name is not None:
-                plugin_classes = _filter_by_name(plugin_classes, name)
-                if len(plugin_classes) == 0:
-                    print(
-                        f"It does not provide any StreamFlow extension with name `{name}`"
-                    )
-            elif len(plugin_classes) == 0:
+            classes = plugin_class.classes_
+            if len(classes) == 0:
                 print("It does not provide any StreamFlow extension")
-            if len(plugin_classes) > 0:
+            else:
                 ext_objs = {}
                 max_sizes = {"name": 0, "class": 0}
-                for extension_point, items in plugin_classes.items():
+                for extension_point, items in classes.items():
                     for item in items:
                         ext_objs.setdefault(extension_point, []).append(
                             {
                                 "name": item["name"],
                                 "class": get_class_fullname(item["class"]),
                             }
                         )
                         for k in max_sizes:
                             max_sizes[k] = max(
                                 max_sizes[k], len(ext_objs[extension_point][-1][k])
                             )
-                        if show_schema:
-                            entity_schema = item["class"].get_schema()
-                            with open(entity_schema) as f:
-                                ext_objs[extension_point][-1]["schema"] = jsonref.loads(
-                                    f.read(),
-                                    base_uri=f"file://{os.path.dirname(entity_schema)}/",
-                                    jsonschema=True,
-                                )
                 format_string = (
                     "{:<"
                     + str(max(max_sizes["name"] + 2, 6))
                     + "}"
                     + "{:<"
                     + str(max(max_sizes["class"] + 2, 10))
                     + "}"
@@ -190,38 +326,13 @@
                     for ext_point in ext_obj:
                         print(
                             format_string.format(
                                 ext_point["name"],
                                 ext_point["class"],
                             )
                         )
-                if show_schema:
-                    print("\nSCHEMAS:")
-                    for extension_point, ext_obj in ext_objs.items():
-                        for ext_point in ext_obj:
-                            title = f"`{ext_point['name']}` {extension_point} ({ext_point['class']})"
-                            print(f"\n{title}")
-                            print("-" * len(title))
-                            property_descs = []
-                            for k, v in (
-                                ext_point["schema"].get("properties", {}).items()
-                            ):
-                                if k in ext_point["schema"].get("required", []):
-                                    property_descs.append(_get_property_desc(k, v))
-                            if property_descs:
-                                print("\nREQUIRED\n")
-                                print("\n---\n".join(property_descs))
-                                property_descs = []
-                            for k, v in (
-                                ext_point["schema"].get("properties", {}).items()
-                            ):
-                                if k not in ext_point["schema"].get("required", []):
-                                    property_descs.append(_get_property_desc(k, v))
-                            if property_descs:
-                                print("\nOPTIONAL\n")
-                                print("\n---\n".join(property_descs))
         else:
             print(
                 "Invalid plugin: it does not extend the streamflow.ext.StreamFlowPlugin class"
             )
     else:
         print(f"No StreamFlow plugin named `{plugin}` detected.", file=sys.stderr)
```

### Comparing `streamflow-0.2.0.dev5/streamflow/log_handler.py` & `streamflow-0.2.0.dev6/streamflow/log_handler.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev5/streamflow/main.py` & `streamflow-0.2.0.dev6/streamflow/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,24 +14,37 @@
 from streamflow.core.context import StreamFlowContext
 from streamflow.core.exception import WorkflowProvenanceException
 from streamflow.core.provenance import ProvenanceManager
 from streamflow.core.workflow import Workflow
 from streamflow.cwl.main import main as cwl_main
 from streamflow.data import data_manager_classes
 from streamflow.deployment import deployment_manager_classes
-from streamflow.ext.utils import list_extensions, load_extensions, show_extension
+from streamflow.ext.utils import (
+    list_extensions,
+    list_plugins,
+    load_extensions,
+    show_extension,
+    show_plugin,
+)
 from streamflow.log_handler import CustomFormatter, HighlitingFilter, logger
 from streamflow.parser import parser
 from streamflow.persistence import database_classes
 from streamflow.persistence.loading_context import DefaultDatabaseLoadingContext
 from streamflow.provenance import prov_classes
 from streamflow.recovery import checkpoint_manager_classes, failure_manager_classes
 from streamflow.scheduling import scheduler_classes
 
 
+async def _async_ext(args: argparse.Namespace):
+    if args.ext_context == "list":
+        list_extensions(args.name, args.type)
+    elif args.ext_context == "show":
+        show_extension(args.name, args.type)
+
+
 async def _async_list(args: argparse.Namespace):
     context = _get_context_from_config(args.file)
     try:
         if workflows := await context.database.list_workflows(args.name):
             max_sizes = {
                 k: len(max(str(w[k]) for w in workflows)) + 1
                 for k in workflows[0].keys()
@@ -76,17 +89,17 @@
             print("No workflow objects found.")
     finally:
         await context.close()
 
 
 async def _async_plugin(args: argparse.Namespace):
     if args.plugin_context == "list":
-        list_extensions()
+        list_plugins()
     elif args.plugin_context == "show":
-        show_extension(args.plugin, args.name, args.type, args.show_schema)
+        show_plugin(args.plugin)
 
 
 async def _async_prov(args: argparse.Namespace):
     context = _get_context_from_config(args.file)
     try:
         db_context = DefaultDatabaseLoadingContext()
         workflows = await context.database.get_workflows_by_name(
@@ -133,15 +146,15 @@
                 additional_properties=args.add_property,
             )
     finally:
         await context.close()
 
 
 async def _async_report(args: argparse.Namespace):
-    context = _get_context_from_config(args.streamflow_file, args.outdir)
+    context = _get_context_from_config(args.file)
     try:
         await report.create_report(context, args)
     finally:
         await context.close()
 
 
 async def _async_run(args: argparse.Namespace):
@@ -161,14 +174,15 @@
             await asyncio.gather(*workflow_tasks)
     finally:
         await context.close()
 
 
 def _get_context_from_config(streamflow_file: str | None) -> StreamFlowContext:
     if os.path.exists(streamflow_file):
+        load_extensions()
         streamflow_config = SfValidator().validate_file(streamflow_file)
         streamflow_config["path"] = streamflow_file
         return build_context(streamflow_config)
     else:
         return build_context({"path": os.getcwd()})
 
 
@@ -230,14 +244,16 @@
 def main(args):
     try:
         args = parser.parse_args(args)
         if args.context == "version":
             from streamflow.version import VERSION
 
             print(f"StreamFlow version {VERSION}")
+        elif args.context == "ext":
+            asyncio.run(_async_ext(args))
         elif args.context == "list":
             asyncio.run(_async_list(args))
         elif args.context == "plugin":
             asyncio.run(_async_plugin(args))
         elif args.context == "prov":
             asyncio.run(_async_prov(args))
         elif args.context == "report":
```

### Comparing `streamflow-0.2.0.dev5/streamflow/parser.py` & `streamflow-0.2.0.dev6/streamflow/parser.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import argparse
 import os
 import re
 
+import streamflow.ext.plugin
 
 UNESCAPED_COMMA = re.compile(r"(?<!\\),")
 UNESCAPED_EQUAL = re.compile(r"(?<!\\)=")
 
 
 class _KeyValueAction(argparse.Action):
     def __call__(self, _parser, namespace, values, option_string=None):
@@ -22,26 +23,61 @@
         setattr(namespace, self.dest, items)
 
 
 parser = argparse.ArgumentParser(description="StreamFlow Command Line")
 subparsers = parser.add_subparsers(dest="context")
 
 
+# streamflow ext
+ext_parser = subparsers.add_parser(
+    "ext", help="Retrieve information on the available StreamFlow extensions"
+)
+ext_subparsers = ext_parser.add_subparsers(dest="ext_context")
+
+# streamflow ext list
+ext_list_parser = ext_subparsers.add_parser(
+    "list", help="List the available StreamFlow extensions"
+)
+ext_list_parser.add_argument("--name", "-n", type=str, help="Filter extensions by name")
+ext_list_parser.add_argument(
+    "--type",
+    "-t",
+    type=str,
+    choices=streamflow.ext.plugin.extension_points,
+    help="Filter extensions by type",
+)
+
+# streamflow ext show
+ext_show_parser = ext_subparsers.add_parser(
+    "show", help="Show the details of a StreamFlow extension"
+)
+ext_show_parser.add_argument(
+    "type",
+    metavar="TYPE",
+    type=str,
+    choices=streamflow.ext.plugin.extension_points,
+    help="Type of the extension to show",
+)
+ext_show_parser.add_argument(
+    "name", metavar="NAME", type=str, help="Name of the extension to show"
+)
+
 # streamflow list
 list_parser = subparsers.add_parser("list", help="List the executed workflows")
 list_parser.add_argument(
     "--file",
     "-f",
     default="streamflow.yml",
     type=str,
     help="Path to the StreamFlow file describing the workflow execution",
 )
 list_parser.add_argument(
     "name",
     metavar="NAME",
+    nargs="?",
     type=str,
     help="List all executions for the given workflow",
 )
 
 # streamflow plugin
 plugin_parser = subparsers.add_parser(
     "plugin", help="Retrieve information on the installed StreamFlow plugins"
@@ -56,40 +92,14 @@
 # streamflow plugin show
 plugin_show_parser = plugin_subparsers.add_parser(
     "show", help="Show the details of a StreamFlow plugin"
 )
 plugin_show_parser.add_argument(
     "plugin", metavar="PLUGIN", type=str, help="Name of the plugin to show"
 )
-plugin_show_parser.add_argument(
-    "--name", "-n", type=str, help="Filter extensions by name"
-)
-plugin_show_parser.add_argument(
-    "--type",
-    "-t",
-    type=str,
-    choices=[
-        "binding_filter",
-        "checkpoint_manager",
-        "cwl_docker_translator",
-        "connector",
-        "data_manager",
-        "database",
-        "deployment_manager",
-        "failure_manager",
-        "policy",
-        "scheduler",
-    ],
-    help="Filter extensions by type",
-)
-plugin_show_parser.add_argument(
-    "--show-schema",
-    action="store_true",
-    help="Print property schemas for selected extension points",
-)
 
 # streamflow prov
 prov_parser = subparsers.add_parser(
     "prov", help="Generate a provenance archive for an executed workflow"
 )
 prov_parser.register("action", "key_value", _KeyValueAction)
 prov_parser.add_argument(
```

### Comparing `streamflow-0.2.0.dev5/streamflow/persistence/base.py` & `streamflow-0.2.0.dev6/streamflow/persistence/base.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev5/streamflow/persistence/loading_context.py` & `streamflow-0.2.0.dev6/streamflow/persistence/loading_context.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev5/streamflow/persistence/schemas/sqlite.json` & `streamflow-0.2.0.dev6/streamflow/persistence/schemas/sqlite.json`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev5/streamflow/persistence/schemas/sqlite.sql` & `streamflow-0.2.0.dev6/streamflow/persistence/schemas/sqlite.sql`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev5/streamflow/persistence/sqlite.py` & `streamflow-0.2.0.dev6/streamflow/persistence/sqlite.py`

 * *Files 4% similar despite different names*

```diff
@@ -219,14 +219,36 @@
             async with db.execute(
                 "INSERT INTO workflow(name, params, status, type) "
                 "VALUES(:name, :params, :status, :type)",
                 {"name": name, "params": params, "status": status, "type": type},
             ) as cursor:
                 return cursor.lastrowid
 
+    async def get_dependees(
+        self, token_id: int
+    ) -> MutableSequence[MutableMapping[str, Any]]:
+        async with self.connection as db:
+            db.row_factory = aiosqlite.Row
+            async with db.execute(
+                "SELECT * FROM provenance WHERE depender = :depender",
+                {"depender": token_id},
+            ) as cursor:
+                return await cursor.fetchall()
+
+    async def get_dependers(
+        self, token_id: int
+    ) -> MutableSequence[MutableMapping[str, Any]]:
+        async with self.connection as db:
+            db.row_factory = aiosqlite.Row
+            async with db.execute(
+                "SELECT * FROM provenance WHERE dependee = :dependee",
+                {"dependee": token_id},
+            ) as cursor:
+                return await cursor.fetchall()
+
     async def get_command(self, command_id: int) -> MutableMapping[str, Any]:
         async with self.connection as db:
             db.row_factory = aiosqlite.Row
             async with db.execute(
                 "SELECT * FROM command WHERE id = :id", {"id": command_id}
             ) as cursor:
                 return await cursor.fetchone()
```

### Comparing `streamflow-0.2.0.dev5/streamflow/provenance/run_crate.py` & `streamflow-0.2.0.dev6/streamflow/provenance/run_crate.py`

 * *Files 0% similar despite different names*

```diff
@@ -567,16 +567,16 @@
         if "src" not in file:
             raise WorkflowProvenanceException(
                 "Property `src` is mandatory when specifying the `--add-file` option."
             )
         src = file["src"]
         dst = file.get("dst", posixpath.sep)
         dst_parent = posixpath.dirname(posixpath.normpath(dst))
-        if logger.isEnabledFor(logging.WARN):
-            if src in self.files_map:
+        if src in self.files_map:
+            if logger.isEnabledFor(logging.WARN):
                 logger.warn(f"File {src} is already present in the archive.")
         else:
             if os.path.isfile(os.path.realpath(src)):
                 checksum = _file_checksum(
                     src, hashlib.new("sha1", usedforsecurity=False)
                 )
                 jsonld_file = {
```

### Comparing `streamflow-0.2.0.dev5/streamflow/recovery/checkpoint_manager.py` & `streamflow-0.2.0.dev6/streamflow/recovery/checkpoint_manager.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev5/streamflow/recovery/failure_manager.py` & `streamflow-0.2.0.dev6/streamflow/recovery/failure_manager.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev5/streamflow/recovery/recovery.py` & `streamflow-0.2.0.dev6/streamflow/recovery/recovery.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev5/streamflow/report.py` & `streamflow-0.2.0.dev6/streamflow/report.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev5/streamflow/scheduling/policy/data_locality.py` & `streamflow-0.2.0.dev6/streamflow/scheduling/policy/data_locality.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev5/streamflow/scheduling/scheduler.py` & `streamflow-0.2.0.dev6/streamflow/scheduling/scheduler.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev5/streamflow/workflow/combinator.py` & `streamflow-0.2.0.dev6/streamflow/workflow/combinator.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,53 +8,14 @@
 from streamflow.core.exception import WorkflowExecutionException
 from streamflow.core.persistence import DatabaseLoadingContext
 from streamflow.core.workflow import Token, Workflow
 from streamflow.workflow.step import Combinator
 from streamflow.workflow.token import IterationTerminationToken
 
 
-def _add_to_list(
-    token: Token | MutableMapping[str, Token],
-    token_values: MutableMapping[str, MutableMapping[str, MutableSequence[Any]]],
-    port_name: str,
-    depth: int = 0,
-):
-    tag = (
-        utils.get_tag(token.values())
-        if isinstance(token, MutableMapping)
-        else token.tag
-    )
-    if depth:
-        tag = ".".join(tag.split(".")[:-depth])
-    for key in list(token_values.keys()):
-        if tag == key:
-            continue
-        elif key.startswith(tag):
-            _add_to_port(token, token_values[key], port_name)
-        elif tag.startswith(key):
-            if tag not in token_values:
-                token_values[tag] = {}
-            for p in token_values[key]:
-                for t in token_values[key][p]:
-                    _add_to_port(t, token_values[tag], p)
-    if tag not in token_values:
-        token_values[tag] = {}
-    _add_to_port(token, token_values[tag], port_name)
-
-
-def _add_to_port(
-    token: Token | MutableMapping[str, Token],
-    tag_values: MutableMapping[str, MutableSequence[Any]],
-    port_name: str,
-):
-    if port_name not in tag_values:
-        tag_values[port_name] = deque()
-    tag_values[port_name].append(token)
-
-
 class CartesianProductCombinator(Combinator):
     def __init__(self, name: str, workflow: Workflow, depth: int = 1):
         super().__init__(name, workflow)
         self.depth: int = depth
         self.token_values: MutableMapping[
             str, MutableMapping[str, MutableSequence[Any]]
         ] = {}
@@ -69,15 +30,17 @@
         return cls(
             name=row["name"],
             workflow=await loading_context.load_workflow(context, row["workflow"]),
             depth=row["depth"],
         )
 
     async def _product(
-        self, port_name: str, token: Token | MutableSequence[Token]
+        self,
+        port_name: str,
+        token: Token | MutableSequence[Token],
     ) -> AsyncIterable[MutableMapping[str, Token]]:
         # Get all combinations of the new element with the others
         tag = ".".join(token.tag.split(".")[: -self.depth])
         if len(self.token_values[tag]) == len(self.items):
             cartesian_product = utils.dict_product(
                 **{
                     k: [token] if k == port_name else v
@@ -88,48 +51,67 @@
             for config in cartesian_product:
                 schema = {}
                 for key in self.items:
                     if key in self.combinators:
                         schema = {**schema, **config[key]}
                     else:
                         schema[key] = config[key]
-                        schema[key] = config[key]
                 suffix = [t.tag.split(".")[-1] for t in schema.values()]
-                schema = {
-                    k: t.retag(".".join(t.tag.split(".")[:-1] + suffix))
+                yield {
+                    k: {
+                        "token": t.retag(".".join(t.tag.split(".")[:-1] + suffix)),
+                        "input_ids": [t.persistent_id],
+                    }
                     for k, t in schema.items()
                 }
-                yield schema
 
     async def _save_additional_params(self, context: StreamFlowContext):
         return {
             **await super()._save_additional_params(context),
             **{"depth": self.depth},
         }
 
     async def combine(
-        self, port_name: str, token: Token
+        self,
+        port_name: str,
+        token: Token,
     ) -> AsyncIterable[MutableMapping[str, Token]]:
-        # If port is associated to an inner combinator, call it and put shcemas in their related list
+        # If port is associated to an inner combinator, call it and put schemas in their related list
         if c := self.get_combinator(port_name):
-            async for schema in cast(AsyncIterable, c.combine(port_name, token)):
-                _add_to_list(schema, self.token_values, c.name, self.depth)
+            async for schema in cast(
+                AsyncIterable,
+                c.combine(port_name, token),
+            ):
+                self._add_to_list(schema, c.name, self.depth)
                 async for product in self._product(port_name, token):
                     yield product
         # If port is associated directly with the current combinator, put the token in the list
         elif port_name in self.items:
-            _add_to_list(token, self.token_values, port_name, self.depth)
+            self._add_to_list(token, port_name, self.depth)
             async for product in self._product(port_name, token):
                 yield product
         # Otherwise throw Exception
         else:
             raise WorkflowExecutionException(
                 f"No item to combine for token '{port_name}'."
             )
 
+    def _add_to_port(
+        self,
+        token: Token | MutableMapping[str, Token],
+        tag_values: MutableMapping[str, MutableSequence[Any]],
+        port_name: str,
+    ):
+        if port_name not in tag_values:
+            tag_values[port_name] = deque()
+        for t in tag_values[port_name]:
+            if t.tag == token.tag:
+                return
+        tag_values[port_name].append(token)
+
 
 class DotProductCombinator(Combinator):
     def __init__(self, name: str, workflow: Workflow):
         super().__init__(name, workflow)
         self.token_values: MutableMapping[
             str, MutableMapping[str, MutableSequence[Any]]
         ] = {}
@@ -143,31 +125,44 @@
                     # Return the relative combination schema
                     schema = {}
                     for key, elements in self.token_values[tag].items():
                         element = elements.pop()
                         if key in self.combinators:
                             schema = {**schema, **element}
                         else:
-                            schema[key] = element
-                    tag = utils.get_tag(schema.values())
-                    schema = {k: t.retag(tag) for k, t in schema.items()}
-                    yield schema
+                            schema[key] = {
+                                "token": element,
+                                "input_ids": [element.persistent_id],
+                            }
+                    tag = utils.get_tag([t["token"] for t in schema.values()])
+                    yield {
+                        k: {
+                            "token": t["token"].retag(tag),
+                            "input_ids": t["input_ids"],
+                        }
+                        for k, t in schema.items()
+                    }
 
     async def combine(
-        self, port_name: str, token: Token
+        self,
+        port_name: str,
+        token: Token,
     ) -> AsyncIterable[MutableMapping[str, Token]]:
-        # If port is associated to an inner combinator, call it and put shcemas in their related list
+        # If port is associated to an inner combinator, call it and put schemas in their related list
         if c := self.get_combinator(port_name):
-            async for schema in cast(AsyncIterable, c.combine(port_name, token)):
-                _add_to_list(schema, self.token_values, c.name)
+            async for schema in cast(
+                AsyncIterable,
+                c.combine(port_name, token),
+            ):
+                self._add_to_list(schema, c.name)
                 async for product in self._product():
                     yield product
         # If port is associated directly with the current combinator, put the token in the list
         elif port_name in self.items:
-            _add_to_list(token, self.token_values, port_name)
+            self._add_to_list(token, port_name)
             async for product in self._product():
                 yield product
         # Otherwise throw Exception
         else:
             raise WorkflowExecutionException(
                 f"No item to combine for token '{port_name}'."
             )
@@ -176,24 +171,26 @@
 class LoopCombinator(DotProductCombinator):
     def __init__(self, name: str, workflow: Workflow):
         super().__init__(name, workflow)
         self.iteration_map: MutableMapping[str, int] = {}
 
     async def _product(self) -> AsyncIterable[MutableMapping[str, Token]]:
         async for schema in super()._product():
-            tag = utils.get_tag(schema.values())
+            tag = utils.get_tag([t["token"] for t in schema.values()])
             prefix = ".".join(tag.split(".")[:-1])
             if prefix not in self.iteration_map:
                 self.iteration_map[tag] = 0
                 tag = ".".join(tag.split(".") + ["0"])
             else:
                 self.iteration_map[prefix] += 1
                 tag = ".".join(tag.split(".")[:-1] + [str(self.iteration_map[prefix])])
-            schema = {k: t.retag(tag) for k, t in schema.items()}
-            yield schema
+            yield {
+                k: {"token": t["token"].retag(tag), "input_ids": t["input_ids"]}
+                for k, t in schema.items()
+            }
 
 
 class LoopTerminationCombinator(DotProductCombinator):
     def __init__(self, name: str, workflow: Workflow):
         super().__init__(name, workflow)
         self.output_items: MutableSequence[str] = []
         self.token_values: MutableMapping[
@@ -201,9 +198,15 @@
         ] = {}
 
     def add_output_item(self, item: str) -> None:
         self.output_items.append(item)
 
     async def _product(self) -> AsyncIterable[MutableMapping[str, Token]]:
         async for schema in super()._product():
-            tag = utils.get_tag(schema.values())
-            yield {k: IterationTerminationToken(tag=tag) for k in self.output_items}
+            tag = utils.get_tag([t["token"] for t in schema.values()])
+            yield {
+                k: {
+                    "token": IterationTerminationToken(tag=tag),
+                    "input_ids": [id for t in schema.values() for id in t["input_ids"]],
+                }
+                for k in self.output_items
+            }
```

### Comparing `streamflow-0.2.0.dev5/streamflow/workflow/executor.py` & `streamflow-0.2.0.dev6/streamflow/workflow/executor.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev5/streamflow/workflow/port.py` & `streamflow-0.2.0.dev6/streamflow/workflow/port.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev5/streamflow/workflow/step.py` & `streamflow-0.2.0.dev6/streamflow/workflow/step.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 import asyncio
 import json
 import logging
 import posixpath
 from abc import ABC, abstractmethod
+from collections import deque
 from types import ModuleType
 from typing import (
     Any,
     AsyncIterable,
     Iterable,
     MutableMapping,
     MutableSequence,
@@ -37,15 +38,19 @@
     Workflow,
 )
 from streamflow.data import remotepath
 from streamflow.deployment.utils import get_path_processor
 from streamflow.log_handler import logger
 from streamflow.workflow.port import ConnectorPort, JobPort
 from streamflow.workflow.token import JobToken, ListToken, TerminationToken
-from streamflow.workflow.utils import check_iteration_termination, check_termination
+from streamflow.workflow.utils import (
+    check_iteration_termination,
+    check_termination,
+    get_job_token,
+)
 
 
 def _get_directory(path_processor: ModuleType, directory: str | None, target: Target):
     return directory or path_processor.join(target.workdir, utils.random_name())
 
 
 def _get_step_status(statuses: MutableSequence[Status]):
@@ -69,14 +74,18 @@
 ) -> None:
     for name, token in inputs.items():
         if token.tag not in inputs_map:
             inputs_map[token.tag] = {}
         inputs_map[token.tag][name] = token
 
 
+def _get_token_ids(token_list):
+    return [t.persistent_id for t in (token_list or []) if t.persistent_id]
+
+
 class BaseStep(Step, ABC):
     def __init__(self, name: str, workflow: Workflow):
         super().__init__(name, workflow)
         self._log_level: int = logging.DEBUG
 
     async def _get_inputs(self, input_ports: MutableMapping[str, Port]):
         inputs = {
@@ -96,20 +105,24 @@
                 logger.debug(f"Step {self.name} received termination token")
             logger.debug(
                 f"Step {self.name} received inputs {[t.tag for t in inputs.values()]}"
             )
         return inputs
 
     async def _persist_token(
-        self, token: Token, port: Port, inputs: Iterable[Token]
+        self, token: Token, port: Port, input_token_ids: Iterable[int]
     ) -> Token:
+        if token.persistent_id:
+            raise WorkflowDefinitionException(
+                f"Token already has an id: {token.persistent_id}"
+            )
         await token.save(self.workflow.context, port_id=port.persistent_id)
-        if inputs:
+        if input_token_ids:
             await self.workflow.context.database.add_provenance(
-                inputs=[i.persistent_id for i in inputs], token=token.persistent_id
+                inputs=input_token_ids, token=token.persistent_id
             )
         return token
 
     async def terminate(self, status: Status):
         if not self.terminated:
             self.terminated = True
             # If not explicitly cancelled, close input ports
@@ -214,14 +227,52 @@
 
     async def save(self, context: StreamFlowContext):
         return {
             "type": utils.get_class_fullname(type(self)),
             "params": await self._save_additional_params(context),
         }
 
+    def _add_to_list(
+        self,
+        token: Token | MutableMapping[str, Token],
+        port_name: str,
+        depth: int = 0,
+    ):
+        tag = (
+            utils.get_tag([t["token"] for t in token.values()])
+            if isinstance(token, MutableMapping)
+            else token.tag
+        )
+        if depth:
+            tag = ".".join(tag.split(".")[:-depth])
+        for key in list(self.token_values.keys()):
+            if tag == key:
+                continue
+            elif key.startswith(tag):
+                self._add_to_port(token, self.token_values[key], port_name)
+            elif tag.startswith(key):
+                if tag not in self.token_values:
+                    self.token_values[tag] = {}
+                for p in self.token_values[key]:
+                    for t in self.token_values[key][p]:
+                        self._add_to_port(t, self.token_values[tag], p)
+        if tag not in self.token_values:
+            self.token_values[tag] = {}
+        self._add_to_port(token, self.token_values[tag], port_name)
+
+    def _add_to_port(
+        self,
+        token: Token | MutableMapping[str, Token],
+        tag_values: MutableMapping[str, MutableSequence[Any]],
+        port_name: str,
+    ):
+        if port_name not in tag_values:
+            tag_values[port_name] = deque()
+        tag_values[port_name].append(token)
+
 
 class CombinatorStep(BaseStep):
     def __init__(self, name: str, workflow: Workflow, combinator: Combinator):
         super().__init__(name, workflow)
         self.combinator: Combinator = combinator
 
     @classmethod
@@ -279,24 +330,27 @@
                     else:
                         if logger.isEnabledFor(logging.DEBUG):
                             logger.debug(
                                 f"Step {self.name} received token {token.tag} on port {task_name}"
                             )
                         status = Status.COMPLETED
                         async for schema in cast(
-                            AsyncIterable, self.combinator.combine(task_name, token)
+                            AsyncIterable,
+                            self.combinator.combine(task_name, token),
                         ):
+                            ins = [id for t in schema.values() for id in t["input_ids"]]
                             for port_name, token in schema.items():
                                 self.get_output_port(port_name).put(
                                     await self._persist_token(
-                                        token=token,
+                                        token=token["token"],
                                         port=self.get_output_port(port_name),
-                                        inputs=schema.values(),
+                                        input_token_ids=ins,
                                     )
                                 )
+
                     # Create a new task in place of the completed one if the port is not terminated
                     if task_name not in terminated:
                         input_tasks.append(
                             asyncio.create_task(
                                 self.get_input_ports()[task_name].get(
                                     posixpath.join(self.name, task_name)
                                 ),
@@ -456,31 +510,31 @@
                             inputs_map.pop(tag)
                             # Deploy the target
                             await self.workflow.context.deployment_manager.deploy(
                                 self.deployment_config
                             )
                             # Propagate the connector in the output port
                             self.get_output_port().put(
-                                await self._persist_token(
+                                await self.persist_token(
                                     token=Token(value=self.deployment_config.name),
                                     port=self.get_output_port(),
-                                    inputs=inputs.values(),
+                                    inputs=_get_token_ids(inputs.values()),
                                 )
                             )
             else:
                 # Deploy the target
                 await self.workflow.context.deployment_manager.deploy(
                     self.deployment_config
                 )
                 # Propagate the connector in the output port
                 self.get_output_port().put(
                     await self._persist_token(
                         token=Token(value=self.deployment_config.name),
                         port=self.get_output_port(),
-                        inputs=[],
+                        input_token_ids=[],
                     )
                 )
             await self.terminate(Status.COMPLETED)
         # When receiving a KeyboardInterrupt, propagate it (to allow debugging)
         except KeyboardInterrupt:
             raise
         # When receiving a CancelledError, mark the step as Cancelled
@@ -547,15 +601,24 @@
         if (
             token := await self.output_processors[output_name].process(
                 job, command_output, connector
             )
         ) is not None:
             output_port.put(
                 await self._persist_token(
-                    token=token, port=output_port, inputs=job.inputs.values()
+                    token=token,
+                    port=output_port,
+                    input_token_ids=_get_token_ids(
+                        list(job.inputs.values())
+                        + [
+                            get_job_token(
+                                job.name, self.get_input_port("__job__").token_list
+                            )
+                        ]
+                    ),
                 )
             )
 
     async def _run_job(
         self,
         job: Job,
         inputs: MutableMapping[str, Token],
@@ -826,15 +889,15 @@
                 for tag, tokens in self.token_map.items():
                     output_port.put(
                         await self._persist_token(
                             token=ListToken(
                                 tag=tag, value=sorted(tokens, key=lambda cur: cur.tag)
                             ),
                             port=output_port,
-                            inputs=tokens,
+                            input_token_ids=_get_token_ids(tokens),
                         )
                     )
                 break
             else:
                 if logger.isEnabledFor(logging.DEBUG):
                     logger.debug(f"Step {self.name} received input {token.tag}")
                 key = ".".join(token.tag.split(".")[: -self.depth])
@@ -911,20 +974,28 @@
                 # Check for termination
                 if check_termination(token) or job is None:
                     break
                 try:
                     await self.workflow.context.scheduler.notify_status(
                         job.name, Status.RUNNING
                     )
+                    in_list = [
+                        get_job_token(
+                            job.name, self.get_input_port("__job__").token_list
+                        )
+                    ]
+                    # if token.persistent is none it means it comes from the dataset
+                    if token.persistent_id:
+                        in_list.append(token)
                     # Process value and inject token in the output port
                     self.get_output_port().put(
                         await self._persist_token(
                             token=await self.process_input(job, token.value),
                             port=self.get_output_port(),
-                            inputs=[token],
+                            input_token_ids=_get_token_ids(in_list),
                         )
                     )
                 finally:
                     # Notify completion to scheduler
                     await self.workflow.context.scheduler.notify_status(
                         job.name, Status.COMPLETED
                     )
@@ -989,23 +1060,26 @@
                         if (
                             ".".join(token.tag.split(".")[:-1])
                             not in self.iteration_terminaton_checklist[task_name]
                         ):
                             self.iteration_terminaton_checklist[task_name].add(
                                 token.tag
                             )
+
                         async for schema in cast(
-                            AsyncIterable, self.combinator.combine(task_name, token)
+                            AsyncIterable,
+                            self.combinator.combine(task_name, token),
                         ):
+                            ins = [id for t in schema.values() for id in t["input_ids"]]
                             for port_name, token in schema.items():
                                 self.get_output_port(port_name).put(
                                     await self._persist_token(
-                                        token=token,
+                                        token=token["token"],
                                         port=self.get_output_port(port_name),
-                                        inputs=schema.values(),
+                                        input_token_ids=ins,
                                     )
                                 )
                     # Create a new task in place of the completed one if the port is not terminated
                     if not (
                         task_name in terminated
                         and len(self.iteration_terminaton_checklist[task_name]) == 0
                     ):
@@ -1066,15 +1140,15 @@
             # If a TerminationToken is received, terminate the step
             if check_termination(token):
                 if logger.isEnabledFor(logging.DEBUG):
                     logger.debug(f"Step {self.name} received termination token")
                 # If no iterations have been performed, just terminate
                 if not self.token_map:
                     break
-                # Otherwise, build termination map to wait for all iteration temrinations
+                # Otherwise, build termination map to wait for all iteration terminations
                 else:
                     self.termination_map = {
                         k: len(self.token_map[k]) == self.size_map.get(k, -1)
                         for k in self.token_map
                     }
             # If an IterationTerminationToken is received, process loop output for the current port
             elif check_iteration_termination(token):
@@ -1091,15 +1165,15 @@
                     self.token_map[prefix] = []
                 self.token_map[prefix].append(token)
             if len(self.token_map.get(prefix, [])) == self.size_map.get(prefix, -1):
                 self.get_output_port().put(
                     await self._persist_token(
                         token=await self._process_output(prefix),
                         port=self.get_output_port(),
-                        inputs=self.token_map.get(prefix),
+                        input_token_ids=_get_token_ids(self.token_map.get(prefix)),
                     )
                 )
             # If all iterations are terminated, terminate the step
             if self.termination_map and all(self.termination_map):
                 break
         # Terminate step
         await self.terminate(
@@ -1194,19 +1268,27 @@
             ]:
                 self.workflow.context.data_manager.register_path(
                     location=location,
                     path=directory,
                     relpath=directory,
                 )
         # Propagate job
+        token_inputs = []
+        for step_port_name in self.input_ports.keys():
+            if step_port_name in job.inputs.keys():
+                token_inputs.append(job.inputs[step_port_name])
+            else:  # other tokens from connector ports
+                for t in self.get_input_port(step_port_name).token_list:
+                    if t.persistent_id:
+                        token_inputs.append(t)
         self.get_output_port().put(
             await self._persist_token(
                 token=JobToken(value=job),
                 port=self.get_output_port(),
-                inputs=job.inputs.values(),
+                input_token_ids=_get_token_ids(token_inputs),
             )
         )
 
     async def _save_additional_params(
         self, context: StreamFlowContext
     ) -> MutableMapping[str, Any]:
         await self.get_output_port("__job__").save(context),
@@ -1342,15 +1424,15 @@
         elif isinstance(token, ListToken):
             output_port = self.get_output_port()
             for i, t in enumerate(token.value):
                 output_port.put(
                     await self._persist_token(
                         token=t.retag(token.tag + "." + str(i)),
                         port=output_port,
-                        inputs=[token],
+                        input_token_ids=_get_token_ids([token]),
                     )
                 )
         else:
             raise WorkflowDefinitionException("Scatter ports require iterable inputs")
 
     def add_input_port(self, name: str, port: Port) -> None:
         if not self.input_ports:
@@ -1452,15 +1534,25 @@
                             status = Status.COMPLETED
                             # Transfer token
                             for port_name, token in inputs.items():
                                 self.get_output_port(port_name).put(
                                     await self._persist_token(
                                         token=await self.transfer(job, token),
                                         port=self.get_output_port(port_name),
-                                        inputs=inputs.values(),
+                                        input_token_ids=_get_token_ids(
+                                            list(inputs.values())
+                                            + [
+                                                get_job_token(
+                                                    job.name,
+                                                    self.get_input_port(
+                                                        "__job__"
+                                                    ).token_list,
+                                                )
+                                            ]
+                                        ),
                                     )
                                 )
             # When receiving a KeyboardInterrupt, propagate it (to allow debugging)
             except KeyboardInterrupt:
                 raise
             # When receiving a CancelledError, mark the step as Cancelled
             except asyncio.CancelledError:
@@ -1497,36 +1589,42 @@
                         if len(inputs_map[tag]) == len(self.input_ports):
                             inputs = inputs_map.pop(tag)
                             # Check for iteration termination and propagate
                             if check_iteration_termination(inputs.values()):
                                 for port_name, token in inputs.items():
                                     self.get_output_port(port_name).put(
                                         await self._persist_token(
-                                            token=token,
+                                            token=token.update(token.value),
                                             port=self.get_output_port(port_name),
-                                            inputs=inputs.values(),
+                                            input_token_ids=_get_token_ids(
+                                                inputs.values()
+                                            ),
                                         )
                                     )
                             # Otherwise, apply transformation and propagate outputs
                             else:
                                 for port_name, token in (
                                     await self.transform(inputs)
                                 ).items():
                                     self.get_output_port(port_name).put(
                                         await self._persist_token(
                                             token=token,
                                             port=self.get_output_port(port_name),
-                                            inputs=inputs.values(),
+                                            input_token_ids=_get_token_ids(
+                                                inputs.values()
+                                            ),
                                         )
                                     )
             else:
                 for port_name, token in (await self.transform({})).items():
                     self.get_output_port(port_name).put(
                         await self._persist_token(
-                            token=token, port=self.get_output_port(port_name), inputs=[]
+                            token=token,
+                            port=self.get_output_port(port_name),
+                            input_token_ids=[],
                         )
                     )
             # Terminate step
             await self.terminate(
                 Status.SKIPPED
                 if any(p.empty() for p in self.get_output_ports().values())
                 else Status.COMPLETED
```

### Comparing `streamflow-0.2.0.dev5/streamflow/workflow/token.py` & `streamflow-0.2.0.dev6/streamflow/workflow/token.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     def __init__(self, tag: str):
         super().__init__(None, tag)
 
     def get_weight(self, context: StreamFlowContext):
         return 0
 
     def update(self, value: Any) -> Token:
-        raise NotImplementedError
+        return self.__class__(tag=self.tag)
 
     def retag(self, tag: str) -> Token:
         raise NotImplementedError
 
     @classmethod
     async def _load(
         cls,
```

### Comparing `streamflow-0.2.0.dev5/streamflow/workflow/transformer.py` & `streamflow-0.2.0.dev6/streamflow/workflow/transformer.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev5/streamflow/workflow/utils.py` & `streamflow-0.2.0.dev6/streamflow/workflow/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from __future__ import annotations
 
 from typing import MutableSequence, TYPE_CHECKING
 
+from streamflow.core.exception import WorkflowExecutionException
 from streamflow.core.workflow import Token
 from streamflow.workflow.token import (
     IterationTerminationToken,
     ListToken,
     ObjectToken,
     TerminationToken,
+    JobToken,
 )
 
 if TYPE_CHECKING:
     from typing import Any, Iterable
 
 
 def check_iteration_termination(inputs: Token | Iterable[Token]) -> bool:
@@ -40,7 +42,16 @@
         return [get_token_value(t) for t in token.value]
     elif isinstance(token, ObjectToken):
         return {k: get_token_value(v) for k, v in token.value.items()}
     elif isinstance(token.value, Token):
         return get_token_value(token.value)
     else:
         return token.value
+
+
+def get_job_token(job_name: str, token_list: MutableSequence[Token]):
+    for token in token_list:
+        if isinstance(token, JobToken) and token.value.name == job_name:
+            return token
+    raise WorkflowExecutionException(
+        f"Impossible to find job {job_name} in token_list {token_list}"
+    )
```

### Comparing `streamflow-0.2.0.dev5/streamflow.egg-info/PKG-INFO` & `streamflow-0.2.0.dev6/streamflow.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamflow
-Version: 0.2.0.dev5
+Version: 0.2.0.dev6
 Summary: StreamFlow framework
 Author-email: Iacopo Colonnelli <iacopo.colonnelli@unito.it>
 License: LGPL-3.0-or-later
 Project-URL: Homepage, https://streamflow.di.unito.it
 Project-URL: Package, https://pypi.org/project/streamflow
 Project-URL: Repository, https://github.com/alpha-unito/streamflow
 Project-URL: Docker, https://hub.docker.com/r/alphaunito/streamflow
```

### Comparing `streamflow-0.2.0.dev5/streamflow.egg-info/SOURCES.txt` & `streamflow-0.2.0.dev6/streamflow.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -84,20 +84,23 @@
 streamflow/deployment/connector/kubernetes.py
 streamflow/deployment/connector/local.py
 streamflow/deployment/connector/occam.py
 streamflow/deployment/connector/queue_manager.py
 streamflow/deployment/connector/ssh.py
 streamflow/deployment/connector/schemas/docker-compose.json
 streamflow/deployment/connector/schemas/docker.json
+streamflow/deployment/connector/schemas/flux.json
 streamflow/deployment/connector/schemas/helm3.json
 streamflow/deployment/connector/schemas/kubernetes.json
 streamflow/deployment/connector/schemas/local.json
 streamflow/deployment/connector/schemas/occam.json
+streamflow/deployment/connector/schemas/pbs.json
 streamflow/deployment/connector/schemas/queue_manager.json
 streamflow/deployment/connector/schemas/singularity.json
+streamflow/deployment/connector/schemas/slurm.json
 streamflow/deployment/connector/schemas/ssh.json
 streamflow/deployment/filter/__init__.py
 streamflow/deployment/filter/shuffle.py
 streamflow/deployment/filter/schemas/shuffle.json
 streamflow/deployment/schemas/deployment_manager.json
 streamflow/ext/__init__.py
 streamflow/ext/plugin.py
@@ -130,11 +133,13 @@
 streamflow/workflow/port.py
 streamflow/workflow/step.py
 streamflow/workflow/token.py
 streamflow/workflow/transformer.py
 streamflow/workflow/utils.py
 tests/test_cwl_loop.py
 tests/test_cwl_persistence.py
+tests/test_cwl_provenance.py
 tests/test_persistence.py
+tests/test_provenance.py
 tests/test_remotepath.py
 tests/test_scheduler.py
 tests/test_transfer.py
```

### Comparing `streamflow-0.2.0.dev5/tests/test_cwl_loop.py` & `streamflow-0.2.0.dev6/tests/test_cwl_loop.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev5/tests/test_cwl_persistence.py` & `streamflow-0.2.0.dev6/tests/test_cwl_persistence.py`

 * *Files 1% similar despite different names*

```diff
@@ -139,15 +139,15 @@
     port = workflow.create_port()
     await workflow.save(context)
     step = workflow.create_step(
         cls=ExecuteStep, name=utils.random_name(), job_port=port
     )
     step.command = CWLExpressionCommand(
         step=step,
-        expression="some js expression",
+        expression="$(some.js.expression)",
         absolute_initial_workdir_allowed=False,
         expression_lib=["a", "b"],
         full_js=False,
         initial_work_dir="/tmp/workdir",
         inplace_update=False,
     )
     await save_load_and_test(step, context)
@@ -679,15 +679,15 @@
         context=context, type="cwl", name=utils.random_name(), config={}
     )
     await workflow.save(context)
 
     step = workflow.create_step(
         cls=CWLConditionalStep,
         name=utils.random_name() + "-when",
-        expression="inputs.name.length == 10",
+        expression="$(inputs.name.length == 10)",
         expression_lib=[],  # MutableSequence[Any]
         full_js=True,
     )
     await save_load_and_test(step, context)
 
 
 @pytest.mark.asyncio
```

### Comparing `streamflow-0.2.0.dev5/tests/test_persistence.py` & `streamflow-0.2.0.dev6/tests/test_persistence.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev5/tests/test_remotepath.py` & `streamflow-0.2.0.dev6/tests/test_remotepath.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev5/tests/test_scheduler.py` & `streamflow-0.2.0.dev6/tests/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev5/tests/test_transfer.py` & `streamflow-0.2.0.dev6/tests/test_transfer.py`

 * *Files identical despite different names*

