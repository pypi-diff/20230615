# Comparing `tmp/thipster-0.16.7.tar.gz` & `tmp/thipster-0.17.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thipster-0.16.7.tar", last modified: Wed Jun 14 09:18:27 2023, max compression
+gzip compressed data, was "thipster-0.17.0.tar", last modified: Thu Jun 15 08:20:12 2023, max compression
```

## Comparing `thipster-0.16.7.tar` & `thipster-0.17.0.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 09:18:27.588561 thipster-0.16.7/
--rw-r--r--   0 root         (0) root         (0)     1052 2023-06-14 09:18:24.000000 thipster-0.16.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)       81 2023-06-14 09:18:24.000000 thipster-0.16.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     5156 2023-06-14 09:18:27.588561 thipster-0.16.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4324 2023-06-14 09:18:24.000000 thipster-0.16.7/README.md
--rw-r--r--   0 root         (0) root         (0)      986 2023-06-14 09:18:24.000000 thipster-0.16.7/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       82 2023-06-14 09:18:24.000000 thipster-0.16.7/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-14 09:18:27.588561 thipster-0.16.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1985 2023-06-14 09:18:25.000000 thipster-0.16.7/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 09:18:27.580561 thipster-0.16.7/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-14 09:18:24.000000 thipster-0.16.7/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 09:18:27.580561 thipster-0.16.7/tests/engine/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-14 09:18:24.000000 thipster-0.16.7/tests/engine/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3202 2023-06-14 09:18:24.000000 thipster-0.16.7/tests/engine/test_engine.py
--rw-r--r--   0 root         (0) root         (0)     4660 2023-06-14 09:18:24.000000 thipster-0.16.7/tests/engine/test_generation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 09:18:27.580561 thipster-0.16.7/tests/parser/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-14 09:18:24.000000 thipster-0.16.7/tests/parser/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 09:18:27.580561 thipster-0.16.7/tests/parser/dsl_parser/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-14 09:18:24.000000 thipster-0.16.7/tests/parser/dsl_parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15286 2023-06-14 09:18:24.000000 thipster-0.16.7/tests/parser/dsl_parser/test_DSLparser.py
--rw-r--r--   0 root         (0) root         (0)     1359 2023-06-14 09:18:24.000000 thipster-0.16.7/tests/parser/dsl_parser/test_ast.py
--rw-r--r--   0 root         (0) root         (0)    13297 2023-06-14 09:18:24.000000 thipster-0.16.7/tests/parser/dsl_parser/test_lexer.py
--rw-r--r--   0 root         (0) root         (0)      865 2023-06-14 09:18:24.000000 thipster-0.16.7/tests/parser/dsl_parser/test_token.py
--rw-r--r--   0 root         (0) root         (0)     3524 2023-06-14 09:18:24.000000 thipster-0.16.7/tests/parser/dsl_parser/test_tokenparser.py
--rw-r--r--   0 root         (0) root         (0)     2405 2023-06-14 09:18:24.000000 thipster-0.16.7/tests/parser/test_ParserFactory.py
--rw-r--r--   0 root         (0) root         (0)     4369 2023-06-14 09:18:24.000000 thipster-0.16.7/tests/parser/test_YAMLParser.py
--rw-r--r--   0 root         (0) root         (0)     4701 2023-06-14 09:18:24.000000 thipster-0.16.7/tests/parser/test_parsedfile.py
--rw-r--r--   0 root         (0) root         (0)     3304 2023-06-14 09:18:24.000000 thipster-0.16.7/tests/test_e2e.py
--rw-r--r--   0 root         (0) root         (0)     4150 2023-06-14 09:18:24.000000 thipster-0.16.7/tests/test_tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 09:18:27.580561 thipster-0.16.7/thipster/
--rw-r--r--   0 root         (0) root         (0)      171 2023-06-14 09:18:24.000000 thipster-0.16.7/thipster/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 09:18:27.584561 thipster-0.16.7/thipster/auth/
--rw-r--r--   0 root         (0) root         (0)      215 2023-06-14 09:18:24.000000 thipster-0.16.7/thipster/auth/__init__.py
--rw-r--r--   0 root         (0) root         (0)      903 2023-06-14 09:18:24.000000 thipster-0.16.7/thipster/auth/google.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 09:18:27.584561 thipster-0.16.7/thipster/engine/
--rw-r--r--   0 root         (0) root         (0)      411 2023-06-14 09:18:24.000000 thipster-0.16.7/thipster/engine/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5079 2023-06-14 09:18:24.000000 thipster-0.16.7/thipster/engine/engine.py
--rw-r--r--   0 root         (0) root         (0)      247 2023-06-14 09:18:24.000000 thipster-0.16.7/thipster/engine/exceptions.py
--rw-r--r--   0 root         (0) root         (0)      410 2023-06-14 09:18:24.000000 thipster-0.16.7/thipster/engine/i_auth.py
--rw-r--r--   0 root         (0) root         (0)      735 2023-06-14 09:18:24.000000 thipster-0.16.7/thipster/engine/i_parser.py
--rw-r--r--   0 root         (0) root         (0)      597 2023-06-14 09:18:24.000000 thipster-0.16.7/thipster/engine/i_repository.py
--rw-r--r--   0 root         (0) root         (0)     1911 2023-06-14 09:18:24.000000 thipster-0.16.7/thipster/engine/i_terraform.py
--rw-r--r--   0 root         (0) root         (0)     4368 2023-06-14 09:18:24.000000 thipster-0.16.7/thipster/engine/parsed_file.py
--rw-r--r--   0 root         (0) root         (0)     3136 2023-06-14 09:18:24.000000 thipster-0.16.7/thipster/engine/resource_model.py
--rw-r--r--   0 root         (0) root         (0)      654 2023-06-14 09:18:24.000000 thipster-0.16.7/thipster/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 09:18:27.584561 thipster-0.16.7/thipster/parser/
--rw-r--r--   0 root         (0) root         (0)      364 2023-06-14 09:18:24.000000 thipster-0.16.7/thipster/parser/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 09:18:27.584561 thipster-0.16.7/thipster/parser/dsl_parser/
--rw-r--r--   0 root         (0) root         (0)       30 2023-06-14 09:18:24.000000 thipster-0.16.7/thipster/parser/dsl_parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9156 2023-06-14 09:18:24.000000 thipster-0.16.7/thipster/parser/dsl_parser/ast.py
--rw-r--r--   0 root         (0) root         (0)     2925 2023-06-14 09:18:24.000000 thipster-0.16.7/thipster/parser/dsl_parser/exceptions.py
--rw-r--r--   0 root         (0) root         (0)    13471 2023-06-14 09:18:24.000000 thipster-0.16.7/thipster/parser/dsl_parser/interpreter.py
--rw-r--r--   0 root         (0) root         (0)    17264 2023-06-14 09:18:24.000000 thipster-0.16.7/thipster/parser/dsl_parser/lexer.py
--rw-r--r--   0 root         (0) root         (0)     4771 2023-06-14 09:18:24.000000 thipster-0.16.7/thipster/parser/dsl_parser/lexer_position.py
--rw-r--r--   0 root         (0) root         (0)     1985 2023-06-14 09:18:24.000000 thipster-0.16.7/thipster/parser/dsl_parser/parser.py
--rw-r--r--   0 root         (0) root         (0)     2085 2023-06-14 09:18:24.000000 thipster-0.16.7/thipster/parser/dsl_parser/token.py
--rw-r--r--   0 root         (0) root         (0)    20105 2023-06-14 09:18:24.000000 thipster-0.16.7/thipster/parser/dsl_parser/token_parser.py
--rw-r--r--   0 root         (0) root         (0)     2474 2023-06-14 09:18:24.000000 thipster-0.16.7/thipster/parser/parser_factory.py
--rw-r--r--   0 root         (0) root         (0)     6549 2023-06-14 09:18:24.000000 thipster-0.16.7/thipster/parser/yaml_parser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 09:18:27.588561 thipster-0.16.7/thipster/repository/
--rw-r--r--   0 root         (0) root         (0)      332 2023-06-14 09:18:24.000000 thipster-0.16.7/thipster/repository/__init__.py
--rw-r--r--   0 root         (0) root         (0)      293 2023-06-14 09:18:24.000000 thipster-0.16.7/thipster/repository/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     1399 2023-06-14 09:18:24.000000 thipster-0.16.7/thipster/repository/github.py
--rw-r--r--   0 root         (0) root         (0)     4653 2023-06-14 09:18:24.000000 thipster-0.16.7/thipster/repository/json.py
--rw-r--r--   0 root         (0) root         (0)      475 2023-06-14 09:18:24.000000 thipster-0.16.7/thipster/repository/local.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 09:18:27.588561 thipster-0.16.7/thipster/terraform/
--rw-r--r--   0 root         (0) root         (0)      327 2023-06-14 09:18:24.000000 thipster-0.16.7/thipster/terraform/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19049 2023-06-14 09:18:24.000000 thipster-0.16.7/thipster/terraform/cdk.py
--rw-r--r--   0 root         (0) root         (0)     1237 2023-06-14 09:18:24.000000 thipster-0.16.7/thipster/terraform/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 09:18:27.584561 thipster-0.16.7/thipster.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5156 2023-06-14 09:18:27.000000 thipster-0.16.7/thipster.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1774 2023-06-14 09:18:27.000000 thipster-0.16.7/thipster.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-14 09:18:27.000000 thipster-0.16.7/thipster.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      390 2023-06-14 09:18:27.000000 thipster-0.16.7/thipster.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-06-14 09:18:27.000000 thipster-0.16.7/thipster.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 08:20:12.316229 thipster-0.17.0/
+-rw-r--r--   0 root         (0) root         (0)     1052 2023-06-15 08:20:08.000000 thipster-0.17.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       81 2023-06-15 08:20:08.000000 thipster-0.17.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     5156 2023-06-15 08:20:12.316229 thipster-0.17.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4324 2023-06-15 08:20:08.000000 thipster-0.17.0/README.md
+-rw-r--r--   0 root         (0) root         (0)      986 2023-06-15 08:20:08.000000 thipster-0.17.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       82 2023-06-15 08:20:08.000000 thipster-0.17.0/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-15 08:20:12.316229 thipster-0.17.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1985 2023-06-15 08:20:08.000000 thipster-0.17.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 08:20:12.308229 thipster-0.17.0/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-15 08:20:08.000000 thipster-0.17.0/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 08:20:12.308229 thipster-0.17.0/tests/engine/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-15 08:20:08.000000 thipster-0.17.0/tests/engine/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3202 2023-06-15 08:20:08.000000 thipster-0.17.0/tests/engine/test_engine.py
+-rw-r--r--   0 root         (0) root         (0)     5360 2023-06-15 08:20:08.000000 thipster-0.17.0/tests/engine/test_generation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 08:20:12.308229 thipster-0.17.0/tests/parser/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-15 08:20:08.000000 thipster-0.17.0/tests/parser/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 08:20:12.308229 thipster-0.17.0/tests/parser/dsl_parser/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-15 08:20:08.000000 thipster-0.17.0/tests/parser/dsl_parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15286 2023-06-15 08:20:08.000000 thipster-0.17.0/tests/parser/dsl_parser/test_DSLparser.py
+-rw-r--r--   0 root         (0) root         (0)     1359 2023-06-15 08:20:08.000000 thipster-0.17.0/tests/parser/dsl_parser/test_ast.py
+-rw-r--r--   0 root         (0) root         (0)    13297 2023-06-15 08:20:08.000000 thipster-0.17.0/tests/parser/dsl_parser/test_lexer.py
+-rw-r--r--   0 root         (0) root         (0)      865 2023-06-15 08:20:08.000000 thipster-0.17.0/tests/parser/dsl_parser/test_token.py
+-rw-r--r--   0 root         (0) root         (0)     3524 2023-06-15 08:20:08.000000 thipster-0.17.0/tests/parser/dsl_parser/test_tokenparser.py
+-rw-r--r--   0 root         (0) root         (0)     2405 2023-06-15 08:20:08.000000 thipster-0.17.0/tests/parser/test_ParserFactory.py
+-rw-r--r--   0 root         (0) root         (0)     4369 2023-06-15 08:20:08.000000 thipster-0.17.0/tests/parser/test_YAMLParser.py
+-rw-r--r--   0 root         (0) root         (0)     4701 2023-06-15 08:20:08.000000 thipster-0.17.0/tests/parser/test_parsedfile.py
+-rw-r--r--   0 root         (0) root         (0)     3305 2023-06-15 08:20:08.000000 thipster-0.17.0/tests/test_e2e.py
+-rw-r--r--   0 root         (0) root         (0)     4150 2023-06-15 08:20:08.000000 thipster-0.17.0/tests/test_tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 08:20:12.308229 thipster-0.17.0/thipster/
+-rw-r--r--   0 root         (0) root         (0)      171 2023-06-15 08:20:08.000000 thipster-0.17.0/thipster/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 08:20:12.312229 thipster-0.17.0/thipster/auth/
+-rw-r--r--   0 root         (0) root         (0)      215 2023-06-15 08:20:08.000000 thipster-0.17.0/thipster/auth/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      903 2023-06-15 08:20:08.000000 thipster-0.17.0/thipster/auth/google.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 08:20:12.312229 thipster-0.17.0/thipster/engine/
+-rw-r--r--   0 root         (0) root         (0)      411 2023-06-15 08:20:08.000000 thipster-0.17.0/thipster/engine/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5079 2023-06-15 08:20:08.000000 thipster-0.17.0/thipster/engine/engine.py
+-rw-r--r--   0 root         (0) root         (0)      247 2023-06-15 08:20:08.000000 thipster-0.17.0/thipster/engine/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)      410 2023-06-15 08:20:08.000000 thipster-0.17.0/thipster/engine/i_auth.py
+-rw-r--r--   0 root         (0) root         (0)      735 2023-06-15 08:20:08.000000 thipster-0.17.0/thipster/engine/i_parser.py
+-rw-r--r--   0 root         (0) root         (0)      597 2023-06-15 08:20:08.000000 thipster-0.17.0/thipster/engine/i_repository.py
+-rw-r--r--   0 root         (0) root         (0)     1911 2023-06-15 08:20:08.000000 thipster-0.17.0/thipster/engine/i_terraform.py
+-rw-r--r--   0 root         (0) root         (0)     4368 2023-06-15 08:20:08.000000 thipster-0.17.0/thipster/engine/parsed_file.py
+-rw-r--r--   0 root         (0) root         (0)     3136 2023-06-15 08:20:08.000000 thipster-0.17.0/thipster/engine/resource_model.py
+-rw-r--r--   0 root         (0) root         (0)      654 2023-06-15 08:20:08.000000 thipster-0.17.0/thipster/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 08:20:12.312229 thipster-0.17.0/thipster/parser/
+-rw-r--r--   0 root         (0) root         (0)      364 2023-06-15 08:20:08.000000 thipster-0.17.0/thipster/parser/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 08:20:12.316229 thipster-0.17.0/thipster/parser/dsl_parser/
+-rw-r--r--   0 root         (0) root         (0)       30 2023-06-15 08:20:08.000000 thipster-0.17.0/thipster/parser/dsl_parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9156 2023-06-15 08:20:08.000000 thipster-0.17.0/thipster/parser/dsl_parser/ast.py
+-rw-r--r--   0 root         (0) root         (0)     2925 2023-06-15 08:20:08.000000 thipster-0.17.0/thipster/parser/dsl_parser/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)    13471 2023-06-15 08:20:08.000000 thipster-0.17.0/thipster/parser/dsl_parser/interpreter.py
+-rw-r--r--   0 root         (0) root         (0)    17264 2023-06-15 08:20:08.000000 thipster-0.17.0/thipster/parser/dsl_parser/lexer.py
+-rw-r--r--   0 root         (0) root         (0)     4771 2023-06-15 08:20:08.000000 thipster-0.17.0/thipster/parser/dsl_parser/lexer_position.py
+-rw-r--r--   0 root         (0) root         (0)     1985 2023-06-15 08:20:08.000000 thipster-0.17.0/thipster/parser/dsl_parser/parser.py
+-rw-r--r--   0 root         (0) root         (0)     2085 2023-06-15 08:20:08.000000 thipster-0.17.0/thipster/parser/dsl_parser/token.py
+-rw-r--r--   0 root         (0) root         (0)    20105 2023-06-15 08:20:08.000000 thipster-0.17.0/thipster/parser/dsl_parser/token_parser.py
+-rw-r--r--   0 root         (0) root         (0)     2474 2023-06-15 08:20:08.000000 thipster-0.17.0/thipster/parser/parser_factory.py
+-rw-r--r--   0 root         (0) root         (0)     6556 2023-06-15 08:20:08.000000 thipster-0.17.0/thipster/parser/yaml_parser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 08:20:12.316229 thipster-0.17.0/thipster/repository/
+-rw-r--r--   0 root         (0) root         (0)      332 2023-06-15 08:20:08.000000 thipster-0.17.0/thipster/repository/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      293 2023-06-15 08:20:08.000000 thipster-0.17.0/thipster/repository/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     1399 2023-06-15 08:20:08.000000 thipster-0.17.0/thipster/repository/github.py
+-rw-r--r--   0 root         (0) root         (0)     4653 2023-06-15 08:20:08.000000 thipster-0.17.0/thipster/repository/json.py
+-rw-r--r--   0 root         (0) root         (0)      475 2023-06-15 08:20:08.000000 thipster-0.17.0/thipster/repository/local.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 08:20:12.316229 thipster-0.17.0/thipster/terraform/
+-rw-r--r--   0 root         (0) root         (0)      327 2023-06-15 08:20:08.000000 thipster-0.17.0/thipster/terraform/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22571 2023-06-15 08:20:08.000000 thipster-0.17.0/thipster/terraform/cdk.py
+-rw-r--r--   0 root         (0) root         (0)     1237 2023-06-15 08:20:08.000000 thipster-0.17.0/thipster/terraform/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 08:20:12.312229 thipster-0.17.0/thipster.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5156 2023-06-15 08:20:12.000000 thipster-0.17.0/thipster.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1774 2023-06-15 08:20:12.000000 thipster-0.17.0/thipster.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-15 08:20:12.000000 thipster-0.17.0/thipster.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      390 2023-06-15 08:20:12.000000 thipster-0.17.0/thipster.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-06-15 08:20:12.000000 thipster-0.17.0/thipster.egg-info/top_level.txt
```

### Comparing `thipster-0.16.7/LICENSE` & `thipster-0.17.0/LICENSE`

 * *Files identical despite different names*

### Comparing `thipster-0.16.7/PKG-INFO` & `thipster-0.17.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thipster
-Version: 0.16.7
+Version: 0.17.0
 Summary: THipster is a tool dedicated to simplifying the difficulty associated with writing Terraform files. It allows users to write infrastructure as code in a simplified format, using either YAML (with JINJA) or the dedicated Thipster DSL.
 Home-page: https://github.com/THipster/THipster
 Download-URL: https://github.com/THipster/THipster.git
 Keywords: thipster,terraform,infrastructure,infrastructure-as-code,iac,generator,dsl,yaml
 Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: thipster Version: 0.16.7 Summary: THipster is a
