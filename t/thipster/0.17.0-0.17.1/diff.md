# Comparing `tmp/thipster-0.17.0.tar.gz` & `tmp/thipster-0.17.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thipster-0.17.0.tar", last modified: Thu Jun 15 08:20:12 2023, max compression
+gzip compressed data, was "thipster-0.17.1.tar", last modified: Thu Jun 15 12:01:58 2023, max compression
```

## Comparing `thipster-0.17.0.tar` & `thipster-0.17.1.tar`

### file list

```diff
@@ -1,75 +1,76 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 08:20:12.316229 thipster-0.17.0/
--rw-r--r--   0 root         (0) root         (0)     1052 2023-06-15 08:20:08.000000 thipster-0.17.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       81 2023-06-15 08:20:08.000000 thipster-0.17.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     5156 2023-06-15 08:20:12.316229 thipster-0.17.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4324 2023-06-15 08:20:08.000000 thipster-0.17.0/README.md
--rw-r--r--   0 root         (0) root         (0)      986 2023-06-15 08:20:08.000000 thipster-0.17.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       82 2023-06-15 08:20:08.000000 thipster-0.17.0/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-15 08:20:12.316229 thipster-0.17.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1985 2023-06-15 08:20:08.000000 thipster-0.17.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 08:20:12.308229 thipster-0.17.0/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-15 08:20:08.000000 thipster-0.17.0/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 08:20:12.308229 thipster-0.17.0/tests/engine/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-15 08:20:08.000000 thipster-0.17.0/tests/engine/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3202 2023-06-15 08:20:08.000000 thipster-0.17.0/tests/engine/test_engine.py
--rw-r--r--   0 root         (0) root         (0)     5360 2023-06-15 08:20:08.000000 thipster-0.17.0/tests/engine/test_generation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 08:20:12.308229 thipster-0.17.0/tests/parser/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-15 08:20:08.000000 thipster-0.17.0/tests/parser/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 08:20:12.308229 thipster-0.17.0/tests/parser/dsl_parser/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-15 08:20:08.000000 thipster-0.17.0/tests/parser/dsl_parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15286 2023-06-15 08:20:08.000000 thipster-0.17.0/tests/parser/dsl_parser/test_DSLparser.py
--rw-r--r--   0 root         (0) root         (0)     1359 2023-06-15 08:20:08.000000 thipster-0.17.0/tests/parser/dsl_parser/test_ast.py
--rw-r--r--   0 root         (0) root         (0)    13297 2023-06-15 08:20:08.000000 thipster-0.17.0/tests/parser/dsl_parser/test_lexer.py
--rw-r--r--   0 root         (0) root         (0)      865 2023-06-15 08:20:08.000000 thipster-0.17.0/tests/parser/dsl_parser/test_token.py
--rw-r--r--   0 root         (0) root         (0)     3524 2023-06-15 08:20:08.000000 thipster-0.17.0/tests/parser/dsl_parser/test_tokenparser.py
--rw-r--r--   0 root         (0) root         (0)     2405 2023-06-15 08:20:08.000000 thipster-0.17.0/tests/parser/test_ParserFactory.py
--rw-r--r--   0 root         (0) root         (0)     4369 2023-06-15 08:20:08.000000 thipster-0.17.0/tests/parser/test_YAMLParser.py
--rw-r--r--   0 root         (0) root         (0)     4701 2023-06-15 08:20:08.000000 thipster-0.17.0/tests/parser/test_parsedfile.py
--rw-r--r--   0 root         (0) root         (0)     3305 2023-06-15 08:20:08.000000 thipster-0.17.0/tests/test_e2e.py
--rw-r--r--   0 root         (0) root         (0)     4150 2023-06-15 08:20:08.000000 thipster-0.17.0/tests/test_tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 08:20:12.308229 thipster-0.17.0/thipster/
--rw-r--r--   0 root         (0) root         (0)      171 2023-06-15 08:20:08.000000 thipster-0.17.0/thipster/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 08:20:12.312229 thipster-0.17.0/thipster/auth/
--rw-r--r--   0 root         (0) root         (0)      215 2023-06-15 08:20:08.000000 thipster-0.17.0/thipster/auth/__init__.py
--rw-r--r--   0 root         (0) root         (0)      903 2023-06-15 08:20:08.000000 thipster-0.17.0/thipster/auth/google.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 08:20:12.312229 thipster-0.17.0/thipster/engine/
--rw-r--r--   0 root         (0) root         (0)      411 2023-06-15 08:20:08.000000 thipster-0.17.0/thipster/engine/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5079 2023-06-15 08:20:08.000000 thipster-0.17.0/thipster/engine/engine.py
--rw-r--r--   0 root         (0) root         (0)      247 2023-06-15 08:20:08.000000 thipster-0.17.0/thipster/engine/exceptions.py
--rw-r--r--   0 root         (0) root         (0)      410 2023-06-15 08:20:08.000000 thipster-0.17.0/thipster/engine/i_auth.py
--rw-r--r--   0 root         (0) root         (0)      735 2023-06-15 08:20:08.000000 thipster-0.17.0/thipster/engine/i_parser.py
--rw-r--r--   0 root         (0) root         (0)      597 2023-06-15 08:20:08.000000 thipster-0.17.0/thipster/engine/i_repository.py
--rw-r--r--   0 root         (0) root         (0)     1911 2023-06-15 08:20:08.000000 thipster-0.17.0/thipster/engine/i_terraform.py
--rw-r--r--   0 root         (0) root         (0)     4368 2023-06-15 08:20:08.000000 thipster-0.17.0/thipster/engine/parsed_file.py
--rw-r--r--   0 root         (0) root         (0)     3136 2023-06-15 08:20:08.000000 thipster-0.17.0/thipster/engine/resource_model.py
--rw-r--r--   0 root         (0) root         (0)      654 2023-06-15 08:20:08.000000 thipster-0.17.0/thipster/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 08:20:12.312229 thipster-0.17.0/thipster/parser/
--rw-r--r--   0 root         (0) root         (0)      364 2023-06-15 08:20:08.000000 thipster-0.17.0/thipster/parser/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 08:20:12.316229 thipster-0.17.0/thipster/parser/dsl_parser/
--rw-r--r--   0 root         (0) root         (0)       30 2023-06-15 08:20:08.000000 thipster-0.17.0/thipster/parser/dsl_parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9156 2023-06-15 08:20:08.000000 thipster-0.17.0/thipster/parser/dsl_parser/ast.py
--rw-r--r--   0 root         (0) root         (0)     2925 2023-06-15 08:20:08.000000 thipster-0.17.0/thipster/parser/dsl_parser/exceptions.py
--rw-r--r--   0 root         (0) root         (0)    13471 2023-06-15 08:20:08.000000 thipster-0.17.0/thipster/parser/dsl_parser/interpreter.py
--rw-r--r--   0 root         (0) root         (0)    17264 2023-06-15 08:20:08.000000 thipster-0.17.0/thipster/parser/dsl_parser/lexer.py
--rw-r--r--   0 root         (0) root         (0)     4771 2023-06-15 08:20:08.000000 thipster-0.17.0/thipster/parser/dsl_parser/lexer_position.py
--rw-r--r--   0 root         (0) root         (0)     1985 2023-06-15 08:20:08.000000 thipster-0.17.0/thipster/parser/dsl_parser/parser.py
--rw-r--r--   0 root         (0) root         (0)     2085 2023-06-15 08:20:08.000000 thipster-0.17.0/thipster/parser/dsl_parser/token.py
--rw-r--r--   0 root         (0) root         (0)    20105 2023-06-15 08:20:08.000000 thipster-0.17.0/thipster/parser/dsl_parser/token_parser.py
--rw-r--r--   0 root         (0) root         (0)     2474 2023-06-15 08:20:08.000000 thipster-0.17.0/thipster/parser/parser_factory.py
--rw-r--r--   0 root         (0) root         (0)     6556 2023-06-15 08:20:08.000000 thipster-0.17.0/thipster/parser/yaml_parser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 08:20:12.316229 thipster-0.17.0/thipster/repository/
--rw-r--r--   0 root         (0) root         (0)      332 2023-06-15 08:20:08.000000 thipster-0.17.0/thipster/repository/__init__.py
--rw-r--r--   0 root         (0) root         (0)      293 2023-06-15 08:20:08.000000 thipster-0.17.0/thipster/repository/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     1399 2023-06-15 08:20:08.000000 thipster-0.17.0/thipster/repository/github.py
--rw-r--r--   0 root         (0) root         (0)     4653 2023-06-15 08:20:08.000000 thipster-0.17.0/thipster/repository/json.py
--rw-r--r--   0 root         (0) root         (0)      475 2023-06-15 08:20:08.000000 thipster-0.17.0/thipster/repository/local.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 08:20:12.316229 thipster-0.17.0/thipster/terraform/
--rw-r--r--   0 root         (0) root         (0)      327 2023-06-15 08:20:08.000000 thipster-0.17.0/thipster/terraform/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22571 2023-06-15 08:20:08.000000 thipster-0.17.0/thipster/terraform/cdk.py
--rw-r--r--   0 root         (0) root         (0)     1237 2023-06-15 08:20:08.000000 thipster-0.17.0/thipster/terraform/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 08:20:12.312229 thipster-0.17.0/thipster.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5156 2023-06-15 08:20:12.000000 thipster-0.17.0/thipster.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1774 2023-06-15 08:20:12.000000 thipster-0.17.0/thipster.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-15 08:20:12.000000 thipster-0.17.0/thipster.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      390 2023-06-15 08:20:12.000000 thipster-0.17.0/thipster.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-06-15 08:20:12.000000 thipster-0.17.0/thipster.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 12:01:58.978078 thipster-0.17.1/
+-rw-r--r--   0 root         (0) root         (0)     1052 2023-06-15 12:01:55.000000 thipster-0.17.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       81 2023-06-15 12:01:55.000000 thipster-0.17.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     5156 2023-06-15 12:01:58.978078 thipster-0.17.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4324 2023-06-15 12:01:55.000000 thipster-0.17.1/README.md
+-rw-r--r--   0 root         (0) root         (0)      995 2023-06-15 12:01:55.000000 thipster-0.17.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       82 2023-06-15 12:01:55.000000 thipster-0.17.1/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-15 12:01:58.978078 thipster-0.17.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1985 2023-06-15 12:01:55.000000 thipster-0.17.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 12:01:58.970078 thipster-0.17.1/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-15 12:01:55.000000 thipster-0.17.1/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 12:01:58.970078 thipster-0.17.1/tests/engine/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-15 12:01:55.000000 thipster-0.17.1/tests/engine/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3196 2023-06-15 12:01:55.000000 thipster-0.17.1/tests/engine/test_engine.py
+-rw-r--r--   0 root         (0) root         (0)     5390 2023-06-15 12:01:55.000000 thipster-0.17.1/tests/engine/test_generation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 12:01:58.970078 thipster-0.17.1/tests/parser/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-15 12:01:55.000000 thipster-0.17.1/tests/parser/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 12:01:58.974078 thipster-0.17.1/tests/parser/dsl_parser/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-15 12:01:55.000000 thipster-0.17.1/tests/parser/dsl_parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1359 2023-06-15 12:01:55.000000 thipster-0.17.1/tests/parser/dsl_parser/test_ast.py
+-rw-r--r--   0 root         (0) root         (0)    15280 2023-06-15 12:01:55.000000 thipster-0.17.1/tests/parser/dsl_parser/test_dslparser.py
+-rw-r--r--   0 root         (0) root         (0)    13619 2023-06-15 12:01:55.000000 thipster-0.17.1/tests/parser/dsl_parser/test_lexer.py
+-rw-r--r--   0 root         (0) root         (0)      876 2023-06-15 12:01:55.000000 thipster-0.17.1/tests/parser/dsl_parser/test_token.py
+-rw-r--r--   0 root         (0) root         (0)     3524 2023-06-15 12:01:55.000000 thipster-0.17.1/tests/parser/dsl_parser/test_tokenparser.py
+-rw-r--r--   0 root         (0) root         (0)     4697 2023-06-15 12:01:55.000000 thipster-0.17.1/tests/parser/test_parsedfile.py
+-rw-r--r--   0 root         (0) root         (0)     3235 2023-06-15 12:01:55.000000 thipster-0.17.1/tests/parser/test_parserfactory.py
+-rw-r--r--   0 root         (0) root         (0)     4379 2023-06-15 12:01:55.000000 thipster-0.17.1/tests/parser/test_yamlparser.py
+-rw-r--r--   0 root         (0) root         (0)     3305 2023-06-15 12:01:55.000000 thipster-0.17.1/tests/test_e2e.py
+-rw-r--r--   0 root         (0) root         (0)     4154 2023-06-15 12:01:55.000000 thipster-0.17.1/tests/test_tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 12:01:58.974078 thipster-0.17.1/thipster/
+-rw-r--r--   0 root         (0) root         (0)      171 2023-06-15 12:01:55.000000 thipster-0.17.1/thipster/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 12:01:58.974078 thipster-0.17.1/thipster/auth/
+-rw-r--r--   0 root         (0) root         (0)      215 2023-06-15 12:01:55.000000 thipster-0.17.1/thipster/auth/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      907 2023-06-15 12:01:55.000000 thipster-0.17.1/thipster/auth/google.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 12:01:58.974078 thipster-0.17.1/thipster/engine/
+-rw-r--r--   0 root         (0) root         (0)      415 2023-06-15 12:01:55.000000 thipster-0.17.1/thipster/engine/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5111 2023-06-15 12:01:55.000000 thipster-0.17.1/thipster/engine/engine.py
+-rw-r--r--   0 root         (0) root         (0)      243 2023-06-15 12:01:55.000000 thipster-0.17.1/thipster/engine/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)      412 2023-06-15 12:01:55.000000 thipster-0.17.1/thipster/engine/i_auth.py
+-rw-r--r--   0 root         (0) root         (0)      754 2023-06-15 12:01:55.000000 thipster-0.17.1/thipster/engine/i_parser.py
+-rw-r--r--   0 root         (0) root         (0)      600 2023-06-15 12:01:55.000000 thipster-0.17.1/thipster/engine/i_repository.py
+-rw-r--r--   0 root         (0) root         (0)     1985 2023-06-15 12:01:55.000000 thipster-0.17.1/thipster/engine/i_terraform.py
+-rw-r--r--   0 root         (0) root         (0)     4346 2023-06-15 12:01:55.000000 thipster-0.17.1/thipster/engine/parsed_file.py
+-rw-r--r--   0 root         (0) root         (0)     3109 2023-06-15 12:01:55.000000 thipster-0.17.1/thipster/engine/resource_model.py
+-rw-r--r--   0 root         (0) root         (0)      654 2023-06-15 12:01:55.000000 thipster-0.17.1/thipster/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 12:01:58.974078 thipster-0.17.1/thipster/parser/
+-rw-r--r--   0 root         (0) root         (0)      364 2023-06-15 12:01:55.000000 thipster-0.17.1/thipster/parser/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 12:01:58.974078 thipster-0.17.1/thipster/parser/dsl_parser/
+-rw-r--r--   0 root         (0) root         (0)       30 2023-06-15 12:01:55.000000 thipster-0.17.1/thipster/parser/dsl_parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9180 2023-06-15 12:01:55.000000 thipster-0.17.1/thipster/parser/dsl_parser/ast.py
+-rw-r--r--   0 root         (0) root         (0)     2892 2023-06-15 12:01:55.000000 thipster-0.17.1/thipster/parser/dsl_parser/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)    13507 2023-06-15 12:01:55.000000 thipster-0.17.1/thipster/parser/dsl_parser/interpreter.py
+-rw-r--r--   0 root         (0) root         (0)    17026 2023-06-15 12:01:55.000000 thipster-0.17.1/thipster/parser/dsl_parser/lexer.py
+-rw-r--r--   0 root         (0) root         (0)     3008 2023-06-15 12:01:55.000000 thipster-0.17.1/thipster/parser/dsl_parser/lexer_position.py
+-rw-r--r--   0 root         (0) root         (0)     1991 2023-06-15 12:01:55.000000 thipster-0.17.1/thipster/parser/dsl_parser/parser.py
+-rw-r--r--   0 root         (0) root         (0)     2089 2023-06-15 12:01:55.000000 thipster-0.17.1/thipster/parser/dsl_parser/token.py
+-rw-r--r--   0 root         (0) root         (0)    20074 2023-06-15 12:01:55.000000 thipster-0.17.1/thipster/parser/dsl_parser/token_parser.py
+-rw-r--r--   0 root         (0) root         (0)      549 2023-06-15 12:01:55.000000 thipster-0.17.1/thipster/parser/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     2310 2023-06-15 12:01:55.000000 thipster-0.17.1/thipster/parser/parser_factory.py
+-rw-r--r--   0 root         (0) root         (0)     6370 2023-06-15 12:01:55.000000 thipster-0.17.1/thipster/parser/yaml_parser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 12:01:58.978078 thipster-0.17.1/thipster/repository/
+-rw-r--r--   0 root         (0) root         (0)      332 2023-06-15 12:01:55.000000 thipster-0.17.1/thipster/repository/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      285 2023-06-15 12:01:55.000000 thipster-0.17.1/thipster/repository/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     1399 2023-06-15 12:01:55.000000 thipster-0.17.1/thipster/repository/github.py
+-rw-r--r--   0 root         (0) root         (0)     4669 2023-06-15 12:01:55.000000 thipster-0.17.1/thipster/repository/json.py
+-rw-r--r--   0 root         (0) root         (0)      475 2023-06-15 12:01:55.000000 thipster-0.17.1/thipster/repository/local.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 12:01:58.978078 thipster-0.17.1/thipster/terraform/
+-rw-r--r--   0 root         (0) root         (0)      327 2023-06-15 12:01:55.000000 thipster-0.17.1/thipster/terraform/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22616 2023-06-15 12:01:55.000000 thipster-0.17.1/thipster/terraform/cdk.py
+-rw-r--r--   0 root         (0) root         (0)     1292 2023-06-15 12:01:55.000000 thipster-0.17.1/thipster/terraform/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 12:01:58.974078 thipster-0.17.1/thipster.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5156 2023-06-15 12:01:58.000000 thipster-0.17.1/thipster.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1804 2023-06-15 12:01:58.000000 thipster-0.17.1/thipster.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-15 12:01:58.000000 thipster-0.17.1/thipster.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      390 2023-06-15 12:01:58.000000 thipster-0.17.1/thipster.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-06-15 12:01:58.000000 thipster-0.17.1/thipster.egg-info/top_level.txt
```

### Comparing `thipster-0.17.0/LICENSE` & `thipster-0.17.1/LICENSE`

 * *Files identical despite different names*

### Comparing `thipster-0.17.0/PKG-INFO` & `thipster-0.17.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thipster
-Version: 0.17.0
+Version: 0.17.1
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
-Metadata-Version: 2.1 Name: thipster Version: 0.17.0 Summary: THipster is a
+Metadata-Version: 2.1 Name: thipster Version: 0.17.1 Summary: THipster is a
 tool dedicated to simplifying the difficulty associated with writing Terraform
 files. It allows users to write infrastructure as code in a simplified format,
 using either YAML (with JINJA) or the dedicated Thipster DSL. Home-page: https:
 //github.com/THipster/THipster Download-URL: https://github.com/THipster/
 THipster.git Keywords: thipster,terraform,infrastructure,infrastructure-as-
 code,iac,generator,dsl,yaml Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python :: 3.11 Classifier: License :: OSI
