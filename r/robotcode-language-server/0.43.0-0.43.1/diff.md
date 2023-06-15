# Comparing `tmp/robotcode_language_server-0.43.0.tar.gz` & `tmp/robotcode_language_server-0.43.1.tar.gz`

## Comparing `robotcode_language_server-0.43.0.tar` & `robotcode_language_server-0.43.1.tar`

### file list

```diff
@@ -1,87 +1,87 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/__init__.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/__version__.py
--rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/cli.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/hooks.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/common/__init__.py
--rw-r--r--   0        0        0     2563 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/common/decorators.py
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/common/has_extend_capabilities.py
--rw-r--r--   0        0        0    11515 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/common/protocol.py
--rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/common/server.py
--rw-r--r--   0        0        0     9485 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/common/text_document.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/common/parts/__init__.py
--rw-r--r--   0        0        0     4411 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/common/parts/code_action.py
--rw-r--r--   0        0        0     4239 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/common/parts/code_lens.py
--rw-r--r--   0        0        0     3438 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/common/parts/commands.py
--rw-r--r--   0        0        0     6206 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/common/parts/completion.py
--rw-r--r--   0        0        0     4648 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/common/parts/declaration.py
--rw-r--r--   0        0        0     4650 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/common/parts/definition.py
--rw-r--r--   0        0        0    21107 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/common/parts/diagnostics.py
--rw-r--r--   0        0        0     2689 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/common/parts/document_highlight.py
--rw-r--r--   0        0        0     5937 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/common/parts/document_symbols.py
--rw-r--r--   0        0        0    14870 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/common/parts/documents.py
--rw-r--r--   0        0        0     2784 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/common/parts/folding_range.py
--rw-r--r--   0        0        0     4399 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/common/parts/formatting.py
--rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/common/parts/hover.py
--rw-r--r--   0        0        0     4651 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/common/parts/implementation.py
--rw-r--r--   0        0        0     3858 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/common/parts/inlay_hint.py
--rw-r--r--   0        0        0     3657 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/common/parts/inline_value.py
--rw-r--r--   0        0        0     2730 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/common/parts/linked_editing_ranges.py
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/common/parts/protocol_part.py
--rw-r--r--   0        0        0     2842 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/common/parts/references.py
--rw-r--r--   0        0        0     5780 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/common/parts/rename.py
--rw-r--r--   0        0        0     2891 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/common/parts/selection_range.py
--rw-r--r--   0        0        0     6963 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/common/parts/semantic_tokens.py
--rw-r--r--   0        0        0     3629 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/common/parts/signature_help.py
--rw-r--r--   0        0        0     9340 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/common/parts/window.py
--rw-r--r--   0        0        0    18981 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/common/parts/workspace.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/__init__.py
--rw-r--r--   0        0        0     3973 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/configuration.py
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/languages.py
--rw-r--r--   0        0        0     8569 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/protocol.py
--rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/server.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/diagnostics/__init__.py
--rw-r--r--   0        0        0    38247 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/diagnostics/analyzer.py
--rw-r--r--   0        0        0     7935 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/diagnostics/entities.py
--rw-r--r--   0        0        0    56507 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/diagnostics/imports_manager.py
--rw-r--r--   0        0        0    66971 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/diagnostics/library_doc.py
--rw-r--r--   0        0        0    83614 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/diagnostics/namespace.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/parts/__init__.py
--rw-r--r--   0        0        0    15318 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/parts/code_action_documentation.py
--rw-r--r--   0        0        0     7151 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/parts/code_action_fixes.py
--rw-r--r--   0        0        0     6670 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/parts/codelens.py
--rw-r--r--   0        0        0    85311 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/parts/completion.py
--rw-r--r--   0        0        0     3701 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/parts/debugging_utils.py
--rw-r--r--   0        0        0    16867 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/parts/diagnostics.py
--rw-r--r--   0        0        0     2629 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/parts/document_highlight.py
--rw-r--r--   0        0        0     9872 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/parts/document_symbols.py
--rw-r--r--   0        0        0    19395 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/parts/documents_cache.py
--rw-r--r--   0        0        0     4384 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/parts/folding_range.py
--rw-r--r--   0        0        0     8495 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/parts/formatting.py
--rw-r--r--   0        0        0    26508 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/parts/goto.py
--rw-r--r--   0        0        0    23815 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/parts/hover.py
--rw-r--r--   0        0        0     8872 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/parts/inlay_hint.py
--rw-r--r--   0        0        0     3420 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/parts/inline_value.py
--rw-r--r--   0        0        0    24217 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/parts/model_helper.py
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/parts/protocol_part.py
--rw-r--r--   0        0        0    19638 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/parts/references.py
--rw-r--r--   0        0        0    24952 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/parts/rename.py
--rw-r--r--   0        0        0     6283 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/parts/robocop_diagnostics.py
--rw-r--r--   0        0        0     8493 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/parts/robot_workspace.py
--rw-r--r--   0        0        0     2724 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/parts/selection_range.py
--rw-r--r--   0        0        0    42861 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/parts/semantic_tokens.py
--rw-r--r--   0        0        0    15709 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/parts/signature_help.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/utils/__init__.py
--rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/utils/_variables.py
--rw-r--r--   0        0        0     7957 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/utils/ast_utils.py
--rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/utils/async_ast.py
--rw-r--r--   0        0        0    11653 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/utils/markdownformatter.py
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/utils/match.py
--rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/utils/robot_path.py
--rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/utils/variables.py
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/utils/version.py
--rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/.gitignore
--rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/LICENSE.txt
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/README.md
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/pyproject.toml
--rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.1/src/robotcode/language_server/__init__.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.1/src/robotcode/language_server/__version__.py
+-rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.1/src/robotcode/language_server/cli.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.1/src/robotcode/language_server/hooks.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.1/src/robotcode/language_server/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.1/src/robotcode/language_server/common/__init__.py
+-rw-r--r--   0        0        0     2563 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.1/src/robotcode/language_server/common/decorators.py
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.1/src/robotcode/language_server/common/has_extend_capabilities.py
+-rw-r--r--   0        0        0    11515 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.1/src/robotcode/language_server/common/protocol.py
+-rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.1/src/robotcode/language_server/common/server.py
+-rw-r--r--   0        0        0     9485 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.1/src/robotcode/language_server/common/text_document.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.1/src/robotcode/language_server/common/parts/__init__.py
+-rw-r--r--   0        0        0     4411 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.1/src/robotcode/language_server/common/parts/code_action.py
+-rw-r--r--   0        0        0     4239 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.1/src/robotcode/language_server/common/parts/code_lens.py
+-rw-r--r--   0        0        0     3438 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.1/src/robotcode/language_server/common/parts/commands.py
+-rw-r--r--   0        0        0     6206 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.1/src/robotcode/language_server/common/parts/completion.py
+-rw-r--r--   0        0        0     4648 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.1/src/robotcode/language_server/common/parts/declaration.py
+-rw-r--r--   0        0        0     4650 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.1/src/robotcode/language_server/common/parts/definition.py
+-rw-r--r--   0        0        0    21107 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.1/src/robotcode/language_server/common/parts/diagnostics.py
+-rw-r--r--   0        0        0     2689 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.1/src/robotcode/language_server/common/parts/document_highlight.py
+-rw-r--r--   0        0        0     5937 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.1/src/robotcode/language_server/common/parts/document_symbols.py
+-rw-r--r--   0        0        0    14870 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.1/src/robotcode/language_server/common/parts/documents.py
+-rw-r--r--   0        0        0     2784 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.1/src/robotcode/language_server/common/parts/folding_range.py
+-rw-r--r--   0        0        0     4399 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.1/src/robotcode/language_server/common/parts/formatting.py
+-rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.1/src/robotcode/language_server/common/parts/hover.py
+-rw-r--r--   0        0        0     4651 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.1/src/robotcode/language_server/common/parts/implementation.py
+-rw-r--r--   0        0        0     3858 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.1/src/robotcode/language_server/common/parts/inlay_hint.py
+-rw-r--r--   0        0        0     3657 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.1/src/robotcode/language_server/common/parts/inline_value.py
+-rw-r--r--   0        0        0     2730 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.1/src/robotcode/language_server/common/parts/linked_editing_ranges.py
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.1/src/robotcode/language_server/common/parts/protocol_part.py
+-rw-r--r--   0        0        0     2842 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.1/src/robotcode/language_server/common/parts/references.py
+-rw-r--r--   0        0        0     5780 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.1/src/robotcode/language_server/common/parts/rename.py
+-rw-r--r--   0        0        0     2891 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.1/src/robotcode/language_server/common/parts/selection_range.py
+-rw-r--r--   0        0        0     6963 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.1/src/robotcode/language_server/common/parts/semantic_tokens.py
+-rw-r--r--   0        0        0     3629 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.1/src/robotcode/language_server/common/parts/signature_help.py
+-rw-r--r--   0        0        0     9340 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.1/src/robotcode/language_server/common/parts/window.py
+-rw-r--r--   0        0        0    18981 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.1/src/robotcode/language_server/common/parts/workspace.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.1/src/robotcode/language_server/robotframework/__init__.py
+-rw-r--r--   0        0        0     3973 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.1/src/robotcode/language_server/robotframework/configuration.py
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.1/src/robotcode/language_server/robotframework/languages.py
+-rw-r--r--   0        0        0     8569 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.1/src/robotcode/language_server/robotframework/protocol.py
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.1/src/robotcode/language_server/robotframework/server.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.1/src/robotcode/language_server/robotframework/diagnostics/__init__.py
+-rw-r--r--   0        0        0    38247 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.1/src/robotcode/language_server/robotframework/diagnostics/analyzer.py
+-rw-r--r--   0        0        0     7935 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.1/src/robotcode/language_server/robotframework/diagnostics/entities.py
+-rw-r--r--   0        0        0    58384 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.1/src/robotcode/language_server/robotframework/diagnostics/imports_manager.py
+-rw-r--r--   0        0        0    67010 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.1/src/robotcode/language_server/robotframework/diagnostics/library_doc.py
+-rw-r--r--   0        0        0    83614 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.1/src/robotcode/language_server/robotframework/diagnostics/namespace.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.1/src/robotcode/language_server/robotframework/parts/__init__.py
+-rw-r--r--   0        0        0    15318 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.1/src/robotcode/language_server/robotframework/parts/code_action_documentation.py
+-rw-r--r--   0        0        0     7151 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.1/src/robotcode/language_server/robotframework/parts/code_action_fixes.py
+-rw-r--r--   0        0        0     6670 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.1/src/robotcode/language_server/robotframework/parts/codelens.py
+-rw-r--r--   0        0        0    85311 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.1/src/robotcode/language_server/robotframework/parts/completion.py
+-rw-r--r--   0        0        0     3701 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.1/src/robotcode/language_server/robotframework/parts/debugging_utils.py
+-rw-r--r--   0        0        0    16867 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.1/src/robotcode/language_server/robotframework/parts/diagnostics.py
+-rw-r--r--   0        0        0     2629 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.1/src/robotcode/language_server/robotframework/parts/document_highlight.py
+-rw-r--r--   0        0        0     9872 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.1/src/robotcode/language_server/robotframework/parts/document_symbols.py
+-rw-r--r--   0        0        0    19395 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.1/src/robotcode/language_server/robotframework/parts/documents_cache.py
+-rw-r--r--   0        0        0     4384 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.1/src/robotcode/language_server/robotframework/parts/folding_range.py
+-rw-r--r--   0        0        0     8495 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.1/src/robotcode/language_server/robotframework/parts/formatting.py
+-rw-r--r--   0        0        0    26508 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.1/src/robotcode/language_server/robotframework/parts/goto.py
+-rw-r--r--   0        0        0    23815 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.1/src/robotcode/language_server/robotframework/parts/hover.py
+-rw-r--r--   0        0        0     8872 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.1/src/robotcode/language_server/robotframework/parts/inlay_hint.py
+-rw-r--r--   0        0        0     3420 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.1/src/robotcode/language_server/robotframework/parts/inline_value.py
+-rw-r--r--   0        0        0    24217 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.1/src/robotcode/language_server/robotframework/parts/model_helper.py
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.1/src/robotcode/language_server/robotframework/parts/protocol_part.py
+-rw-r--r--   0        0        0    19638 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.1/src/robotcode/language_server/robotframework/parts/references.py
+-rw-r--r--   0        0        0    24952 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.1/src/robotcode/language_server/robotframework/parts/rename.py
+-rw-r--r--   0        0        0     6283 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.1/src/robotcode/language_server/robotframework/parts/robocop_diagnostics.py
+-rw-r--r--   0        0        0     8493 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.1/src/robotcode/language_server/robotframework/parts/robot_workspace.py
+-rw-r--r--   0        0        0     2724 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.1/src/robotcode/language_server/robotframework/parts/selection_range.py
+-rw-r--r--   0        0        0    42861 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.1/src/robotcode/language_server/robotframework/parts/semantic_tokens.py
+-rw-r--r--   0        0        0    15709 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.1/src/robotcode/language_server/robotframework/parts/signature_help.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.1/src/robotcode/language_server/robotframework/utils/__init__.py
+-rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.1/src/robotcode/language_server/robotframework/utils/_variables.py
+-rw-r--r--   0        0        0     7957 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.1/src/robotcode/language_server/robotframework/utils/ast_utils.py
+-rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.1/src/robotcode/language_server/robotframework/utils/async_ast.py
+-rw-r--r--   0        0        0    11653 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.1/src/robotcode/language_server/robotframework/utils/markdownformatter.py
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.1/src/robotcode/language_server/robotframework/utils/match.py
+-rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.1/src/robotcode/language_server/robotframework/utils/robot_path.py
+-rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.1/src/robotcode/language_server/robotframework/utils/variables.py
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.1/src/robotcode/language_server/robotframework/utils/version.py
+-rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.1/.gitignore
+-rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.1/LICENSE.txt
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.1/README.md
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.1/pyproject.toml
+-rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.1/PKG-INFO
```