+Metadata-Version: 2.1 Name: thipster Version: 0.17.0 Summary: THipster is a
 tool dedicated to simplifying the difficulty associated with writing Terraform
 files. It allows users to write infrastructure as code in a simplified format,
 using either YAML (with JINJA) or the dedicated Thipster DSL. Home-page: https:
 //github.com/THipster/THipster Download-URL: https://github.com/THipster/
 THipster.git Keywords: thipster,terraform,infrastructure,infrastructure-as-
 code,iac,generator,dsl,yaml Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python :: 3.11 Classifier: License :: OSI
```

### Comparing `thipster-0.16.7/README.md` & `thipster-0.17.0/README.md`

 * *Files identical despite different names*

### Comparing `thipster-0.16.7/pyproject.toml` & `thipster-0.17.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `thipster-0.16.7/setup.py` & `thipster-0.17.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import find_packages, setup
 
-__version__ = '0.16.7'
+__version__ = '0.17.0'
 
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 with open('README.md') as rm:
     readme = rm.read()
```

### Comparing `thipster-0.16.7/tests/engine/test_engine.py` & `thipster-0.17.0/tests/engine/test_engine.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.7/tests/engine/test_generation.py` & `thipster-0.17.0/tests/engine/test_generation.py`

 * *Files 7% similar despite different names*

