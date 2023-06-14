# Comparing `tmp/invoke-2.1.2.tar.gz` & `tmp/invoke-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/tmp/tmpn5z_zgln/dist/invoke-2.1.2.tar", last modified: Mon May 15 22:15:29 2023, max compression
+gzip compressed data, was "/tmp/tmpwaifj4z_/dist/invoke-2.1.3.tar", last modified: Wed Jun 14 23:05:37 2023, max compression
```

## Comparing `invoke-2.1.2.tar` & `invoke-2.1.3.tar`

### file list

```diff
@@ -1,218 +1,222 @@
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-15 22:15:29.000000 invoke-2.1.2/
--rw-r--r--   0 jforcier  (1000) users      (100)     2711 2023-02-17 20:13:42.000000 invoke-2.1.2/setup.py
--rw-r--r--   0 jforcier  (1000) users      (100)     4061 2023-05-02 02:04:35.000000 invoke-2.1.2/tasks.py
--rw-r--r--   0 jforcier  (1000) users      (100)     3290 2023-05-15 22:15:29.000000 invoke-2.1.2/PKG-INFO
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-15 22:15:29.000000 invoke-2.1.2/invoke/
--rw-r--r--   0 jforcier  (1000) users      (100)     5097 2023-05-02 02:04:35.000000 invoke-2.1.2/invoke/watchers.py
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-15 22:15:29.000000 invoke-2.1.2/invoke/vendor/
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-15 22:15:29.000000 invoke-2.1.2/invoke/vendor/lexicon/
--rw-r--r--   0 jforcier  (1000) users      (100)       80 2023-02-16 19:54:15.000000 invoke-2.1.2/invoke/vendor/lexicon/_version.py
--rw-r--r--   0 jforcier  (1000) users      (100)      407 2023-02-16 19:54:15.000000 invoke-2.1.2/invoke/vendor/lexicon/attribute_dict.py
--rw-r--r--   0 jforcier  (1000) users      (100)     1133 2023-02-16 19:54:15.000000 invoke-2.1.2/invoke/vendor/lexicon/__init__.py
--rw-r--r--   0 jforcier  (1000) users      (100)     3223 2023-02-16 19:54:15.000000 invoke-2.1.2/invoke/vendor/lexicon/alias_dict.py
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-15 22:15:29.000000 invoke-2.1.2/invoke/vendor/yaml/
--rw-r--r--   0 jforcier  (1000) users      (100)     1440 2023-02-16 19:54:22.000000 invoke-2.1.2/invoke/vendor/yaml/nodes.py
--rw-r--r--   0 jforcier  (1000) users      (100)    28639 2023-02-16 19:54:15.000000 invoke-2.1.2/invoke/vendor/yaml/constructor.py
--rw-r--r--   0 jforcier  (1000) users      (100)    25495 2023-02-16 19:54:15.000000 invoke-2.1.2/invoke/vendor/yaml/parser.py
--rw-r--r--   0 jforcier  (1000) users      (100)     4165 2023-02-16 19:54:15.000000 invoke-2.1.2/invoke/vendor/yaml/serializer.py
--rw-r--r--   0 jforcier  (1000) users      (100)    51277 2023-02-16 19:54:15.000000 invoke-2.1.2/invoke/vendor/yaml/scanner.py
--rw-r--r--   0 jforcier  (1000) users      (100)     6794 2023-02-16 19:54:22.000000 invoke-2.1.2/invoke/vendor/yaml/reader.py
--rw-r--r--   0 jforcier  (1000) users      (100)    13170 2023-02-16 19:54:15.000000 invoke-2.1.2/invoke/vendor/yaml/__init__.py
--rw-r--r--   0 jforcier  (1000) users      (100)     3851 2023-02-16 19:54:15.000000 invoke-2.1.2/invoke/vendor/yaml/cyaml.py
--rw-r--r--   0 jforcier  (1000) users      (100)     4883 2023-02-16 19:54:15.000000 invoke-2.1.2/invoke/vendor/yaml/composer.py
--rw-r--r--   0 jforcier  (1000) users      (100)     2533 2023-02-16 19:54:15.000000 invoke-2.1.2/invoke/vendor/yaml/error.py
--rw-r--r--   0 jforcier  (1000) users      (100)     2837 2023-02-16 19:54:15.000000 invoke-2.1.2/invoke/vendor/yaml/dumper.py
--rw-r--r--   0 jforcier  (1000) users      (100)     8999 2023-02-16 19:54:15.000000 invoke-2.1.2/invoke/vendor/yaml/resolver.py
--rw-r--r--   0 jforcier  (1000) users      (100)    14184 2023-02-16 19:54:15.000000 invoke-2.1.2/invoke/vendor/yaml/representer.py
--rw-r--r--   0 jforcier  (1000) users      (100)    43006 2023-02-16 19:54:15.000000 invoke-2.1.2/invoke/vendor/yaml/emitter.py
--rw-r--r--   0 jforcier  (1000) users      (100)     2061 2023-02-16 19:54:15.000000 invoke-2.1.2/invoke/vendor/yaml/loader.py
--rw-r--r--   0 jforcier  (1000) users      (100)     2573 2023-02-16 19:54:22.000000 invoke-2.1.2/invoke/vendor/yaml/tokens.py
--rw-r--r--   0 jforcier  (1000) users      (100)     2445 2023-02-16 19:54:22.000000 invoke-2.1.2/invoke/vendor/yaml/events.py
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-15 22:15:29.000000 invoke-2.1.2/invoke/vendor/fluidity/
--rw-r--r--   0 jforcier  (1000) users      (100)      196 2023-02-16 19:54:15.000000 invoke-2.1.2/invoke/vendor/fluidity/__init__.py
--rw-r--r--   0 jforcier  (1000) users      (100)     8686 2023-02-16 19:54:22.000000 invoke-2.1.2/invoke/vendor/fluidity/machine.py
--rw-r--r--   0 jforcier  (1000) users      (100)      135 2023-02-16 19:54:15.000000 invoke-2.1.2/invoke/vendor/fluidity/backwardscompat.py
--rw-r--r--   0 jforcier  (1000) users      (100)        0 2023-02-16 19:54:15.000000 invoke-2.1.2/invoke/vendor/__init__.py
--rw-r--r--   0 jforcier  (1000) users      (100)     2229 2023-05-02 02:04:35.000000 invoke-2.1.2/invoke/__init__.py
--rw-r--r--   0 jforcier  (1000) users      (100)     8855 2023-05-02 02:04:35.000000 invoke-2.1.2/invoke/executor.py
--rw-r--r--   0 jforcier  (1000) users      (100)      235 2023-02-16 19:54:15.000000 invoke-2.1.2/invoke/main.py
--rw-r--r--   0 jforcier  (1000) users      (100)    10018 2023-05-02 02:04:35.000000 invoke-2.1.2/invoke/util.py
--rw-r--r--   0 jforcier  (1000) users      (100)    50005 2023-05-02 02:04:35.000000 invoke-2.1.2/invoke/config.py
--rw-r--r--   0 jforcier  (1000) users      (100)     4394 2023-05-02 02:04:35.000000 invoke-2.1.2/invoke/env.py
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-15 22:15:29.000000 invoke-2.1.2/invoke/parser/
--rw-r--r--   0 jforcier  (1000) users      (100)     6045 2023-05-02 02:04:35.000000 invoke-2.1.2/invoke/parser/argument.py
--rw-r--r--   0 jforcier  (1000) users      (100)    19809 2023-05-02 02:04:35.000000 invoke-2.1.2/invoke/parser/parser.py
--rw-r--r--   0 jforcier  (1000) users      (100)     9815 2023-05-02 02:04:35.000000 invoke-2.1.2/invoke/parser/context.py
--rw-r--r--   0 jforcier  (1000) users      (100)      181 2023-02-16 19:54:15.000000 invoke-2.1.2/invoke/parser/__init__.py
--rw-r--r--   0 jforcier  (1000) users      (100)       80 2023-05-15 22:15:28.000000 invoke-2.1.2/invoke/_version.py
--rw-r--r--   0 jforcier  (1000) users      (100)    65509 2023-05-12 19:29:07.000000 invoke-2.1.2/invoke/runners.py
--rw-r--r--   0 jforcier  (1000) users      (100)    38177 2023-05-12 19:55:50.000000 invoke-2.1.2/invoke/program.py
--rw-r--r--   0 jforcier  (1000) users      (100)    25486 2023-05-02 02:04:35.000000 invoke-2.1.2/invoke/context.py
--rw-r--r--   0 jforcier  (1000) users      (100)       47 2023-02-16 19:54:15.000000 invoke-2.1.2/invoke/__main__.py
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-15 22:15:29.000000 invoke-2.1.2/invoke/completion/
--rw-r--r--   0 jforcier  (1000) users      (100)     1429 2021-12-23 21:30:34.000000 invoke-2.1.2/invoke/completion/zsh.completion
--rw-r--r--   0 jforcier  (1000) users      (100)     1356 2021-12-23 21:30:34.000000 invoke-2.1.2/invoke/completion/bash.completion
--rw-r--r--   0 jforcier  (1000) users      (100)        0 2023-02-16 19:54:15.000000 invoke-2.1.2/invoke/completion/__init__.py
--rw-r--r--   0 jforcier  (1000) users      (100)     5222 2023-05-02 02:04:35.000000 invoke-2.1.2/invoke/completion/complete.py
--rw-r--r--   0 jforcier  (1000) users      (100)      382 2021-12-23 21:30:34.000000 invoke-2.1.2/invoke/completion/fish.completion
--rw-r--r--   0 jforcier  (1000) users      (100)     8065 2023-05-02 02:04:35.000000 invoke-2.1.2/invoke/terminals.py
--rw-r--r--   0 jforcier  (1000) users      (100)     5305 2023-05-02 02:12:54.000000 invoke-2.1.2/invoke/loader.py
--rw-r--r--   0 jforcier  (1000) users      (100)    12227 2023-05-02 02:04:35.000000 invoke-2.1.2/invoke/exceptions.py
--rw-r--r--   0 jforcier  (1000) users      (100)        0 2023-05-12 22:23:53.000000 invoke-2.1.2/invoke/py.typed
--rw-r--r--   0 jforcier  (1000) users      (100)    23060 2023-05-02 02:04:35.000000 invoke-2.1.2/invoke/collection.py
--rw-r--r--   0 jforcier  (1000) users      (100)    19946 2023-05-02 02:04:35.000000 invoke-2.1.2/invoke/tasks.py
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-15 22:15:29.000000 invoke-2.1.2/sites/
--rw-r--r--   0 jforcier  (1000) users      (100)     1367 2023-02-16 19:54:15.000000 invoke-2.1.2/sites/shared_conf.py
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-15 22:15:29.000000 invoke-2.1.2/sites/www/
--rw-r--r--   0 jforcier  (1000) users      (100)    77308 2023-05-15 22:15:26.000000 invoke-2.1.2/sites/www/changelog.rst
--rw-r--r--   0 jforcier  (1000) users      (100)     8153 2023-01-07 00:40:50.000000 invoke-2.1.2/sites/www/faq.rst
--rw-r--r--   0 jforcier  (1000) users      (100)      703 2023-02-16 19:54:15.000000 invoke-2.1.2/sites/www/conf.py
--rw-r--r--   0 jforcier  (1000) users      (100)     1791 2022-05-11 15:59:13.000000 invoke-2.1.2/sites/www/development.rst
--rw-r--r--   0 jforcier  (1000) users      (100)     2537 2022-03-25 22:40:47.000000 invoke-2.1.2/sites/www/prior-art.rst
--rw-r--r--   0 jforcier  (1000) users      (100)      753 2023-01-07 00:40:50.000000 invoke-2.1.2/sites/www/installing.rst
--rw-r--r--   0 jforcier  (1000) users      (100)     1218 2022-05-11 15:59:13.000000 invoke-2.1.2/sites/www/contact.rst
--rw-r--r--   0 jforcier  (1000) users      (100)     2801 2022-05-11 15:59:13.000000 invoke-2.1.2/sites/www/index.rst
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-15 22:15:29.000000 invoke-2.1.2/sites/docs/
--rw-r--r--   0 jforcier  (1000) users      (100)      943 2022-05-11 15:59:13.000000 invoke-2.1.2/sites/docs/index.rst
--rw-r--r--   0 jforcier  (1000) users      (100)     7640 2022-05-11 15:59:13.000000 invoke-2.1.2/sites/docs/getting-started.rst
--rw-r--r--   0 jforcier  (1000) users      (100)      445 2023-02-16 19:54:15.000000 invoke-2.1.2/sites/docs/conf.py
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-15 22:15:29.000000 invoke-2.1.2/sites/docs/api/
--rw-r--r--   0 jforcier  (1000) users      (100)      401 2023-01-12 23:12:21.000000 invoke-2.1.2/sites/docs/api/parser.rst
--rw-r--r--   0 jforcier  (1000) users      (100)       64 2022-03-25 22:40:47.000000 invoke-2.1.2/sites/docs/api/config.rst
--rw-r--r--   0 jforcier  (1000) users      (100)      156 2022-03-25 22:40:47.000000 invoke-2.1.2/sites/docs/api/collection.rst
--rw-r--r--   0 jforcier  (1000) users      (100)       63 2022-03-25 22:40:47.000000 invoke-2.1.2/sites/docs/api/__init__.rst
--rw-r--r--   0 jforcier  (1000) users      (100)      229 2022-03-25 22:40:47.000000 invoke-2.1.2/sites/docs/api/loader.rst
--rw-r--r--   0 jforcier  (1000) users      (100)       68 2022-03-25 22:40:47.000000 invoke-2.1.2/sites/docs/api/context.rst
--rw-r--r--   0 jforcier  (1000) users      (100)       76 2022-03-25 22:40:47.000000 invoke-2.1.2/sites/docs/api/terminals.rst
--rw-r--r--   0 jforcier  (1000) users      (100)       80 2022-03-25 22:40:47.000000 invoke-2.1.2/sites/docs/api/executor.rst
--rw-r--r--   0 jforcier  (1000) users      (100)       60 2022-03-25 22:40:47.000000 invoke-2.1.2/sites/docs/api/tasks.rst
--rw-r--r--   0 jforcier  (1000) users      (100)       72 2022-03-25 22:40:47.000000 invoke-2.1.2/sites/docs/api/watchers.rst
--rw-r--r--   0 jforcier  (1000) users      (100)       96 2022-03-25 22:40:47.000000 invoke-2.1.2/sites/docs/api/runners.rst
--rw-r--r--   0 jforcier  (1000) users      (100)       80 2022-03-25 22:40:47.000000 invoke-2.1.2/sites/docs/api/exceptions.rst
--rw-r--r--   0 jforcier  (1000) users      (100)      157 2022-03-25 22:40:47.000000 invoke-2.1.2/sites/docs/api/util.rst
--rw-r--r--   0 jforcier  (1000) users      (100)       68 2022-03-25 22:40:47.000000 invoke-2.1.2/sites/docs/api/program.rst
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-15 22:15:29.000000 invoke-2.1.2/sites/docs/_static/
--rw-r--r--   0 jforcier  (1000) users      (100)    15260 2021-12-23 21:30:34.000000 invoke-2.1.2/sites/docs/_static/rtd.css
--rw-r--r--   0 jforcier  (1000) users      (100)    12466 2022-05-11 15:59:13.000000 invoke-2.1.2/sites/docs/invoke.rst
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-15 22:15:29.000000 invoke-2.1.2/sites/docs/concepts/
--rw-r--r--   0 jforcier  (1000) users      (100)    11750 2022-03-25 22:40:47.000000 invoke-2.1.2/sites/docs/concepts/namespaces.rst
--rw-r--r--   0 jforcier  (1000) users      (100)     2917 2022-05-11 15:59:13.000000 invoke-2.1.2/sites/docs/concepts/loading.rst
--rw-r--r--   0 jforcier  (1000) users      (100)    17701 2023-01-07 00:40:50.000000 invoke-2.1.2/sites/docs/concepts/configuration.rst
--rw-r--r--   0 jforcier  (1000) users      (100)    10180 2023-01-07 00:40:50.000000 invoke-2.1.2/sites/docs/concepts/testing.rst
--rw-r--r--   0 jforcier  (1000) users      (100)     9234 2023-02-17 20:13:42.000000 invoke-2.1.2/sites/docs/concepts/library.rst
--rw-r--r--   0 jforcier  (1000) users      (100)     2424 2022-03-25 22:40:47.000000 invoke-2.1.2/sites/docs/concepts/watchers.rst
--rw-r--r--   0 jforcier  (1000) users      (100)    16705 2023-01-07 00:40:53.000000 invoke-2.1.2/sites/docs/concepts/invoking-tasks.rst
--rw-r--r--   0 jforcier  (1000) users      (100)      302 2023-05-15 22:15:04.000000 invoke-2.1.2/MANIFEST.in
--rw-r--r--   0 jforcier  (1000) users      (100)     1314 2021-12-23 21:30:34.000000 invoke-2.1.2/LICENSE
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-15 22:15:29.000000 invoke-2.1.2/tests/
--rw-r--r--   0 jforcier  (1000) users      (100)    44633 2023-02-17 20:13:42.000000 invoke-2.1.2/tests/config.py
--rw-r--r--   0 jforcier  (1000) users      (100)    17268 2023-02-17 20:13:42.000000 invoke-2.1.2/tests/task.py
--rw-r--r--   0 jforcier  (1000) users      (100)     9820 2023-02-17 20:13:42.000000 invoke-2.1.2/tests/_util.py
--rw-r--r--   0 jforcier  (1000) users      (100)     2945 2023-02-16 19:54:15.000000 invoke-2.1.2/tests/terminals.py
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-15 22:15:29.000000 invoke-2.1.2/tests/_support/
--rw-r--r--   0 jforcier  (1000) users      (100)      194 2023-02-16 19:54:15.000000 invoke-2.1.2/tests/_support/deeper_ns_list.py
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-15 22:15:29.000000 invoke-2.1.2/tests/_support/configs/
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-15 22:15:29.000000 invoke-2.1.2/tests/_support/configs/json/
--rw-r--r--   0 jforcier  (1000) users      (100)       41 2021-12-23 21:30:34.000000 invoke-2.1.2/tests/_support/configs/json/invoke.json
--rw-r--r--   0 jforcier  (1000) users      (100)       23 2021-12-23 21:30:34.000000 invoke-2.1.2/tests/_support/configs/no-dedupe.yaml
--rw-r--r--   0 jforcier  (1000) users      (100)       89 2023-02-16 19:54:15.000000 invoke-2.1.2/tests/_support/configs/runtime.py
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-15 22:15:29.000000 invoke-2.1.2/tests/_support/configs/json-and-python/
--rw-r--r--   0 jforcier  (1000) users      (100)       44 2023-02-16 19:54:15.000000 invoke-2.1.2/tests/_support/configs/json-and-python/invoke.py
--rw-r--r--   0 jforcier  (1000) users      (100)       46 2021-12-23 21:30:34.000000 invoke-2.1.2/tests/_support/configs/json-and-python/invoke.json
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-15 22:15:29.000000 invoke-2.1.2/tests/_support/configs/three-of-em/
--rw-r--r--   0 jforcier  (1000) users      (100)       46 2021-12-23 21:30:34.000000 invoke-2.1.2/tests/_support/configs/three-of-em/invoke.json
--rw-r--r--   0 jforcier  (1000) users      (100)       38 2021-12-23 21:30:34.000000 invoke-2.1.2/tests/_support/configs/three-of-em/invoke.yml
--rw-r--r--   0 jforcier  (1000) users      (100)       44 2023-02-16 19:54:15.000000 invoke-2.1.2/tests/_support/configs/three-of-em/invoke.py
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-15 22:15:29.000000 invoke-2.1.2/tests/_support/configs/python/
--rw-r--r--   0 jforcier  (1000) users      (100)       40 2023-02-16 19:54:15.000000 invoke-2.1.2/tests/_support/configs/python/invoke.py
--rw-r--r--   0 jforcier  (1000) users      (100)       18 2021-12-23 21:30:34.000000 invoke-2.1.2/tests/_support/configs/echo.yaml
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-15 22:15:29.000000 invoke-2.1.2/tests/_support/configs/nested/
--rw-r--r--   0 jforcier  (1000) users      (100)       35 2021-12-23 21:30:34.000000 invoke-2.1.2/tests/_support/configs/nested/invoke.yaml
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-15 22:15:29.000000 invoke-2.1.2/tests/_support/configs/yaml/
--rw-r--r--   0 jforcier  (1000) users      (100)      127 2023-02-16 19:54:15.000000 invoke-2.1.2/tests/_support/configs/yaml/explicit.py
--rw-r--r--   0 jforcier  (1000) users      (100)       89 2023-02-16 19:54:15.000000 invoke-2.1.2/tests/_support/configs/yaml/tasks.py
--rw-r--r--   0 jforcier  (1000) users      (100)       35 2021-12-23 21:30:34.000000 invoke-2.1.2/tests/_support/configs/yaml/invoke.yaml
--rw-r--r--   0 jforcier  (1000) users      (100)       19 2021-12-23 21:30:34.000000 invoke-2.1.2/tests/_support/configs/no-echo.yaml
--rw-r--r--   0 jforcier  (1000) users      (100)      173 2023-02-16 19:54:15.000000 invoke-2.1.2/tests/_support/configs/collection.py
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-15 22:15:29.000000 invoke-2.1.2/tests/_support/configs/underscores/
--rw-r--r--   0 jforcier  (1000) users      (100)       68 2023-02-16 19:54:15.000000 invoke-2.1.2/tests/_support/configs/underscores/tasks.py
--rw-r--r--   0 jforcier  (1000) users      (100)       32 2021-12-23 21:30:34.000000 invoke-2.1.2/tests/_support/configs/underscores/invoke.yaml
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-15 22:15:29.000000 invoke-2.1.2/tests/_support/configs/yml/
--rw-r--r--   0 jforcier  (1000) users      (100)       34 2021-12-23 21:30:34.000000 invoke-2.1.2/tests/_support/configs/yml/invoke.yml
--rw-r--r--   0 jforcier  (1000) users      (100)      126 2023-02-16 19:54:15.000000 invoke-2.1.2/tests/_support/configs/yml/explicit.py
--rw-r--r--   0 jforcier  (1000) users      (100)       88 2023-02-16 19:54:15.000000 invoke-2.1.2/tests/_support/configs/yml/tasks.py
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-15 22:15:29.000000 invoke-2.1.2/tests/_support/configs/all-four/
--rw-r--r--   0 jforcier  (1000) users      (100)       46 2021-12-23 21:30:34.000000 invoke-2.1.2/tests/_support/configs/all-four/invoke.json
--rw-r--r--   0 jforcier  (1000) users      (100)       44 2023-02-16 19:54:15.000000 invoke-2.1.2/tests/_support/configs/all-four/invoke.py
--rw-r--r--   0 jforcier  (1000) users      (100)       40 2021-12-23 21:30:34.000000 invoke-2.1.2/tests/_support/configs/all-four/invoke.yaml
--rw-r--r--   0 jforcier  (1000) users      (100)       38 2021-12-23 21:30:34.000000 invoke-2.1.2/tests/_support/configs/all-four/invoke.yml
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-15 22:15:29.000000 invoke-2.1.2/tests/_support/branch/
--rw-r--r--   0 jforcier  (1000) users      (100)       73 2023-02-16 19:54:15.000000 invoke-2.1.2/tests/_support/branch/explicit.py
--rw-r--r--   0 jforcier  (1000) users      (100)       86 2023-02-16 19:54:15.000000 invoke-2.1.2/tests/_support/branch/tasks.py
--rw-r--r--   0 jforcier  (1000) users      (100)     4146 2021-12-23 21:30:34.000000 invoke-2.1.2/tests/_support/tree.json
--rw-r--r--   0 jforcier  (1000) users      (100)      116 2023-02-16 19:54:15.000000 invoke-2.1.2/tests/_support/decorator_multi_default.py
--rw-r--r--   0 jforcier  (1000) users      (100)       35 2023-02-16 19:54:15.000000 invoke-2.1.2/tests/_support/has_modules.py
--rw-r--r--   0 jforcier  (1000) users      (100)      178 2023-02-16 19:54:15.000000 invoke-2.1.2/tests/_support/simple_ns_list.py
--rw-r--r--   0 jforcier  (1000) users      (100)      121 2023-02-16 19:54:15.000000 invoke-2.1.2/tests/_support/empty_subcollection.py
--rw-r--r--   0 jforcier  (1000) users      (100)      264 2023-02-16 19:54:15.000000 invoke-2.1.2/tests/_support/explicit_root.py
--rw-r--r--   0 jforcier  (1000) users      (100)       44 2023-02-16 19:54:15.000000 invoke-2.1.2/tests/_support/oops.py
--rw-r--r--   0 jforcier  (1000) users      (100)      511 2023-02-16 19:54:15.000000 invoke-2.1.2/tests/_support/depth_first.py
--rw-r--r--   0 jforcier  (1000) users      (100)       96 2023-02-16 19:54:15.000000 invoke-2.1.2/tests/_support/tasks.py
--rw-r--r--   0 jforcier  (1000) users      (100)       57 2023-02-16 19:54:15.000000 invoke-2.1.2/tests/_support/custom_executor.py
--rw-r--r--   0 jforcier  (1000) users      (100)      189 2023-05-02 02:12:54.000000 invoke-2.1.2/tests/_support/namespacing.py
--rw-r--r--   0 jforcier  (1000) users      (100)      666 2023-02-16 19:54:15.000000 invoke-2.1.2/tests/_support/integration.py
--rw-r--r--   0 jforcier  (1000) users      (100)       99 2023-02-16 19:54:15.000000 invoke-2.1.2/tests/_support/debugging.py
--rw-r--r--   0 jforcier  (1000) users      (100)       85 2023-02-16 19:54:15.000000 invoke-2.1.2/tests/_support/subcollection_task_name.py
--rw-r--r--   0 jforcier  (1000) users      (100)        7 2023-02-16 19:54:15.000000 invoke-2.1.2/tests/_support/empty.py
--rw-r--r--   0 jforcier  (1000) users      (100)      395 2023-02-16 19:54:15.000000 invoke-2.1.2/tests/_support/contextualized.py
--rw-r--r--   0 jforcier  (1000) users      (100)      226 2023-02-16 19:54:15.000000 invoke-2.1.2/tests/_support/foo.py
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-15 22:15:29.000000 invoke-2.1.2/tests/_support/subspace/
--rw-r--r--   0 jforcier  (1000) users      (100)       77 2023-05-02 02:12:54.000000 invoke-2.1.2/tests/_support/subspace/__init__.py
--rw-r--r--   0 jforcier  (1000) users      (100)       56 2023-05-02 02:12:54.000000 invoke-2.1.2/tests/_support/subspace/module.py
--rw-r--r--   0 jforcier  (1000) users      (100)      157 2023-02-16 19:54:15.000000 invoke-2.1.2/tests/_support/sudo_prompt.py
--rw-r--r--   0 jforcier  (1000) users      (100)      365 2023-02-16 19:54:15.000000 invoke-2.1.2/tests/_support/autoprint.py
--rw-r--r--   0 jforcier  (1000) users      (100)      425 2023-02-16 19:54:15.000000 invoke-2.1.2/tests/_support/nontrivial_docstrings.py
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-15 22:15:29.000000 invoke-2.1.2/tests/_support/tree/
--rw-r--r--   0 jforcier  (1000) users      (100)      653 2023-02-16 19:54:15.000000 invoke-2.1.2/tests/_support/tree/__init__.py
--rw-r--r--   0 jforcier  (1000) users      (100)      171 2023-02-16 19:54:15.000000 invoke-2.1.2/tests/_support/tree/provision.py
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-15 22:15:29.000000 invoke-2.1.2/tests/_support/tree/build/
--rw-r--r--   0 jforcier  (1000) users      (100)      278 2023-02-16 19:54:15.000000 invoke-2.1.2/tests/_support/tree/build/python.py
--rw-r--r--   0 jforcier  (1000) users      (100)      421 2023-02-16 19:54:15.000000 invoke-2.1.2/tests/_support/tree/build/__init__.py
--rw-r--r--   0 jforcier  (1000) users      (100)      274 2023-02-16 19:54:15.000000 invoke-2.1.2/tests/_support/tree/build/docs.py
--rw-r--r--   0 jforcier  (1000) users      (100)      301 2023-02-16 19:54:15.000000 invoke-2.1.2/tests/_support/tree/deploy.py
--rw-r--r--   0 jforcier  (1000) users      (100)      919 2023-02-16 19:54:15.000000 invoke-2.1.2/tests/_support/decorators.py
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-15 22:15:29.000000 invoke-2.1.2/tests/_support/ignoreme/
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-15 22:15:29.000000 invoke-2.1.2/tests/_support/ignoreme/ignoremetoo/
--rw-r--r--   0 jforcier  (1000) users      (100)        0 2021-12-23 21:30:34.000000 invoke-2.1.2/tests/_support/ignoreme/ignoremetoo/.no
--rw-r--r--   0 jforcier  (1000) users      (100)      276 2023-02-16 19:54:15.000000 invoke-2.1.2/tests/_support/docstrings.py
--rw-r--r--   0 jforcier  (1000) users      (100)       78 2023-02-16 19:54:15.000000 invoke-2.1.2/tests/_support/alias_sorting.py
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-15 22:15:29.000000 invoke-2.1.2/tests/_support/package/
--rw-r--r--   0 jforcier  (1000) users      (100)       56 2023-02-16 19:54:15.000000 invoke-2.1.2/tests/_support/package/module.py
--rw-r--r--   0 jforcier  (1000) users      (100)       77 2023-05-02 02:12:54.000000 invoke-2.1.2/tests/_support/package/__init__.py
--rw-r--r--   0 jforcier  (1000) users      (100)     7179 2023-02-16 19:54:15.000000 invoke-2.1.2/tests/parser_argument.py
--rw-r--r--   0 jforcier  (1000) users      (100)     1661 2023-02-17 20:13:42.000000 invoke-2.1.2/tests/util.py
--rw-r--r--   0 jforcier  (1000) users      (100)    33509 2023-02-17 20:13:42.000000 invoke-2.1.2/tests/collection.py
--rw-r--r--   0 jforcier  (1000) users      (100)     4550 2023-02-16 19:54:15.000000 invoke-2.1.2/tests/merge_dicts.py
--rw-r--r--   0 jforcier  (1000) users      (100)    12415 2023-02-16 19:54:15.000000 invoke-2.1.2/tests/executor.py
--rw-r--r--   0 jforcier  (1000) users      (100)    22668 2023-02-16 19:54:15.000000 invoke-2.1.2/tests/parser_parser.py
--rw-r--r--   0 jforcier  (1000) users      (100)     4371 2023-05-02 02:12:54.000000 invoke-2.1.2/tests/loader.py
--rw-r--r--   0 jforcier  (1000) users      (100)    70584 2023-05-02 02:12:54.000000 invoke-2.1.2/tests/runners.py
--rw-r--r--   0 jforcier  (1000) users      (100)     4239 2023-02-16 19:54:15.000000 invoke-2.1.2/tests/watchers.py
--rw-r--r--   0 jforcier  (1000) users      (100)     3261 2023-02-17 20:13:42.000000 invoke-2.1.2/tests/concurrency.py
--rw-r--r--   0 jforcier  (1000) users      (100)    29680 2023-02-17 20:13:42.000000 invoke-2.1.2/tests/context.py
--rw-r--r--   0 jforcier  (1000) users      (100)     4053 2023-02-16 19:54:15.000000 invoke-2.1.2/tests/init.py
--rw-r--r--   0 jforcier  (1000) users      (100)     2895 2023-02-16 19:54:15.000000 invoke-2.1.2/tests/conftest.py
--rw-r--r--   0 jforcier  (1000) users      (100)    12116 2023-02-16 19:54:15.000000 invoke-2.1.2/tests/parser_context.py
--rw-r--r--   0 jforcier  (1000) users      (100)    56042 2023-04-28 19:58:26.000000 invoke-2.1.2/tests/program.py
--rw-r--r--   0 jforcier  (1000) users      (100)     7687 2023-02-17 20:13:42.000000 invoke-2.1.2/tests/completion.py
--rw-r--r--   0 jforcier  (1000) users      (100)     5361 2023-02-16 19:54:15.000000 invoke-2.1.2/tests/cli.py
--rw-r--r--   0 jforcier  (1000) users      (100)     1328 2022-05-11 15:59:13.000000 invoke-2.1.2/README.rst
--rw-r--r--   0 jforcier  (1000) users      (100)      435 2023-05-15 22:04:31.000000 invoke-2.1.2/dev-requirements.txt
--rw-r--r--   0 jforcier  (1000) users      (100)     1250 2023-05-02 02:04:35.000000 invoke-2.1.2/pyproject.toml
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-15 22:15:29.000000 invoke-2.1.2/invoke.egg-info/
--rw-r--r--   0 jforcier  (1000) users      (100)     5152 2023-05-15 22:15:29.000000 invoke-2.1.2/invoke.egg-info/SOURCES.txt
--rw-r--r--   0 jforcier  (1000) users      (100)        7 2023-05-15 22:15:29.000000 invoke-2.1.2/invoke.egg-info/top_level.txt
--rw-r--r--   0 jforcier  (1000) users      (100)        1 2023-05-15 22:15:29.000000 invoke-2.1.2/invoke.egg-info/dependency_links.txt
--rw-r--r--   0 jforcier  (1000) users      (100)       82 2023-05-15 22:15:29.000000 invoke-2.1.2/invoke.egg-info/entry_points.txt
--rw-r--r--   0 jforcier  (1000) users      (100)     3290 2023-05-15 22:15:29.000000 invoke-2.1.2/invoke.egg-info/PKG-INFO
--rw-r--r--   0 jforcier  (1000) users      (100)       38 2023-05-15 22:15:29.000000 invoke-2.1.2/setup.cfg
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-06-14 23:05:37.000000 invoke-2.1.3/
+-rw-r--r--   0 jforcier  (1000) users      (100)     1314 2021-12-23 21:30:34.000000 invoke-2.1.3/LICENSE
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-06-14 23:05:37.000000 invoke-2.1.3/tests/
+-rw-r--r--   0 jforcier  (1000) users      (100)     4432 2023-06-14 23:05:06.000000 invoke-2.1.3/tests/loader.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     4239 2023-02-16 19:54:15.000000 invoke-2.1.3/tests/watchers.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    12116 2023-02-16 19:54:15.000000 invoke-2.1.3/tests/parser_context.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    12415 2023-02-16 19:54:15.000000 invoke-2.1.3/tests/executor.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    33509 2023-02-17 20:13:42.000000 invoke-2.1.3/tests/collection.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    70584 2023-05-02 02:12:54.000000 invoke-2.1.3/tests/runners.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     2895 2023-02-16 19:54:15.000000 invoke-2.1.3/tests/conftest.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    56287 2023-06-14 23:05:06.000000 invoke-2.1.3/tests/program.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    29680 2023-02-17 20:13:42.000000 invoke-2.1.3/tests/context.py
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-06-14 23:05:37.000000 invoke-2.1.3/tests/_support/
+-rw-r--r--   0 jforcier  (1000) users      (100)      116 2023-02-16 19:54:15.000000 invoke-2.1.3/tests/_support/decorator_multi_default.py
+-rw-r--r--   0 jforcier  (1000) users      (100)       99 2023-02-16 19:54:15.000000 invoke-2.1.3/tests/_support/debugging.py
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-06-14 23:05:37.000000 invoke-2.1.3/tests/_support/configs/
+-rw-r--r--   0 jforcier  (1000) users      (100)       23 2021-12-23 21:30:34.000000 invoke-2.1.3/tests/_support/configs/no-dedupe.yaml
+-rw-r--r--   0 jforcier  (1000) users      (100)       89 2023-02-16 19:54:15.000000 invoke-2.1.3/tests/_support/configs/runtime.py
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-06-14 23:05:37.000000 invoke-2.1.3/tests/_support/configs/json/
+-rw-r--r--   0 jforcier  (1000) users      (100)       41 2021-12-23 21:30:34.000000 invoke-2.1.3/tests/_support/configs/json/invoke.json
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-06-14 23:05:37.000000 invoke-2.1.3/tests/_support/configs/three-of-em/
+-rw-r--r--   0 jforcier  (1000) users      (100)       46 2021-12-23 21:30:34.000000 invoke-2.1.3/tests/_support/configs/three-of-em/invoke.json
+-rw-r--r--   0 jforcier  (1000) users      (100)       44 2023-02-16 19:54:15.000000 invoke-2.1.3/tests/_support/configs/three-of-em/invoke.py
+-rw-r--r--   0 jforcier  (1000) users      (100)       38 2021-12-23 21:30:34.000000 invoke-2.1.3/tests/_support/configs/three-of-em/invoke.yml
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-06-14 23:05:37.000000 invoke-2.1.3/tests/_support/configs/json-and-python/
+-rw-r--r--   0 jforcier  (1000) users      (100)       44 2023-02-16 19:54:15.000000 invoke-2.1.3/tests/_support/configs/json-and-python/invoke.py
+-rw-r--r--   0 jforcier  (1000) users      (100)       46 2021-12-23 21:30:34.000000 invoke-2.1.3/tests/_support/configs/json-and-python/invoke.json
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-06-14 23:05:37.000000 invoke-2.1.3/tests/_support/configs/yml/
+-rw-r--r--   0 jforcier  (1000) users      (100)       88 2023-02-16 19:54:15.000000 invoke-2.1.3/tests/_support/configs/yml/tasks.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      126 2023-02-16 19:54:15.000000 invoke-2.1.3/tests/_support/configs/yml/explicit.py
+-rw-r--r--   0 jforcier  (1000) users      (100)       34 2021-12-23 21:30:34.000000 invoke-2.1.3/tests/_support/configs/yml/invoke.yml
+-rw-r--r--   0 jforcier  (1000) users      (100)       18 2021-12-23 21:30:34.000000 invoke-2.1.3/tests/_support/configs/echo.yaml
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-06-14 23:05:37.000000 invoke-2.1.3/tests/_support/configs/all-four/
+-rw-r--r--   0 jforcier  (1000) users      (100)       46 2021-12-23 21:30:34.000000 invoke-2.1.3/tests/_support/configs/all-four/invoke.json
+-rw-r--r--   0 jforcier  (1000) users      (100)       38 2021-12-23 21:30:34.000000 invoke-2.1.3/tests/_support/configs/all-four/invoke.yml
+-rw-r--r--   0 jforcier  (1000) users      (100)       44 2023-02-16 19:54:15.000000 invoke-2.1.3/tests/_support/configs/all-four/invoke.py
+-rw-r--r--   0 jforcier  (1000) users      (100)       40 2021-12-23 21:30:34.000000 invoke-2.1.3/tests/_support/configs/all-four/invoke.yaml
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-06-14 23:05:37.000000 invoke-2.1.3/tests/_support/configs/package/
+-rw-r--r--   0 jforcier  (1000) users      (100)       38 2023-06-14 23:05:06.000000 invoke-2.1.3/tests/_support/configs/package/invoke.yml
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-06-14 23:05:37.000000 invoke-2.1.3/tests/_support/configs/package/tasks/
+-rw-r--r--   0 jforcier  (1000) users      (100)       92 2023-06-14 23:05:06.000000 invoke-2.1.3/tests/_support/configs/package/tasks/__init__.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      173 2023-02-16 19:54:15.000000 invoke-2.1.3/tests/_support/configs/collection.py
+-rw-r--r--   0 jforcier  (1000) users      (100)       19 2021-12-23 21:30:34.000000 invoke-2.1.3/tests/_support/configs/no-echo.yaml
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-06-14 23:05:37.000000 invoke-2.1.3/tests/_support/configs/underscores/
+-rw-r--r--   0 jforcier  (1000) users      (100)       68 2023-02-16 19:54:15.000000 invoke-2.1.3/tests/_support/configs/underscores/tasks.py
+-rw-r--r--   0 jforcier  (1000) users      (100)       32 2021-12-23 21:30:34.000000 invoke-2.1.3/tests/_support/configs/underscores/invoke.yaml
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-06-14 23:05:37.000000 invoke-2.1.3/tests/_support/configs/yaml/
+-rw-r--r--   0 jforcier  (1000) users      (100)       35 2021-12-23 21:30:34.000000 invoke-2.1.3/tests/_support/configs/yaml/invoke.yaml
+-rw-r--r--   0 jforcier  (1000) users      (100)      127 2023-02-16 19:54:15.000000 invoke-2.1.3/tests/_support/configs/yaml/explicit.py
+-rw-r--r--   0 jforcier  (1000) users      (100)       89 2023-02-16 19:54:15.000000 invoke-2.1.3/tests/_support/configs/yaml/tasks.py
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-06-14 23:05:37.000000 invoke-2.1.3/tests/_support/configs/python/
+-rw-r--r--   0 jforcier  (1000) users      (100)       40 2023-02-16 19:54:15.000000 invoke-2.1.3/tests/_support/configs/python/invoke.py
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-06-14 23:05:37.000000 invoke-2.1.3/tests/_support/configs/nested/
+-rw-r--r--   0 jforcier  (1000) users      (100)       35 2021-12-23 21:30:34.000000 invoke-2.1.3/tests/_support/configs/nested/invoke.yaml
+-rw-r--r--   0 jforcier  (1000) users      (100)      264 2023-02-16 19:54:15.000000 invoke-2.1.3/tests/_support/explicit_root.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      365 2023-02-16 19:54:15.000000 invoke-2.1.3/tests/_support/autoprint.py
+-rw-r--r--   0 jforcier  (1000) users      (100)       44 2023-02-16 19:54:15.000000 invoke-2.1.3/tests/_support/oops.py
+-rw-r--r--   0 jforcier  (1000) users      (100)       96 2023-02-16 19:54:15.000000 invoke-2.1.3/tests/_support/tasks.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      226 2023-02-16 19:54:15.000000 invoke-2.1.3/tests/_support/foo.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      157 2023-02-16 19:54:15.000000 invoke-2.1.3/tests/_support/sudo_prompt.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      425 2023-02-16 19:54:15.000000 invoke-2.1.3/tests/_support/nontrivial_docstrings.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      395 2023-02-16 19:54:15.000000 invoke-2.1.3/tests/_support/contextualized.py
+-rw-r--r--   0 jforcier  (1000) users      (100)       78 2023-02-16 19:54:15.000000 invoke-2.1.3/tests/_support/alias_sorting.py
+-rw-r--r--   0 jforcier  (1000) users      (100)        7 2023-02-16 19:54:15.000000 invoke-2.1.3/tests/_support/empty.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      511 2023-02-16 19:54:15.000000 invoke-2.1.3/tests/_support/depth_first.py
+-rw-r--r--   0 jforcier  (1000) users      (100)       85 2023-02-16 19:54:15.000000 invoke-2.1.3/tests/_support/subcollection_task_name.py
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-06-14 23:05:37.000000 invoke-2.1.3/tests/_support/tree/
+-rw-r--r--   0 jforcier  (1000) users      (100)      171 2023-02-16 19:54:15.000000 invoke-2.1.3/tests/_support/tree/provision.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      653 2023-02-16 19:54:15.000000 invoke-2.1.3/tests/_support/tree/__init__.py
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-06-14 23:05:37.000000 invoke-2.1.3/tests/_support/tree/build/
+-rw-r--r--   0 jforcier  (1000) users      (100)      274 2023-02-16 19:54:15.000000 invoke-2.1.3/tests/_support/tree/build/docs.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      421 2023-02-16 19:54:15.000000 invoke-2.1.3/tests/_support/tree/build/__init__.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      278 2023-02-16 19:54:15.000000 invoke-2.1.3/tests/_support/tree/build/python.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      301 2023-02-16 19:54:15.000000 invoke-2.1.3/tests/_support/tree/deploy.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     4146 2021-12-23 21:30:34.000000 invoke-2.1.3/tests/_support/tree.json
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-06-14 23:05:37.000000 invoke-2.1.3/tests/_support/subspace/
+-rw-r--r--   0 jforcier  (1000) users      (100)       56 2023-05-02 02:12:54.000000 invoke-2.1.3/tests/_support/subspace/module.py
+-rw-r--r--   0 jforcier  (1000) users      (100)       77 2023-05-02 02:12:54.000000 invoke-2.1.3/tests/_support/subspace/__init__.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      121 2023-02-16 19:54:15.000000 invoke-2.1.3/tests/_support/empty_subcollection.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      189 2023-05-02 02:12:54.000000 invoke-2.1.3/tests/_support/namespacing.py
+-rw-r--r--   0 jforcier  (1000) users      (100)       57 2023-02-16 19:54:15.000000 invoke-2.1.3/tests/_support/custom_executor.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      666 2023-02-16 19:54:15.000000 invoke-2.1.3/tests/_support/integration.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      919 2023-02-16 19:54:15.000000 invoke-2.1.3/tests/_support/decorators.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      276 2023-02-16 19:54:15.000000 invoke-2.1.3/tests/_support/docstrings.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      178 2023-02-16 19:54:15.000000 invoke-2.1.3/tests/_support/simple_ns_list.py
+-rw-r--r--   0 jforcier  (1000) users      (100)       35 2023-02-16 19:54:15.000000 invoke-2.1.3/tests/_support/has_modules.py
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-06-14 23:05:37.000000 invoke-2.1.3/tests/_support/package/
+-rw-r--r--   0 jforcier  (1000) users      (100)       77 2023-05-02 02:12:54.000000 invoke-2.1.3/tests/_support/package/__init__.py
+-rw-r--r--   0 jforcier  (1000) users      (100)       56 2023-02-16 19:54:15.000000 invoke-2.1.3/tests/_support/package/module.py
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-06-14 23:05:37.000000 invoke-2.1.3/tests/_support/branch/
+-rw-r--r--   0 jforcier  (1000) users      (100)       73 2023-02-16 19:54:15.000000 invoke-2.1.3/tests/_support/branch/explicit.py
+-rw-r--r--   0 jforcier  (1000) users      (100)       86 2023-02-16 19:54:15.000000 invoke-2.1.3/tests/_support/branch/tasks.py
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-06-14 23:05:37.000000 invoke-2.1.3/tests/_support/ignoreme/
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-06-14 23:05:37.000000 invoke-2.1.3/tests/_support/ignoreme/ignoremetoo/
+-rw-r--r--   0 jforcier  (1000) users      (100)        0 2021-12-23 21:30:34.000000 invoke-2.1.3/tests/_support/ignoreme/ignoremetoo/.no
+-rw-r--r--   0 jforcier  (1000) users      (100)      194 2023-02-16 19:54:15.000000 invoke-2.1.3/tests/_support/deeper_ns_list.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     9820 2023-02-17 20:13:42.000000 invoke-2.1.3/tests/_util.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     4053 2023-02-16 19:54:15.000000 invoke-2.1.3/tests/init.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     3261 2023-02-17 20:13:42.000000 invoke-2.1.3/tests/concurrency.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    44633 2023-06-14 19:45:37.000000 invoke-2.1.3/tests/config.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     4550 2023-02-16 19:54:15.000000 invoke-2.1.3/tests/merge_dicts.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    22668 2023-02-16 19:54:15.000000 invoke-2.1.3/tests/parser_parser.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     7179 2023-02-16 19:54:15.000000 invoke-2.1.3/tests/parser_argument.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     5361 2023-02-16 19:54:15.000000 invoke-2.1.3/tests/cli.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     2945 2023-02-16 19:54:15.000000 invoke-2.1.3/tests/terminals.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     7687 2023-02-17 20:13:42.000000 invoke-2.1.3/tests/completion.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     1661 2023-02-17 20:13:42.000000 invoke-2.1.3/tests/util.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    17268 2023-02-17 20:13:42.000000 invoke-2.1.3/tests/task.py
+-rw-r--r--   0 jforcier  (1000) users      (100)       38 2023-06-14 23:05:37.000000 invoke-2.1.3/setup.cfg
+-rw-r--r--   0 jforcier  (1000) users      (100)     1328 2022-05-11 15:59:13.000000 invoke-2.1.3/README.rst
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-06-14 23:05:37.000000 invoke-2.1.3/sites/
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-06-14 23:05:37.000000 invoke-2.1.3/sites/www/
+-rw-r--r--   0 jforcier  (1000) users      (100)     2537 2022-03-25 22:40:47.000000 invoke-2.1.3/sites/www/prior-art.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)      753 2023-01-07 00:40:50.000000 invoke-2.1.3/sites/www/installing.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)      703 2023-02-16 19:54:15.000000 invoke-2.1.3/sites/www/conf.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     8153 2023-01-07 00:40:50.000000 invoke-2.1.3/sites/www/faq.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)     2801 2022-05-11 15:59:13.000000 invoke-2.1.3/sites/www/index.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)     1791 2022-05-11 15:59:13.000000 invoke-2.1.3/sites/www/development.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)     1218 2022-05-11 15:59:13.000000 invoke-2.1.3/sites/www/contact.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)    77739 2023-06-14 23:05:33.000000 invoke-2.1.3/sites/www/changelog.rst
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-06-14 23:05:37.000000 invoke-2.1.3/sites/docs/
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-06-14 23:05:37.000000 invoke-2.1.3/sites/docs/api/
+-rw-r--r--   0 jforcier  (1000) users      (100)       72 2022-03-25 22:40:47.000000 invoke-2.1.3/sites/docs/api/watchers.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)      156 2022-03-25 22:40:47.000000 invoke-2.1.3/sites/docs/api/collection.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)       68 2022-03-25 22:40:47.000000 invoke-2.1.3/sites/docs/api/context.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)      157 2022-03-25 22:40:47.000000 invoke-2.1.3/sites/docs/api/util.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)       80 2022-03-25 22:40:47.000000 invoke-2.1.3/sites/docs/api/executor.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)       76 2022-03-25 22:40:47.000000 invoke-2.1.3/sites/docs/api/terminals.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)       68 2022-03-25 22:40:47.000000 invoke-2.1.3/sites/docs/api/program.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)       80 2022-03-25 22:40:47.000000 invoke-2.1.3/sites/docs/api/exceptions.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)       60 2022-03-25 22:40:47.000000 invoke-2.1.3/sites/docs/api/tasks.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)       96 2022-03-25 22:40:47.000000 invoke-2.1.3/sites/docs/api/runners.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)      229 2022-03-25 22:40:47.000000 invoke-2.1.3/sites/docs/api/loader.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)       63 2022-03-25 22:40:47.000000 invoke-2.1.3/sites/docs/api/__init__.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)      401 2023-01-12 23:12:21.000000 invoke-2.1.3/sites/docs/api/parser.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)       64 2022-03-25 22:40:47.000000 invoke-2.1.3/sites/docs/api/config.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)    12466 2022-05-11 15:59:13.000000 invoke-2.1.3/sites/docs/invoke.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)      445 2023-02-16 19:54:15.000000 invoke-2.1.3/sites/docs/conf.py
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-06-14 23:05:37.000000 invoke-2.1.3/sites/docs/concepts/
+-rw-r--r--   0 jforcier  (1000) users      (100)    11750 2022-03-25 22:40:47.000000 invoke-2.1.3/sites/docs/concepts/namespaces.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)     9234 2023-02-17 20:13:42.000000 invoke-2.1.3/sites/docs/concepts/library.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)     2917 2022-05-11 15:59:13.000000 invoke-2.1.3/sites/docs/concepts/loading.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)     2424 2022-03-25 22:40:47.000000 invoke-2.1.3/sites/docs/concepts/watchers.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)    17701 2023-01-07 00:40:50.000000 invoke-2.1.3/sites/docs/concepts/configuration.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)    10180 2023-01-07 00:40:50.000000 invoke-2.1.3/sites/docs/concepts/testing.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)    16705 2023-01-07 00:40:53.000000 invoke-2.1.3/sites/docs/concepts/invoking-tasks.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)     7640 2022-05-11 15:59:13.000000 invoke-2.1.3/sites/docs/getting-started.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)      943 2022-05-11 15:59:13.000000 invoke-2.1.3/sites/docs/index.rst
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-06-14 23:05:37.000000 invoke-2.1.3/sites/docs/_static/
+-rw-r--r--   0 jforcier  (1000) users      (100)    15260 2021-12-23 21:30:34.000000 invoke-2.1.3/sites/docs/_static/rtd.css
+-rw-r--r--   0 jforcier  (1000) users      (100)     1367 2023-02-16 19:54:15.000000 invoke-2.1.3/sites/shared_conf.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     2711 2023-02-17 20:13:42.000000 invoke-2.1.3/setup.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     4047 2023-05-23 15:52:36.000000 invoke-2.1.3/tasks.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     3290 2023-06-14 23:05:37.000000 invoke-2.1.3/PKG-INFO
+-rw-r--r--   0 jforcier  (1000) users      (100)      435 2023-05-23 15:52:36.000000 invoke-2.1.3/dev-requirements.txt
+-rw-r--r--   0 jforcier  (1000) users      (100)      302 2023-05-23 15:52:36.000000 invoke-2.1.3/MANIFEST.in
+-rw-r--r--   0 jforcier  (1000) users      (100)     1250 2023-05-23 15:52:36.000000 invoke-2.1.3/pyproject.toml
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-06-14 23:05:37.000000 invoke-2.1.3/invoke.egg-info/
+-rw-r--r--   0 jforcier  (1000) users      (100)        1 2023-06-14 23:05:37.000000 invoke-2.1.3/invoke.egg-info/dependency_links.txt
+-rw-r--r--   0 jforcier  (1000) users      (100)     5243 2023-06-14 23:05:37.000000 invoke-2.1.3/invoke.egg-info/SOURCES.txt
+-rw-r--r--   0 jforcier  (1000) users      (100)     3290 2023-06-14 23:05:37.000000 invoke-2.1.3/invoke.egg-info/PKG-INFO
+-rw-r--r--   0 jforcier  (1000) users      (100)        7 2023-06-14 23:05:37.000000 invoke-2.1.3/invoke.egg-info/top_level.txt
+-rw-r--r--   0 jforcier  (1000) users      (100)       82 2023-06-14 23:05:37.000000 invoke-2.1.3/invoke.egg-info/entry_points.txt
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-06-14 23:05:37.000000 invoke-2.1.3/invoke/
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-06-14 23:05:37.000000 invoke-2.1.3/invoke/vendor/
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-06-14 23:05:37.000000 invoke-2.1.3/invoke/vendor/lexicon/
+-rw-r--r--   0 jforcier  (1000) users      (100)       80 2023-02-16 19:54:15.000000 invoke-2.1.3/invoke/vendor/lexicon/_version.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      407 2023-02-16 19:54:15.000000 invoke-2.1.3/invoke/vendor/lexicon/attribute_dict.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     1133 2023-02-16 19:54:15.000000 invoke-2.1.3/invoke/vendor/lexicon/__init__.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     3223 2023-02-16 19:54:15.000000 invoke-2.1.3/invoke/vendor/lexicon/alias_dict.py
+-rw-r--r--   0 jforcier  (1000) users      (100)        0 2023-02-16 19:54:15.000000 invoke-2.1.3/invoke/vendor/__init__.py
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-06-14 23:05:37.000000 invoke-2.1.3/invoke/vendor/yaml/
+-rw-r--r--   0 jforcier  (1000) users      (100)     1440 2023-02-16 19:54:22.000000 invoke-2.1.3/invoke/vendor/yaml/nodes.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    43006 2023-02-16 19:54:15.000000 invoke-2.1.3/invoke/vendor/yaml/emitter.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     4165 2023-02-16 19:54:15.000000 invoke-2.1.3/invoke/vendor/yaml/serializer.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    25495 2023-02-16 19:54:15.000000 invoke-2.1.3/invoke/vendor/yaml/parser.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    28639 2023-02-16 19:54:15.000000 invoke-2.1.3/invoke/vendor/yaml/constructor.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    51277 2023-02-16 19:54:15.000000 invoke-2.1.3/invoke/vendor/yaml/scanner.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     2061 2023-02-16 19:54:15.000000 invoke-2.1.3/invoke/vendor/yaml/loader.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     2573 2023-02-16 19:54:22.000000 invoke-2.1.3/invoke/vendor/yaml/tokens.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     2445 2023-02-16 19:54:22.000000 invoke-2.1.3/invoke/vendor/yaml/events.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     3851 2023-02-16 19:54:15.000000 invoke-2.1.3/invoke/vendor/yaml/cyaml.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    13170 2023-02-16 19:54:15.000000 invoke-2.1.3/invoke/vendor/yaml/__init__.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    14184 2023-02-16 19:54:15.000000 invoke-2.1.3/invoke/vendor/yaml/representer.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     4883 2023-02-16 19:54:15.000000 invoke-2.1.3/invoke/vendor/yaml/composer.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     2533 2023-02-16 19:54:15.000000 invoke-2.1.3/invoke/vendor/yaml/error.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     2837 2023-02-16 19:54:15.000000 invoke-2.1.3/invoke/vendor/yaml/dumper.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     6794 2023-02-16 19:54:22.000000 invoke-2.1.3/invoke/vendor/yaml/reader.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     8999 2023-02-16 19:54:15.000000 invoke-2.1.3/invoke/vendor/yaml/resolver.py
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-06-14 23:05:37.000000 invoke-2.1.3/invoke/vendor/fluidity/
+-rw-r--r--   0 jforcier  (1000) users      (100)     8686 2023-02-16 19:54:22.000000 invoke-2.1.3/invoke/vendor/fluidity/machine.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      135 2023-02-16 19:54:15.000000 invoke-2.1.3/invoke/vendor/fluidity/backwardscompat.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      196 2023-02-16 19:54:15.000000 invoke-2.1.3/invoke/vendor/fluidity/__init__.py
+-rw-r--r--   0 jforcier  (1000) users      (100)       80 2023-06-14 23:05:36.000000 invoke-2.1.3/invoke/_version.py
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-06-14 23:05:37.000000 invoke-2.1.3/invoke/parser/
+-rw-r--r--   0 jforcier  (1000) users      (100)      181 2023-02-16 19:54:15.000000 invoke-2.1.3/invoke/parser/__init__.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     9815 2023-05-23 15:52:36.000000 invoke-2.1.3/invoke/parser/context.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     6045 2023-05-23 15:52:36.000000 invoke-2.1.3/invoke/parser/argument.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    19809 2023-05-23 15:52:36.000000 invoke-2.1.3/invoke/parser/parser.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     4394 2023-05-23 15:52:36.000000 invoke-2.1.3/invoke/env.py
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-06-14 23:05:37.000000 invoke-2.1.3/invoke/completion/
+-rw-r--r--   0 jforcier  (1000) users      (100)     1356 2021-12-23 21:30:34.000000 invoke-2.1.3/invoke/completion/bash.completion
+-rw-r--r--   0 jforcier  (1000) users      (100)        0 2023-02-16 19:54:15.000000 invoke-2.1.3/invoke/completion/__init__.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     1429 2021-12-23 21:30:34.000000 invoke-2.1.3/invoke/completion/zsh.completion
+-rw-r--r--   0 jforcier  (1000) users      (100)     5222 2023-05-23 15:52:36.000000 invoke-2.1.3/invoke/completion/complete.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      382 2021-12-23 21:30:34.000000 invoke-2.1.3/invoke/completion/fish.completion
+-rw-r--r--   0 jforcier  (1000) users      (100)    50005 2023-05-23 15:52:36.000000 invoke-2.1.3/invoke/config.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     5097 2023-05-23 15:52:36.000000 invoke-2.1.3/invoke/watchers.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     8855 2023-05-23 15:52:36.000000 invoke-2.1.3/invoke/executor.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     2229 2023-05-23 15:52:36.000000 invoke-2.1.3/invoke/__init__.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    65509 2023-05-23 15:52:36.000000 invoke-2.1.3/invoke/runners.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    38177 2023-06-14 22:02:41.000000 invoke-2.1.3/invoke/program.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    25486 2023-05-23 15:52:36.000000 invoke-2.1.3/invoke/context.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     6005 2023-06-14 23:05:06.000000 invoke-2.1.3/invoke/loader.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      235 2023-02-16 19:54:15.000000 invoke-2.1.3/invoke/main.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    10018 2023-05-23 15:52:36.000000 invoke-2.1.3/invoke/util.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    12227 2023-05-23 15:52:36.000000 invoke-2.1.3/invoke/exceptions.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    23060 2023-05-23 15:52:36.000000 invoke-2.1.3/invoke/collection.py
+-rw-r--r--   0 jforcier  (1000) users      (100)        0 2023-05-23 15:52:36.000000 invoke-2.1.3/invoke/py.typed
+-rw-r--r--   0 jforcier  (1000) users      (100)       47 2023-02-16 19:54:15.000000 invoke-2.1.3/invoke/__main__.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     8065 2023-05-23 15:52:36.000000 invoke-2.1.3/invoke/terminals.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    19946 2023-05-23 15:52:36.000000 invoke-2.1.3/invoke/tasks.py
```

### Comparing `invoke-2.1.2/setup.py` & `invoke-2.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.2/tasks.py` & `invoke-2.1.3/tasks.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,25 +114,25 @@
     release,
     www,
     docs,
     sites,
     watch_docs,
     ci,
     checks.blacken,