### Comparing `robotcode_language_server-0.43.0/src/robotcode/language_server/cli.py` & `robotcode_language_server-0.43.1/src/robotcode/language_server/cli.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.0/src/robotcode/language_server/common/decorators.py` & `robotcode_language_server-0.43.1/src/robotcode/language_server/common/decorators.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.0/src/robotcode/language_server/common/protocol.py` & `robotcode_language_server-0.43.1/src/robotcode/language_server/common/protocol.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.0/src/robotcode/language_server/common/server.py` & `robotcode_language_server-0.43.1/src/robotcode/language_server/common/server.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.0/src/robotcode/language_server/common/text_document.py` & `robotcode_language_server-0.43.1/src/robotcode/language_server/common/text_document.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.0/src/robotcode/language_server/common/parts/code_action.py` & `robotcode_language_server-0.43.1/src/robotcode/language_server/common/parts/code_action.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.0/src/robotcode/language_server/common/parts/code_lens.py` & `robotcode_language_server-0.43.1/src/robotcode/language_server/common/parts/code_lens.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.0/src/robotcode/language_server/common/parts/commands.py` & `robotcode_language_server-0.43.1/src/robotcode/language_server/common/parts/commands.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.0/src/robotcode/language_server/common/parts/completion.py` & `robotcode_language_server-0.43.1/src/robotcode/language_server/common/parts/completion.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.0/src/robotcode/language_server/common/parts/declaration.py` & `robotcode_language_server-0.43.1/src/robotcode/language_server/common/parts/declaration.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.0/src/robotcode/language_server/common/parts/definition.py` & `robotcode_language_server-0.43.1/src/robotcode/language_server/common/parts/definition.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.0/src/robotcode/language_server/common/parts/diagnostics.py` & `robotcode_language_server-0.43.1/src/robotcode/language_server/common/parts/diagnostics.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.0/src/robotcode/language_server/common/parts/document_highlight.py` & `robotcode_language_server-0.43.1/src/robotcode/language_server/common/parts/document_highlight.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.0/src/robotcode/language_server/common/parts/document_symbols.py` & `robotcode_language_server-0.43.1/src/robotcode/language_server/common/parts/document_symbols.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.0/src/robotcode/language_server/common/parts/documents.py` & `robotcode_language_server-0.43.1/src/robotcode/language_server/common/parts/documents.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.0/src/robotcode/language_server/common/parts/folding_range.py` & `robotcode_language_server-0.43.1/src/robotcode/language_server/common/parts/folding_range.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.0/src/robotcode/language_server/common/parts/formatting.py` & `robotcode_language_server-0.43.1/src/robotcode/language_server/common/parts/formatting.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.0/src/robotcode/language_server/common/parts/hover.py` & `robotcode_language_server-0.43.1/src/robotcode/language_server/common/parts/hover.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.0/src/robotcode/language_server/common/parts/implementation.py` & `robotcode_language_server-0.43.1/src/robotcode/language_server/common/parts/implementation.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.0/src/robotcode/language_server/common/parts/inlay_hint.py` & `robotcode_language_server-0.43.1/src/robotcode/language_server/common/parts/inlay_hint.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.0/src/robotcode/language_server/common/parts/inline_value.py` & `robotcode_language_server-0.43.1/src/robotcode/language_server/common/parts/inline_value.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.0/src/robotcode/language_server/common/parts/linked_editing_ranges.py` & `robotcode_language_server-0.43.1/src/robotcode/language_server/common/parts/linked_editing_ranges.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.0/src/robotcode/language_server/common/parts/references.py` & `robotcode_language_server-0.43.1/src/robotcode/language_server/common/parts/references.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.0/src/robotcode/language_server/common/parts/rename.py` & `robotcode_language_server-0.43.1/src/robotcode/language_server/common/parts/rename.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.0/src/robotcode/language_server/common/parts/selection_range.py` & `robotcode_language_server-0.43.1/src/robotcode/language_server/common/parts/selection_range.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.0/src/robotcode/language_server/common/parts/semantic_tokens.py` & `robotcode_language_server-0.43.1/src/robotcode/language_server/common/parts/semantic_tokens.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.0/src/robotcode/language_server/common/parts/signature_help.py` & `robotcode_language_server-0.43.1/src/robotcode/language_server/common/parts/signature_help.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.0/src/robotcode/language_server/common/parts/window.py` & `robotcode_language_server-0.43.1/src/robotcode/language_server/common/parts/window.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.0/src/robotcode/language_server/common/parts/workspace.py` & `robotcode_language_server-0.43.1/src/robotcode/language_server/common/parts/workspace.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/configuration.py` & `robotcode_language_server-0.43.1/src/robotcode/language_server/robotframework/configuration.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/protocol.py` & `robotcode_language_server-0.43.1/src/robotcode/language_server/robotframework/protocol.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/server.py` & `robotcode_language_server-0.43.1/src/robotcode/language_server/robotframework/server.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/diagnostics/analyzer.py` & `robotcode_language_server-0.43.1/src/robotcode/language_server/robotframework/diagnostics/analyzer.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/diagnostics/entities.py` & `robotcode_language_server-0.43.1/src/robotcode/language_server/robotframework/diagnostics/entities.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/diagnostics/imports_manager.py` & `robotcode_language_server-0.43.1/src/robotcode/language_server/robotframework/diagnostics/imports_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -581,38 +581,61 @@
                     for k, v in (self.parent_protocol.profile.variables or {}).items()
                 ]
 
                 for variable_file in self.parent_protocol.profile.variable_files or []:
                     name, args = split_args_from_name_or_path(str(variable_file))
                     try:
                         lib_doc = await self.get_libdoc_for_variables_import(
-                            name, tuple(args), str(self.folder.to_path()), self, resolve_command_line_vars=False
+                            name,
+                            tuple(args),
+                            str(self.folder.to_path()),
+                            self,
+                            resolve_variables=False,
+                            resolve_command_line_vars=False,
                         )
                         if lib_doc is not None:
                             command_line_vars += lib_doc.variables
 