```diff
@@ -222,7 +222,36 @@
     assert_number_of_resource_type_is('google_storage_bucket', 1)
     bucket = assert_resource_created('google_storage_bucket', bucket_name)
     cors_block = get_resource_parameter(bucket, 'cors')
 
     assert len(cors_block) == 2
 
     clean_up()
+
+
+def test_subnetwork_in_network():
+    function_name = get_function_name()
+
+    network_name = f'network-{uuid.uuid4().int}'
+    clean_up = process_file(
+        directory=function_name,
+        file=f"""
+network:
+  name: {network_name}
+  auto_create_subnetworks: false
+  subnetwork:
+    - region: europe-west1
+      ip_range: 10.0.1.0/24
+    - region: us-west1
+      ip_range: 10.0.2.0/24
+""",
+        file_type='yaml',
+        mock_auth=True,
+    )
+
+    # Assertions on plan
+    assert_number_of_resource_type_is('google_compute_network', 1)
+    assert_resource_created('google_compute_network', network_name)
+
+    assert_number_of_resource_type_is('google_compute_subnetwork', 2)
+
+    clean_up()
```

### Comparing `thipster-0.16.7/tests/parser/dsl_parser/test_DSLparser.py` & `thipster-0.17.0/tests/parser/dsl_parser/test_DSLparser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.7/tests/parser/dsl_parser/test_ast.py` & `thipster-0.17.0/tests/parser/dsl_parser/test_ast.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.7/tests/parser/dsl_parser/test_lexer.py` & `thipster-0.17.0/tests/parser/dsl_parser/test_lexer.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.7/tests/parser/dsl_parser/test_token.py` & `thipster-0.17.0/tests/parser/dsl_parser/test_token.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.7/tests/parser/dsl_parser/test_tokenparser.py` & `thipster-0.17.0/tests/parser/dsl_parser/test_tokenparser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.7/tests/parser/test_ParserFactory.py` & `thipster-0.17.0/tests/parser/test_ParserFactory.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.7/tests/parser/test_YAMLParser.py` & `thipster-0.17.0/tests/parser/test_YAMLParser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.7/tests/parser/test_parsedfile.py` & `thipster-0.17.0/tests/parser/test_parsedfile.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.7/tests/test_e2e.py` & `thipster-0.17.0/tests/test_e2e.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,15 +97,15 @@
         clean_up()
 
 
 def test_lb(apply_output, authentication):
     _ = authentication
     function_name = get_function_name()
 