```

### Comparing `thipster-0.17.0/README.md` & `thipster-0.17.1/README.md`

 * *Files identical despite different names*

### Comparing `thipster-0.17.0/pyproject.toml` & `thipster-0.17.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -33,8 +33,9 @@
 select = [
     "F",
     "E",
     "W",
     "I",
     "UP",
     "C90",
+    "N",
 ]
```

### Comparing `thipster-0.17.0/setup.py` & `thipster-0.17.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import find_packages, setup
 
-__version__ = '0.17.0'
+__version__ = '0.17.1'
 
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 with open('README.md') as rm:
     readme = rm.read()
```

### Comparing `thipster-0.17.0/tests/engine/test_engine.py` & `thipster-0.17.1/tests/engine/test_engine.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,38 +14,38 @@
             res = function(*args, **kwargs)
             print(f'{name} returned :\n{str(res)}')
             return res
         return internal_wrapper
     return wrapper
 
 
-class MockException(Exception):
+class MockError(Exception):
     def __init__(self, message):
         self.message = message
 
 
-class MockAuth(eng.I_Auth):
+class MockAuth(eng.AuthPort):
     @logger('- Authentifier')
     def authenticate(self):
         return (None, None)
 
 
-class MockParser(eng.I_Parser):
+class MockParser(eng.ParserPort):
     @logger('- Parser')
     def run(self, filename) -> str:
         return ParsedFile()
 
 
-class MockRepository(eng.I_Repository):
+class MockRepository(eng.RepositoryPort):
     @logger('- Repo')
-    def get(self, resourceNames: list[str]) -> dict[str, ResourceModel]:
+    def get(self, resource_names: list[str]) -> dict[str, ResourceModel]:
         return []
 
 
-class MockTerraform(eng.I_Terraform):
+class MockTerraform(eng.TerraformPort):
     @logger('- Terraform:apply')
     def apply(self):
         pass
 
     @logger('- Terraform:generate')
     def generate(self, a, b, auth):
         pass
@@ -93,42 +93,42 @@
     engine = eng.Engine(parser, repository, auth, terraform)
     res = engine.run('test.file')
 
     assert res is None
 
 
 def test_parser_failure(mocker):
-    def parserFail(self, filename: str):
-        raise MockException('Parser failure')
+    def parser_fail(self, filename: str):
+        raise MockError('Parser failure')
 
     mocker.patch(
         'tests.engine.test_engine.MockParser.run',
-        parserFail,
+        parser_fail,
     )
 
     parser = MockParser()
     repository = MockRepository()
     auth = MockAuth()
     terraform = MockTerraform()
 
-    with pytest.raises(MockException):
+    with pytest.raises(MockError):
         engine = eng.Engine(parser, repository, auth, terraform)
         engine.run('test.file')
 
 
 def test_repository_failure(mocker):
-    def repositoryFail(self, resourceNames: list[str]) -> dict[str, ResourceModel]:
-        raise MockException('Repository failure')
+    def repository_fail(self, resource_names: list[str]) -> dict[str, ResourceModel]:
+        raise MockError('Repository failure')
 
     mocker.patch(
         'tests.engine.test_engine.MockRepository.get',
-        repositoryFail,
+        repository_fail,
     )
 
     parser = MockParser()
     repository = MockRepository()
     auth = MockAuth()
     terraform = MockTerraform()
 
-    with pytest.raises(MockException):
+    with pytest.raises(MockError):
         engine = eng.Engine(parser, repository, auth, terraform)
         engine.run('test.file')