+                            if lib_doc.errors:
+                                # TODO add diagnostics
+                                for error in lib_doc.errors:
+                                    self._logger.error(
+                                        lambda: f"{error.type_name}: {error.message} in {error.source}:{error.line_no}"
+                                    )
                     except (SystemExit, KeyboardInterrupt, asyncio.CancelledError):
                         raise
                     except BaseException as e:
                         # TODO add diagnostics
                         self._logger.exception(e)
 
                 command_line_vars += [
                     CommandLineVariableDefinition(0, 0, 0, 0, "", f"${{{k}}}", None, has_value=True, value=v)
                     for k, v in self.config.robot.variables.items()
                 ]
                 for variable_file in self.config.robot.variable_files:
                     name, args = split_args_from_name_or_path(variable_file)
                     try:
                         lib_doc = await self.get_libdoc_for_variables_import(
-                            name, tuple(args), str(self.folder.to_path()), self, resolve_command_line_vars=False
+                            name,
+                            tuple(args),
+                            str(self.folder.to_path()),
+                            self,
+                            resolve_variables=False,
+                            resolve_command_line_vars=False,
                         )
                         if lib_doc is not None:
                             command_line_vars += lib_doc.variables
 
+                            if lib_doc.errors:
+                                # TODO add diagnostics
+                                for error in lib_doc.errors:
+                                    self._logger.error(
+                                        lambda: f"{error.type_name}: {error.message} in {error.source}:{error.line_no}"
+                                    )
+
                     except (SystemExit, KeyboardInterrupt, asyncio.CancelledError):
                         raise
                     except BaseException as e:
                         # TODO add diagnostics
                         self._logger.exception(e)
 
                 self._command_line_variables = command_line_vars