-    test_id = random.randint(0, 1000)
+    test_id = random.randint(0, 10000)
     clean_up = process_file(
         directory=function_name,
         file=f"""
 network lb-net-{test_id}:
 
 subnetwork lb-subnet-{test_id}:
 \tnetwork: lb-net-{test_id}
```

### Comparing `thipster-0.16.7/tests/test_tools.py` & `thipster-0.17.0/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.7/thipster/auth/google.py` & `thipster-0.17.0/thipster/auth/google.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.7/thipster/engine/engine.py` & `thipster-0.17.0/thipster/engine/engine.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.7/thipster/engine/i_parser.py` & `thipster-0.17.0/thipster/engine/i_parser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.7/thipster/engine/i_repository.py` & `thipster-0.17.0/thipster/engine/i_repository.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.7/thipster/engine/i_terraform.py` & `thipster-0.17.0/thipster/engine/i_terraform.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.7/thipster/engine/parsed_file.py` & `thipster-0.17.0/thipster/engine/parsed_file.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.7/thipster/engine/resource_model.py` & `thipster-0.17.0/thipster/engine/resource_model.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.7/thipster/helpers.py` & `thipster-0.17.0/thipster/helpers.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.7/thipster/parser/dsl_parser/ast.py` & `thipster-0.17.0/thipster/parser/dsl_parser/ast.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.7/thipster/parser/dsl_parser/exceptions.py` & `thipster-0.17.0/thipster/parser/dsl_parser/exceptions.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.7/thipster/parser/dsl_parser/interpreter.py` & `thipster-0.17.0/thipster/parser/dsl_parser/interpreter.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.7/thipster/parser/dsl_parser/lexer.py` & `thipster-0.17.0/thipster/parser/dsl_parser/lexer.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.7/thipster/parser/dsl_parser/lexer_position.py` & `thipster-0.17.0/thipster/parser/dsl_parser/lexer_position.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.7/thipster/parser/dsl_parser/parser.py` & `thipster-0.17.0/thipster/parser/dsl_parser/parser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.7/thipster/parser/dsl_parser/token.py` & `thipster-0.17.0/thipster/parser/dsl_parser/token.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.7/thipster/parser/dsl_parser/token_parser.py` & `thipster-0.17.0/thipster/parser/dsl_parser/token_parser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.7/thipster/parser/parser_factory.py` & `thipster-0.17.0/thipster/parser/parser_factory.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.7/thipster/parser/yaml_parser.py` & `thipster-0.17.0/thipster/parser/yaml_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,30 +77,30 @@
         Returns
         -------
         ParsedFile
             A ParsedFile object with the content of all the files in the input path
         """
         try:
             files = cls.__getfiles(path)
-            parsedFile = pf.ParsedFile()
+            parsed_file = pf.ParsedFile()
 
             for file in files:
                 filedir, filename = os.path.split(file)
 
                 environment = Environment(
                     loader=FileSystemLoader(filedir),
                     autoescape=True,
                 )
                 template = environment.get_template(filename)
                 rendered = template.render()
                 content = yaml.safe_load(rendered)
 
-                parsedFile.resources += cls.__convert(content)
+                parsed_file.resources += cls.__convert(content)
 
-            return parsedFile
+            return parsed_file
         except yaml.YAMLError as exc:
             raise exc
         except YAMLParserBaseException as e:
             raise e
         except Exception as e:
             raise e
 
@@ -127,34 +127,34 @@
                         name = res['name']
                         del res['name']
                     else:
                         raise YAMLParserNoName(key)
 
                     resources.append(
                         cls.__get_resource(
-                            content=res, resourceType=key, name=name,
+                            content=res, resource_type=key, name=name,
                         ),
                     )
             elif type(val) == dict:
                 if 'name' in val:
                     name = val['name']
                     del val['name']
                 else:
                     raise YAMLParserNoName(key)
 
                 resources.append(
                     cls.__get_resource(
-                        content=val, resourceType=key, name=name,
+                        content=val, resource_type=key, name=name,
                     ),
                 )
 
         return resources
 
     @classmethod
-    def __get_resource(cls, content: dict, resourceType: str, name: str)\
+    def __get_resource(cls, content: dict, resource_type: str, name: str)\
             -> pf.ParsedResource:
         """Converts a dict in a ParsedResource
 
         Parameters
         ----------
         content: dict
             Dict of attributes of the resource
@@ -170,15 +170,15 @@
         """
         attr = []
 
         for key, val in content.items():
             attr.append(cls.__get__attr(key, val))
 
         return pf.ParsedResource(
-            type=resourceType,
+            type=resource_type,
             name=name,
             position=None,
             attributes=attr,
         )
 
     @classmethod
     def __get__attr(cls, name: str, value: object) -> pf.ParsedAttribute:
```

### Comparing `thipster-0.16.7/thipster/repository/github.py` & `thipster-0.17.0/thipster/repository/github.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.7/thipster/repository/json.py` & `thipster-0.17.0/thipster/repository/json.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.7/thipster/terraform/cdk.py` & `thipster-0.17.0/thipster/terraform/cdk.py`

 * *Files 21% similar despite different names*

```diff
@@ -10,24 +10,30 @@
 from constructs import Construct
 from python_terraform import Terraform
 
 import thipster.engine.parsed_file as pf
 import thipster.engine.resource_model as rm
 import thipster.terraform.exceptions as cdk_exceptions
 from thipster.engine import I_Auth, I_Terraform
-from thipster.helpers import create_logger as Logger
+from thipster.helpers import create_logger
+
+
+class ResourceCreationContext():
+    def __init__(self) -> None:
+        pass
 
 
 class CDK(I_Terraform):
     _models = []
     _parent_resources_stack = []
+    _resources_to_create = []
 
     _inherited_attributes: list[pf.ParsedAttribute] = []
     _created_resources = {}
-    _logger = Logger(__name__)
+    _logger = create_logger(__name__)
 
     @classmethod
     def apply(cls, plan_file_path: str | None = None):
         """Applies generated Terraform plan
 
         Parameters
         ----------
@@ -179,31 +185,35 @@
         class_ = getattr(module, class_name)
 
         return class_
 
 
 def _create_default_resource(
     resource_self, resource_type: str, parent_name: str | None = None,
-    no_modif: bool = True, no_dependencies: bool = False,
+    no_modif: bool = True, no_dependencies: bool = False, arg_to_complete: str = None,
 ):
     """Create a resource with all default values
 
     Parameters
     ----------
     self : _ResourceStack
         Terraform CDK stack that contains the resource
     resource_type : str
         type of the resource to create
+    parent_name : str
+        name of the parent resource
     parent_name : str, optional
         name of its parent, default None
     no_modif : bool, optional
         if True, raise errors if resource can't be created with default values, \
 default False
     no_dependencies : bool, optional
         if True, create the default dependencies, default False
+    arg_to_complete: str
+        name of the argument that will get a value after parent resource creation
 
     Returns
     -------
     (type, str, dict[str, object]) :
         all the information needed to instantiate the class with default values
     """
     # Checks for cyclic dependency
@@ -241,15 +251,15 @@
     # Import package and class
     CDK._pip_install(model.cdk_provider)
     resource_class = CDK._import(
         model.cdk_provider, model.cdk_module, model.cdk_name,
     )
 
     # Process name + default values
-    dependencies = copy.deepcopy(model.dependencies)
+    dependencies = _get_dependency_list(model, arg_to_complete)
     resource_args = {}
 
     name = f'{parent_name}-{uuid.uuid4()}'
     if model.name_key:
         resource_args[model.name_key] = name
 
     for attribute_name, attribute_value in attributes.items():
@@ -273,76 +283,95 @@
         )
 
     CDK._logger.debug('Created default %s named %s', resource_class, name)
 
     return (resource_class, name, resource_args)
 
 
-def _create_resource(resource_self, resource_args: object, resource_type: str = None):
+def _create_resource(
+        resource_self, resource_args: object, parent_name: str,
+        resource_type: str = None, arg_to_complete: bool = True,
+):
     """Create a resource with the given values
 
     Parameters
     ----------
     self : _ResourceStack
         Terraform CDK stack that contains the resource
     resource_args : object
         data source to create the resource
+    parent_name : str
+        name of the parent resource
     resource_type : str, optional
         type of the resource to create, default None
+    arg_to_complete: str
+        name of the argument that will get a value after parent resource creation
 
     Returns
     -------
     object :
         the created resource
     """
 
     if isinstance(resource_args, pf.ParsedResource):
-        return _create_resource_from_resource(resource_self, resource_args)
+        return _create_resource_from_resource(
+            resource_self, resource_args, parent_name, arg_to_complete,
+        )
 
-    return _create_resource_from_args(resource_self, resource_type, resource_args)
+    return _create_resource_from_args(
+        resource_self, resource_type, parent_name, resource_args, arg_to_complete,
+    )
 
 
 def _create_resource_from_args(
-    resource_self, resource_type: str, input_args: list[pf.ParsedAttribute] | None,
+    resource_self, resource_type: str, parent_name: str,
+    input_args: list[pf.ParsedAttribute] | None, arg_to_complete: str = None,
 ):
     """Create a resource from a list of ParsedAttributes
 
     Parameters
     ----------
     self : _ResourceStack
         Terraform CDK stack that contains the resource
     resource_type : str, optional
         type of the resource to create, default None
+    parent_name : str
+        name of the parent resource
     input_args : list[ParsedAttribute]
         data source to create the resource
+    arg_to_complete: str
+        name of the argument that will get a value after parent resource creation
 
     Returns
     -------
     object :
         the created resource
     """
     resource_class, resource_name, resource_args = _create_default_resource(
         resource_self,
         resource_type,
+        parent_name=parent_name,
         no_modif=False,
         no_dependencies=True,
+        arg_to_complete=arg_to_complete,
     )
     model = CDK._models[resource_type]
 
     # Process attributes
-    dependencies = copy.deepcopy(model.dependencies)
+    dependencies = _get_dependency_list(model, arg_to_complete)
 
     def attributes(attribute_list):
         for attribute in attribute_list:
-            if attribute.name and model.name_key:
+            if attribute.name == model.name_key:
                 resource_args[model.name_key] = attribute.name
-
-            _process_attribute(
-                resource_self, model, attribute, resource_args, dependencies,
-            )
+            else:
+                _process_attribute(
+                    resource_self, model,
+                    attribute, resource_args, dependencies, parent_name,
+                )
 
     attributes(input_args)
     attributes(CDK._inherited_attributes)
 
     CDK._inherited_attributes += input_args
     _generate_default_dependencies(
         resource_self, dependencies, model, resource_args, resource_name,
@@ -357,57 +386,86 @@
     CDK._parent_resources_stack.remove(resource_type)
 
     CDK._logger.debug(
         'Created default %s named %s',
         resource_class, resource_name,
     )
 
-    if not model.name_key:
-        return resource_class(**resource_args)
-    return resource_class(resource_self, resource_name, **resource_args)
+    if not arg_to_complete:
+        if not model.name_key:
+            class_ = resource_class(**resource_args)
+        else:
+            class_ = resource_class(
+                resource_self, resource_name, **resource_args,
+            )
+
+        while len(CDK._resources_to_create) != 0:
+            to_create_class, to_create_name, to_create_args, to_create_complete = \
+                CDK._resources_to_create.pop()
+            to_create_args[to_create_complete] = class_.id
 
+            to_create_class(
+                resource_self, to_create_name, **to_create_args,
+            )
+        return class_
 
-def _create_resource_from_resource(resource_self, resource: pf.ParsedResource):
-    # Create resource with default values
-    resource_class, _, resource_args = _create_default_resource(
-        resource_self,
-        resource.resource_type,
-        no_modif=False,
-        no_dependencies=True,
+    CDK._resources_to_create.append(
+        (resource_class, resource_name, resource_args, arg_to_complete),
     )
+
+
+def _create_resource_from_resource(
+        resource_self, resource: pf.ParsedResource,
+        parent_name: str = None, arg_to_complete: str = None,
+):
     """Create a resource from a list of ParsedAttributes
 
     Parameters
     ----------
-    self : _ResourceStack
+    resource_self : _ResourceStack
         Terraform CDK stack that contains the resource
     resource : ParsedResource
         data source to create the resource
+    parent_name : str
+        name of the parent resource
+    arg_to_complete: str
+        name of the argument that will get a value after parent resource creation
 
     Returns
     -------
     object :
         the created resource
     """
+
+    # Create resource with default values
+    resource_class, _, resource_args = _create_default_resource(
+        resource_self,
+        resource.resource_type,
+        parent_name=parent_name,
+        no_modif=False,
+        no_dependencies=True,
+        arg_to_complete=arg_to_complete,
+    )
     model = CDK._models[resource.resource_type]
 
     if model.name_key:
         resource_args[model.name_key] = resource.name
 
     # Process attributes
-    dependencies = copy.deepcopy(model.dependencies)
+    dependencies = _get_dependency_list(model, arg_to_complete)
 
     def attributes(attribute_list):
         for attribute in attribute_list:
             _process_attribute(
                 resource_self,
                 model,
                 attribute,
                 resource_args,
                 dependencies,
+                resource.name,
             )
 
     attributes(resource.attributes)
     attributes(CDK._inherited_attributes)
 
     CDK._inherited_attributes += resource.attributes
     _generate_default_dependencies(
@@ -423,38 +481,62 @@
     CDK._parent_resources_stack.remove(resource.resource_type)
 
     CDK._logger.debug(
         'Created resource %s named %s',
         resource_class, resource.name,
     )
 
-    return resource_class(resource_self, resource.name, **resource_args)
+    if not arg_to_complete:
+        if not model.name_key:
+            class_ = resource_class(**resource_args)
+        else:
+            class_ = resource_class(
+                resource_self, resource.name, **resource_args,
+            )
+
+        while len(CDK._resources_to_create) != 0:
+            to_create_class, to_create_name, to_create_args, to_create_complete = \
+                CDK._resources_to_create.pop()
+            to_create_args[to_create_complete] = class_.id
+
+            to_create_class(
+                resource_self, to_create_name, **to_create_args,
+            )
+        return class_
+
+    CDK._resources_to_create.append(
+        (resource_class, resource.name, resource_args, arg_to_complete),
+    )
+    return True
 
 
 def _process_attribute(
     resource_self,
     model: rm.ResourceModel,
     attribute: pf.ParsedAttribute,
     resource_args: dict[str, object],
     dependencies: dict[str, dict[str, object]] | None,
+    parent_name: str,
 ):
     """Process an attribute
 
     Parameters
     ----------
-    self : _ResourceStack
+    resource_self : _ResourceStack
         Terraform CDK stack that contains the resource
     model : ResourceModel
         model of the resource that is being created
     attribute : ParsedAttribute
         attribute to handle
     resource_args : object
         data source needed to create the resource
     dependencies : dict[str, dict[str, object]]
         dependencies needed to create the resource
+    parent_name : str
+        name of the parent resource
     """
     if attribute.name in dependencies:
         _check_explicit_dependency(
             resource_self, resource_args, dependencies[attribute.name]['resource'],
             attribute.value, attribute.name,
         )
         del dependencies[attribute.name]
@@ -464,14 +546,15 @@
     if attribute.name in model.internal_objects:
         _create_internal_object(
             resource_self,
             attribute.name,
             model.internal_objects[attribute.name],
             attribute.value,
             resource_args,
+            parent_name,
         )
         return
 
     # Checks if attribute is expected as an attibute
     if attribute.name not in model.attributes:
         return
 
@@ -532,75 +615,96 @@
 
                 _create_internal_object(
                     resource_self,
                     internal_object_name,
                     model.internal_objects[internal_object_name],
                     default_args,
                     resource_args,
+                    resource_name,
                 )
 
 
 def _create_internal_object(
     resource_self,
     name: str,
-    internal_object_model,
+    internal_object_model: dict,
     internal_object_args,
     resource_args: dict,
+    parent_name: str,
 ):
     """Create an internal object in a resource
 
     Parameters
     ----------
-    self : _ResourceStack
+    resource_self : _ResourceStack
         Terraform CDK stack that contains the resource
     name : str
         name of the internal object
     internal_object_model : ResourceModel
         model of the internal object
     internal_object_args : object
         data source to create the internal object
     resource_args : dict
         data source needed to create the resource
+    parent_name : str
+        name of the parent resource
     """
     internal_object_type = internal_object_model['var_type'] \
         if 'var_type' in internal_object_model else 'Unknown'
 
+    arg_to_complete = internal_object_model.get('arg_to_complete')
+
     if internal_object_type.startswith('list'):
-        if name not in resource_args:
+        if name not in resource_args and not arg_to_complete:
             resource_args[name] = []
 
         if isinstance(internal_object_args, list) \
                 and isinstance(internal_object_args[0], pf.ParsedDict):
 
-            for internalObject in internal_object_args:
+            for internal_object in internal_object_args:
                 res = _create_resource(
                     resource_self,
-                    internalObject.value,
+                    internal_object.value,
+                    parent_name,
                     internal_object_model['resource'],
+                    arg_to_complete=arg_to_complete,
                 )
-                resource_args[name] += [res]
-
-            return
+                if not arg_to_complete:
+                    resource_args[name] += [res]
+            return True
 
         res = _create_resource(
             resource_self,
             internal_object_args,
+            parent_name,
             internal_object_model['resource'],
+            arg_to_complete=arg_to_complete,
         )
-        resource_args[name] += [res]
-        return
+        if not arg_to_complete:
+            resource_args[name] += [res]
+        return True
 
     res = _create_resource(
         resource_self,
         internal_object_args,
+        parent_name,
         internal_object_model['resource'],
+        arg_to_complete=arg_to_complete,
     )
-    resource_args[name] = res
+    if not arg_to_complete:
+        resource_args[name] = res
 
-    return
+    return True
+
+
+def _get_dependency_list(model, arg_to_complete):
+    dependencies = copy.deepcopy(model.dependencies)
+    if arg_to_complete in dependencies.keys():
+        del dependencies[arg_to_complete]
+    return dependencies
 
 
 def _create_dependency(resource_self, dep_name, dep_value, resource_args, parent_name):
     """Create an internal object in a resource
 
     Parameters
     ----------
```

### Comparing `thipster-0.16.7/thipster/terraform/exceptions.py` & `thipster-0.17.0/thipster/terraform/exceptions.py`

 * *Files identical despite different names*

### Comparing `thipster-0.16.7/thipster.egg-info/PKG-INFO` & `thipster-0.17.0/thipster.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thipster
-Version: 0.16.7
+Version: 0.17.0
 Summary: THipster is a tool dedicated to simplifying the difficulty associated with writing Terraform files. It allows users to write infrastructure as code in a simplified format, using either YAML (with JINJA) or the dedicated Thipster DSL.
 Home-page: https://github.com/THipster/THipster
 Download-URL: https://github.com/THipster/THipster.git
 Keywords: thipster,terraform,infrastructure,infrastructure-as-code,iac,generator,dsl,yaml
 Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: thipster Version: 0.16.7 Summary: THipster is a
+Metadata-Version: 2.1 Name: thipster Version: 0.17.0 Summary: THipster is a
 tool dedicated to simplifying the difficulty associated with writing Terraform
 files. It allows users to write infrastructure as code in a simplified format,
 using either YAML (with JINJA) or the dedicated Thipster DSL. Home-page: https:
 //github.com/THipster/THipster Download-URL: https://github.com/THipster/
 THipster.git Keywords: thipster,terraform,infrastructure,infrastructure-as-
 code,iac,generator,dsl,yaml Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python :: 3.11 Classifier: License :: OSI
```

### Comparing `thipster-0.16.7/thipster.egg-info/SOURCES.txt` & `thipster-0.17.0/thipster.egg-info/SOURCES.txt`

 * *Files identical despite different names*