+    checks,
 )
 ns.configure(
     {
         "blacken": {
             # Skip vendor, build dirs when blackening.
             # TODO: this is making it seem like I really do want an explicit
             # arg/conf-opt in the blacken task for "excluded paths"...ha
             "find_opts": "-and -not \( -path './invoke/vendor*' -or -path './build*' \)"  # noqa
         },
         "packaging": {
-            "sign": True,
             "wheel": True,
             "check_desc": True,
             "changelog_file": os.path.join(
                 www.configuration()["sphinx"]["source"], "changelog.rst"
             ),
         },
     }
```

### Comparing `invoke-2.1.2/PKG-INFO` & `invoke-2.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invoke
-Version: 2.1.2
+Version: 2.1.3
 Summary: Pythonic task execution
 Home-page: https://pyinvoke.org
 Author: Jeff Forcier
 Author-email: jeff@bitprophet.org
 License: BSD
 Project-URL: Docs, https://docs.pyinvoke.org
 Project-URL: Source, https://github.com/pyinvoke/invoke
```

### Comparing `invoke-2.1.2/invoke/watchers.py` & `invoke-2.1.3/invoke/watchers.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.2/invoke/vendor/lexicon/__init__.py` & `invoke-2.1.3/invoke/vendor/lexicon/__init__.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.2/invoke/vendor/lexicon/alias_dict.py` & `invoke-2.1.3/invoke/vendor/lexicon/alias_dict.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.2/invoke/vendor/yaml/nodes.py` & `invoke-2.1.3/invoke/vendor/yaml/nodes.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.2/invoke/vendor/yaml/constructor.py` & `invoke-2.1.3/invoke/vendor/yaml/constructor.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.2/invoke/vendor/yaml/parser.py` & `invoke-2.1.3/invoke/vendor/yaml/parser.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.2/invoke/vendor/yaml/serializer.py` & `invoke-2.1.3/invoke/vendor/yaml/serializer.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.2/invoke/vendor/yaml/scanner.py` & `invoke-2.1.3/invoke/vendor/yaml/scanner.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.2/invoke/vendor/yaml/reader.py` & `invoke-2.1.3/invoke/vendor/yaml/reader.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.2/invoke/vendor/yaml/__init__.py` & `invoke-2.1.3/invoke/vendor/yaml/__init__.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.2/invoke/vendor/yaml/cyaml.py` & `invoke-2.1.3/invoke/vendor/yaml/cyaml.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.2/invoke/vendor/yaml/composer.py` & `invoke-2.1.3/invoke/vendor/yaml/composer.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.2/invoke/vendor/yaml/error.py` & `invoke-2.1.3/invoke/vendor/yaml/error.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.2/invoke/vendor/yaml/dumper.py` & `invoke-2.1.3/invoke/vendor/yaml/dumper.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.2/invoke/vendor/yaml/resolver.py` & `invoke-2.1.3/invoke/vendor/yaml/resolver.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.2/invoke/vendor/yaml/representer.py` & `invoke-2.1.3/invoke/vendor/yaml/representer.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.2/invoke/vendor/yaml/emitter.py` & `invoke-2.1.3/invoke/vendor/yaml/emitter.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.2/invoke/vendor/yaml/loader.py` & `invoke-2.1.3/invoke/vendor/yaml/loader.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.2/invoke/vendor/yaml/tokens.py` & `invoke-2.1.3/invoke/vendor/yaml/tokens.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.2/invoke/vendor/yaml/events.py` & `invoke-2.1.3/invoke/vendor/yaml/events.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.2/invoke/vendor/fluidity/machine.py` & `invoke-2.1.3/invoke/vendor/fluidity/machine.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.2/invoke/__init__.py` & `invoke-2.1.3/invoke/__init__.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.2/invoke/executor.py` & `invoke-2.1.3/invoke/executor.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.2/invoke/util.py` & `invoke-2.1.3/invoke/util.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.2/invoke/config.py` & `invoke-2.1.3/invoke/config.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.2/invoke/env.py` & `invoke-2.1.3/invoke/env.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.2/invoke/parser/argument.py` & `invoke-2.1.3/invoke/parser/argument.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.2/invoke/parser/parser.py` & `invoke-2.1.3/invoke/parser/parser.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.2/invoke/parser/context.py` & `invoke-2.1.3/invoke/parser/context.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.2/invoke/runners.py` & `invoke-2.1.3/invoke/runners.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.2/invoke/program.py` & `invoke-2.1.3/invoke/program.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.2/invoke/context.py` & `invoke-2.1.3/invoke/context.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.2/invoke/completion/zsh.completion` & `invoke-2.1.3/invoke/completion/zsh.completion`

 * *Files identical despite different names*

### Comparing `invoke-2.1.2/invoke/completion/bash.completion` & `invoke-2.1.3/invoke/completion/bash.completion`

 * *Files identical despite different names*

### Comparing `invoke-2.1.2/invoke/completion/complete.py` & `invoke-2.1.3/invoke/completion/complete.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.2/invoke/terminals.py` & `invoke-2.1.3/invoke/terminals.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.2/invoke/loader.py` & `invoke-2.1.3/invoke/loader.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 import sys
 from importlib.machinery import ModuleSpec
 from importlib.util import module_from_spec, spec_from_file_location
+from pathlib import Path
 from types import ModuleType
 from typing import Any, Optional, Tuple
 
 from . import Config
 from .exceptions import CollectionNotFound
 from .util import debug
 
@@ -64,26 +65,36 @@
 
         .. versionadded:: 1.0
         """
         if name is None:
             name = self.config.tasks.collection_name
         spec = self.find(name)
         if spec and spec.loader and spec.origin:
-            path = spec.origin
-            # Ensure containing directory is on sys.path in case the module
-            # being imported is trying to load local-to-it names.
-            if os.path.isfile(spec.origin):
-                path = os.path.dirname(spec.origin)
-            if path not in sys.path:
-                sys.path.insert(0, path)
+            # Typically either tasks.py or tasks/__init__.py
+            source_file = Path(spec.origin)
+            # Will be 'the dir tasks.py is in', or 'tasks/', in both cases this
+            # is what wants to be in sys.path for "from . import sibling"
+            enclosing_dir = source_file.parent
+            # Will be "the directory above the spot that 'import tasks' found",
+            # namely the parent of "your task tree", i.e. "where project level
+            # config files are looked for". So, same as enclosing_dir for
+            # tasks.py, but one more level up for tasks/__init__.py...
+            module_parent = enclosing_dir
+            if spec.parent:  # it's a package, so we have to go up again
+                module_parent = module_parent.parent
+            # Get the enclosing dir on the path
+            enclosing_str = str(enclosing_dir)
+            if enclosing_str not in sys.path:
+                sys.path.insert(0, enclosing_str)
             # Actual import
             module = module_from_spec(spec)
             sys.modules[spec.name] = module  # so 'from . import xxx' works
             spec.loader.exec_module(module)
-            return module, os.path.dirname(spec.origin)
+            # Return the module and the folder it was found in
+            return module, str(module_parent)
         msg = "ImportError loading {!r}, raising ImportError"
         debug(msg.format(name))
         raise ImportError
 
 
 class FilesystemLoader(Loader):
     """
```

### Comparing `invoke-2.1.2/invoke/exceptions.py` & `invoke-2.1.3/invoke/exceptions.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.2/invoke/collection.py` & `invoke-2.1.3/invoke/collection.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.2/invoke/tasks.py` & `invoke-2.1.3/invoke/tasks.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.2/sites/shared_conf.py` & `invoke-2.1.3/sites/shared_conf.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.2/sites/www/changelog.rst` & `invoke-2.1.3/sites/www/changelog.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 =========
 Changelog
 =========
 
+- :release:`2.1.3 <2023-06-14>`
+- :bug:`944` After the release of 2.1, package-style task modules started
+  looking in the wrong place for project-level config files (inside one's eg
+  ``tasks/`` dir, instead of *next to* that dir) due to a subtlety in the new
+  import/discovery mechanism used. This has been fixed. Thanks to Arnaud V. and
+  Hunter Kelly for the reports and to Jesse P. Johnson for initial
+  debugging/diagnosis.
 - :release:`2.1.2 <2023-05-15>`
 - :support:`936 backported` Make sure ``py.typed`` is in our packaging
   manifest; without it, users working from a regular installation
   can't perform type checks. Thanks to Nikita Sobolev for catch & patch.
 - :release:`2.1.1 <2023-05-01>`
 - :bug:`934` The `importlib` upgrade in 2.1 had a corner case bug (regarding
   ``from . import <submodule>`` functionality within package-like task trees)
```

### Comparing `invoke-2.1.2/sites/www/faq.rst` & `invoke-2.1.3/sites/www/faq.rst`

 * *Files identical despite different names*

### Comparing `invoke-2.1.2/sites/www/conf.py` & `invoke-2.1.3/sites/www/conf.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.2/sites/www/development.rst` & `invoke-2.1.3/sites/www/development.rst`

 * *Files identical despite different names*

### Comparing `invoke-2.1.2/sites/www/prior-art.rst` & `invoke-2.1.3/sites/www/prior-art.rst`

 * *Files identical despite different names*

### Comparing `invoke-2.1.2/sites/www/installing.rst` & `invoke-2.1.3/sites/www/installing.rst`

 * *Files identical despite different names*

### Comparing `invoke-2.1.2/sites/www/contact.rst` & `invoke-2.1.3/sites/www/contact.rst`

 * *Files identical despite different names*

### Comparing `invoke-2.1.2/sites/www/index.rst` & `invoke-2.1.3/sites/www/index.rst`

 * *Files identical despite different names*

### Comparing `invoke-2.1.2/sites/docs/index.rst` & `invoke-2.1.3/sites/docs/index.rst`

 * *Files identical despite different names*

### Comparing `invoke-2.1.2/sites/docs/getting-started.rst` & `invoke-2.1.3/sites/docs/getting-started.rst`

 * *Files identical despite different names*

### Comparing `invoke-2.1.2/sites/docs/_static/rtd.css` & `invoke-2.1.3/sites/docs/_static/rtd.css`

 * *Files identical despite different names*

### Comparing `invoke-2.1.2/sites/docs/invoke.rst` & `invoke-2.1.3/sites/docs/invoke.rst`

 * *Files identical despite different names*

### Comparing `invoke-2.1.2/sites/docs/concepts/namespaces.rst` & `invoke-2.1.3/sites/docs/concepts/namespaces.rst`

 * *Files identical despite different names*

### Comparing `invoke-2.1.2/sites/docs/concepts/loading.rst` & `invoke-2.1.3/sites/docs/concepts/loading.rst`

 * *Files identical despite different names*

### Comparing `invoke-2.1.2/sites/docs/concepts/configuration.rst` & `invoke-2.1.3/sites/docs/concepts/configuration.rst`

 * *Files identical despite different names*

### Comparing `invoke-2.1.2/sites/docs/concepts/testing.rst` & `invoke-2.1.3/sites/docs/concepts/testing.rst`

 * *Files identical despite different names*

### Comparing `invoke-2.1.2/sites/docs/concepts/library.rst` & `invoke-2.1.3/sites/docs/concepts/library.rst`

 * *Files identical despite different names*

### Comparing `invoke-2.1.2/sites/docs/concepts/watchers.rst` & `invoke-2.1.3/sites/docs/concepts/watchers.rst`

 * *Files identical despite different names*

### Comparing `invoke-2.1.2/sites/docs/concepts/invoking-tasks.rst` & `invoke-2.1.3/sites/docs/concepts/invoking-tasks.rst`

 * *Files identical despite different names*

### Comparing `invoke-2.1.2/LICENSE` & `invoke-2.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `invoke-2.1.2/tests/config.py` & `invoke-2.1.3/tests/config.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.2/tests/task.py` & `invoke-2.1.3/tests/task.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.2/tests/_util.py` & `invoke-2.1.3/tests/_util.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.2/tests/terminals.py` & `invoke-2.1.3/tests/terminals.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.2/tests/_support/tree.json` & `invoke-2.1.3/tests/_support/tree.json`

 * *Files identical despite different names*

### Comparing `invoke-2.1.2/tests/_support/integration.py` & `invoke-2.1.3/tests/_support/integration.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.2/tests/_support/tree/__init__.py` & `invoke-2.1.3/tests/_support/tree/__init__.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.2/tests/_support/decorators.py` & `invoke-2.1.3/tests/_support/decorators.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.2/tests/parser_argument.py` & `invoke-2.1.3/tests/parser_argument.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.2/tests/util.py` & `invoke-2.1.3/tests/util.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.2/tests/collection.py` & `invoke-2.1.3/tests/collection.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.2/tests/merge_dicts.py` & `invoke-2.1.3/tests/merge_dicts.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.2/tests/executor.py` & `invoke-2.1.3/tests/executor.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.2/tests/parser_parser.py` & `invoke-2.1.3/tests/parser_parser.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.2/tests/loader.py` & `invoke-2.1.3/tests/loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,19 +57,19 @@
         # If the bug is present, this will be 2 at least (and often more, since
         # other tests will pollute it (!).
         assert sys.path.count(support) == 1
 
     def can_load_package(self):
         loader = _BasicLoader()
         # Load itself doesn't explode (tests 'from . import xxx' internally)
-        mod, loc = loader.load("package")
+        mod, enclosing_dir = loader.load("package")
         # Properties of returned values look as expected
-        package = Path(support) / "package"
-        assert loc == str(package)
-        assert mod.__file__ == str(package / "__init__.py")
+        # (enclosing dir is always the one above the module-or-package)
+        assert enclosing_dir == support
+        assert mod.__file__ == str(Path(support) / "package" / "__init__.py")
 
     def load_name_defaults_to_config_tasks_collection_name(self):
         "load() name defaults to config.tasks.collection_name"
 
         class MockLoader(_BasicLoader):
             def find(self, name):
                 # Sanity
```

### Comparing `invoke-2.1.2/tests/runners.py` & `invoke-2.1.3/tests/runners.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.2/tests/watchers.py` & `invoke-2.1.3/tests/watchers.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.2/tests/concurrency.py` & `invoke-2.1.3/tests/concurrency.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.2/tests/context.py` & `invoke-2.1.3/tests/context.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.2/tests/init.py` & `invoke-2.1.3/tests/init.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.2/tests/conftest.py` & `invoke-2.1.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.2/tests/parser_context.py` & `invoke-2.1.3/tests/parser_context.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.2/tests/program.py` & `invoke-2.1.3/tests/program.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import json
 import os
 import sys
 from io import BytesIO
+from pathlib import Path
 
 from invoke.util import Lexicon
 from unittest.mock import patch, Mock, ANY
 import pytest
 from pytest import skip
 from pytest_relaxed import trap
 
@@ -31,14 +32,15 @@
     ROOT,
     expect,
     load,
     run,
     skip_if_windows,
     support_file,
     support_path,
+    support,
 )
 
 
 pytestmark = pytest.mark.usefixtures("integration")
 
 
 class Program_:
@@ -237,14 +239,18 @@
 
         @trap
         def uses_loader_class_given(self):
             klass = Mock(side_effect=FilesystemLoader)
             Program(loader_class=klass).run("myapp --help foo", exit=False)
             klass.assert_called_with(start=ANY, config=ANY)
 
+        def config_location_correct_for_package_type_task_trees(self):
+            with cd(Path(support) / "configs" / "package"):
+                expect("mytask")  # will assert if config not loaded right
+
     class execute:
         def uses_executor_class_given(self):
             klass = Mock()
             Program(executor_class=klass).run("myapp foo", exit=False)
             klass.assert_called_with(ANY, ANY, ANY)
             klass.return_value.execute.assert_called_with(ANY)
```

### Comparing `invoke-2.1.2/tests/completion.py` & `invoke-2.1.3/tests/completion.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.2/tests/cli.py` & `invoke-2.1.3/tests/cli.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.2/README.rst` & `invoke-2.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `invoke-2.1.2/pyproject.toml` & `invoke-2.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `invoke-2.1.2/invoke.egg-info/SOURCES.txt` & `invoke-2.1.3/invoke.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -153,14 +153,16 @@
 tests/_support/configs/all-four/invoke.py
 tests/_support/configs/all-four/invoke.yaml
 tests/_support/configs/all-four/invoke.yml
 tests/_support/configs/json/invoke.json
 tests/_support/configs/json-and-python/invoke.json
 tests/_support/configs/json-and-python/invoke.py
 tests/_support/configs/nested/invoke.yaml
+tests/_support/configs/package/invoke.yml
+tests/_support/configs/package/tasks/__init__.py
 tests/_support/configs/python/invoke.py
 tests/_support/configs/three-of-em/invoke.json
 tests/_support/configs/three-of-em/invoke.py
 tests/_support/configs/three-of-em/invoke.yml
 tests/_support/configs/underscores/invoke.yaml
 tests/_support/configs/underscores/tasks.py
 tests/_support/configs/yaml/explicit.py
```

### Comparing `invoke-2.1.2/invoke.egg-info/PKG-INFO` & `invoke-2.1.3/invoke.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invoke
-Version: 2.1.2
+Version: 2.1.3
 Summary: Pythonic task execution
 Home-page: https://pyinvoke.org
 Author: Jeff Forcier
 Author-email: jeff@bitprophet.org
 License: BSD
 Project-URL: Docs, https://docs.pyinvoke.org
 Project-URL: Source, https://github.com/pyinvoke/invoke
```