@@ -874,20 +897,24 @@
         return None, import_name
 
     async def get_variables_meta(
         self,
         name: str,
         base_dir: str = ".",
         variables: Optional[Dict[str, Optional[Any]]] = None,
+        resolve_variables: bool = True,
+        resolve_command_line_vars: bool = True,
     ) -> Tuple[Optional[LibraryMetaData], str]:
         try:
             import_name = await self.find_variables(
                 name,
                 base_dir=base_dir,
                 variables=variables,
+                resolve_variables=resolve_variables,
+                resolve_command_line_vars=resolve_command_line_vars,
             )
 
             result: Optional[LibraryMetaData] = None
             module_spec: Optional[ModuleSpec] = None
             if is_variables_by_path(import_name):
                 if (p := Path(import_name)).exists():
                     result = LibraryMetaData(__version__, p.stem, import_name, None, True)
@@ -931,15 +958,15 @@
 
             return result, import_name
         except (SystemExit, KeyboardInterrupt):
             raise
         except BaseException:
             pass
 
-        return None, import_name
+        return None, name
 
     async def find_library(self, name: str, base_dir: str, variables: Optional[Dict[str, Any]] = None) -> str:
         return await self._library_files_cache.get(self._find_library, name, base_dir, variables)
 
     async def _find_library(self, name: str, base_dir: str, variables: Optional[Dict[str, Any]] = None) -> str:
         from robot.libraries import STDLIBS
         from robot.variables.search import contains_variable