```

### Comparing `thipster-0.17.0/tests/engine/test_generation.py` & `thipster-0.17.1/tests/engine/test_generation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import uuid
 
 import pytest
 
 from thipster.terraform.exceptions import (
-    CDKCyclicDependencies,
-    CDKDependencyNotDeclared,
-    CDKMissingAttributeInDependency,
+    CDKCyclicDependenciesError,
+    CDKDependencyNotDeclaredError,
+    CDKMissingAttributeInDependencyError,
 )
 
 from ..test_tools import (
     assert_number_of_resource_type_is,
     assert_resource_created,
     get_function_name,
     get_resource_parameter,
@@ -60,15 +60,15 @@
 
     clean_up()
 
 
 def test_dep_with_no_options():
     function_name = get_function_name()
 
-    with pytest.raises(CDKMissingAttributeInDependency):
+    with pytest.raises(CDKMissingAttributeInDependencyError):
         clean_up = process_file(
             directory=function_name,
             file="""
 bucket_bad_dep_parent my-bucket:
 \tregion : euw
 """,
             mock_auth=True,
@@ -76,15 +76,15 @@
 
         clean_up()
 
 
 def test_cyclic_deps():
     function_name = get_function_name()
 
-    with pytest.raises(CDKCyclicDependencies):
+    with pytest.raises(CDKCyclicDependenciesError):
         clean_up = process_file(
             directory=function_name,
             file="""
 bucket_bad_dep_cyclic my-bucket:
 \tregion : euw
 """,
             mock_auth=True,
@@ -124,15 +124,15 @@
 
     clean_up()
 
 
 def test_missing_explicit_dependency():
     function_name = get_function_name()
 
-    with pytest.raises(CDKDependencyNotDeclared):
+    with pytest.raises(CDKDependencyNotDeclaredError):
         clean_up = process_file(
             directory=function_name,
             file="""
 subnetwork lb-subnet:
 \tnetwork: lb-net
 \tregion: europe-west1b
 \tip_range: 10.0.1.0/24
```

### Comparing `thipster-0.17.0/tests/parser/dsl_parser/test_DSLparser.py` & `thipster-0.17.1/tests/parser/dsl_parser/test_dslparser.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import os
 
 import pytest
 
 import thipster.engine.parsed_file as pf
 from thipster.parser import DSLParser
 from thipster.parser.dsl_parser.exceptions import (
-    DSLArithmeticException,
-    DSLConditionException,
-    DSLParserPathNotFound,
-    DSLSyntaxException,
-    DSLUnexpectedEOF,
+    DSLArithmeticError,
+    DSLConditionError,
+    DSLParserPathNotFoundError,
+    DSLSyntaxError,
+    DSLUnexpectedEOFError,
 )
 from thipster.parser.dsl_parser.token import TOKENTYPES as TT
 
 from ...test_tools import create_dir
 
 
 def test_get_files():
@@ -34,15 +34,15 @@
         assert 'test_file' in k
         assert v == 'content'
 
     _destroy_dir()
 
 
 def test_get_absent_files():
-    with pytest.raises(DSLParserPathNotFound):
+    with pytest.raises(DSLParserPathNotFoundError):
 
         parser = DSLParser
         parser._DSLParser__getfiles('inexistant_path')
 
 
 def __test_file(file: str):
     path_input = 'test'
@@ -410,18 +410,18 @@
 
         region = bucket.attributes[0]
         assert region.name == 'region'
         assert region.value == i
 
 
 def test_comparisons():
-    def test_cmp(cmpExpr: str, result: str):
+    def test_cmp(cmp_expr: str, result: str):
         out = __test_file(
             file=f"""bucket my-bucket:
-\tregion: truCase if {cmpExpr} else falsCase
+\tregion: truCase if {cmp_expr} else falsCase
 """,
         )
 
         assert len(out.resources) == 1
 
         bucket = out.resources[0]
         assert bucket.resource_type == 'bucket'
@@ -543,15 +543,15 @@
 
 
 def __test_syntax_error(
     mocker, input: str, ln: int, col: int,
     expected: str, got: str,
 ):
 
-    exc_info = __test_parser_raises(mocker, input, DSLSyntaxException)
+    exc_info = __test_parser_raises(mocker, input, DSLSyntaxError)
 
     exp = str(' or '.join(list(map(str, expected))))\
         if isinstance(expected, list) else str(expected.value)
 
     assert str(exc_info.value) == f'(File : \
 {os.getcwd()}/test/test_file.thips, Ln {str(ln)}, Col {str(col)}) :\n\t\
 Syntax error : Expected {exp}, got {str(got.value)}'
@@ -606,15 +606,15 @@
 
 
 
 
 
 """
     exc_info = __test_parser_raises(
-        mocker, input=input, exception=DSLUnexpectedEOF,
+        mocker, input=input, exception=DSLUnexpectedEOFError,
     )
 
     assert str(exc_info.value) == 'Unexpected EOF'
 
 
 def test_syntax_error_amount(mocker):
     # MISSING COLON
@@ -639,15 +639,15 @@
 
 
 def test_syntax_error_if(mocker):
     # MISSING CONDITION
     input = """
 bucket my-bucket: if
 """
-    __test_parser_raises(mocker, input=input, exception=DSLConditionException)
+    __test_parser_raises(mocker, input=input, exception=DSLConditionError)
 
     # UNEXPECTED IF ELSE
     input = """
 bucket my-bucket: if 1 == 1 else bbb
 """
     __test_syntax_error(
         mocker, input=input, ln=2, col=29,
@@ -669,15 +669,15 @@
 
     # MISSING CONDITION VALUE
     input = """
 bucket my-bucket:
 \ttoto:
 \t\tfoo : bar if  else bbb
 """
-    __test_parser_raises(mocker, input=input, exception=DSLConditionException)
+    __test_parser_raises(mocker, input=input, exception=DSLConditionError)
 
 
 def test_syntax_error_unexpected_token(mocker):
     # RESERVED TOKEN NAME
     input = """
 bucket if:
 \tregion: euw
@@ -690,8 +690,8 @@
 
 def test_amount_error(mocker):
     # RESERVED TOKEN NAME
     input = """
 bucket my-bucket: amount: 3/2
 \tregion: euw
 """
-    __test_parser_raises(mocker, input=input, exception=DSLArithmeticException)
+    __test_parser_raises(mocker, input=input, exception=DSLArithmeticError)
```

### Comparing `thipster-0.17.0/tests/parser/dsl_parser/test_ast.py` & `thipster-0.17.1/tests/parser/dsl_parser/test_ast.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import thipster.parser.dsl_parser.ast as ast
 from thipster.engine.parsed_file import Position
 from thipster.parser.dsl_parser.token import Token
 
 
-def test_create_AST():
+def test_create_ast():
     # bucket nom-#test \n\t toto: tata
     tree = ast.FileNode()
 
     tree.add(
         ast.ResourceNode(
             resource_type=ast.StringNode(
                 Token(Position('file', 1, 1), 'STRING', 'bucket'),
```

### Comparing `thipster-0.17.0/tests/parser/dsl_parser/test_token.py` & `thipster-0.17.1/tests/parser/dsl_parser/test_token.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from thipster.engine.parsed_file import Position
 from thipster.parser.dsl_parser.token import Token
 
 
 def test_create_token():
     position = Position(filename='testFile', ln=2, col=6)
-    tokenType = 'test_type'
+    token_type = 'test_type'
     value = 'test_value'
 
-    token = Token(position, token_type=tokenType, value=value)
+    token = Token(position, token_type=token_type, value=value)
 
     assert isinstance(token, Token)
     assert token.position == position
-    assert token.token_type == tokenType
+    assert token.token_type == token_type
     assert token.value == value
 
 
 def test_token_to_string():
     position = Position(filename='testFile', ln=2, col=6)
-    positionStr = '(File : testFile, Ln 2, Col 6)'
-    assert str(position) == positionStr
+    position_str = '(File : testFile, Ln 2, Col 6)'
+    assert str(position) == position_str
 
-    tokenType = 'test_type'
+    token_type = 'test_type'
     value = 'test_value'
-    token = Token(position, token_type=tokenType, value=value)
-    tokenStr = f'(Type: {str(tokenType)}, Position: {positionStr}, Value: {value})'
-    assert repr(token) == tokenStr
+    token = Token(position, token_type=token_type, value=value)
+    token_str = f'(Type: {str(token_type)}, Position: {position_str}, Value: {value})'
+    assert repr(token) == token_str
```

### Comparing `thipster-0.17.0/tests/parser/dsl_parser/test_tokenparser.py` & `thipster-0.17.1/tests/parser/dsl_parser/test_tokenparser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.0/tests/parser/test_ParserFactory.py` & `thipster-0.17.1/tests/parser/test_parserfactory.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,12 @@
+import pytest
+
 from thipster.engine.parsed_file import ParsedFile
 from thipster.parser import ParserFactory
+from thipster.parser.exceptions import NoFileFoundError
 
 from ..test_tools import create_dir
 
 
 def __test_file(files: str):
     path_input = 'test'
     _destroy_dir = create_dir(
@@ -109,7 +112,43 @@
         assert bucket.resource_type == 'bucket'
         assert 'my-bucket' in bucket.name
         assert len(bucket.attributes) == 1
 
         region = bucket.attributes[0]
         assert region.name == 'region'
         assert region.value == 'euw'
+
+
+def test_no_parsable_file():
+    with pytest.raises(NoFileFoundError):
+        __test_file(
+            {
+                'test_file.txt':
+                """ """,
+                'test_file2.txt':
+                """ """,
+            },
+        )
+
+
+def test_one_parsable_file():
+    out = __test_file(
+        {
+            'test_file.thips':
+            """bucket my-bucket1:
+\tregion: euw
+""",
+            'test_file2.txt':
+            """ """,
+        },
+    )
+
+    assert len(out.resources) == 1
+
+    bucket = out.resources[0]
+    assert bucket.resource_type == 'bucket'
+    assert bucket.name == 'my-bucket1'
+    assert len(bucket.attributes) == 1
+
+    region = bucket.attributes[0]
+    assert region.name == 'region'
+    assert region.value == 'euw'
```

### Comparing `thipster-0.17.0/tests/parser/test_YAMLParser.py` & `thipster-0.17.1/tests/parser/test_yamlparser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import pytest
 
 import thipster.engine.parsed_file as pf
 from thipster.parser import YAMLParser
-from thipster.parser.yaml_parser import YAMLParserNoName
+from thipster.parser.yaml_parser import YAMLParserNoNameError
 
 from ..test_tools import create_dir
 
 
 def __test_parser_raises(mocker, input: str, exception: Exception)\
         -> pytest.ExceptionInfo:
     with pytest.raises(exception) as exc_info:
@@ -186,8 +186,8 @@
 
 def test_syntax_error_no_name(mocker):
     input = """bucket:
   toto:
     - aaa
     - bbb
 """
-    __test_parser_raises(mocker, input, YAMLParserNoName)
+    __test_parser_raises(mocker, input, YAMLParserNoNameError)
```

### Comparing `thipster-0.17.0/tests/parser/test_parsedfile.py` & `thipster-0.17.1/tests/parser/test_parsedfile.py`

 * *Files 1% similar despite different names*

```diff
@@ -132,23 +132,23 @@
     assert isinstance(resource, pf.ParsedResource)
     assert resource.resource_type == 'test_type'
     assert isinstance(resource.attributes, list)
     for attribute in resource.attributes:
         assert isinstance(attribute, pf.ParsedAttribute)
         assert isinstance(
             attribute._ParsedAttribute__value,
-            pf.I_ParsedValue,
+            pf.ParsedValue,
         )
         if isinstance(attribute._ParsedAttribute__value, pf.ParsedDict):
             for val in attribute.value:
                 assert isinstance(val, pf.ParsedAttribute)
 
         elif isinstance(attribute._ParsedAttribute__value, pf.ParsedList):
             for val in attribute.value:
-                assert isinstance(val, pf.I_ParsedValue)
+                assert isinstance(val, pf.ParsedValue)
 
 
 def test_add_resource():
     file = pf.ParsedFile()
 
     pos = pf.Position('test_file', 3, 7)
     resource = pf.ParsedResource(
```

### Comparing `thipster-0.17.0/tests/test_e2e.py` & `thipster-0.17.1/tests/test_e2e.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.0/tests/test_tools.py` & `thipster-0.17.1/tests/test_tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 import os
 import shutil
 
 from cdktf_cdktf_provider_google.provider import GoogleProvider
 
 from thipster import Engine
 from thipster.auth import Google
-from thipster.engine import I_Auth
+from thipster.engine import AuthPort
 from thipster.parser import ParserFactory
 from thipster.repository import LocalRepo
 from thipster.terraform import Terraform
 
 LOCAL_REPO = 'tests/resources/e2e/models'
 REMOTE_REPO = 'THipster/models'
 
 
-class MockAuth(I_Auth):
+class MockAuth(AuthPort):
     def authenticate(self, app):
         GoogleProvider(
             app, 'default_google',
             project='project_id',
             credentials='credentials.token',
         )
```

### Comparing `thipster-0.17.0/thipster/auth/google.py` & `thipster-0.17.1/thipster/auth/google.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import google.auth
 from cdktf_cdktf_provider_google.provider import GoogleProvider
 
-from thipster.engine import I_Auth
+from thipster.engine import AuthPort
 
 
-class GoogleAuth(I_Auth):
+class GoogleAuth(AuthPort):
     """Authenticate to Google Cloud Platform (GCP) projects
 
     To use this module, you need to have a GCP account and a project created.
     You also need to have gcloud installed : https://cloud.google.com/sdk/docs/install
     Then login using glcloud : gcloud auth application-default login
     """
```

### Comparing `thipster-0.17.0/thipster/engine/engine.py` & `thipster-0.17.1/thipster/engine/engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,90 +1,90 @@
 """_Engine.py module.
 """
 
 import thipster.engine.parsed_file as pf
 
-from .i_auth import I_Auth
-from .i_parser import I_Parser
-from .i_repository import I_Repository
-from .i_terraform import I_Terraform
+from .i_auth import AuthPort
+from .i_parser import ParserPort
+from .i_repository import RepositoryPort
+from .i_terraform import TerraformPort
 from .resource_model import ResourceModel
 
 
 class Engine():
     """The engine of thipster
 
     The core of the application, it is used to call and link all
     interfaces together.
     """
 
     def __init__(
-            self, parser: I_Parser,
-            repository: I_Repository,
-            auth: I_Auth,
-            terraform:  I_Terraform,
+            self, parser: ParserPort,
+            repository: RepositoryPort,
+            auth: AuthPort,
+            terraform:  TerraformPort,
     ):
         """
         Parameters
         ----------
-        parser : I_Parser
+        parser : ParserPort
             Instance of a Parser class
-        repository : I_Repository
+        repository : RepositoryPort
             Instance of a Respository class
-        auth : I_Auth
+        auth : AuthPort
             Instance of an Auth class
-        terraform : I_Terraform
+        terraform : TerraformPort
             Instance of a Terraform class
 
         """
         self.__parser = parser
         self.__repository = repository
         self.__auth = auth
         self.__terraform = terraform
 
     @property
     def parser(self):
         return self.__parser
 
     @parser.setter
     def parser(self, value):
-        if not isinstance(value, I_Parser):
+        if not isinstance(value, ParserPort):
             raise Exception()
 
         self.__parser = value
 
     @property
     def repository(self):
         return self.__repository
 
     @repository.setter
     def repository(self, value):
-        if not isinstance(value, I_Repository):
+        if not isinstance(value, RepositoryPort):
             raise Exception()
 
         self.__repository = value
 
     @property
     def auth(self):
         return self.__auth
 
     @auth.setter
     def auth(self, value):
-        if not isinstance(value, I_Auth):
+        if not isinstance(value, AuthPort):
             raise Exception()
 
         self.__auth = value
 
     @property
     def terraform(self):
         return self.__terraform
 
     @terraform.setter
     def terraform(self, value):
-        if not isinstance(value, I_Terraform):
+        if not isinstance(value, TerraformPort):
             raise Exception()
 
         self.__terraform = value
 
     def run(self, path: str) -> tuple[list[str], str]:
         """Returns json Terraform files from the input file name
```

### Comparing `thipster-0.17.0/thipster/engine/i_parser.py` & `thipster-0.17.1/thipster/engine/i_parser.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from abc import ABC, abstractclassmethod
 
 from thipster.engine.parsed_file import ParsedFile
 
 
-class I_Parser(ABC):
+class ParserPort(ABC):
     """Parser module interface
     """
+    @classmethod
     @abstractclassmethod
     def run(cls, path: str) -> ParsedFile:
         """Abstract run method
 
         Parameters
         ----------
         path : str
```

### Comparing `thipster-0.17.0/thipster/engine/i_repository.py` & `thipster-0.17.1/thipster/engine/i_repository.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from abc import ABC, abstractmethod
 
 from thipster.engine.resource_model import ResourceModel
 
 
-class I_Repository(ABC):
+class RepositoryPort(ABC):
     """Repository module interface
     """
     @abstractmethod
-    def get(self, resourceNames: list[str]) -> dict[str, ResourceModel]:
+    def get(self, resource_names: list[str]) -> dict[str, ResourceModel]:
         """Abstract get method
 
         Parameters
         ----------
         resourceNames : list[str]
             List of resource names to be retrieved from the repository
```

### Comparing `thipster-0.17.0/thipster/engine/i_terraform.py` & `thipster-0.17.1/thipster/engine/i_terraform.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from abc import ABC, abstractclassmethod
 
 import thipster.engine.parsed_file as pf
 import thipster.engine.resource_model as rm
 
-from .i_auth import I_Auth
+from .i_auth import AuthPort
 
 
-class I_Terraform(ABC):
+class TerraformPort(ABC):
     """Terraform module interface
     """
+    @classmethod
     @abstractclassmethod
     def apply(cls, plan_file_path: str | None = None):
         """Apply generated terraform code
 
         Parameters
         ----------
         plan_file_path : str, optional
@@ -22,18 +23,19 @@
         ------
         NotImplementedError
             If method is not implemented in inheriting classes
 
         """
         raise NotImplementedError('Should implement apply()')
 
+    @classmethod
     @abstractclassmethod
     def generate(
         cls, file: pf.ParsedFile, models: dict[str, rm.ResourceModel],
-        _authenticator: I_Auth,
+        _authenticator: AuthPort,
     ):
         """Generates Terraform code from parsed file and models
 
         Parameters
         ----------
         file : pf.ParsedFile
             The ParsedFile object containing the resources defined in the input file
@@ -44,26 +46,28 @@
         ------
         NotImplementedError
             If method is not implemented in inheriting classes
 
         """
         raise NotImplementedError('Should implement generate()')
 
+    @classmethod
     @abstractclassmethod
     def init(cls):
         """Init Terraform for generated terraform code
 
         Raises
         ------
         NotImplementedError
             If method is not implemented in inheriting classes
 
         """
         raise NotImplementedError('Should implement generate()')
 
+    @classmethod
     @abstractclassmethod
     def plan(cls):
         """Get plan from generated terraform code
 
         Raises
         ------
         NotImplementedError
```

### Comparing `thipster-0.17.0/thipster/engine/parsed_file.py` & `thipster-0.17.1/thipster/engine/parsed_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """parsedFile.py Module
 """
 
 from abc import ABC
 
 
-class I_ParsedValue(ABC):
+class ParsedValue(ABC):
     """Parsed Value Interface
     """
 
     pass
 
 
 class Position():
@@ -74,48 +74,48 @@
             raise TypeError('Value must be a Position')
 
 
 class ParsedAttribute():
     """Class reprensenting a Parsed Attribute Object
     """
 
-    def __init__(self, name: str, position: Position | None, value: I_ParsedValue):
+    def __init__(self, name: str, position: Position | None, value: ParsedValue):
         """
         Parameters
         ----------
         name : str
         position : Position
-        value : I_parsed_Value
+        value : ParsedValue
         """
 
         self.name: str = name
         self.position: Position | None = position
         self.__value = value
 
     @property
     def value(self):
         """Value of the parsed attribute
         """
 
         return self.__value.value
 
 
-class ParsedList(I_ParsedValue):
+class ParsedList(ParsedValue):
     """Class representing a Parsed List Object
     """
 
-    def __init__(self, value: list[I_ParsedValue]):
+    def __init__(self, value: list[ParsedValue]):
         """
         Parameters
         ----------
-        value : list[I_Parsed_Value]
+        value : list[ParsedValue]
         """
 
         super().__init__()
-        self.value: list[I_ParsedValue] = value
+        self.value: list[ParsedValue] = value
 
     def __iter__(self):
         self.i = 0
         return self
 
     def __next__(self):
         if self.i > len(self.__value):
@@ -123,38 +123,38 @@
         else:
             ret = self.value[self.i]
             self.i += 1
 
         return ret
 
 
-class ParsedLiteral(I_ParsedValue):
+class ParsedLiteral(ParsedValue):
     """Class representing a Parsed Literal Object
     """
 
     def __init__(self, value: bool | int | float | str):
         """
         Parameters
         ----------
         value : Literal
         """
 
         super().__init__()
         self.value: bool | int | float | str = value
 
 
-class ParsedDict(I_ParsedValue):
+class ParsedDict(ParsedValue):
     """Class representing a Parsed Dictionnary Object
     """
 
     def __init__(self, value: list[ParsedAttribute]):
         """
         Parameters
         ----------
-        value : list[Parsed_Attribute]
+        value : list[ParsedAttribute]
         """
 
         super().__init__()
         self.value: list[ParsedAttribute] = value
 
 
 class ParsedResource():
@@ -172,15 +172,15 @@
         Parameters
         ----------
         type : str
         name : str
             name of the resource
         position : Position
             position of the resource in its origin file
-        attributes : list[Parsed_Attribute]
+        attributes : list[ParsedAttribute]
             list of attributes of the resource
         """
 
         self.resource_type: str = type
         self.name: str = name
         self.position: Position | None = position
         self.attributes: list[ParsedAttribute] = attributes
```

### Comparing `thipster-0.17.0/thipster/engine/resource_model.py` & `thipster-0.17.1/thipster/engine/resource_model.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 """ResourceModel.py module.
 """
 
 from abc import ABC
 
 
-class I_Model_Value(ABC):
+class ModelValue(ABC):
     """Model Attribute Value Interface
     """
     value = None
 
 
-class Model_Attribute():
+class ModelAttribute():
     """Represents a Resource Model attribute
     """
 
     def __init__(
             self, cdk_name: str,
-            default: I_Model_Value | None = None,
+            default: ModelValue | None = None,
             optional: bool = True,
             is_list: bool = False,
     ):
         """
         Parameters
         ----------
         name : str
             Attribute name
-        default : I_Model_Value, optional
+        default : ModelValue, optional
             Default Attribute value if there is one, by default None
         optional : bool, optional
             Is attribute optional ?, by default True
         is_list : bool, optional
             Is attribute a list ?, by default False
         """
         self.cdk_name = cdk_name
@@ -42,19 +42,19 @@
         return self.__default.value if self.__default else None
 
     @default.setter
     def default(self, value):
         self.__default = value
 
 
-class Model_List(I_Model_Value):
+class ModelList(ModelValue):
     """Represents a List of values for a Resource Model attribute
     """
 
-    def __init__(self, value: list[I_Model_Value | None] | None):
+    def __init__(self, value: list[ModelValue | None] | None):
         super().__init__()
         self.value = value
 
     def __iter__(self):
         self.i = 0
         return self
 
@@ -66,28 +66,28 @@
             raise StopIteration
         else:
             self.i += 1
 
         return ret
 
 
-class Model_Literal(I_Model_Value):
+class ModelLiteral(ModelValue):
     """Represents a literal value for a Resource Model attribute
     """
 
     def __init__(self, value):
         super().__init__()
         self.value = value
 
 
-class Model_Dict(I_Model_Value):
+class ModelDict(ModelValue):
     """Represents a dictionary value for a Resource Model attribute
     """
 
-    def __init__(self, value: dict[str, Model_Attribute] | None):
+    def __init__(self, value: dict[str, ModelAttribute] | None):
         super().__init__()
         self.value = value
 
     def __iter__(self):
         self.i = 0
         return self
 
@@ -106,15 +106,15 @@
 class ResourceModel():
     """Represents a Resource Model
     """
 
     def __init__(
             self,
             resource_type: str,
-            attributes: dict[str, Model_Attribute] | None,
+            attributes: dict[str, ModelAttribute] | None,
             dependencies: dict[str, dict[str, object]] | None,
             internal_objects: dict[str, dict[str, object]] | None,
             name_key: str | None,
             cdk_provider: str,
             cdk_module: str,
             cdk_name: str,
     ):
```

### Comparing `thipster-0.17.0/thipster/helpers.py` & `thipster-0.17.1/thipster/helpers.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.0/thipster/parser/dsl_parser/ast.py` & `thipster-0.17.1/thipster/parser/dsl_parser/ast.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         return f'<STRING {self.token}>'
 
     @property
     def position(self) -> Position:
         return self.token.position
 
     def accept(self, visitor):
-        return visitor.visitString(self)
+        return visitor.visit_string(self)
 
 
 class StringExprNode(Node):
     def __init__(self, *values: Node | list[Node]) -> None:
         super().__init__()
         self.values: list[Node] = []
         for v in values:
@@ -46,15 +46,15 @@
         return f"<STRING-EXPR {' '.join(list(map(str, self.values)))}>"
 
     @property
     def position(self) -> Token:
         return self.values[0].position
 
     def accept(self, visitor):
-        return visitor.visitStringExpr(self)
+        return visitor.visit_string_expr(self)
 
 
 class VariableNode(Node):
     def __init__(self, token: Token) -> None:
         super().__init__()
         self.token = token
 
@@ -66,15 +66,15 @@
         return self.token.value
 
     @property
     def position(self) -> Position:
         return self.token.position
 
     def accept(self, visitor):
-        return visitor.visitVariable(self)
+        return visitor.visit_variable(self)
 
 
 class BoolNode(Node):
     def __init__(self, token: Token) -> None:
         super().__init__()
         self.token = token
 
@@ -82,15 +82,15 @@
         return f'<BOOL {self.token}>'
 
     @property
     def position(self) -> Position:
         return self.token.position
 
     def accept(self, visitor):
-        return visitor.visitBool(self)
+        return visitor.visit_bool(self)
 
 
 class IntNode(Node):
     def __init__(self, token: Token) -> None:
         super().__init__()
         self.token = token
 
@@ -98,15 +98,15 @@
         return f'<INT {self.token}>'
 
     @property
     def position(self) -> Position:
         return self.token.position
 
     def accept(self, visitor):
-        return visitor.visitInt(self)
+        return visitor.visit_int(self)
 
 
 class FloatNode(Node):
     def __init__(self, token: Token) -> None:
         super().__init__()
         self.token = token
 
@@ -114,15 +114,15 @@
         return f'<FLOAT {self.token}>'
 
     @property
     def position(self) -> Position:
         return self.token.position
 
     def accept(self, visitor):
-        return visitor.visitFloat(self)
+        return visitor.visit_float(self)
 
 
 class VariableDefinitionNode(Node):
     def __init__(self, name: Token, value: IntNode) -> None:
         super().__init__()
         self.__name = name
         self.value = value
@@ -135,15 +135,15 @@
         return self.__name.value
 
     @property
     def position(self) -> Position:
         return self.__name.position
 
     def accept(self, visitor):
-        return visitor.visitVariableDefinition(self)
+        return visitor.visit_variable_definition(self)
 
 
 class IfNode(Node):
     def __init__(self, condition: StringNode, if_case: Node) -> None:
         super().__init__()
         self.condition = condition
         self.if_case = if_case
@@ -152,15 +152,15 @@
         return f'<IF {self.condition}: {self.if_case}>'
 
     @property
     def position(self) -> Position:
         return self.if_case.position
 
     def accept(self, visitor):
-        return visitor.visitIf(self)
+        return visitor.visit_if(self)
 
 
 class IfElseNode(IfNode):
     def __init__(
         self, condition: StringNode, if_case: Node,
         else_case: Node | None,
     ) -> None:
@@ -168,15 +168,15 @@
         self.else_case = else_case
 
     def __str__(self) -> str:
         return f'<IF_E {str(self.condition)}: {str(self.if_case)}, ELSE : \
 {str(self.else_case)}>'
 
     def accept(self, visitor):
-        return visitor.visitIfElse(self)
+        return visitor.visit_ifelse(self)
 
 
 class AmountNode(Node):
     def __init__(
         self, position: Token,
         amount: Node, variable: VariableDefinitionNode | None, node: Node | None,
     )\
@@ -195,15 +195,15 @@
         return self.__position
 
     @position.setter
     def position(self, _value) -> Position:
         self.__position = _value
 
     def accept(self, visitor):
-        return visitor.visitAmount(self)
+        return visitor.visit_amount(self)
 
 
 class ValueNode(Node, ABC):
     pass
 
 
 class ParameterNode(Node):
@@ -216,15 +216,15 @@
         return f'<PARAMETER name = {str(self.name)}, value = {str(self.value)}>'
 
     @property
     def position(self) -> Position:
         return self.name.position
 
     def accept(self, visitor):
-        return visitor.visitParameter(self)
+        return visitor.visit_parameter(self)
 
 
 class DictNode(ValueNode):
     def __init__(self, values: list[ParameterNode]) -> None:
         super().__init__()
         self.values = values
 
@@ -232,15 +232,15 @@
         return f"<DICT {' '.join(list(map(str, self.values)))}>"
 
     @property
     def position(self) -> Position:
         return self.values[0].position
 
     def accept(self, visitor):
-        return visitor.visitDict(self)
+        return visitor.visit_dict(self)
 
 
 class LiteralNode(ValueNode):
     def __init__(self, values: Node) -> None:
         super().__init__()
         self.value = values
 
@@ -248,15 +248,15 @@
         return f'<LITERAL {str(self.value)}>'
 
     @property
     def position(self) -> Position:
         return self.value.position
 
     def accept(self, visitor):
-        return visitor.visitLiteral(self)
+        return visitor.visit_literal(self)
 
 
 class ListNode(ValueNode):
     def __init__(self, values: list[ValueNode]) -> None:
         super().__init__()
         self.values = values
 
@@ -264,15 +264,15 @@
         return f"<LIST {' '.join(list(map(str, self.values)))}>"
 
     @property
     def position(self) -> Position:
         return self.values[0].position
 
     def accept(self, visitor):
-        return visitor.visitList(self)
+        return visitor.visit_list(self)
 
 
 class CompExprNode(Node):
     def __init__(
             self, left_value: Node, operation, right_value: Node | None = None,
     ) -> None:
         super().__init__()
@@ -281,15 +281,15 @@
         self.right_value = right_value
 
     @property
     def position(self) -> Position:
         return self.left_value.position
 
     def accept(self, visitor):
-        return visitor.visitCompExpr(self)
+        return visitor.visit_comp_expr(self)
 
 
 class TermNode(Node):
     def __init__(self, factors, operation) -> None:
         super().__init__()
         if len(factors) != len(operation) + 1:
             raise
@@ -297,15 +297,15 @@
         self.operation = operation
 
     @property
     def position(self) -> Position:
         return self.factors[0].position
 
     def accept(self, visitor):
-        return visitor.visitTerm(self)
+        return visitor.visit_term(self)
 
 
 class ArithExprNode(Node):
     def __init__(self, terms: list[TermNode], operations) -> None:
         super().__init__()
         if len(terms) != len(operations) + 1:
             raise
@@ -313,29 +313,29 @@
         self.operations = operations
 
     @property
     def position(self) -> Position:
         return self.terms[0].position
 
     def accept(self, visitor):
-        return visitor.visitArithExpr(self)
+        return visitor.visit_arith_expr(self)
 
 
 class FactorNode(Node):
     def __init__(self, factors: list[Node], operation) -> None:
         super().__init__()
         self.factors = factors
         self.operation = operation
 
     @property
     def position(self) -> Position:
         return self.factors[0].position
 
     def accept(self, visitor):
-        return visitor.visitFactor(self)
+        return visitor.visit_factor(self)
 
 
 class ResourceNode(Node):
     def __init__(
         self,
         resource_type: StringNode,
         name: StringNode,
@@ -351,15 +351,15 @@
 name = {str(self.name)}, parameters = {str(self.parameters)}>'
 
     @property
     def position(self) -> Position:
         return self.type.position
 
     def accept(self, visitor):
-        return visitor.visitResource(self)
+        return visitor.visit_resource(self)
 
 
 class FileNode(Node):
     def __init__(self) -> None:
         super().__init__()
         self.resources: list[ResourceNode | IfNode | AmountNode] = []
 
@@ -370,8 +370,8 @@
         return '\n'.join(list(map(str, self.resources)))
 
     @property
     def position(self) -> Position:
         return self.resources[0].position
 
     def accept(self, visitor):
-        return visitor.visitFile(self)
+        return visitor.visit_file(self)
```

### Comparing `thipster-0.17.0/thipster/parser/dsl_parser/exceptions.py` & `thipster-0.17.1/thipster/parser/dsl_parser/exceptions.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-from thipster.engine import THipsterException
+from thipster.engine import THipsterError
 from thipster.engine.parsed_file import Position
 
 from .token import TOKENTYPES as TT
 from .token import Token
 
 
-class DSLParserBaseException(THipsterException):
+class DSLParserBaseError(THipsterError):
     def __init__(self, *args: object) -> None:
         super().__init__(*args)
 
 
-class DSLParserPathNotFound(DSLParserBaseException):
+class DSLParserPathNotFoundError(DSLParserBaseError):
     def __init__(self, file, *args: object) -> None:
         super().__init__(*args)
         self.file = file
 
     @property
     def message(self) -> str:
         return f'Path not found : {self.file}'
 
 
-class DSLSyntaxException(DSLParserBaseException):
+class DSLSyntaxError(DSLParserBaseError):
     def __init__(self, token: Token, expected: TT | list[TT], *args: object) -> None:
         super().__init__(*args)
         self.token = token
         self.expected = expected
 
     @property
     def message(self) -> str:
@@ -33,65 +33,65 @@
 {str(self.expected.value)}, got {str(self.token.token_type)}"""
         else:
             return f"""{str(self.token.position)} :\n\tSyntax error : Expected \
 {str(' or '.join(list(map(str, self.expected))))}, got {
     str(self.token.token_type)}"""
 
 
-class DSLConditionException(DSLParserBaseException):
+class DSLConditionError(DSLParserBaseError):
     def __init__(self, token: Token, *args: object) -> None:
         super().__init__(*args)
         self.token = token
 
     @property
     def message(self) -> str:
         return f'{str(self.token.position)} :\n\tBad condition'
 
 
-class DSLArithmeticException(DSLParserBaseException):
+class DSLArithmeticError(DSLParserBaseError):
     def __init__(self, position: Position, error_message: str, *args: object) -> None:
         super().__init__(*args)
         self.position = position
         self.error_message = error_message
 
     @property
     def message(self) -> str:
         return f'{str(self.position)} :\n\tArithmetic error :{self.error_message}'
 
 
-class DSLUnexpectedEOF(DSLParserBaseException):
+class DSLUnexpectedEOFError(DSLParserBaseError):
     def __init__(self, *args: object) -> None:
         super().__init__(*args)
 
     @property
     def message(self) -> str:
         return 'Unexpected EOF'
 
 
-class DSLParserNoEndingQuotes(DSLParserBaseException):
+class DSLParserNoEndingQuotesError(DSLParserBaseError):
     def __init__(self, position, *args: object) -> None:
         super().__init__(*args)
         self.position = position
 
     @property
     def message(self) -> str:
         return f'Invalid syntax, missing ending quotes at : {self.position}'
 
 
-class DSLParserVariableAlreadyUsed(DSLParserBaseException):
+class DSLParserVariableAlreadyUsedError(DSLParserBaseError):
     def __init__(self, var: str, *args: object) -> None:
         super().__init__(*args)
         self.variable = var
 
     @property
     def message(self) -> str:
-        return f'Variable already used : {self.variable}',
+        return f'Variable already used : {self.variable}'
 
 
-class DSLParserVariableNotDeclared(DSLParserBaseException):
+class DSLParserVariableNotDeclaredError(DSLParserBaseError):
     def __init__(self, var: str, *args: object) -> None:
         super().__init__(*args)
         self.variable = var
 
     @property
     def message(self) -> str:
-        return f'Variable not declared : {self.variable}',
+        return f'Variable not declared : {self.variable}'
```

### Comparing `thipster-0.17.0/thipster/parser/dsl_parser/interpreter.py` & `thipster-0.17.1/thipster/parser/dsl_parser/interpreter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import thipster.engine.parsed_file as pf
 import thipster.parser.dsl_parser.ast as ast
 
 from .exceptions import (
-    DSLArithmeticException,
-    DSLParserVariableAlreadyUsed,
-    DSLParserVariableNotDeclared,
+    DSLArithmeticError,
+    DSLParserVariableAlreadyUsedError,
+    DSLParserVariableNotDeclaredError,
 )
 from .token import TOKENTYPES as TT
 
 
 class Interpreter():
     """Interpreter class for the DSL Parser
 
@@ -31,15 +31,15 @@
         Returns
         -------
         ParsedFile
             The parsed file stucture assiociated to the given AST
         """
         return tree.accept(self)
 
-    def visitCompExpr(self, element: ast.CompExprNode) -> bool:
+    def visit_comp_expr(self, element: ast.CompExprNode) -> bool:
         """Visitor for a StringNode
 
         Parameters
         ----------
         element: StringNode
             The visited node
 
@@ -96,15 +96,15 @@
 
             case TT.GTE:
                 return pf.ParsedLiteral(
                     element.left_value.accept(self).value >=
                     element.right_value.accept(self).value,
                 )
 
-    def visitArithExpr(self, element: ast.ArithExprNode) -> int | float:
+    def visit_arith_expr(self, element: ast.ArithExprNode) -> int | float:
         """Visitor for a StringNode
 
         Parameters
         ----------
         element: StringNode
             The visited node
 
@@ -129,15 +129,15 @@
                     rm = element.terms[i+1].accept(self)
                     if isinstance(rm, pf.ParsedLiteral):
                         rm = rm.value
                     total -= rm
 
         return pf.ParsedLiteral(total)
 
-    def visitTerm(self, element: ast.TermNode) -> int | float:
+    def visit_term(self, element: ast.TermNode) -> int | float:
         """Visitor for a StringNode
 
         Parameters
         ----------
         element: StringNode
             The visited node
 
@@ -162,15 +162,15 @@
                     div = element.factors[i+1].accept(self)
                     if isinstance(div, pf.ParsedLiteral):
                         div = div.value
                     total /= div
 
         return total
 
-    def visitFactor(self, element: ast.FactorNode) -> int | float:
+    def visit_factor(self, element: ast.FactorNode) -> int | float:
         """Visitor for a StringNode
 
         Parameters
         ----------
         element: StringNode
             The visited node
 
@@ -194,15 +194,15 @@
                 for f in element.factors[1:]:
                     pow = f.accept(self)
                     if isinstance(pow, pf.ParsedLiteral):
                         pow = pow.value
                     total = total**pow
                 return pf.ParsedLiteral(total)
 
-    def visitStringExpr(self, element: ast.StringExprNode) -> str:
+    def visit_string_expr(self, element: ast.StringExprNode) -> str:
         """Visitor for a StringExprNode
 
         Parameters
         ----------
         element: StringExprNode
             The visited node
 
@@ -213,15 +213,15 @@
         """
         ret = ''
         for value in element.values:
             ret += str(value.accept(self))
 
         return pf.ParsedLiteral(ret)
 
-    def visitVariableDefinition(self, element: ast.VariableDefinitionNode) -> str:
+    def visit_variable_definition(self, element: ast.VariableDefinitionNode) -> str:
         """Visitor for a VariableDefinitionNode
 
         Parameters
         ----------
         element: VariableDefinitionNode
             The visited node
 
@@ -232,21 +232,21 @@
 
         Raises
         ------
         DSLParserVariableAlreadyUsed
             Tried to declare a varible that was already declared
         """
         if element.name in self.__variables:
-            raise DSLParserVariableAlreadyUsed(element.name)
+            raise DSLParserVariableAlreadyUsedError(element.name)
 
         self.__variables[element.name] = element.value.accept(self)
 
         return element.name
 
-    def visitVariable(self, element: ast.VariableNode) -> object:
+    def visit_variable(self, element: ast.VariableNode) -> object:
         """Visitor for a VariableNode
 
         Parameters
         ----------
         element: VariableNode
             The visited node
 
@@ -257,79 +257,79 @@
 
         Raises
         ------
         DSLParserVariableNotDeclared
             Tried to use a varible that was not declared
         """
         if element.name not in self.__variables:
-            raise DSLParserVariableNotDeclared(element.name)
+            raise DSLParserVariableNotDeclaredError(element.name)
 
         return self.__variables[element.name]
 
-    def visitInt(self, element: ast.IntNode) -> int:
+    def visit_int(self, element: ast.IntNode) -> int:
         """Visitor for an IntNode
 
         Parameters
         ----------
         element: IntNode
             The visited node
 
         Returns
         -------
         int
             The value of the node
         """
         return int(element.token.value)
 
-    def visitFloat(self, element: ast.FloatNode) -> float:
+    def visit_float(self, element: ast.FloatNode) -> float:
         """Visitor for a FloatNode
 
         Parameters
         ----------
         element: FloatNode
             The visited node
 
         Returns
         -------
         float
             The value of the node
         """
         return float(element.token.value)
 
-    def visitBool(self, element: ast.BoolNode) -> bool:
+    def visit_bool(self, element: ast.BoolNode) -> bool:
         """Visitor for a BoolNode
 
         Parameters
         ----------
         element: BoolNode
             The visited node
 
         Returns
         -------
         bool
             The value of the node
         """
         return bool(element.token.value)
 
-    def visitString(self, element: ast.StringNode) -> str:
+    def visit_string(self, element: ast.StringNode) -> str:
         """Visitor for a BoolNode
 
         Parameters
         ----------
         element: BoolNode
             The visited node
 
         Returns
         -------
         bool
             The value of the node
         """
         return str(element.token.value)
 
-    def visitIf(self, element: ast.IfNode) -> object | None:
+    def visit_if(self, element: ast.IfNode) -> object | None:
         """Visitor for an IfNode
 
         Parameters
         ----------
         element: IfNode
             The visited node
 
@@ -337,15 +337,15 @@
         -------
         object | None
             The value of the child node if the condition is true, else None
         """
         return element.if_case.accept(self) if element.condition.accept(self).value\
             else None
 
-    def visitIfElse(self, element: ast.IfElseNode):
+    def visit_ifelse(self, element: ast.IfElseNode):
         """Visitor for an IfElseNode
 
         Parameters
         ----------
         element: IfElseNode
             The visited node
 
@@ -354,15 +354,15 @@
         object | None
             The value of the "if" child node if the condition is true, else the value\
                   of the "else" child node
         """
         return element.if_case.accept(self) if element.condition.accept(self).value\
             else element.else_case.accept(self)
 
-    def visitAmount(self, element: ast.AmountNode) -> list[object]:
+    def visit_amount(self, element: ast.AmountNode) -> list[object]:
         """Visitor for an AmountNode
 
         Parameters
         ----------
         element: AmountNode
             The visited node
 
@@ -371,25 +371,25 @@
         list[object]
             A list with the required number of object (resource, list item, ...)
         """
         var = element.variable.accept(self) if element.variable else None
         res = []
         amount = element.amount.accept(self).value
         if not isinstance(amount, int):
-            raise DSLArithmeticException(
+            raise DSLArithmeticError(
                 element.amount.position, 'Integer expected',
             )
 
         for _ in range(amount):
             res += element.node.accept(self)
             if var:
                 self.__variables[var] += 1
         return res
 
-    def visitParameter(self, element: ast.ParameterNode) -> pf.ParsedAttribute:
+    def visit_parameter(self, element: ast.ParameterNode) -> pf.ParsedAttribute:
         """Visitor for an ParameterNode
 
         Parameters
         ----------
         element: ParameterNode
             The visited node
 
@@ -401,60 +401,60 @@
         """
         return pf.ParsedAttribute(
             name=element.name.accept(self),
             position=element.position,
             value=element.value.accept(self),
         )
 
-    def visitDict(self, element: ast.DictNode) -> pf.ParsedDict:
+    def visit_dict(self, element: ast.DictNode) -> pf.ParsedDict:
         """Visitor for an DictNode
 
         Parameters
         ----------
         element: DictNode
             The visited node
 
         Returns
         -------
         ParsedDict
             A ParsedDict object based on the node attributes
         """
         return pf.ParsedDict([v.accept(self) for v in element.values])
 
-    def visitLiteral(self, element: ast.LiteralNode) -> pf.ParsedLiteral:
+    def visit_literal(self, element: ast.LiteralNode) -> pf.ParsedLiteral:
         """Visitor for an LiteralNode
 
         Parameters
         ----------
         element: LiteralNode
             The visited node
 
         Returns
         -------
         ParsedLiteral
             A ParsedLiteral object based on the node value
         """
         return pf.ParsedLiteral(element.value.accept(self))
 
-    def visitList(self, element: ast.ListNode) -> pf.ParsedList:
+    def visit_list(self, element: ast.ListNode) -> pf.ParsedList:
         """Visitor for an ListNode
 
         Parameters
         ----------
         element: ListNode
             The visited node
 
         Returns
         -------
         ParsedList
             A ParsedLiteral object based on the node elements
         """
         return pf.ParsedList([v.accept(self) for v in element.values])
 
-    def visitResource(self, element: ast.ResourceNode) -> list[pf.ParsedResource]:
+    def visit_resource(self, element: ast.ResourceNode) -> list[pf.ParsedResource]:
         """Visitor for an ResourceNode
 
         Parameters
         ----------
         element: ResourceNode
             The visited node
 
@@ -468,15 +468,15 @@
                 type=element.type.accept(self).value,
                 name=element.name.accept(self).value,
                 position=element.position,
                 attributes=[v.accept(self) for v in element.parameters.values],
             ),
         ]
 
-    def visitFile(self, element: ast.FileNode):
+    def visit_file(self, element: ast.FileNode):
         """Visitor for an FileNode
 
         Parameters
         ----------
         element: FileNode
             The visited node
```

### Comparing `thipster-0.17.0/thipster/parser/dsl_parser/lexer.py` & `thipster-0.17.1/thipster/parser/dsl_parser/lexer.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from thipster.engine.parsed_file import Position
 from thipster.helpers import create_logger
 
-from .exceptions import DSLParserNoEndingQuotes
+from .exceptions import DSLParserNoEndingQuotesError
 from .lexer_position import LexerPosition
 from .token import TOKENTYPES as TT
 from .token import Token
 
 
 class Lexer():
     """Lexer class for the DSL Parser
@@ -15,525 +15,508 @@
         """
         Parameters
         ----------
         files : dict[str, str]
             Dictionnary of files to tokenize, fileName : fileContent
         """
         self.__logger = create_logger(__name__)
-        self.__files = files
-        self.__tokenList = []
+        self.files = files
+        self.tokenList = []
         self.__lexerPosition = LexerPosition()
         self.__currentChar = ''
 
-    @property
-    def files(self):
-        return self.__files
-
-    @property
-    def tokenList(self):
-        return self.__tokenList
-
     def run(self) -> list[Token]:
         """Launch the Lexer
 
         Returns
         -------
         list[Token]
             List of Tokens representing the input files
         """
         self.__logger.info('Start Lexer')
-        for fileName, fileContent in self.files.items():
-            self.lex(fileContent, fileName, 1, 1)
+        for filename, file_content in self.files.items():
+            self.lex(filename, file_content)
 
         self.__logger.info(
             'Shuting down Lexer, processed %d file(s) and generated %d tokens',
-            len(self.__files),
-            len(self.__tokenList),
+            len(self.files),
+            len(self.tokenList),
         )
-        return self.__tokenList
+        return self.tokenList
 
     def lex(
         self,
-        codeString: str,
-        fileName: str,
-        startLine: int = 1,
-        startColumn: int = 1,
+        filename: str,
+        file_content: str,
     ) -> None:
         """Tokenize a file contents
 
         Parameters
         ----------
-        codeString : str
-            Content of the file
-        fileName : str
+        filename : str
             Name of the file
-        startLine : int, optional
-            Starting line of the content in the file, by default 1
-        startColumn : int, optional
-            Starting column of the content in the file, by default 1
+        file_content : str
+            Content of the file
 
         Raises
         ------
         DSLParserNoEndingQuotes
             Syntax error : detected a starting quote but no ending one
         """
-        self.__logger.debug('Lex file %s', fileName)
-        self.__lexerPosition = LexerPosition(fileName, startLine, startColumn)
 
-        for char in codeString:
+        self.__logger.debug('Lex file %s', filename)
+        self.__lexerPosition = LexerPosition(filename)
+
+        for char in file_content:
             self.__logger.debug('char %s', char)
             self.__currentChar = char
             if not self.__lexerPosition.isQuotedString:
-                self.__handleSyntaxTokens()
+                self.__handle_syntax_tokens()
                 continue
 
             if char in ['"', "'"]:
-                self.__handleDoubleQuotes(char)()
+                self.__handle_quotes(char)()
                 continue
 
             if char == '\n':
-                if self.__lexerPosition.isCurrentTokenMultiLine:
-                    self.__lexerPosition.newLine()
+                if self.__lexerPosition.isMultiLine:
+                    self.__lexerPosition.new_line()
                     continue
                 position = str(
                     Position(
                         self.__lexerPosition.currentFile,
                         self.__lexerPosition.currentLine,
                         self.__lexerPosition.currentColumn,
                     ),
                 )
                 self.__logger.error(
                     f'Invalid syntax, missing ending quotes at : {position}',
                 )
-                raise DSLParserNoEndingQuotes(position)
+                raise DSLParserNoEndingQuotesError(position)
 
-            self.__iterateNextChar()
+            self.__add_next_char()
 
-        self.__addFileEnd()
-        self.__logger.debug('Finished lexing file %s', fileName)
+        self.__end_file()
+        self.__logger.debug('Finished lexing file %s', filename)
 
-    def __iterateNextChar(self):
-        """Iterate to the next character
-
-        Add the current character to the current Token
+    def __add_next_char(self):
+        """Add the current character to the current Token
         """
-        self.__lexerPosition.addCharToCurrentToken(self.__currentChar)
-        self.__lexerPosition.nextColumn()
+        self.__lexerPosition.add_to_current_token(self.__currentChar)
+        self.__lexerPosition.next_column()
 
-    def __handleEmptyToken(self):
+    def __handle_empty_token(self):
         pass
 
-    def __handleSyntaxTokens(self) -> None:
+    def __handle_syntax_tokens(self) -> None:
         """Handle single character tokens
 
         Check if the current character is a special token and calls the corresponding
         function.
         If it isn't, it calls the '__iterateNextChar' function
         """
-        singleCharTokens = {
-            ':': self.__handleColonToken,
-            ',': self.__handleCommaToken,
-            '[': self.__handleBracketsStartToken,
-            ']': self.__handleBracketsEndToken,
-            '(': self.__handleParenthesesStartToken,
-            ')': self.__handleParenthesesEndToken,
-            '"': self.__handleDoubleQuotes('"'),
-            "'": self.__handleDoubleQuotes("'"),
-            '#': self.__handleHashToken,
-            '\n': self.__handleNewlineToken,
-            '\\': self.__handleBackSlashToken,
-            '\t': self.__handleTabToken,
-            ' ': self.__handleWhitespace,
-
-            '=': self._handleEQToken,
-            '/': self._handleDivToken,
-            '-': self._handleMinusToken,
-            '+': self._handlePlusToken,
-            '*': self._handleMulToken,
-            '^': self._handlePowToken,
-            '<': self._handleLTToken,
-            '>': self._handleGTToken,
-            '!': self._handleExclamationToken,
+        single_char_tokens = {
+            ':': self.__handle_colon_oken,
+            ',': self.__handle_comma_token,
+            '[': self.__handle_brackets_start_token,
+            ']': self.__handle_brackets_end_token,
+            '(': self.__handle_parentheses_start_token,
+            ')': self.__handle_parentheses_end_token,
+            '"': self.__handle_quotes('"'),
+            "'": self.__handle_quotes("'"),
+            '#': self.__handle_hash_token,
+            '\n': self.__handle_newline_token,
+            '\\': self.__handle_backslash_token,
+            '\t': self.__handle_tab_token,
+            ' ': self.__handle_whitespace,
+
+            '=': self.__handle_eq_token,
+            '/': self.__handle_div_token,
+            '-': self.__handle_minus_token,
+            '+': self.__handle_plus_token,
+            '*': self.__handle_mul_token,
+            '^': self.__handle_pow_token,
+            '<': self.__handle_lt_token,
+            '>': self.__handle_gt_token,
+            '!': self.__handle_exclamation_token,
         }
 
-        singleCharTokens.get(self.__currentChar, self.__iterateNextChar)()
+        single_char_tokens.get(self.__currentChar, self.__add_next_char)()
 
-    def __handleCurrentToken(self) -> None:
+    def __handle_current_token(self) -> None:
         """Process the current stored token
 
         Check if the current token is a keyword, calls the cprresponding function, or
         the '__handleLiteralsAndVariables' otherwise.
         """
-        currentTokenLower = self.__lexerPosition.currentToken.lower()
+        current_token = self.__lexerPosition.currentToken.lower()
 
-        keyWordsAndTokens = {
-            '': self.__handleEmptyToken,
-            'amount': self.__handleAmountToken,
-            'and': self.__handleAndToken,
-            'if': self.__handleIfToken,
-            'elif': self.__handleElifToken,
-            'else': self.__handleElseToken,
-            'or': self.__handleOrToken,
-            'true': self.__handleBooleanToken,
-            'false': self.__handleBooleanToken,
-            'not': self.__handleNotToken,
+        keywords = {
+            '': self.__handle_empty_token,
+            'amount': self.__handle_amount_token,
+            'and': self.__handle_and_token,
+            'if': self.__handle_if_token,
+            'elif': self.__handle_elif_token,
+            'else': self.__handle_else_token,
+            'or': self.__handle_or_token,
+            'true': self.__handle_boolean_token,
+            'false': self.__handle_boolean_token,
+            'not': self.__handle_not_token,
         }
 
-        keyWordsAndTokens.get(
-            currentTokenLower, self.__handleLiteralsAndVariables,
-        )()
+        keywords.get(current_token, self.__handle_literals_and_variables)()
 
-    def __handleLiteralsAndVariables(self) -> None:
+    def __handle_literals_and_variables(self) -> None:
         """Create a literal or var token
 
         Checks the current token to create a var, int, float or string token
         """
-        currentToken = self.__lexerPosition.currentToken
-        if self.__lexerPosition.isCurrentTokenAVariable:
-            self.__addLiteralTokenToList(TT.VAR, currentToken)
-            self.__lexerPosition.setIsVariable(False)
+        current_token = self.__lexerPosition.currentToken
+        if self.__lexerPosition.isVariable:
+            self.__add_literal_token_to_list(TT.VAR, current_token)
+            self.__lexerPosition.isVariable = False
 
-        elif currentToken.isdigit():
-            self.__addLiteralTokenToList(TT.INT, currentToken)
+        elif current_token.isdigit():
+            self.__add_literal_token_to_list(TT.INT, current_token)
 
-        elif self.__isfloat(currentToken):
-            self.__addLiteralTokenToList(TT.FLOAT, currentToken)
+        elif self.__isfloat(current_token):
+            self.__add_literal_token_to_list(TT.FLOAT, current_token)
 
         else:
-            self.__addLiteralTokenToList(TT.STRING, currentToken)
+            self.__add_literal_token_to_list(TT.STRING, current_token)
 
-    def __addLiteralTokenToList(self, tokenType: str, value: str):
+    def __add_literal_token_to_list(self, token_type: str, value: str):
         """Add a literal token to the token list
 
         Parameters
         ----------
         tokenType : str
             Type of the token
         value : str
             Value of the token
         """
-        self.__lexerPosition.resetConsecutiveWhitespaces()
-        self.__addBaseToken(
-            tokenType,
+        self.__lexerPosition.reset_consecutive_whitespaces()
+        self.__add_base_token(
+            token_type,
             value,
-            isCurrentToken=True,
+            is_current_token=True,
         )
 
-    def __addBaseToken(
+    def __add_base_token(
         self,
-        tokenType: str,
+        token_type: str,
         value: str | None = None,
-        isCurrentToken: bool = False,
+        is_current_token: bool = False,
     ) -> None:
         """Add a token to the token list
 
         Parameters
         ----------
         tokenType : str
             Type of the token
         value : str, optional
             Value of the token, by default None
         isCurrentToken : bool, optional
             Indicates if this token is the current stored token, by default False
         """
-        if not isCurrentToken:
-            self.__addTokenToList(
+        if not is_current_token:
+            self.__add_token_to_list(
                 Token(
                     self.__lexerPosition.currentCharPosition,
-                    tokenType,
+                    token_type,
                     value,
                 ),
             )
             return
 
-        self.__addTokenToList(
+        self.__add_token_to_list(
             Token(
                 self.__lexerPosition.currentTokenPosition,
-                tokenType,
+                token_type,
                 value,
             ),
         )
 
-    def __basePositionUpdate(
+    def __update_position(
         self,
-        resetCurrentToken: bool = True,
+        reset_current_token: bool = True,
     ) -> None:
         """Update the lexer's current position
 
         Parameters
         ----------
         resetCurrentToken : bool, optional
             Indicates if the current stored token should be reset, by default True
         """
-        self.__lexerPosition.nextColumn()
-        if resetCurrentToken:
-            self.__lexerPosition.resetCurrentToken()
+        self.__lexerPosition.next_column()
+        if reset_current_token:
+            self.__lexerPosition.reset_current_token()
 
-        self.__lexerPosition.resetConsecutiveWhitespaces()
-        self.__lexerPosition.setIsVariable(False)
+        self.__lexerPosition.reset_consecutive_whitespaces()
+        self.__lexerPosition.isVariable = False
 
-    def __handleBaseToken(
+    def __handle_base_token(
         self,
-        tokenType: str,
+        token_type: str,
         value: str | None = None,
-        isCurrentToken: bool = False,
-        handleCurrentToken: bool = True,
-        resetCurrentToken: bool = True,
+        is_current_token: bool = False,
+        handle_current_token: bool = True,
+        reset_current_token: bool = True,
     ) -> None:
         """Handle a token creation and lexer position
 
         Parameters
         ----------
-        tokenType : str
+        token_type : str
             Type of the token
         value : str, optional
             Value of the token, by default None
-        isCurrentToken : bool, optional
+        is_current_token : bool, optional
             Indicates if this token is the current stored token, by default False
-        handleCurrentToken : bool, optional
+        handle_current_token : bool, optional
             Indicates if the current stored token should be processed, by default True
-        resetCurrentToken : bool, optional
+        reset_current_token : bool, optional
             Indicates if the current stored token should be reset, by default True
         """
-        if handleCurrentToken:
-            self.__handleCurrentToken()
-        self.__addBaseToken(tokenType, value, isCurrentToken)
-        self.__basePositionUpdate(resetCurrentToken)
+        if handle_current_token:
+            self.__handle_current_token()
+        self.__add_base_token(token_type, value, is_current_token)
+        self.__update_position(reset_current_token)
 
-    def __handleColonToken(self):
+    def __handle_colon_oken(self):
         """Handle a COLON token ':'
         """
-        self.__handleBaseToken(TT.COLON)
+        self.__handle_base_token(TT.COLON)
 
-    def __handleCommaToken(self):
+    def __handle_comma_token(self):
         """Handle a COMMA token ','
         """
-        self.__handleBaseToken(TT.COMMA)
+        self.__handle_base_token(TT.COMMA)
 
-    def __handleBracketsStartToken(self):
+    def __handle_brackets_start_token(self):
         """Handle a BRACKETS_START token '['
         """
-        self.__handleBaseToken(TT.BRACKETS_START)
+        self.__handle_base_token(TT.BRACKETS_START)
 
-    def __handleBracketsEndToken(self):
+    def __handle_brackets_end_token(self):
         """Handle a BRACKETS_END token ']'
         """
-        self.__handleBaseToken(TT.BRACKETS_END)
+        self.__handle_base_token(TT.BRACKETS_END)
 
-    def __handleParenthesesStartToken(self):
-        """Handle a PARENTESES_START token '('
+    def __handle_parentheses_start_token(self):
+        """Handle a PARENTHESES_START token '('
         """
-        self.__handleBaseToken(TT.PARENTHESES_START)
+        self.__handle_base_token(TT.PARENTHESES_START)
 
-    def __handleParenthesesEndToken(self):
+    def __handle_parentheses_end_token(self):
         """Handle a PARENTHESES_END token ')'
         """
-        self.__handleBaseToken(TT.PARENTHESES_END)
+        self.__handle_base_token(TT.PARENTHESES_END)
 
-    def _handlePlusToken(self):
+    def __handle_plus_token(self):
         """Handle a PLUS token '+'
         """
-        self.__handleBaseToken(TT.PLUS)
+        self.__handle_base_token(TT.PLUS)
 
-    def _handleMinusToken(self):
+    def __handle_minus_token(self):
         """Handle a MINUS token '-'
         """
-        self.__handleBaseToken(TT.MINUS)
+        self.__handle_base_token(TT.MINUS)
 
-    def _handleMulToken(self):
+    def __handle_mul_token(self):
         """Handle a MUL token '*'
         """
-        self.__handleBaseToken(TT.MUL)
+        self.__handle_base_token(TT.MUL)
 
-    def _handleDivToken(self):
+    def __handle_div_token(self):
         """Handle a DIV token '/'
         """
-        self.__handleBaseToken(TT.DIV)
+        self.__handle_base_token(TT.DIV)
 
-    def _handleEQToken(self):
+    def __handle_eq_token(self):
         """Handle a EQ token '='
         """
-        self.__handleBaseToken(TT.EQ)
+        self.__handle_base_token(TT.EQ)
 
-    def _handleExclamationToken(self):
-        """Handle a NE token '!='
+    def __handle_exclamation_token(self):
+        """Handle a EXCLAMATION token '!'
         """
-        self.__handleBaseToken(TT.EXCLAMATION)
+        self.__handle_base_token(TT.EXCLAMATION)
 
-    def _handleLTToken(self):
+    def __handle_lt_token(self):
         """Handle a LT token '<'
         """
-        self.__handleBaseToken(TT.LT)
+        self.__handle_base_token(TT.LT)
 
-    def _handleGTToken(self):
+    def __handle_gt_token(self):
         """Handle a GT token '>'
         """
-        self.__handleBaseToken(TT.GT)
+        self.__handle_base_token(TT.GT)
 
-    def _handlePowToken(self):
+    def __handle_pow_token(self):
         """Handle a POW token '^'
         """
-        self.__handleBaseToken(TT.POW)
+        self.__handle_base_token(TT.POW)
 
-    def __handleHashToken(self) -> None:
+    def __handle_hash_token(self) -> None:
         """Handle a HASH token '#'
 
         Sets a variable to indicate that the following literal is a Variable
         """
-        self.__handleCurrentToken()
-        self.__basePositionUpdate()
-        self.__lexerPosition.setIsVariable(True)
+        self.__handle_current_token()
+        self.__update_position()
+        self.__lexerPosition.isVariable = True
 
-    def __handleWhitespace(self) -> None:
+    def __handle_whitespace(self) -> None:
         """Handle a WHITESPACE token ' '
 
         Replaces 4 following whitespaces by a TAB token
         """
-        self.__handleCurrentToken()
-        self.__addBaseToken(TT.WHITESPACE)
-        self.__lexerPosition.nextColumn()
-        self.__lexerPosition.resetCurrentToken()
-        self.__lexerPosition.setIsVariable(False)
-        self.__lexerPosition.addConsecutiveWhitespace()
+        self.__handle_current_token()
+        self.__add_base_token(TT.WHITESPACE)
+        self.__lexerPosition.next_column()
+        self.__lexerPosition.reset_current_token()
+        self.__lexerPosition.isVariable = False
+        self.__lexerPosition.increment_consecutive_whitespaces()
         if self.__lexerPosition.consecutiveWhitespaces == 4:
-            self.__lexerPosition.nextColumn(-4)
-            self.__rmLastTokens(4)
-            self.__addBaseToken(TT.TAB)
-            self.__lexerPosition.nextColumn(4)
-            self.__lexerPosition.resetConsecutiveWhitespaces()
-            self.__lexerPosition.setCurrentTokenIndex()
+            self.__lexerPosition.next_column(-4)
+            self.__rm_last_tokens(4)
+            self.__add_base_token(TT.TAB)
+            self.__lexerPosition.next_column(4)
+            self.__lexerPosition.reset_consecutive_whitespaces()
+            self.__lexerPosition.set_current_token_index()
 
-    def __handleNewlineToken(self) -> None:
+    def __handle_newline_token(self) -> None:
         """Handle a NEWLINE token '\\n'
         """
-        if not self.__lexerPosition.isCurrentTokenMultiLine:
-            self.__handleBaseToken(TT.NEWLINE)
+        if not self.__lexerPosition.isMultiLine:
+            self.__handle_base_token(TT.NEWLINE)
 
-        self.__lexerPosition.newLine()
-        if not self.__lexerPosition.isCurrentTokenMultiLine:
-            self.__lexerPosition.setCurrentTokenIndex()
+        self.__lexerPosition.new_line()
+        if not self.__lexerPosition.isMultiLine:
+            self.__lexerPosition.set_current_token_index()
 
-        self.__lexerPosition.setIsMultiLine(value=False)
+        self.__lexerPosition.isMultiLine = False
 
-    def __handleBackSlashToken(self) -> None:
+    def __handle_backslash_token(self) -> None:
         """Handle a BACKSLASH token '\\'
 
         Sets a variable to indicate that the following line is part of the same token.
         """
-        self.__lexerPosition.setIsMultiLine(value=True)
-        self.__lexerPosition.nextColumn()
+        self.__lexerPosition.isMultiLine = True
+        self.__lexerPosition.next_column()
 
-    def __handleTabToken(self) -> None:
+    def __handle_tab_token(self) -> None:
         """Handle a TAB token '\\t'
         """
-        self.__handleBaseToken(TT.TAB)
+        self.__handle_base_token(TT.TAB)
 
-    def __handleDoubleQuotes(self, char) -> None:
+    def __handle_quotes(self, char) -> None:
         """Handle a DOUBLEQUOTES token '"'
 
         Sets a variable to indicate that the following characters are a STRING token.
         """
 
-        def quoteHandler(self=self):
+        def quote_handler(self=self):
 
             if self.__lexerPosition.isQuotedString:
                 if char == self.__lexerPosition.isQuotedString:
-                    self.__addLiteralTokenToList(
+                    self.__add_literal_token_to_list(
                         TT.STRING, self.__lexerPosition.currentToken,
                     )
                     self.__lexerPosition.isQuotedString = False
-                    self.__basePositionUpdate()
+                    self.__update_position()
                 else:
-                    self.__iterateNextChar()
+                    self.__add_next_char()
             else:
-                self.__handleCurrentToken()
-                self.__lexerPosition.nextColumn()
+                self.__handle_current_token()
+                self.__lexerPosition.next_column()
                 self.__lexerPosition.isQuotedString = char
-                self.__lexerPosition.resetCurrentToken()
+                self.__lexerPosition.reset_current_token()
 
-        return quoteHandler
+        return quote_handler
 
-    def __handleAmountToken(self):
+    def __handle_amount_token(self):
         """Handle an AMOUNT token 'amount'
         """
-        self.__lexerPosition.resetConsecutiveWhitespaces()
-        self.__addBaseToken(TT.AMOUNT, isCurrentToken=True)
+        self.__lexerPosition.reset_consecutive_whitespaces()
+        self.__add_base_token(TT.AMOUNT, is_current_token=True)
 
-    def __handleAndToken(self):
+    def __handle_and_token(self):
         """Handle an AND token 'and'
         """
-        self.__lexerPosition.resetConsecutiveWhitespaces()
-        self.__addBaseToken(TT.AND, isCurrentToken=True)
+        self.__lexerPosition.reset_consecutive_whitespaces()
+        self.__add_base_token(TT.AND, is_current_token=True)
 
-    def __handleIfToken(self):
+    def __handle_if_token(self):
         """Handle an IF token 'if'
         """
-        self.__lexerPosition.resetConsecutiveWhitespaces()
-        self.__addBaseToken(TT.IF, isCurrentToken=True)
+        self.__lexerPosition.reset_consecutive_whitespaces()
+        self.__add_base_token(TT.IF, is_current_token=True)
 
-    def __handleElifToken(self):
+    def __handle_elif_token(self):
         """Handle an ELIF token 'elif'
         """
-        self.__lexerPosition.resetConsecutiveWhitespaces()
-        self.__addBaseToken(TT.ELIF, isCurrentToken=True)
+        self.__lexerPosition.reset_consecutive_whitespaces()
+        self.__add_base_token(TT.ELIF, is_current_token=True)
 
-    def __handleElseToken(self):
+    def __handle_else_token(self):
         """Handle an ELSE token 'else'
         """
-        self.__lexerPosition.resetConsecutiveWhitespaces()
-        self.__addBaseToken(TT.ELSE, isCurrentToken=True)
+        self.__lexerPosition.reset_consecutive_whitespaces()
+        self.__add_base_token(TT.ELSE, is_current_token=True)
 
-    def __handleNotToken(self):
+    def __handle_not_token(self):
         """Handle an OR token 'or'
         """
-        self.__lexerPosition.resetConsecutiveWhitespaces()
-        self.__addBaseToken(TT.NOT, isCurrentToken=True)
+        self.__lexerPosition.reset_consecutive_whitespaces()
+        self.__add_base_token(TT.NOT, is_current_token=True)
 
-    def __handleOrToken(self):
+    def __handle_or_token(self):
         """Handle an OR token 'or'
         """
-        self.__lexerPosition.resetConsecutiveWhitespaces()
-        self.__addBaseToken(TT.OR, isCurrentToken=True)
+        self.__lexerPosition.reset_consecutive_whitespaces()
+        self.__add_base_token(TT.OR, is_current_token=True)
 
-    def __handleBooleanToken(self):
+    def __handle_boolean_token(self):
         """Handle a BOOLEAN token 'true' or 'false'
         """
-        self.__lexerPosition.resetConsecutiveWhitespaces()
-        self.__addBaseToken(
+        self.__lexerPosition.reset_consecutive_whitespaces()
+        self.__add_base_token(
             TT.BOOLEAN, self.__lexerPosition.currentToken, True,
         )
 
-    def __handleEofToken(self) -> None:
+    def __handle_eof_token(self) -> None:
         """Add an EOF token at the end of each file
         """
-        self.__addBaseToken(TT.EOF)
+        self.__add_base_token(TT.EOF)
 
-    def __addTokenToList(self, token: Token | None) -> None:
+    def __add_token_to_list(self, token: Token | None) -> None:
         """Add a new token to the parser's token list
 
         Parameters
         ----------
         token : Token | None
             New token to add
         """
         if not token:
             pass
-        self.__tokenList.append(token)
+        self.tokenList.append(token)
 
-    def __rmLastTokens(self, amount: int = 1):
-        self.__tokenList = self.__tokenList[:-amount]
+    def __rm_last_tokens(self, amount: int = 1):
+        self.tokenList = self.tokenList[:-amount]
 
-    def __addFileEnd(self) -> None:
+    def __end_file(self) -> None:
         """Add a NEWLINE and an EOF token at the end of each file
         """
         if len(self.__lexerPosition.currentToken.strip()) > 0:
-            self.__handleCurrentToken()
-            self.__lexerPosition.resetCurrentToken()
-        self.__handleNewlineToken()
-        self.__handleEofToken()
+            self.__handle_current_token()
+            self.__lexerPosition.reset_current_token()
+        self.__handle_newline_token()
+        self.__handle_eof_token()
 
     def __isfloat(self, num: str) -> bool:
         """Check if the string is a float
 
         Parameters
         ----------
         num : str
```

### Comparing `thipster-0.17.0/thipster/parser/dsl_parser/parser.py` & `thipster-0.17.1/thipster/parser/dsl_parser/parser.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import os
 
-from thipster.engine import I_Parser
+from thipster.engine import ParserPort
 from thipster.engine.parsed_file import ParsedFile
 
-from .exceptions import DSLParserBaseException, DSLParserPathNotFound
+from .exceptions import DSLParserBaseError, DSLParserPathNotFoundError
 from .interpreter import Interpreter
 from .lexer import Lexer
 from .token_parser import TokenParser
 
 
-class DSLParser(I_Parser):
+class DSLParser(ParserPort):
 
     @classmethod
     def __getfiles(cls, path: str) -> dict[str, str]:
         """Recursively get all files in the requested directory and its sudirectories
         Can be run on a path file aswell
 
         Parameters
@@ -26,15 +26,15 @@
         dict[str, str]
             A dictionary that links a filename to its content, fileName : fileContent
         """
 
         path = os.path.abspath(path)
 
         if not os.path.exists(path):
-            raise DSLParserPathNotFound(path)
+            raise DSLParserPathNotFoundError(path)
 
         files = {}
 
         if os.path.isdir(path):
             for content in os.listdir(path):
                 files.update(DSLParser.__getfiles(f'{path}/{content}'))
 
@@ -68,11 +68,11 @@
             parser = TokenParser(token_list)
             ast = parser.run()
 
             interpreter = Interpreter()
             parsed_file = interpreter.run(ast)
 
             return parsed_file
-        except DSLParserBaseException as e:
+        except DSLParserBaseError as e:
             raise e
         except Exception as e:
             raise e
```

### Comparing `thipster-0.17.0/thipster/parser/dsl_parser/token.py` & `thipster-0.17.1/thipster/parser/dsl_parser/token.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,16 +75,16 @@
                 self.token_type == __value.token_type and
                 self.value == __value.value
             )
         else:
             raise TypeError('Value must be a Token')
 
     def __repr__(self) -> str:
-        tokenString = f'(Type: {str(self.token_type)}, Position: {str(self.position)}'
+        token_string = f'(Type: {str(self.token_type)}, Position: {str(self.position)}'
         if self.value:
-            tokenString += f', Value: {self.value}'
-        tokenString += ')'
+            token_string += f', Value: {self.value}'
+        token_string += ')'
 
-        return tokenString
+        return token_string
 
     def __str__(self) -> str:
         return f'({self.token_type} {self.value})'
```

### Comparing `thipster-0.17.0/thipster/parser/dsl_parser/token_parser.py` & `thipster-0.17.1/thipster/parser/dsl_parser/token_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import thipster.parser.dsl_parser.ast as ast
 
 from .exceptions import (
-    DSLConditionException,
-    DSLSyntaxException,
-    DSLUnexpectedEOF,
+    DSLConditionError,
+    DSLSyntaxError,
+    DSLUnexpectedEOFError,
 )
 from .token import TOKENTYPES as TT
 from .token import Token
 
 
 class TokenParser():
     def __init__(self, tokens: list[Token]) -> None:
@@ -31,32 +31,32 @@
     def __next(self, expected: TT | list[TT] | None = None) -> Token:
         """Get next token and pop it from the list"""
         next_token_type = self.__get_next_type()
 
         if expected:
             if type(expected) is list:
                 if next_token_type not in expected:
-                    raise DSLSyntaxException(self.__tokens[0], expected)
+                    raise DSLSyntaxError(self.__tokens[0], expected)
             elif next_token_type != expected:
-                raise DSLSyntaxException(self.__tokens[0], expected)
+                raise DSLSyntaxError(self.__tokens[0], expected)
         return self.__tokens.pop(0)
 
     def __check(self, expected: TT, index: int = 0) -> Token | None:
         """Check if the type of the next token is equal to the expected parameter. \
         Pop it from the list in that case"""
         token = self.__get_next_type(index=index)
         if token != expected:
             return None
 
         return self.__next(expected)
 
     def __get_next_type(self, index: int = 0):
         """Get the type of the next token"""
         if len(self.__tokens) <= index:
-            raise DSLUnexpectedEOF
+            raise DSLUnexpectedEOFError
 
         return self.__tokens[index].token_type
 
     def __trim_newlines(self):
         while self.__check(TT.NEWLINE):
             pass
 
@@ -115,15 +115,15 @@
             if_ctrl = self.__get_if_ctrl()
             self.__get_whitespaces()
 
             self.__get_newline()
 
             properties = self.__get_properties(indent+1)
 
-        except DSLSyntaxException as e:
+        except DSLSyntaxError as e:
             raise e
 
         resource = ast.ResourceNode(
             resource_type=resource_type,
             name=name,
             parameters=properties,
         )
@@ -141,15 +141,15 @@
     def __get_parameter(self, indent: int) -> ast.ParameterNode:
         """name, ":", (value, [if_else_ctrl] | [if_ctrl], "\\n", (list | dict))"""
         try:
             name = self.__next(TT.STRING)
             self.__get_whitespaces()
             self.__next(TT.COLON)
             self.__get_whitespaces()
-        except DSLSyntaxException as e:
+        except DSLSyntaxError as e:
             raise e
 
         next_token_type = self.__get_next_type()
 
         if next_token_type not in [
             TT.IF,
             TT.NEWLINE,
@@ -176,17 +176,17 @@
 
         # [if_ctrl], "\n" (liste | dict)
         try:
             if_ctrl = self.__get_if_ctrl()
             self.__get_whitespaces()
             newline = self.__get_newline()
             properties = self.__get_properties(indent+1)
-        except DSLSyntaxException as e:
+        except DSLSyntaxError as e:
             if e.token.token_type == TT.TAB:
-                raise DSLSyntaxException(
+                raise DSLSyntaxError(
                     token=newline,
                     expected=TT.STRING,
                 )
 
             raise e
 
         parameter = ast.ParameterNode(
@@ -213,22 +213,22 @@
             if next_token_type == TT.STRING:
                 props = self.__get_dict(indent)
 
             elif next_token_type == TT.MINUS:
                 props = self.__get_list(indent)
 
             else:
-                raise DSLSyntaxException(self.__next(), TT.TAB)
+                raise DSLSyntaxError(self.__next(), TT.TAB)
 
-        except DSLUnexpectedEOF as eof:
+        except DSLUnexpectedEOFError as eof:
             if indent > 1:
-                raise DSLUnexpectedEOF from eof
+                raise DSLUnexpectedEOFError from eof
 
             if eof.__cause__:
-                raise DSLUnexpectedEOF from eof.__cause__
+                raise DSLUnexpectedEOFError from eof.__cause__
 
             props = ast.DictNode([])
 
         return props
 
     def __get_list(self, indent: int) -> ast.ListNode:
         """{ "-", value, [amt_ctrl], [if_else_ctrl], "\\n"}"""
@@ -334,15 +334,15 @@
             self.__get_whitespaces()
             self.__next(TT.COLON)
 
             self.__get_whitespaces()
             amount = self.__get_arith_expr()
 
             self.__get_whitespaces()
-        except DSLSyntaxException as e:
+        except DSLSyntaxError as e:
             raise e
 
         amount_variable = self.__check(TT.VAR)
 
         return ast.AmountNode(
             position=amount_token,
             amount=amount,
@@ -360,15 +360,15 @@
         if not condition:
             return None
 
         self.__get_whitespaces()
         try:
             condition = self.__get_comp_expr()
             self.__get_whitespaces()
-        except DSLSyntaxException as e:
+        except DSLSyntaxError as e:
             raise e
 
         return ast.IfNode(
             condition=condition,
             if_case=None,
         )
 
@@ -481,16 +481,16 @@
                                 operator = Token(operator.position, TT.GTE)
 
                     self.__get_whitespaces()
                     right_expression = self.__get_arith_expr()
                     self.__get_whitespaces()
                     return ast.CompExprNode(left_expression, operator, right_expression)
 
-        except DSLSyntaxException as e:
-            raise DSLConditionException(e.token)
+        except DSLSyntaxError as e:
+            raise DSLConditionError(e.token)
 
     def __get_arith_expr(self) -> ast.ArithExprNode:
         terms = []
         operator = []
         terms.append(self.__get_term())
         self.__get_whitespaces()
 
@@ -559,15 +559,15 @@
                 expression = self.__get_arith_expr()
                 self.__get_whitespaces()
                 self.__next(TT.PARENTHESES_END)
                 self.__get_whitespaces()
                 return expression
 
             case _:
-                raise DSLSyntaxException(
+                raise DSLSyntaxError(
                     self.__tokens[0], [TT.INT, TT.FLOAT, TT.PARENTHESES_START],
                 )
 
     def __get_string_expr(self):
         values = []
         token = self.__next([TT.STRING, TT.VAR])
         match token.token_type:
```

### Comparing `thipster-0.17.0/thipster/parser/parser_factory.py` & `thipster-0.17.1/thipster/parser/parser_factory.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,46 +1,37 @@
 import os
 
-from thipster.engine import I_Parser, THipsterException
+from thipster.engine import ParserPort
 from thipster.engine.parsed_file import ParsedFile
 
 from .dsl_parser import DSLParser
+from .exceptions import (
+    NoFileFoundError,
+    ParserPathNotFoundError,
+)
 from .yaml_parser import YAMLParser
 
 
-def _noParser(pathExtension):
-    class noParser():
-        def run(path):
-            raise Exception(f'{pathExtension} files can\'t be parsed')
-
-    return noParser
-
-
-class ParserPathNotFound(THipsterException):
-    def __init__(cls, path, *args: object) -> None:
-        super().__init__(*args)
-
-        cls.__path = path
-
-    @property
-    def message(cls) -> str:
-        return f'Path not found : {cls.__path}'
+class NoParser(ParserPort):
+    @classmethod
+    def run(cls, path) -> ParsedFile:
+        return ParsedFile()
 
 
-class ParserFactory(I_Parser):
+class ParserFactory(ParserPort):
 
     __parsers = {
         '.yaml': YAMLParser,
         '.yml': YAMLParser,
         '.jinja': YAMLParser,
         '.thips': DSLParser,
     }
 
     @classmethod
-    def addParser(cls, parser: I_Parser, extensions: list[str]):
+    def add_parser(cls, parser: ParserPort, extensions: list[str]):
         cls.__parsers.update({e: parser for e in extensions})
 
     @classmethod
     def __getfiles(cls, path: str) -> list[str]:
         """Recursively get all files names in the requested directory and its\
               sudirectories
         Can be run on a path file aswell
@@ -55,15 +46,15 @@
         list[str]
             A list of all the filenames
         """
 
         path = os.path.abspath(path)
 
         if not os.path.exists(path):
-            raise ParserPathNotFound(path)
+            raise ParserPathNotFoundError(path)
 
         files = []
 
         if os.path.isdir(path):
             for content in os.listdir(path):
                 files += cls.__getfiles(f'{path}/{content}')
 
@@ -86,20 +77,23 @@
         ParsedFile
             A ParsedFile object with the content of all the files in the input path
         """
         files = cls.__getfiles(path)
 
         res = ParsedFile()
         for file in files:
-            parsedFile = cls.__getParser(file).run(file)
-            res.resources += parsedFile.resources
+            parsed_file = cls.__get_parser(file).run(file)
+            res.resources += parsed_file.resources
+
+        if len(res.resources) == 0:
+            raise NoFileFoundError(path)
 
         return res
 
     @classmethod
-    def __getParser(cls, path) -> I_Parser:
+    def __get_parser(cls, path) -> ParserPort:
 
-        _, pathExtension = os.path.splitext(path)
+        _, path_extension = os.path.splitext(path)
 
         return cls.__parsers.get(
-            pathExtension, _noParser(pathExtension),
+            path_extension, NoParser,
         )
```

### Comparing `thipster-0.17.0/thipster/parser/yaml_parser.py` & `thipster-0.17.1/thipster/parser/yaml_parser.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,42 +1,35 @@
 import os
+from abc import ABC
 
 import yaml
 from jinja2 import Environment, FileSystemLoader
 
 import thipster.engine.parsed_file as pf
-from thipster.engine import I_Parser, THipsterException
+from thipster.engine import ParserPort, THipsterError
 
+from .exceptions import ParserPathNotFoundError
 
-class YAMLParserBaseException(THipsterException):
-    def __init__(self, *args: object) -> None:
-        super().__init__(*args)
 
-
-class YAMLParserPathNotFound(YAMLParserBaseException):
-    def __init__(self, file, *args: object) -> None:
+class YAMLParserBaseError(THipsterError, ABC):
+    def __init__(self, *args: object) -> None:
         super().__init__(*args)
-        self.file = file
-
-    @property
-    def message(self) -> str:
-        return f'Path not found : {self.file}',
 
 
-class YAMLParserNoName(YAMLParserBaseException):
+class YAMLParserNoNameError(YAMLParserBaseError):
     def __init__(self, resource, *args: object) -> None:
         super().__init__(*args)
         self.resource = resource
 
     @property
     def message(self) -> str:
         return f'No name for resource : {self.resource}'
 
 
-class YAMLParser(I_Parser):
+class YAMLParser(ParserPort):
     @classmethod
     def __getfiles(cls, path: str) -> list[str]:
         """Recursively get all files names in the requested directory and its\
               sudirectories
         Can be run on a path file aswell
 
         Parameters
@@ -48,15 +41,15 @@
         -------
         list[str]
             A list of all the filenames
         """
         path = os.path.abspath(path)
 
         if not os.path.exists(path):
-            raise YAMLParserPathNotFound(path)
+            raise ParserPathNotFoundError(path)
 
         files = []
 
         if os.path.isdir(path):
             for content in os.listdir(path):
                 files += cls.__getfiles(f'{path}/{content}')
 
@@ -95,15 +88,15 @@
                 content = yaml.safe_load(rendered)
 
                 parsed_file.resources += cls.__convert(content)
 
             return parsed_file
         except yaml.YAMLError as exc:
             raise exc
-        except YAMLParserBaseException as e:
+        except YAMLParserBaseError as e:
             raise e
         except Exception as e:
             raise e
 
     @classmethod
     def __convert(cls, file: dict) -> list[pf.ParsedResource]:
         """Converts a dictionnary into a list of ParsedResources
@@ -123,27 +116,27 @@
         for key, val in file.items():
             if type(val) == list:
                 for res in val:
                     if 'name' in res:
                         name = res['name']
                         del res['name']
                     else:
-                        raise YAMLParserNoName(key)
+                        raise YAMLParserNoNameError(key)
 
                     resources.append(
                         cls.__get_resource(
                             content=res, resource_type=key, name=name,
                         ),
                     )
             elif type(val) == dict:
                 if 'name' in val:
                     name = val['name']
                     del val['name']
                 else:
-                    raise YAMLParserNoName(key)
+                    raise YAMLParserNoNameError(key)
 
                 resources.append(
                     cls.__get_resource(
                         content=val, resource_type=key, name=name,
                     ),
                 )
```

### Comparing `thipster-0.17.0/thipster/repository/github.py` & `thipster-0.17.1/thipster/repository/github.py`

 * *Files identical despite different names*

### Comparing `thipster-0.17.0/thipster/repository/json.py` & `thipster-0.17.1/thipster/repository/json.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,85 +1,85 @@
 """JSONRepo.py module.
 """
 
 import json
 from abc import ABC, abstractmethod
 
 import thipster.engine.resource_model as rm
-from thipster.engine import I_Repository
+from thipster.engine import RepositoryPort
 
 
-class JSONRepo(I_Repository, ABC):
-    _parentStack = []
+class JSONRepo(RepositoryPort, ABC):
+    _parent_stack = []
     """Class representing a JSON resources Repository
 
     JSON Models of resources and services offered by supported cloud providers are
     stored in a repository.
     """
 
     def __init__(self) -> None:
         super().__init__()
         self.model_list = {}
 
     @abstractmethod
     def get_json(self, name: str) -> str | bytes | bytearray:
         raise Exception()
 
-    def get(self, resourceNames: list[str]) -> dict[str, rm.ResourceModel]:
+    def get(self, resource_names: list[str]) -> dict[str, rm.ResourceModel]:
         """Get the corresponding resource Models from a list of names
 
         Parameters
         ----------
         resourceNames : list[str]
             List of the desired resource models names
 
         Returns
         -------
         dict[str, rm.ResourceModel]
             Dictionnary of the corresponding resource models
         """
-        for resource in resourceNames:
+        for resource in resource_names:
             self.__add_model(resource)
 
         return self.model_list
 
-    def __create_value(self, val: object | None) -> rm.I_Model_Value | None:
+    def __create_value(self, val: object | None) -> rm.ModelValue | None:
         """Creates the right Model value implementation from the raw JSON
 
         Parameters
         ----------
         val : object
             Raw JSON model's attribute value
 
         Returns
         -------
-        I_Model_Value | None
-            Value of the attribute, implementation of I_Model_Value : Model_Dict,
-            Model_List, Model_Literal or None
+        ModelValue | None
+            Value of the attribute, implementation of ModelValue : ModelDict,
+            ModelList, ModelLiteral or None
         """
         if val is None:
             return None
         elif isinstance(val, dict):
-            return rm.Model_Dict(None)
+            return rm.ModelDict(None)
         elif isinstance(val, list):
-            return rm.Model_List([self.__create_value(i) for i in val])
+            return rm.ModelList([self.__create_value(i) for i in val])
 
-        return rm.Model_Literal(val)
+        return rm.ModelLiteral(val)
 
-    def __create_attribute(self, raw: dict[str, str]) -> list[rm.Model_Attribute]:
+    def __create_attribute(self, raw: dict[str, str]) -> list[rm.ModelAttribute]:
         """Creates a model's attributes from the raw JSON input
 
         Parameters
         ----------
         raw : dict[str, str]
             Json model's raw attributes
 
         Returns
         -------
-        list[Model_Attribute]
+        list[ModelAttribute]
             Attributes of the resource model
         """
 
         attributes = {}
 
         for name, attr in raw.items():
             optional = attr['optional'] if 'optional' in attr.keys(
@@ -89,15 +89,15 @@
             ) else None
 
             is_list = 'list' in attr['var_type'] if 'var_type' in attr.keys(
             ) else False
 
             default = self.__create_value(value)
 
-            attributes[name] = rm.Model_Attribute(
+            attributes[name] = rm.ModelAttribute(
                 attr['cdk_key'],
                 default=default,
                 optional=optional,
                 is_list=is_list,
             )
 
         return attributes
@@ -120,17 +120,17 @@
 
         json_model = json.loads(model)
 
         for _, dep in json_model['dependencies'].items():
             if dep['resource'] not in self.model_list.keys():
                 self.__add_model(dep['resource'])
 
-        for _, intObj in json_model['internalObjects'].items():
-            if intObj['resource'] not in self.model_list.keys():
-                self.__add_model(intObj['resource'])
+        for _, internal_object in json_model['internalObjects'].items():
+            if internal_object['resource'] not in self.model_list.keys():
+                self.__add_model(internal_object['resource'])
 
         res = rm.ResourceModel(
             name,
             attributes=self.__create_attribute(json_model['attributes']),
             dependencies=json_model['dependencies'],
             internal_objects=json_model['internalObjects'],
             name_key=json_model['cdk_name_key']
```

### Comparing `thipster-0.17.0/thipster/terraform/cdk.py` & `thipster-0.17.1/thipster/terraform/cdk.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,24 +9,24 @@
 from cdktf import App, TerraformStack
 from constructs import Construct
 from python_terraform import Terraform
 
 import thipster.engine.parsed_file as pf
 import thipster.engine.resource_model as rm
 import thipster.terraform.exceptions as cdk_exceptions
-from thipster.engine import I_Auth, I_Terraform
+from thipster.engine import AuthPort, TerraformPort
 from thipster.helpers import create_logger
 
 
 class ResourceCreationContext():
     def __init__(self) -> None:
         pass
 
 
-class CDK(I_Terraform):
+class CDK(TerraformPort):
     _models = []
     _parent_resources_stack = []
     _resources_to_create = []
 
     _inherited_attributes: list[pf.ParsedAttribute] = []
     _created_resources = {}
     _logger = create_logger(__name__)
@@ -48,25 +48,25 @@
         t = Terraform()
         _, stdout, stderr = t.apply(plan_file_path)
         return stdout + stderr
 
     @classmethod
     def generate(
         cls, file: pf.ParsedFile, models: dict[str, rm.ResourceModel],
-        _authenticator: I_Auth,
+        _authenticator: AuthPort,
     ):
         """Generate Terraform file from given parsed file and models
 
         Parameters
         ----------
         file : pf.ParsedFile
             parsedFile object to transform
         models : dict[str, rm.ResourceModel]
             associated models
-        _auth : I_Auth
+        _auth : AuthPort
             authenticator to use
         """
         cls._created_resources = {}
         cls._models = models
         cls._parent_resources_stack = []
 
         # Init CDK
@@ -217,40 +217,42 @@
         all the information needed to instantiate the class with default values
     """
     # Checks for cyclic dependency
     if resource_type in CDK._parent_resources_stack:
         CDK._logger.error(
             '%s already present in parent Stack', resource_type,
         )
-        raise cdk_exceptions.CDKCyclicDependencies(
+        raise cdk_exceptions.CDKCyclicDependenciesError(
             CDK._parent_resources_stack,
         )
 
     CDK._parent_resources_stack.append(resource_type)
 
     model = CDK._models[resource_type]
 
     attributes = copy.deepcopy(model.attributes)
 
     for a in CDK._inherited_attributes:
         if a.name in attributes.keys():
-            attributes[a.name].default = rm.Model_Literal(a.value)
+            attributes[a.name].default = rm.ModelLiteral(a.value)
 
         else:
-            attributes[a.name] = rm.Model_Attribute(
+            attributes[a.name] = rm.ModelAttribute(
                 cdk_name=a.name,
-                default=rm.Model_Literal(a.value),
+                default=rm.ModelLiteral(a.value),
             )
 
     # Checks that all attributes have a default value
     if (
         no_modif
         and not all(map(lambda x: x.default is not None, attributes.values()))
     ):
-        raise cdk_exceptions.CDKMissingAttributeInDependency(resource_type)
+        raise cdk_exceptions.CDKMissingAttributeInDependencyError(
+            resource_type,
+        )
 
     # Import package and class
     CDK._pip_install(model.cdk_provider)
     resource_class = CDK._import(
         model.cdk_provider, model.cdk_module, model.cdk_name,
     )
 
@@ -736,15 +738,15 @@
     created_name = f'{dependency_type}/'\
         f'{dependency_value}'
 
     # Checks if attribute is an explicit dependency
     if created_name not in CDK._created_resources.keys():
 
         if isinstance(dependency_value, str):
-            raise cdk_exceptions.CDKDependencyNotDeclared(
+            raise cdk_exceptions.CDKDependencyNotDeclaredError(
                 attribute_name, dependency_value,
             )
 
         # Creates explicit dependency
         _create_dependency(
             resource_self, attribute_name, dependency_value,
             resource_args, attribute_name,
```

### Comparing `thipster-0.17.0/thipster.egg-info/PKG-INFO` & `thipster-0.17.1/thipster.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thipster
-Version: 0.17.0
+Version: 0.17.1
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
-Metadata-Version: 2.1 Name: thipster Version: 0.17.0 Summary: THipster is a
+Metadata-Version: 2.1 Name: thipster Version: 0.17.1 Summary: THipster is a
 tool dedicated to simplifying the difficulty associated with writing Terraform
 files. It allows users to write infrastructure as code in a simplified format,
 using either YAML (with JINJA) or the dedicated Thipster DSL. Home-page: https:
 //github.com/THipster/THipster Download-URL: https://github.com/THipster/
 THipster.git Keywords: thipster,terraform,infrastructure,infrastructure-as-
 code,iac,generator,dsl,yaml Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python :: 3.11 Classifier: License :: OSI
```

### Comparing `thipster-0.17.0/thipster.egg-info/SOURCES.txt` & `thipster-0.17.1/thipster.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -7,20 +7,20 @@
 tests/__init__.py
 tests/test_e2e.py
 tests/test_tools.py
 tests/engine/__init__.py
 tests/engine/test_engine.py
 tests/engine/test_generation.py
 tests/parser/__init__.py
-tests/parser/test_ParserFactory.py
-tests/parser/test_YAMLParser.py
 tests/parser/test_parsedfile.py
+tests/parser/test_parserfactory.py
+tests/parser/test_yamlparser.py
 tests/parser/dsl_parser/__init__.py
-tests/parser/dsl_parser/test_DSLparser.py
 tests/parser/dsl_parser/test_ast.py
+tests/parser/dsl_parser/test_dslparser.py
 tests/parser/dsl_parser/test_lexer.py
 tests/parser/dsl_parser/test_token.py
 tests/parser/dsl_parser/test_tokenparser.py
 thipster/__init__.py
 thipster/helpers.py
 thipster.egg-info/PKG-INFO
 thipster.egg-info/SOURCES.txt
@@ -35,14 +35,15 @@
 thipster/engine/i_auth.py
 thipster/engine/i_parser.py
 thipster/engine/i_repository.py
 thipster/engine/i_terraform.py
 thipster/engine/parsed_file.py
 thipster/engine/resource_model.py
 thipster/parser/__init__.py
+thipster/parser/exceptions.py
 thipster/parser/parser_factory.py
 thipster/parser/yaml_parser.py
 thipster/parser/dsl_parser/__init__.py
 thipster/parser/dsl_parser/ast.py
 thipster/parser/dsl_parser/exceptions.py
 thipster/parser/dsl_parser/interpreter.py
 thipster/parser/dsl_parser/lexer.py
```