@@ -982,27 +1009,43 @@
                 await self.get_resolvable_command_line_variables(),
                 variables,
                 file_type,
             )
 
         return str(find_file_ex(name, base_dir, file_type))
 
-    async def find_variables(self, name: str, base_dir: str, variables: Optional[Dict[str, Any]] = None) -> str:
-        return await self._variables_files_cache.get(self.__find_variables, name, base_dir, variables)
+    async def find_variables(
+        self,
+        name: str,
+        base_dir: str,
+        variables: Optional[Dict[str, Any]] = None,
+        resolve_variables: bool = True,
+        resolve_command_line_vars: bool = True,
+    ) -> str:
+        return await self._variables_files_cache.get(
+            self.__find_variables, name, base_dir, variables, resolve_command_line_vars
+        )
 
     @_logger.call
-    async def __find_variables(self, name: str, base_dir: str, variables: Optional[Dict[str, Any]] = None) -> str:
+    async def __find_variables(
+        self,
+        name: str,
+        base_dir: str,
+        variables: Optional[Dict[str, Any]] = None,
+        resolve_variables: bool = True,
+        resolve_command_line_vars: bool = True,
+    ) -> str:
         from robot.variables.search import contains_variable
 
-        if contains_variable(name, "$@&%"):
+        if resolve_variables and contains_variable(name, "$@&%"):
             return find_variables(
                 name,
                 str(self.folder.to_path()),
                 base_dir,
-                await self.get_resolvable_command_line_variables(),
+                await self.get_resolvable_command_line_variables() if resolve_command_line_vars else None,
                 variables,
             )
 
         if get_robot_version() >= (5, 0):
             if is_variables_by_path(name):
                 return str(find_file_ex(name, base_dir, "Variables"))
 
@@ -1254,27 +1297,31 @@
     async def get_libdoc_for_variables_import(
         self,
         name: str,
         args: Tuple[Any, ...],
         base_dir: str,
         sentinel: Any = None,
         variables: Optional[Dict[str, Any]] = None,
+        resolve_variables: bool = True,
         resolve_command_line_vars: bool = True,
     ) -> VariablesDoc:
         source = await self.find_variables(
             name,
             base_dir,
             variables,
+            resolve_variables=resolve_variables,
+            resolve_command_line_vars=resolve_command_line_vars,
         )
 
         async def _get_libdoc(name: str, args: Tuple[Any, ...], working_dir: str, base_dir: str) -> VariablesDoc:
             meta, source = await self.get_variables_meta(
                 name,
                 base_dir,
                 variables,
+                resolve_command_line_vars=resolve_command_line_vars,
             )
 
             self._logger.debug(lambda: f"Load variables {source}{args!r}")
             if meta is not None:
                 meta_file = Path(self.variables_doc_cache_path, meta.filepath_base.with_suffix(".meta.json"))
                 if meta_file.exists():
                     try:
```

### Comparing `robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/diagnostics/library_doc.py` & `robotcode_language_server-0.43.1/src/robotcode/language_server/robotframework/diagnostics/library_doc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1542,15 +1542,16 @@
         with _std_capture() as std_capturer:
             import_name = find_variables(name, working_dir, base_dir, command_line_variables, variables)
             get_variables = None
 
             if import_name.lower().endswith((".yaml", ".yml")):
                 source = import_name
                 importer = YamlImporter()
-            if get_robot_version() >= (6, 1) and import_name.lower().endswith(".json"):
+            elif get_robot_version() >= (6, 1) and import_name.lower().endswith(".json"):
+                source = import_name
                 importer = JsonImporter()
             else:
                 if not is_variables_by_path(import_name):
                     module_spec = get_module_spec(import_name)
 
                 # skip antigravity easter egg
                 # see https://python-history.blogspot.com/2010/06/import-antigravity.html
```

### Comparing `robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/diagnostics/namespace.py` & `robotcode_language_server-0.43.1/src/robotcode/language_server/robotframework/diagnostics/namespace.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/parts/code_action_documentation.py` & `robotcode_language_server-0.43.1/src/robotcode/language_server/robotframework/parts/code_action_documentation.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/parts/code_action_fixes.py` & `robotcode_language_server-0.43.1/src/robotcode/language_server/robotframework/parts/code_action_fixes.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/parts/codelens.py` & `robotcode_language_server-0.43.1/src/robotcode/language_server/robotframework/parts/codelens.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/parts/completion.py` & `robotcode_language_server-0.43.1/src/robotcode/language_server/robotframework/parts/completion.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/parts/debugging_utils.py` & `robotcode_language_server-0.43.1/src/robotcode/language_server/robotframework/parts/debugging_utils.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/parts/diagnostics.py` & `robotcode_language_server-0.43.1/src/robotcode/language_server/robotframework/parts/diagnostics.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/parts/document_highlight.py` & `robotcode_language_server-0.43.1/src/robotcode/language_server/robotframework/parts/document_highlight.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/parts/document_symbols.py` & `robotcode_language_server-0.43.1/src/robotcode/language_server/robotframework/parts/document_symbols.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/parts/documents_cache.py` & `robotcode_language_server-0.43.1/src/robotcode/language_server/robotframework/parts/documents_cache.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/parts/folding_range.py` & `robotcode_language_server-0.43.1/src/robotcode/language_server/robotframework/parts/folding_range.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/parts/formatting.py` & `robotcode_language_server-0.43.1/src/robotcode/language_server/robotframework/parts/formatting.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/parts/goto.py` & `robotcode_language_server-0.43.1/src/robotcode/language_server/robotframework/parts/goto.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/parts/hover.py` & `robotcode_language_server-0.43.1/src/robotcode/language_server/robotframework/parts/hover.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/parts/inlay_hint.py` & `robotcode_language_server-0.43.1/src/robotcode/language_server/robotframework/parts/inlay_hint.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/parts/inline_value.py` & `robotcode_language_server-0.43.1/src/robotcode/language_server/robotframework/parts/inline_value.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/parts/model_helper.py` & `robotcode_language_server-0.43.1/src/robotcode/language_server/robotframework/parts/model_helper.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/parts/references.py` & `robotcode_language_server-0.43.1/src/robotcode/language_server/robotframework/parts/references.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/parts/rename.py` & `robotcode_language_server-0.43.1/src/robotcode/language_server/robotframework/parts/rename.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/parts/robocop_diagnostics.py` & `robotcode_language_server-0.43.1/src/robotcode/language_server/robotframework/parts/robocop_diagnostics.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/parts/robot_workspace.py` & `robotcode_language_server-0.43.1/src/robotcode/language_server/robotframework/parts/robot_workspace.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/parts/selection_range.py` & `robotcode_language_server-0.43.1/src/robotcode/language_server/robotframework/parts/selection_range.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/parts/semantic_tokens.py` & `robotcode_language_server-0.43.1/src/robotcode/language_server/robotframework/parts/semantic_tokens.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/parts/signature_help.py` & `robotcode_language_server-0.43.1/src/robotcode/language_server/robotframework/parts/signature_help.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/utils/_variables.py` & `robotcode_language_server-0.43.1/src/robotcode/language_server/robotframework/utils/_variables.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/utils/ast_utils.py` & `robotcode_language_server-0.43.1/src/robotcode/language_server/robotframework/utils/ast_utils.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/utils/async_ast.py` & `robotcode_language_server-0.43.1/src/robotcode/language_server/robotframework/utils/async_ast.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/utils/markdownformatter.py` & `robotcode_language_server-0.43.1/src/robotcode/language_server/robotframework/utils/markdownformatter.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/utils/robot_path.py` & `robotcode_language_server-0.43.1/src/robotcode/language_server/robotframework/utils/robot_path.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/utils/variables.py` & `robotcode_language_server-0.43.1/src/robotcode/language_server/robotframework/utils/variables.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.0/.gitignore` & `robotcode_language_server-0.43.1/.gitignore`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.0/LICENSE.txt` & `robotcode_language_server-0.43.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.0/README.md` & `robotcode_language_server-0.43.1/README.md`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.43.0/pyproject.toml` & `robotcode_language_server-0.43.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -23,16 +23,16 @@
   "Topic :: Utilities",
   "Typing :: Typed",
   "Framework :: Robot Framework",
   "Framework :: Robot Framework :: Tool",
 ]
 dependencies = [
   "robotframework>=4.1.0",
-  "robotcode-jsonrpc2==0.43.0",
-  "robotcode==0.43.0",
+  "robotcode-jsonrpc2==0.43.1",
+  "robotcode==0.43.1",
 ]
 dynamic = ["version"]
 
 [project.entry-points.robotcode]
 langserver = "robotcode.language_server.hooks"
 
 [project.urls]
```

### Comparing `robotcode_language_server-0.43.0/PKG-INFO` & `robotcode_language_server-0.43.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotcode-language-server
-Version: 0.43.0
+Version: 0.43.1
 Summary: RobotCode Language Server for Robot Framework
 Project-URL: Homepage, https://robotcode.io
 Project-URL: Donate, https://github.com/sponsors/d-biehl
 Project-URL: Documentation, https://github.com/d-biehl/robotcode#readme
 Project-URL: Changelog, https://github.com/d-biehl/robotcode/blob/main/CHANGELOG.md
 Project-URL: Issues, https://github.com/d-biehl/robotcode/issues
 Project-URL: Source, https://github.com/d-biehl/robotcode
@@ -21,16 +21,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
-Requires-Dist: robotcode-jsonrpc2==0.43.0
-Requires-Dist: robotcode==0.43.0
+Requires-Dist: robotcode-jsonrpc2==0.43.1
+Requires-Dist: robotcode==0.43.1
 Requires-Dist: robotframework>=4.1.0
 Description-Content-Type: text/markdown
 
 # robotcode-language-server
 
 [![PyPI - Version](https://img.shields.io/pypi/v/robotcode-language-server.svg)](https://pypi.org/project/robotcode-language-server)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/robotcode-language-server.svg)](https://pypi.org/project/robotcode-language-server)
```

