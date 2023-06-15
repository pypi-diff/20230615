# Comparing `tmp/robotframework-robocop-3.1.1.tar.gz` & `tmp/robotframework-robocop-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework-robocop-3.1.1.tar", last modified: Thu Apr 20 10:35:01 2023, max compression
+gzip compressed data, was "robotframework-robocop-3.2.0.tar", last modified: Thu Jun 15 15:41:07 2023, max compression
```

## Comparing `robotframework-robocop-3.1.1.tar` & `robotframework-robocop-3.2.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:35:01.849020 robotframework-robocop-3.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-20 10:34:42.000000 robotframework-robocop-3.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-20 10:34:42.000000 robotframework-robocop-3.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    14103 2023-04-20 10:35:01.849020 robotframework-robocop-3.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12529 2023-04-20 10:34:42.000000 robotframework-robocop-3.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-04-20 10:34:42.000000 robotframework-robocop-3.1.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:35:01.845019 robotframework-robocop-3.1.1/robocop/
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-20 10:34:42.000000 robotframework-robocop-3.1.1/robocop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 10:34:42.000000 robotframework-robocop-3.1.1/robocop/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:35:01.845019 robotframework-robocop-3.1.1/robocop/checkers/
--rw-r--r--   0 runner    (1001) docker     (123)     5897 2023-04-20 10:34:42.000000 robotframework-robocop-3.1.1/robocop/checkers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9388 2023-04-20 10:34:42.000000 robotframework-robocop-3.1.1/robocop/checkers/comments.py
--rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-04-20 10:34:42.000000 robotframework-robocop-3.1.1/robocop/checkers/documentation.py
--rw-r--r--   0 runner    (1001) docker     (123)    17331 2023-04-20 10:34:42.000000 robotframework-robocop-3.1.1/robocop/checkers/duplications.py
--rw-r--r--   0 runner    (1001) docker     (123)    21919 2023-04-20 10:34:42.000000 robotframework-robocop-3.1.1/robocop/checkers/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    27365 2023-04-20 10:34:42.000000 robotframework-robocop-3.1.1/robocop/checkers/lengths.py
--rw-r--r--   0 runner    (1001) docker     (123)    26679 2023-04-20 10:34:42.000000 robotframework-robocop-3.1.1/robocop/checkers/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    32141 2023-04-20 10:34:42.000000 robotframework-robocop-3.1.1/robocop/checkers/naming.py
--rw-r--r--   0 runner    (1001) docker     (123)    33520 2023-04-20 10:34:42.000000 robotframework-robocop-3.1.1/robocop/checkers/spacing.py
--rw-r--r--   0 runner    (1001) docker     (123)    11490 2023-04-20 10:34:42.000000 robotframework-robocop-3.1.1/robocop/checkers/tags.py
--rw-r--r--   0 runner    (1001) docker     (123)    23822 2023-04-20 10:34:42.000000 robotframework-robocop-3.1.1/robocop/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-04-20 10:34:42.000000 robotframework-robocop-3.1.1/robocop/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-04-20 10:34:42.000000 robotframework-robocop-3.1.1/robocop/files.py
--rw-r--r--   0 runner    (1001) docker     (123)    17544 2023-04-20 10:34:42.000000 robotframework-robocop-3.1.1/robocop/reports.py
--rw-r--r--   0 runner    (1001) docker     (123)    14683 2023-04-20 10:34:42.000000 robotframework-robocop-3.1.1/robocop/rules.py
--rw-r--r--   0 runner    (1001) docker     (123)    11038 2023-04-20 10:34:42.000000 robotframework-robocop-3.1.1/robocop/run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:35:01.845019 robotframework-robocop-3.1.1/robocop/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-04-20 10:34:42.000000 robotframework-robocop-3.1.1/robocop/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5086 2023-04-20 10:34:42.000000 robotframework-robocop-3.1.1/robocop/utils/disablers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-04-20 10:34:42.000000 robotframework-robocop-3.1.1/robocop/utils/file_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    11733 2023-04-20 10:34:42.000000 robotframework-robocop-3.1.1/robocop/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-04-20 10:34:42.000000 robotframework-robocop-3.1.1/robocop/utils/run_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)    13535 2023-04-20 10:34:42.000000 robotframework-robocop-3.1.1/robocop/utils/version_matching.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-20 10:34:42.000000 robotframework-robocop-3.1.1/robocop/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:35:01.845019 robotframework-robocop-3.1.1/robotframework_robocop.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14103 2023-04-20 10:35:01.000000 robotframework-robocop-3.1.1/robotframework_robocop.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-04-20 10:35:01.000000 robotframework-robocop-3.1.1/robotframework_robocop.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 10:35:01.000000 robotframework-robocop-3.1.1/robotframework_robocop.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-20 10:35:01.000000 robotframework-robocop-3.1.1/robotframework_robocop.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-20 10:35:01.000000 robotframework-robocop-3.1.1/robotframework_robocop.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-20 10:35:01.000000 robotframework-robocop-3.1.1/robotframework_robocop.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 10:35:01.849020 robotframework-robocop-3.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-04-20 10:34:42.000000 robotframework-robocop-3.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:41:07.664914 robotframework-robocop-3.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-15 15:40:54.000000 robotframework-robocop-3.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-15 15:40:54.000000 robotframework-robocop-3.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    14103 2023-06-15 15:41:07.664914 robotframework-robocop-3.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12529 2023-06-15 15:40:54.000000 robotframework-robocop-3.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-15 15:40:54.000000 robotframework-robocop-3.2.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:41:07.664914 robotframework-robocop-3.2.0/robocop/
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-15 15:40:54.000000 robotframework-robocop-3.2.0/robocop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 15:40:54.000000 robotframework-robocop-3.2.0/robocop/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:41:07.664914 robotframework-robocop-3.2.0/robocop/checkers/
+-rw-r--r--   0 runner    (1001) docker     (123)     5897 2023-06-15 15:40:54.000000 robotframework-robocop-3.2.0/robocop/checkers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9388 2023-06-15 15:40:54.000000 robotframework-robocop-3.2.0/robocop/checkers/comments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-06-15 15:40:54.000000 robotframework-robocop-3.2.0/robocop/checkers/documentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17339 2023-06-15 15:40:54.000000 robotframework-robocop-3.2.0/robocop/checkers/duplications.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22768 2023-06-15 15:40:54.000000 robotframework-robocop-3.2.0/robocop/checkers/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27361 2023-06-15 15:40:54.000000 robotframework-robocop-3.2.0/robocop/checkers/lengths.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40684 2023-06-15 15:40:54.000000 robotframework-robocop-3.2.0/robocop/checkers/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44284 2023-06-15 15:40:54.000000 robotframework-robocop-3.2.0/robocop/checkers/naming.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33602 2023-06-15 15:40:54.000000 robotframework-robocop-3.2.0/robocop/checkers/spacing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11490 2023-06-15 15:40:54.000000 robotframework-robocop-3.2.0/robocop/checkers/tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24721 2023-06-15 15:40:54.000000 robotframework-robocop-3.2.0/robocop/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-06-15 15:40:54.000000 robotframework-robocop-3.2.0/robocop/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-06-15 15:40:54.000000 robotframework-robocop-3.2.0/robocop/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18783 2023-06-15 15:40:54.000000 robotframework-robocop-3.2.0/robocop/reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14683 2023-06-15 15:40:54.000000 robotframework-robocop-3.2.0/robocop/rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11064 2023-06-15 15:40:54.000000 robotframework-robocop-3.2.0/robocop/run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:41:07.664914 robotframework-robocop-3.2.0/robocop/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-15 15:40:54.000000 robotframework-robocop-3.2.0/robocop/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5086 2023-06-15 15:40:54.000000 robotframework-robocop-3.2.0/robocop/utils/disablers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-06-15 15:40:54.000000 robotframework-robocop-3.2.0/robocop/utils/file_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12577 2023-06-15 15:40:54.000000 robotframework-robocop-3.2.0/robocop/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-06-15 15:40:54.000000 robotframework-robocop-3.2.0/robocop/utils/run_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13535 2023-06-15 15:40:54.000000 robotframework-robocop-3.2.0/robocop/utils/version_matching.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-15 15:40:54.000000 robotframework-robocop-3.2.0/robocop/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:41:07.664914 robotframework-robocop-3.2.0/robotframework_robocop.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14103 2023-06-15 15:41:07.000000 robotframework-robocop-3.2.0/robotframework_robocop.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-15 15:41:07.000000 robotframework-robocop-3.2.0/robotframework_robocop.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 15:41:07.000000 robotframework-robocop-3.2.0/robotframework_robocop.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-15 15:41:07.000000 robotframework-robocop-3.2.0/robotframework_robocop.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-15 15:41:07.000000 robotframework-robocop-3.2.0/robotframework_robocop.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-15 15:41:07.000000 robotframework-robocop-3.2.0/robotframework_robocop.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 15:41:07.664914 robotframework-robocop-3.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-06-15 15:40:54.000000 robotframework-robocop-3.2.0/setup.py
```

### Comparing `robotframework-robocop-3.1.1/LICENSE` & `robotframework-robocop-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-3.1.1/PKG-INFO` & `robotframework-robocop-3.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-robocop
-Version: 3.1.1
+Version: 3.2.0
 Summary: Static code analysis tool (linter) for Robot Framework
 Home-page: https://github.com/MarketSquare/robotframework-robocop
 Download-URL: https://pypi.org/project/robotframework-robocop
 Author: Bartlomiej Hirsz, Mateusz Nojek
 Author-email: bartek.hirsz@gmail.com, matnojek@gmail.com
 License: Apache License 2.0
 Project-URL: Documentation, https://robocop.readthedocs.io/en/stable
```

### Comparing `robotframework-robocop-3.1.1/README.md` & `robotframework-robocop-3.2.0/README.md`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-3.1.1/robocop/checkers/__init__.py` & `robotframework-robocop-3.2.0/robocop/checkers/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-3.1.1/robocop/checkers/comments.py` & `robotframework-robocop-3.2.0/robocop/checkers/comments.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-3.1.1/robocop/checkers/documentation.py` & `robotframework-robocop-3.2.0/robocop/checkers/documentation.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-3.1.1/robocop/checkers/duplications.py` & `robotframework-robocop-3.2.0/robocop/checkers/duplications.py`

 * *Files 0% similar despite different names*

```diff
@@ -368,16 +368,16 @@
     def visit_Metadata(self, node):  # noqa
         if node.name is not None:
             self.metadata[node.name + node.value].append(node)
 
     def visit_VariablesImport(self, node):  # noqa
         if not node.name:
             return
-        # only python files can have arguments - covered in E0404 variables-import-with-args
-        if not node.name.endswith(".py") and node.get_token(Token.ARGUMENT):
+        # only YAML files can't have arguments - covered in E0404 variables-import-with-args
+        if node.name.endswith((".yaml", ".yml")) and node.get_token(Token.ARGUMENT):
             return
         name_with_args = node.name + "".join(token.value for token in node.data_tokens[2:])
         self.variable_imports[name_with_args].append(node)
 
     def visit_Arguments(self, node):  # noqa
         args = set()
         for arg in node.get_tokens(Token.ARGUMENT):
```

### Comparing `robotframework-robocop-3.1.1/robocop/checkers/errors.py` & `robotframework-robocop-3.2.0/robocop/checkers/errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,22 +56,23 @@
                 ${one}      ${two}
 
         """,
     ),
     "0404": Rule(
         rule_id="0404",
         name="variables-import-with-args",
-        msg="Robot and YAML variable files do not take arguments",
+        msg="YAML variable files do not take arguments",
         severity=RuleSeverity.ERROR,
         docs="""
         Example of rule violation::
         
             *** Settings ***
-            Variables    vars.yaml    arg1
-            Variables    variables.robot    arg
+            Variables    vars.yaml        arg1
+            Variables    variables.yml    arg2
+            Variables    module           arg3  # valid from RF > 5
         
         """,
     ),
     "0405": Rule(
         rule_id="0405",
         name="invalid-continuation-mark",
         msg="Invalid continuation mark '{{ mark }}'. It should be '...'",
@@ -277,15 +278,21 @@
         "testtimeout": "Test Timeout",
         "forcetags": "Force Tags",
         "defaulttags": "Default Tags",
         "library": "Library",
         "resource": "Resource",
         "variables": "Variables",
     }
-    ignore_errors = ("can only be used inside a loop",)
+    ignore_errors = (
+        "can only be used inside a loop",
+        "is allowed only once. Only the first value is used",
+        "Test name cannot be empty",  # handled by test-case-name-is-empty
+        "User keyword name cannot be empty",  # handled by keyword-name-is-empty
+        "END is not allowed in this context",  # handled by statement-outside-loop
+    )
 
     def __init__(self):
         super().__init__()
         self.in_block = None
 
     def visit_File(self, node):
         self.generic_visit(node)
@@ -302,14 +309,25 @@
             col = node.data_tokens[0].col_offset + 1
             self.report("not-enough-whitespace-after-newline-marker", node=node, col=col, end_col=col + 3)
         self.generic_visit(node)
 
     def visit_Statement(self, node):  # noqa
         self.parse_errors(node)
 
+    def visit_InvalidSection(self, node):  # noqa
+        invalid_header = node.header.get_token(Token.INVALID_HEADER)
+        if "Resource file with" in invalid_header.error:
+            section_name = invalid_header.value
+            self.report(
+                "invalid-section-in-resource",
+                section_name=section_name,
+                node=node,
+                end_col=node.col_offset + len(section_name) + 1,
+            )
+
     def parse_errors(self, node):  # noqa
         if node is None:
             return
         if ROBOT_VERSION.major != 3:
             for index, error in enumerate(node.errors):
                 self.handle_error(node, error, error_index=index)
         else:
@@ -324,25 +342,23 @@
             self.handle_invalid_syntax(node, error)
         elif "is not allowed with" in error:
             self.handle_not_allowed_setting(node, error)
         elif "Non-existing setting" in error:
             self.handle_invalid_setting(node, error)
         elif "Invalid variable name" in error:
             self.handle_invalid_variable(node, error)
-        elif "RETURN can only be used inside" in error:
+        elif "RETURN can only be used inside" in error or "RETURN is not allowed in this context" in error:
             token = node.data_tokens[0]
             self.report("return-in-test-case", node=node, col=token.col_offset + 1, end_col=token.end_col_offset)
         elif "IF" in error or ("ELSE" in error and If and isinstance(self.in_block, If)):
             self.handle_invalid_block(node, error, "invalid-if")
         elif "FOR loop" in error:
             self.handle_invalid_block(node, error, "invalid-for-loop")
         elif "Non-default argument after default arguments" in error or "Only last argument can be kwargs" in error:
             self.handle_positional_after_named(node, error_index)
-        elif "is allowed only once. Only the first value is used" in error:
-            return
         elif "Resource file with" in error:
             self.handle_invalid_section_in_resource(node, error)
         else:
             error = error.replace("\n   ", "")
             token = node.header if hasattr(node, "header") else node
             end_col = token.col_offset + len(node.name) + 1 if hasattr(node, "name") else token.end_col_offset + 1
             # TODO: 'col' location here can be specified more precisely
@@ -578,28 +594,31 @@
 
 
 class MissingKeywordName(VisitorChecker):
     """Checker for missing keyword name."""
 
     reports = ("missing-keyword-name",)
 
+    def visit_File(self, node):
+        self.generic_visit(node)
+
     def visit_EmptyLine(self, node):  # noqa
         if ROBOT_VERSION.major < 5:
             return
         assign_token = node.get_token(Token.ASSIGN)
         if assign_token:
             self.report(
                 "missing-keyword-name",
                 node=node,
                 lineno=node.lineno,
                 col=assign_token.col_offset + 1,
             )
 
     def visit_KeywordCall(self, node):  # noqa
-        if node.keyword is None:
+        if not node.keyword:
             self.report(
                 "missing-keyword-name",
                 node=node,
                 lineno=node.lineno,
                 col=node.data_tokens[0].col_offset + 1,
                 end_col=node.data_tokens[0].end_col_offset + 1,
             )
@@ -607,9 +626,9 @@
 
 class VariablesImportErrorChecker(VisitorChecker):
     """Checker for syntax error in variables import."""
 
     reports = ("variables-import-with-args",)
 
     def visit_VariablesImport(self, node):  # noqa
-        if node.name and not node.name.endswith(".py") and node.get_token(Token.ARGUMENT):
+        if node.name and node.name.endswith((".yaml", ".yml")) and node.get_token(Token.ARGUMENT):
             self.report("variables-import-with-args", node=node)
```

### Comparing `robotframework-robocop-3.1.1/robocop/checkers/lengths.py` & `robotframework-robocop-3.2.0/robocop/checkers/lengths.py`

 * *Files 0% similar despite different names*

```diff
@@ -565,15 +565,15 @@
         if node.name:
             self.parent_node_name = f"'{node.name}' Keyword"
         else:
             self.parent_node_name = ""
         self.generic_visit(node)
 
     def visit_Metadata(self, node):  # noqa
-        if node.name is None:
+        if not node.name:
             self.report("empty-metadata", node=node, col=node.col_offset + 1)
 
     def visit_Documentation(self, node):  # noqa
         if not node.value:
             self.report(
                 "empty-documentation",
                 block_name=self.parent_node_name,
```

### Comparing `robotframework-robocop-3.1.1/robocop/checkers/misc.py` & `robotframework-robocop-3.2.0/robocop/checkers/misc.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 """
 Miscellaneous checkers
 """
+from collections import namedtuple
 from pathlib import Path
 
 from robot.api import Token
+from robot.errors import VariableError
 from robot.parsing.model.blocks import TestCaseSection
-from robot.parsing.model.statements import KeywordCall, Return, Teardown
+from robot.parsing.model.statements import Arguments, KeywordCall, Return, Teardown
+from robot.utils import unescape
+from robot.variables import VariableIterator
+from robot.variables.search import search_variable
 
 try:
     from robot.api.parsing import Comment, EmptyLine, If, Variable
 except ImportError:
     from robot.parsing.model.statements import Comment, EmptyLine, Variable
 try:
     from robot.api.parsing import Break, Continue, InlineIfHeader, ReturnStatement
@@ -21,17 +26,19 @@
 from robocop.rules import Rule, RuleParam, RuleSeverity, SeverityThreshold
 from robocop.utils import (
     ROBOT_VERSION,
     AssignmentTypeDetector,
     get_errors,
     keyword_col,
     normalize_robot_name,
+    normalize_robot_var_name,
     parse_assignment_sign_type,
     token_col,
 )
+from robocop.utils.misc import find_escaped_variables
 
 rules = {
     "0901": Rule(
         rule_id="0901",
         name="keyword-after-return",
         msg="{{ error_msg }}",
         severity=RuleSeverity.WARNING,
@@ -295,25 +302,26 @@
         severity=RuleSeverity.WARNING,
         version=">=5.0",
         docs="""
         Detect the unreachable code after RETURN, BREAK or CONTINUE statements.
 
         For example::
 
-        Example Keyword
-            FOR    ${animal}    IN    cat    dog
-                IF    '${animal}' == 'cat'
-                    CONTINUE
-                    Log  ${animal}  # unreachable log
+            Example Keyword
+                FOR    ${animal}    IN    cat    dog
+                    IF    '${animal}' == 'cat'
+                        CONTINUE
+                        Log  ${animal}  # unreachable log
+                    END
+                    BREAK
+                    Log    Unreachable log
                 END
-                BREAK
+                RETURN
                 Log    Unreachable log
-            END
-            RETURN
-            Log    Unreachable log
+
         """,
     ),
     "0918": Rule(
         rule_id="0918",
         name="multiline-inline-if",
         msg="Avoid splitting inline IF to multiple lines",
         severity=RuleSeverity.WARNING,
@@ -326,23 +334,110 @@
 
             IF  ${condition}  Log  hello
             ...    ELSE       Log  hi!
 
         Good::
 
             IF  ${condition}    Log  hello     ELSE    Log  hi!
+
         or::
 
             IF  ${condition}
                 Log  hello
             ELSE
                 Log  hi!
             END
         """,
     ),
+    "0919": Rule(
+        rule_id="0919",
+        name="unused-argument",
+        msg="Keyword argument '{{ name }}' is not used",
+        severity=RuleSeverity.WARNING,
+        docs="""
+        Keyword argument was defined but not used::
+        
+            *** Keywords ***
+            Keyword
+                [Arguments]    ${used}    ${not_used}  # will report ${not_used}
+                Log    ${used}
+                IF    $used
+                    Log    Escaped syntax is supported.
+                END
+
+            Keyword with ${embedded} and ${not_used}  # will report ${not_used}
+                Log    ${embedded}
+
+        """,
+    ),
+    "0920": Rule(
+        rule_id="0920",
+        name="unused-variable",
+        msg="Variable '{{ name }}' is assigned but not used",
+        severity=RuleSeverity.INFO,
+        docs="""
+        Variable was assigned but not used::
+    
+            *** Keywords ***
+            Get Triangle Base Points
+                [Arguments]       ${triangle}
+                ${p1}    ${p2}    ${p3}    Get Triangle Points    ${triangle}
+                Log      Triangle base points are: ${p1} and ${p2}.
+                RETURN   ${p1}    ${p2}  # ${p3} is never used
+    
+        Use ``${_}`` variable name if you purposefully do not use variable::
+    
+            *** Keywords ***
+            Process Value 10 Times
+                [Arguments]    ${value}
+                FOR    ${_}   IN RANGE    10
+                    Process Value    ${value}
+                END
+
+    """,
+    ),
+    "0921": Rule(
+        rule_id="0921",
+        name="argument-overwritten-before-usage",
+        msg="Keyword argument '{{ name }}' is overwritten before usage",
+        severity=RuleSeverity.WARNING,
+        docs="""
+        Keyword argument was overwritten before it is used::
+        
+            *** Keywords ***
+            Overwritten Argument
+                [Arguments]    ${overwritten}  # we do not use ${overwritten} value at all
+                ${overwritten}    Set Variable    value  # we only overwrite it
+
+        """,
+    ),
+    "0922": Rule(
+        rule_id="0922",
+        name="variable-overwritten-before-usage",
+        msg="Local variable '{{ name }}' is overwritten before usage",
+        severity=RuleSeverity.WARNING,
+        docs="""
+        Local variable in Keyword, Test Case or Task is overwritten before it is used::
+
+            *** Keywords ***
+            Overwritten Variable
+                ${value}    Keyword
+                ${value}    Keyword
+
+        In case the value of the variable is not important, it is possible to use `${_}` name::
+        
+            *** Test Cases ***
+            Call keyword and ignore some return values
+                ${_}    ${item}    Unpack List    @{LIST}
+                FOR    ${_}    IN RANGE  10
+                    Log    Run this code 10 times.
+                END
+
+        """,
+    ),
 }
 
 
 class ReturnChecker(VisitorChecker):
     """Checker for [Return] and Return From Keyword violations."""
 
     reports = (
@@ -751,17 +846,264 @@
 
     def visit_Continue(self, node):  # noqa
         self.check_statement_in_loop(node, "CONTINUE")  # type: ignore[arg-type]
 
     def visit_Break(self, node):  # noqa
         self.check_statement_in_loop(node, "BREAK")  # type: ignore[arg-type]
 
+    def visit_Error(self, node):  # noqa
+        """Support for RF >= 6.1"""
+        for error_token in node.get_tokens(Token.ERROR):
+            if "is not allowed in this context" in error_token.error:
+                self.report(
+                    "statement-outside-loop",
+                    name=error_token.value,
+                    statement_type="statement",
+                    node=node,
+                    col=error_token.col_offset + 1,
+                )
+
     def check_statement_in_loop(self, node, token_type):
         if self.loops or node.errors and f"{token_type} can only be used inside a loop." not in node.errors:
             return
         self.report(
             "statement-outside-loop",
             name=token_type,
             statement_type="statement",
             node=node,
             col=token_col(node, token_type),
         )
+
+
+CachedVariable = namedtuple("CachedVariable", "name token")
+
+
+class UnusedVariablesChecker(VisitorChecker):
+    reports = (
+        "unused-argument",
+        "unused-variable",
+        "argument-overwritten-before-usage",
+        "variable-overwritten-before-usage",
+    )
+
+    def __init__(self):
+        self.arguments = {}
+        self.variables = [{}]  # variables are list of scope-dictionaries, to support IF branches
+        self.ignore_overwriting = False  # temporarily ignore overwriting, e.g. in FOR loops
+        super().__init__()
+
+    def visit_TestCase(self, node):  # noqa
+        self.variables = [{}]
+        self.generic_visit(node)
+        self.check_unused_variables()
+
+    def visit_Keyword(self, node):  # noqa
+        self.arguments = {}
+        self.variables = [{}]
+        name_token = node.header.get_token(Token.KEYWORD_NAME)
+        self.parse_embedded_arguments(name_token)
+        # iterating there instead of using visit_Arguments, so we don't check keywords without arguments
+        for statement in node.body:
+            if isinstance(statement, Arguments):
+                self.parse_arguments(statement)
+        self.generic_visit(node)
+        for arg in self.arguments.values():
+            value, *_ = arg.token.value.split("=", maxsplit=1)
+            self.report_arg_or_var_rule("unused-argument", arg.token, value)
+        self.check_unused_variables()
+
+    def check_unused_variables(self):
+        for scope in self.variables:
+            for variable in scope.values():
+                self.report_arg_or_var_rule("unused-variable", variable.token, variable.name)
+
+    def report_arg_or_var_rule(self, rule, token, value=None):
+        if value is None:
+            value = token.value
+        self.report(
+            rule,
+            name=value,
+            node=token,
+            lineno=token.lineno,
+            col=token.col_offset + 1,
+            end_col=token.col_offset + len(value) + 1,
+        )
+
+    def add_argument(self, argument, normalized_name, token):
+        self.arguments[normalized_name] = CachedVariable(argument, token)
+
+    def parse_arguments(self, node):
+        """Store arguments from [Arguments]. Ignore @{args} and &{kwargs}, strip default values."""
+        if get_errors(node):
+            return
+        for arg in node.get_tokens(Token.ARGUMENT):
+            if arg.value[0] in ("@", "&"):  # ignore *args and &kwargs
+                continue
+            name, *_ = arg.value.split("=", maxsplit=1)
+            normalized_name = normalize_robot_var_name(name)
+            self.add_argument(name, normalized_name, token=arg)
+
+    def parse_embedded_arguments(self, name_token):
+        """Store embedded arguments from keyword name. Ignore embedded variables patterns (${var:pattern})."""
+        try:
+            for token in name_token.tokenize_variables():
+                if token.type == Token.VARIABLE:
+                    normalized_name = normalize_robot_var_name(token.value)
+                    name, *_ = normalized_name.split(":", maxsplit=1)
+                    self.add_argument(token.value, name, token=token)
+        except VariableError:
+            pass
+
+    def visit_If(self, node):  # noqa
+        if node.header.errors:
+            return node
+        for token in node.header.get_tokens(Token.ARGUMENT):
+            self.find_not_nested_variable(token.value, is_var=False)
+        for token in node.header.get_tokens(Token.ASSIGN):
+            self.handle_assign_variable(token, remove_equal=True)
+        self.variables.append({})
+        for item in node.body:
+            self.visit(item)
+        self.variables.pop()
+        if node.orelse:
+            self.visit(node.orelse)
+
+    def visit_While(self, node):  # noqa
+        if node.header.errors:
+            return node
+        for token in node.header.get_tokens(Token.ARGUMENT):
+            self.find_not_nested_variable(token.value, is_var=False)
+        if node.limit:
+            self.find_not_nested_variable(node.limit, is_var=False)
+        return self.generic_visit(node)
+
+    def visit_For(self, node):  # noqa
+        if getattr(node.header, "errors", None):
+            return node
+        self.ignore_overwriting = True
+        for token in node.header.get_tokens(Token.ARGUMENT):
+            self.find_not_nested_variable(token.value, is_var=False)
+        for token in node.header.get_tokens(Token.VARIABLE):
+            self.handle_assign_variable(token, remove_equal=False)
+        self.generic_visit(node)
+        self.ignore_overwriting = False
+
+    visit_ForLoop = visit_For
+
+    def visit_Try(self, node):  # noqa
+        if node.errors or node.header.errors:
+            return node
+        if node.variable is not None:
+            error_var = node.header.get_token(Token.VARIABLE)
+            if error_var is not None:
+                self.handle_assign_variable(error_var, remove_equal=False)
+        return self.generic_visit(node)
+
+    def visit_KeywordCall(self, node):  # noqa
+        for token in node.get_tokens(Token.ARGUMENT, Token.KEYWORD):  # argument can be used in keyword name
+            self.find_not_nested_variable(token.value, is_var=False)
+        for token in node.get_tokens(Token.ASSIGN):  # we first check args, then assign for used and then overwritten
+            self.handle_assign_variable(token, remove_equal=True)
+
+    def visit_Return(self, node):  # noqa
+        for token in node.get_tokens(Token.ARGUMENT):
+            self.find_not_nested_variable(token.value, is_var=False)
+
+    visit_ReturnStatement = visit_Teardown = visit_Timeout = visit_Return
+
+    def visit_TemplateArguments(self, node):  # noqa
+        for argument in node.data_tokens:
+            self.find_not_nested_variable(argument.value, is_var=False)
+
+    def handle_assign_variable(self, token, remove_equal):
+        """Check if assign does not overwrite arguments or variables.
+
+        Store assign variables for future overwriting checks."""
+        value = token.value
+        if remove_equal:
+            value = value.rstrip("=").strip()  # remove possible '=' and ' ='
+        normalized = normalize_robot_var_name(value)  # remove ${ } and normalize
+        if not normalized:  # ie. "${_}" -> ""
+            return
+        arg = self.arguments.pop(normalized, None)
+        if arg is not None:
+            self.report_arg_or_var_rule("argument-overwritten-before-usage", arg.token)
+        for variable_scope in self.variables[::-1]:
+            variable = variable_scope.pop(normalized, None)
+            if variable is not None and not self.ignore_overwriting:
+                self.report_arg_or_var_rule("variable-overwritten-before-usage", variable.token, value)
+        self.variables[-1][normalized] = CachedVariable(value, token)
+
+    def find_not_nested_variable(self, value, is_var):
+        """Find and process not nested variable.
+
+        Search `value` string until there is ${variable} without other variables inside. Unescaped escaped syntax
+        ($var or \\${var}). If variable does exist in assign variables or arguments, it is removed to denote it was
+        used.
+        """
+        try:
+            variables = list(VariableIterator(value))
+        except VariableError:  # for example ${variable which wasn't closed properly
+            return
+        if not variables:
+            if is_var:
+                self.update_used_variables(value)
+            elif "$" in value:
+                self.find_escaped_variables(value)  # $var
+                if r"\${" in value:  # \\${var}
+                    unescaped = unescape(value)
+                    self.find_not_nested_variable(unescaped, is_var=False)
+            return
+        remaining = ""
+        for before, variable, remaining in variables:
+            if before:
+                if "$" in before:
+                    self.find_escaped_variables(before)
+                elif is_var:  # ${test.kws[0].msgs[${index}]}
+                    self.update_used_variables(before)
+            # handle ${variable}[item][${syntax}]
+            match = search_variable(variable, ignore_errors=True)
+            if match.base and match.base.startswith("{") and match.base.endswith("}"):  # inline val
+                self.find_not_nested_variable(match.base[1:-1].strip(), is_var=False)
+            else:
+                self.find_not_nested_variable(match.base, is_var=True)
+            for item in match.items:
+                self.find_not_nested_variable(item, is_var=False)
+        if remaining:
+            if "$" in remaining:
+                self.find_escaped_variables(remaining)
+            elif is_var:  # ${test.kws[0].msgs[${index}]}
+                self.update_used_variables(remaining)
+
+    def find_escaped_variables(self, value):
+        """Find all $var escaped variables in the value string and process them."""
+        for var in find_escaped_variables(value):
+            self.update_used_variables(var)
+
+    def update_used_variables(self, variable_name):
+        """Remove used variable from the arguments and variables store.
+
+        If the normalized variable name was already defined, we need to remove it to know which variables are not used.
+        If the variable is not found, we try to remove possible attribute access from the name and search again.
+        For example:
+
+          arg.attr -> arg
+          arg["value"] -> arg
+        """
+        normalized = normalize_robot_name(variable_name)
+        arg = self.arguments.pop(normalized, None)
+        if arg is None:
+            self.search_by_removing_attr_access(normalized, self.arguments)
+        for variable_scope in self.variables[::-1]:
+            arg_var = variable_scope.pop(normalized, None)
+            if arg_var is None:
+                self.search_by_removing_attr_access(normalized, variable_scope)
+
+    @staticmethod
+    def search_by_removing_attr_access(variable_name, variable_scope):
+        """Search and remove variables from variable_scope by removing attribute access elements from the name."""
+        for attr_access in (".", "[", "("):  # ${arg.attr}
+            if attr_access in variable_name:
+                name, _ = variable_name.split(attr_access, maxsplit=1)
+                arg_var = variable_scope.pop(name, None)
+                if arg_var is not None:
+                    return
```

### Comparing `robotframework-robocop-3.1.1/robocop/checkers/naming.py` & `robotframework-robocop-3.2.0/robocop/checkers/naming.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import string
 from collections import defaultdict
 from pathlib import Path
 
 from robot.api import Token
 from robot.errors import VariableError
 from robot.parsing.model.statements import Arguments
+from robot.variables import VariableIterator
 from robot.variables.search import search_variable
 
 from robocop.checkers import VisitorChecker
 from robocop.rules import Rule, RuleParam, RuleSeverity
 from robocop.utils import (
     ROBOT_VERSION,
     find_robot_vars,
@@ -238,14 +239,27 @@
     ),
     "0316": Rule(
         rule_id="0316",
         name="possible-variable-overwriting",
         msg="Variable '{{ variable_name }}' may overwrite similar variable inside '{{ block_name }}' {{ block_type }}. "
         "Note that variables are case-insensitive, and also spaces and underscores are ignored.",
         severity=RuleSeverity.INFO,
+        docs="""
+        Following assignments overwrite the same variable::
+        
+            *** Keywords ***
+            Keyword
+                ${variable}    Keyword Call
+                ${VARIABLE}    Keyword Call
+                ${vari_ab le}    Keyword Call
+        
+        Use consistent variable naming guidelines to avoid unintended variable overwriting.
+        Remember that variable names in Robot Framework are case-insensitive and
+        underscores and whitespaces are ignored.
+        """,
     ),
     "0317": Rule(
         rule_id="0317",
         name="hyphen-in-variable-name",
         msg="Use underscore in variable name '{{ variable_name }}' instead of hyphens to "
         "avoid treating them like minus sign",
         severity=RuleSeverity.INFO,
@@ -337,22 +351,86 @@
             Library    Collections    AS    AliasedName
 
         """,
     ),
     "0322": Rule(
         rule_id="0322",
         name="deprecated-singular-header",
-        msg="'{{ singular_header }}' singular header form is deprecated since RF 6.0 and will be removed in the future releases. Use '{{ plural_header }}' instead",
+        msg="'{{ singular_header }}' singular header form is deprecated since RF 6.0 and "
+        "will be removed in the future releases. Use '{{ plural_header }}' instead",
         severity=RuleSeverity.WARNING,
         version=">=6.0",
         docs="""
         Robot Framework 6.0 starts deprecation period for singular headers forms. The rationale behind this change
         is available at https://github.com/robotframework/robotframework/issues/4431 .
         """,
     ),
+    "0323": Rule(
+        rule_id="0323",
+        name="inconsistent-variable-name",
+        msg="Variable '{{ name }}' has inconsistent naming. First used as '{{ first_use }}'",
+        severity=RuleSeverity.WARNING,
+        docs="""
+        Variable names are case-insensitive and ignore underscores and spaces. It is possible to 
+        write the variable in multiple ways and it will be a valid Robot Framework code. However,
+        it makes it harder to maintain the code that does not follow the consistent naming.
+        
+        Example::
+        
+            *** Keywords ***
+            Keyword
+                [Arguments]    ${argument}
+                ${variable}    Keyword Call
+                IF    ${ARGUMENT}  # inconsistent name with ${argument}
+                    Should Be True    ${vari_able}  # inconsistent name with ${variable}
+                END
+                Log    ${variable}  # consistent name
+
+        """,
+    ),
+    "0324": Rule(
+        rule_id="0324",
+        name="overwriting-reserved-variable",
+        msg="{{ var_or_arg }} '{{ variable_name }}' overwrites reserved variable '{{ reserved_variable }}'",
+        severity=RuleSeverity.WARNING,
+        docs="""
+        Overwriting reserved variables may bring unexpected results.
+        For example, overwriting variable with name ``${LOG_LEVEL}`` can break Robot Framework logging.
+        See full list of reserved variables at
+        `Robot Framework User Guide <https://robotframework.org/robotframework/latest/RobotFrameworkUserGuide.html#automatic-variables>`_
+        """,
+    ),
+    "0325": Rule(
+        rule_id="0325",
+        name="invalid-section",
+        msg="Invalid section '{{ invalid_section }}'. Consider using --language parameter if the file is defined with different language.",
+        severity=RuleSeverity.ERROR,
+        version=">=6.1",
+        docs="""
+            Robot Framework 6.1 detects unrecognized sections based on the language defined for the specific files.
+            Consider using --language parameter if the file is defined with different language.
+            
+            It is also possible to configure language in the file:
+            
+            ```
+            language: pl
+            
+            *** Przypadki Testowe ***
+            Test case
+                Step
+            ```
+            """,
+    ),
+}
+
+SET_VARIABLE_VARIANTS = {
+    "settaskvariable",
+    "settestvariable",
+    "setsuitevariable",
+    "setglobalvariable",
 }
 
 
 class InvalidCharactersInNameChecker(VisitorChecker):
     """Checker for invalid characters in suite, test case or keyword name."""
 
     reports = (
@@ -550,23 +628,38 @@
     """Checker for settings and sections naming violations."""
 
     reports = (
         "setting-name-not-in-title-case",
         "section-name-invalid",
         "empty-library-alias",
         "duplicated-library-alias",
+        "invalid-section",
     )
     ALIAS_TOKENS = [Token.WITH_NAME] if ROBOT_VERSION.major < 5 else [Token.WITH_NAME, "AS"]
     # Separating alias values since RF 3 uses WITH_NAME instead of WITH NAME
     ALIAS_TOKENS_VALUES = ["WITH NAME"] if ROBOT_VERSION.major < 5 else [Token.WITH_NAME, "AS"]
 
     def __init__(self):
         self.section_name_pattern = re.compile(r"\*\*\*\s.+\s\*\*\*")
         super().__init__()
 
+    def visit_InvalidSection(self, node):  # noqa
+        name = node.header.data_tokens[0].value
+        invalid_header = node.header.get_token(Token.INVALID_HEADER)
+        if "Resource file with" in invalid_header.error:
+            return
+        if invalid_header:
+            self.report(
+                "invalid-section",
+                invalid_section=name,
+                node=node,
+                col=node.header.col_offset + 1,
+                end_col=node.header.end_col_offset + 1,
+            )
+
     def visit_SectionHeader(self, node):  # noqa
         name = node.data_tokens[0].value
         if not self.section_name_pattern.match(name) or not (name.istitle() or name.isupper()):
             valid_name = f"*** {node.name.title()} ***"
             self.report(
                 "section-name-invalid",
                 section_title_case=valid_name,
@@ -651,24 +744,46 @@
 class VariableNamingChecker(VisitorChecker):
     """Checker for variable naming violations."""
 
     reports = (
         "section-variable-not-uppercase",
         "non-local-variables-should-be-uppercase",
         "hyphen-in-variable-name",
+        "overwriting-reserved-variable",
     )
+    RESERVED_VARIABLES = {
+        "testname": "${TEST_NAME}",
+        "testtags": "@{TEST_TAGS}",
+        "testdocumentation": "${TEST_DOCUMENTATION}",
+        "teststatus": "${TEST_STATUS}",
+        "testmessage": "${TEST_MESSAGE}",
+        "prevtestname": "${PREV_TEST_NAME}",
+        "prevteststatus": "${PREV_TEST_STATUS}",
+        "prevtestmessage": "${PREV_TEST_MESSAGE}",
+        "suitename": "${SUITE_NAME}",
+        "suitesource": "${SUITE_SOURCE}",
+        "suitedocumentation": "${SUITE_DOCUMENTATION}",
+        "suitemetadata": "&{SUITE_METADATA}",
+        "suitestatus": "${SUITE_STATUS}",
+        "suitemessage": "${SUITE_MESSAGE}",
+        "keywordstatus": "${KEYWORD_STATUS}",
+        "keywordmessage": "${KEYWORD_MESSAGE}",
+        "loglevel": "${LOG_LEVEL}",
+        "outputfile": "${OUTPUT_FILE}",
+        "logfile": "${LOG_FILE}",
+        "reportfile": "${REPORT_FILE}",
+        "debugfile": "${DEBUG_FILE}",
+        "outputdir": "${OUTPUT_DIR}",
+        # "options": "&{OPTIONS}", This variable is widely used and is relatively safe to overwrite
+    }
 
-    def __init__(self):
-        self.set_variable_variants = {
-            "settaskvariable",
-            "settestvariable",
-            "setsuitevariable",
-            "setglobalvariable",
-        }
-        super().__init__()
+    def visit_Keyword(self, node):  # noqa
+        name_token = node.header.get_token(Token.KEYWORD_NAME)
+        self.parse_embedded_arguments(name_token)
+        self.generic_visit(node)
 
     def visit_Variable(self, node):  # noqa
         token = node.data_tokens[0]
         try:
             var_name = search_variable(token.value).base
         except VariableError:
             return  # TODO: Ignore for now, for example ${not  closed in variables will throw it
@@ -680,29 +795,31 @@
             self.report(
                 "section-variable-not-uppercase",
                 variable_name=token.value.strip(),
                 lineno=token.lineno,
                 col=token.col_offset + 1,
                 end_col=token.col_offset + len(token.value) + 1,
             )
+        self.check_for_reserved_naming(token, "Variable")
 
     def visit_KeywordCall(self, node):  # noqa
         for token in node.get_tokens(Token.ASSIGN):
             if "-" in token.value:
                 self.report(
                     "hyphen-in-variable-name",
                     variable_name=token.value,
                     lineno=token.lineno,
                     col=token.col_offset + 1,
                     end_col=token.end_col_offset + 1,
                 )
+            self.check_for_reserved_naming(token, "Variable")
 
         if not node.keyword:
             return
-        if normalize_robot_name(node.keyword, remove_prefix="builtin.") in self.set_variable_variants:
+        if normalize_robot_name(node.keyword, remove_prefix="builtin.") in SET_VARIABLE_VARIANTS:
             if len(node.data_tokens) < 2:
                 return
             token = node.data_tokens[1]
             if not token.value:
                 return
             try:
                 var_name = search_variable(token.value).base
@@ -717,73 +834,220 @@
                 self.report(
                     "non-local-variables-should-be-uppercase",
                     node=node,
                     col=token.col_offset + 1,
                     end_col=token.end_col_offset + 1,
                 )
 
+    def visit_If(self, node):  # noqa
+        for token in node.header.get_tokens(Token.ASSIGN):
+            self.check_for_reserved_naming(token, "Variable")
+        self.generic_visit(node)
+
+    def visit_Arguments(self, node):  # noqa
+        for arg in node.get_tokens(Token.ARGUMENT):
+            self.check_for_reserved_naming(arg, "Argument")
+
+    def parse_embedded_arguments(self, name_token):
+        """Store embedded arguments from keyword name. Ignore embedded variables patterns like (${var:pattern})."""
+        try:
+            for token in name_token.tokenize_variables():
+                if token.type == Token.VARIABLE:
+                    self.check_for_reserved_naming(token, "Embedded argument", has_pattern=True)
+        except VariableError:
+            pass
+
+    def check_for_reserved_naming(self, token, var_or_arg, has_pattern=False):
+        """Check if variable name is a reserved Robot Framework name."""
+        name, *_ = token.value.split("=", maxsplit=1)
+        name = name.rstrip()
+        if has_pattern:
+            name, *pattern = name.split(":", maxsplit=1)
+            if pattern:
+                name += "}"  # recreate, so it handles ${variable:pattern} -> ${variable} matching
+        normalized_name = normalize_robot_var_name(name)
+        if normalized_name in self.RESERVED_VARIABLES:
+            reserved_variable = self.RESERVED_VARIABLES[normalized_name]
+            self.report(
+                "overwriting-reserved-variable",
+                var_or_arg=var_or_arg,
+                variable_name=name,
+                reserved_variable=reserved_variable,
+                node=token,
+                lineno=token.lineno,
+                col=token.col_offset + 1,
+                end_col=token.col_offset + len(name) + 1,
+            )
+
 
 class SimilarVariableChecker(VisitorChecker):
     """Checker for finding same variables with similar names."""
 
-    reports = ("possible-variable-overwriting",)
+    reports = ("possible-variable-overwriting", "inconsistent-variable-name")
 
     def __init__(self):
-        self.variables = defaultdict(set)
+        self.assigned_variables = defaultdict(list)
         self.parent_name = ""
         self.parent_type = ""
         super().__init__()
 
     def visit_Keyword(self, node):  # noqa
-        self.variables = defaultdict(set)
+        self.assigned_variables = defaultdict(list)
         self.parent_name = node.name
         self.parent_type = type(node).__name__
+        name_token = node.header.get_token(Token.KEYWORD_NAME)
+        self.parse_embedded_arguments(name_token)
         self.visit_vars_and_find_similar(node)
         self.generic_visit(node)
 
-    visit_TestCase = visit_Keyword
+    def visit_TestCase(self, node):  # noqa
+        self.assigned_variables = defaultdict(list)
+        self.parent_name = node.name
+        self.parent_type = type(node).__name__
+        self.generic_visit(node)
 
     def visit_KeywordCall(self, node):  # noqa
+        if normalize_robot_name(node.keyword, remove_prefix="builtin.") in SET_VARIABLE_VARIANTS:
+            normalized, assign_value = "", ""
+            for index, token in enumerate(node.data_tokens[1:]):
+                if index == 0:  # First argument is assign-like
+                    normalized = normalize_robot_var_name(token.value)
+                    assign_value = token.value  # process assign last, cache for now
+                else:
+                    self.find_not_nested_variable(token, token.value, is_var=False)
+            self.assigned_variables[normalized].append(assign_value)
+        else:
+            for token in node.get_tokens(Token.ARGUMENT, Token.KEYWORD):  # argument can be used in keyword name
+                self.find_not_nested_variable(token, token.value, is_var=False)
         tokens = node.get_tokens(Token.ASSIGN)
         self.find_similar_variables(tokens, node)
 
+    def visit_If(self, node):  # noqa
+        for token in node.header.get_tokens(Token.ARGUMENT):
+            self.find_not_nested_variable(token, token.value, is_var=False)
+        tokens = node.header.get_tokens(Token.ASSIGN)
+        self.find_similar_variables(tokens, node)
+        self.generic_visit(node)
+
+    def visit_While(self, node):  # noqa
+        for token in node.header.get_tokens(Token.ARGUMENT):
+            self.find_not_nested_variable(token, token.value, is_var=False)
+        return self.generic_visit(node)
+
     def visit_For(self, node):  # noqa
+        for token in node.header.get_tokens(Token.ARGUMENT):
+            self.find_not_nested_variable(token, token.value, is_var=False)
         for var in node.variables:
-            self.variables[normalize_robot_var_name(var)].add(var)
+            self.assigned_variables[normalize_robot_var_name(var)].append(var)
         self.generic_visit(node)
 
     visit_ForLoop = visit_For
 
+    def visit_Return(self, node):  # noqa
+        for token in node.get_tokens(Token.ARGUMENT):
+            self.find_not_nested_variable(token, token.value, is_var=False)
+
+    visit_ReturnStatement = visit_Teardown = visit_Timeout = visit_Return
+
+    def parse_embedded_arguments(self, name_token):
+        """Store embedded arguments from keyword name. Ignore embedded variables patterns (${var:pattern})."""
+        try:
+            for token in name_token.tokenize_variables():
+                if token.type == Token.VARIABLE:
+                    var_name, *pattern = token.value.split(":", maxsplit=1)
+                    if pattern:
+                        var_name = var_name + "}"  # recreate, so it handles ${variable:pattern} -> ${variable} matching
+                    normalized_name = normalize_robot_var_name(var_name)
+                    self.assigned_variables[normalized_name].append(var_name)
+        except VariableError:
+            pass
+
+    def check_inconsistent_naming(self, token, value: str, offset: int):
+        """Check if variable name ``value`` was already defined under matching but not the same name.
+        :param token: ast token representing the string with variable
+        :param value: name of variable found in token value string
+        :param offset: starting position of variable in token value string
+        """
+        normalized = normalize_robot_name(value)
+        if normalized not in self.assigned_variables:
+            return  # we could handle attr access here, ignoring now
+        latest_assign = self.assigned_variables[normalized][-1]
+        assign_normalized = latest_assign.lstrip("$@%&").lstrip("{").rstrip("}")
+        if value != assign_normalized:
+            name = "${" + value + "}"
+            self.report(
+                "inconsistent-variable-name",
+                name=name,
+                first_use=latest_assign,
+                node=token,
+                lineno=token.lineno,
+                col=token.col_offset + offset + 1,
+                end_col=token.col_offset + offset + len(name) + 1,
+            )
+
+    def find_not_nested_variable(self, token, value, is_var: bool, offset: int = 0):
+        """Find and process not nested variable.
+
+        Search `value` string until there is ${variable} without other variables inside.
+        Unescaped escaped syntax ($var or \\${var}) is ignored.
+        Offset is to determine position of the variable in the string.
+        For example 'This is ${var}' contains ${var} at 8th position.
+        """
+        try:
+            variables = list(VariableIterator(value))
+        except VariableError:  # for example ${variable which wasn't closed properly
+            return
+        if not variables:
+            if is_var:
+                self.check_inconsistent_naming(token, value, offset)
+            return
+        if is_var:
+            offset += 2  # handle ${var_${var}} case
+        for before, variable, _ in variables:
+            if before:
+                offset += len(before)
+            match = search_variable(variable, ignore_errors=True)
+            if match.base and match.base.startswith("{") and match.base.endswith("}"):  # inline val
+                self.find_not_nested_variable(token, match.base[1:-1].strip(), is_var=False, offset=offset + 1)
+            else:
+                self.find_not_nested_variable(token, match.base, is_var=True, offset=offset)
+            offset += len(variable)
+            for item in match.items:
+                self.find_not_nested_variable(token, item, is_var=False, offset=offset)
+                offset += len(item)
+
     def visit_vars_and_find_similar(self, node):
         """
-        Creates a dictionary `variables` with normalized variable name as a key
+        Updates a dictionary `assign_variables` with normalized variable name as a key
         and ads a list of all detected variations of this variable in the node as a value,
         then it checks if similar variable was found.
         """
         for child in node.body:
-            # read arguments from Test Case or Keyword
+            # read arguments from Keywords
             if isinstance(child, Arguments):
                 for token in child.get_tokens(Token.ARGUMENT):
-                    self.variables[normalize_robot_var_name(token.value)].add(token.value)
+                    name, *_ = token.value.split("=", maxsplit=1)
+                    self.assigned_variables[normalize_robot_var_name(name)].append(name.strip())
 
     def find_similar_variables(self, tokens, node):
         for token in tokens:
-            normalized_token = normalize_robot_var_name(token.value)
-            if normalized_token in self.variables and token.value not in self.variables[normalized_token]:
+            name, *_ = token.value.split("=", maxsplit=1)
+            normalized_token = normalize_robot_var_name(name)
+            if normalized_token in self.assigned_variables and name not in self.assigned_variables[normalized_token]:
                 self.report(
                     "possible-variable-overwriting",
-                    variable_name=token.value,
+                    variable_name=name,
                     block_name=self.parent_name,
                     block_type=self.parent_type,
                     node=node,
                     lineno=token.lineno,
                     col=token.col_offset + 1,
                     end_col=token.end_col_offset + 1,
                 )
-            self.variables[normalized_token].add(token.value)
+            self.assigned_variables[normalized_token].append(name.strip())
 
 
 class DeprecatedStatementChecker(VisitorChecker):
     """Checker for deprecated statements."""
 
     reports = ("deprecated-statement", "deprecated-with-name", "deprecated-singular-header")
     deprecated_keywords = {
```

### Comparing `robotframework-robocop-3.1.1/robocop/checkers/spacing.py` & `robotframework-robocop-3.2.0/robocop/checkers/spacing.py`

 * *Files 0% similar despite different names*

```diff
@@ -443,14 +443,15 @@
     def visit_File(self, node):  # noqa
         for section in node.sections:
             self.check_empty_lines_after_section(section)
         for section in node.sections[:-1]:
             if not section.header:  # for comment section
                 continue
             empty_lines = 0
+            child = section  # workaround for empty sections when reporting issue
             for child in reversed(section.body):
                 if isinstance(child, (Keyword, TestCase)):
                     for statement in reversed(child.body):
                         if isinstance(statement, EmptyLine):
                             empty_lines += 1
                         else:
                             break
```

### Comparing `robotframework-robocop-3.1.1/robocop/checkers/tags.py` & `robotframework-robocop-3.2.0/robocop/checkers/tags.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-3.1.1/robocop/config.py` & `robotframework-robocop-3.2.0/robocop/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from robot.utils import FileReader
 
 from robocop.exceptions import (
     ArgumentFileNotFoundError,
     CircularArgumentFileError,
     ConfigGeneralError,
     InvalidArgumentError,
+    TomlFileNotFoundError,
 )
 from robocop.files import DEFAULT_EXCLUDES, find_file_in_project_root, find_project_root
 from robocop.rules import RuleSeverity
 from robocop.utils import RecommendationFinder
 from robocop.version import __version__
 
 
@@ -59,14 +60,20 @@
     def __call__(self, parser, namespace, values, option_string=None):
         pattern = values if values else "*"
         if "*" in pattern:
             pattern = translate_pattern(pattern)
         setattr(namespace, self.dest, pattern)
 
 
+class SetOptionalValue(argparse.Action):
+    def __call__(self, parser, namespace, value, option_string=None):
+        value = value if value else "default"
+        setattr(namespace, self.dest, value)
+
+
 class CustomArgParser(argparse.ArgumentParser):
     def __init__(self, *args, from_cli=False, **kwargs):
         self.from_cli = from_cli
         super().__init__(*args, **kwargs)
 
     def error(self, message):
         if self.from_cli:
@@ -186,15 +193,15 @@
         self.ext_rules = set()
         self.include_patterns = []
         self.exclude_patterns = []
         self.filetypes = {".robot", ".resource", ".tsv"}
         self.language = []
         self.list = ""
         self.list_configurables = ""
-        self.list_reports = False
+        self.list_reports = ""
         self.output = None
         self.recursive = True
         self.verbose = False
         self.config_from = ""
         self.root = find_project_root(root, ["."])
         self.parse()
 
@@ -329,17 +336,21 @@
             help="List all available rules with configurable parameters. You can use optional PATTERN argument "
             "to match rule names (for example --list *doc*). "
             "PATTERN can be also ENABLED/DISABLED keyword to list only enabled/disabled rules.",
         )
         optional.add_argument(
             "-lr",
             "--list-reports",
-            action="store_true",
+            action=SetOptionalValue,
+            nargs="?",
+            const="",
             default=self.list_reports,
-            help="List all available reports.",
+            metavar="ENABLED/DISABLED",
+            help="List all available reports. "
+            "Pass ENABLED or DISABLED as argument to list only enabled/disabled reports.",
         )
         optional.add_argument(
             "-o",
             "--output",
             type=argparse.FileType("w"),
             default=self.output,
             metavar="PATH",
@@ -357,14 +368,15 @@
             "--threshold",
             action=SetRuleThreshold,
             default=self.threshold,
             help=f"Disable rules below given threshold. Available message levels: "
             f'{" < ".join(sev.value for sev in RuleSeverity)}',
         )
         optional.add_argument("-A", "--argumentfile", metavar="PATH", help="Path to file with arguments.")
+        optional.add_argument("--config", metavar="PATH", help="Path to TOML configuration file.")
         optional.add_argument(
             "-g",
             "--ignore",
             action=ParseDelimitedArgAction,
             default=self.ignore,
             metavar="PATH",
             help="Ignore file(s) and path(s) provided. Glob patterns are supported.",
@@ -411,24 +423,22 @@
         return parser
 
     def parse(self):
         if not self.from_cli:
             self.load_default_config_file()
             return
         args = sys.argv[1:]
-        if not self.argument_file_in_cli(args):
+        if not self.config_file_in_cli(args):
             self.load_default_config_file()
         self.parse_args(args)
 
-    def argument_file_in_cli(self, args):
-        argument_options = {"-A", "--argumentfile"}
-        for arg in args:
-            if arg in argument_options:
-                return True
-        return False
+    @staticmethod
+    def config_file_in_cli(args):
+        config_options = {"-A", "--argumentfile", "--config"}
+        return any(arg in config_options for arg in args)
 
     def reload(self, rules):
         self.remove_severity()
         self.translate_patterns()
         self.print_config_source()
         self.validate_rule_names(rules)
         self.check_deprecations(rules)
@@ -439,45 +449,53 @@
             return
         if self.config_from:
             print(f"Loaded configuration from {self.config_from}")
         else:
             print("No config file found or configuration is empty. Using default configuration")
 
     def load_default_config_file(self):
-        if not self.load_robocop_file():
-            self.load_pyproject_file()
+        """Find and load default configuration file.
+
+        First look for .robocop file. If it does not exist, search for pyproject.toml file."""
+        if self.load_robocop_file():
+            return
+        pyproject_path = find_file_in_project_root("pyproject.toml", self.root)
+        if pyproject_path.is_file():
+            self.load_pyproject_file(pyproject_path)
 
     def load_robocop_file(self):
         """Returns True if .robocop exists"""
         robocop_path = find_file_in_project_root(".robocop", self.root)
         if not robocop_path.is_file():
             return False
         argument_files_parser = ArgumentFileParser()
         args = argument_files_parser.load_argument_file(robocop_path, robocop_path.parent)
         self.config_from = argument_files_parser.config_from
         self.parse_args(args)
         return True
 
-    def load_pyproject_file(self):
-        pyproject_path = find_file_in_project_root("pyproject.toml", self.root)
-        if not pyproject_path.is_file():
-            return
+    def load_pyproject_file(self, pyproject_path):
         config_dir = pyproject_path.parent
         try:
             with Path(pyproject_path).open("rb") as fp:
                 config = tomli.load(fp)
         except tomli.TOMLDecodeError as err:
             raise InvalidArgumentError(f"Failed to decode {str(pyproject_path)}: {err}") from None
         config = config.get("tool", {}).get("robocop", {})
         if self.parse_toml_to_config(config, config_dir):
             self.config_from = pyproject_path
 
     def parse_args_to_config(self, args):
         parser = self._create_parser()
         args = parser.parse_args(args)
+        if args.config is not None:
+            config_path = Path(args.config)
+            if not config_path.is_file():
+                raise TomlFileNotFoundError(str(config_path)) from None
+            self.load_pyproject_file(config_path)
         for key, value in dict(**vars(args)).items():
             if key in self.__dict__:
                 self.__dict__[key] = value
 
     def parse_args(self, args):
         argument_files_parser = ArgumentFileParser()
         args = argument_files_parser.expand_argument_files(args)
@@ -500,15 +518,16 @@
 
     def check_deprecations(self, rules):
         renamed = {
             # "old-name": "new-name"
         }
         deprecated = {
             # "rule-name": "deprecation message"
-            "bad-indent": "'strict' and 'ignore_uneven' parameters are no longer available for this rule. Take a look at new E1017 bad-block-indent rule that replaces them."  # warning added in v.3.0.0
+            "bad-indent": "'strict' and 'ignore_uneven' parameters are no longer available for this rule. "
+            "Take a look at new E1017 bad-block-indent rule that replaces them."  # warning added in v.3.0.0
         }
         deprecation_header = "### DEPRECATION WARNING ###"
         deprecation_footer = "This information will disappear in the next version.\n\n"
         # get all rules mentioned in include and exclude CLI options
         mentioned_rules = self.include.union(self.exclude)
         # add the rules mentioned in configure CLI option
         mentioned_rules.update(configured.split(":", 1)[0] for configured in self.configure)
```

### Comparing `robotframework-robocop-3.1.1/robocop/exceptions.py` & `robotframework-robocop-3.2.0/robocop/exceptions.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,14 +17,20 @@
 
 class FileError(RobocopFatalError):
     def __init__(self, source):
         msg = f'File "{source}" does not exist'
         super().__init__(msg)
 
 
+class TomlFileNotFoundError(RobocopFatalError):
+    def __init__(self, source):
+        msg = f'TOML configuration file "{source}" does not exist'
+        super().__init__(msg)
+
+
 class ArgumentFileNotFoundError(RobocopFatalError):
     def __init__(self, source):
         msg = f'Argument file "{source}" does not exist'
         super().__init__(msg)
 
 
 class CircularArgumentFileError(RobocopFatalError):
```

### Comparing `robotframework-robocop-3.1.1/robocop/files.py` & `robotframework-robocop-3.2.0/robocop/files.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-3.1.1/robocop/reports.py` & `robotframework-robocop-3.2.0/robocop/reports.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,21 +5,29 @@
 Each report class collects rules messages from linter and parses it. At the end of the scan it will print the report.
 
 To enable report use ``-r`` / ``--reports`` argument and the name of the report.
 You can use separate arguments (``-r report1 -r report2``) or comma-separated list (``-r report1,report2``). Example::
 
     robocop --reports rules_by_id,some_other_report path/to/file.robot
 
-To enable all default reports use ``--reports all``.
+To enable all default reports use ``--reports all``.  Non-default reports can be only enabled using report name.
 
 The order of the reports is preserved. For example, if you want ``timestamp`` report to be printed before any
 other reports, you can use following configuration::
 
     robocop --reports timestamp,all src.robot
 
+Print list of all reports with their configured status by using ``--list-reports``::
+
+    robocop --reports all --list-reports
+
+You can filter the list using optional ENABLED/DISABLED argument::
+
+    robocop --reports timestamp,sarif --list-reports DISABLED
+
 """
 import inspect
 import json
 import sys
 from collections import OrderedDict, defaultdict
 from datetime import datetime, timezone
 from operator import itemgetter
@@ -27,28 +35,28 @@
 from timeit import default_timer as timer
 from warnings import warn
 
 import pytz
 
 import robocop.exceptions
 from robocop.rules import Message
-from robocop.utils import RecommendationFinder
 from robocop.version import __version__
 
 
 class Report:
     """
     Base class for report class.
     Override `configure` method if you want to allow report configuration.
     Override `add_message`` if your report processes the Robocop issues.
 
     Set class attribute `DEFAULT` to `False` if you don't want your report to be included in `all` reports.
     """
 
     DEFAULT = True
+    INTERNAL = False
 
     def configure(self, name, value):
         raise robocop.exceptions.ConfigGeneralError(
             f"Provided param '{name}' for report '{getattr(self, 'name')}' does not exist"
         )  # noqa
 
     def add_message(self, *args):
@@ -73,14 +81,18 @@
     return reports
 
 
 def is_report_default(report):
     return getattr(report, "DEFAULT", False)
 
 
+def is_report_internal(report):
+    return getattr(report, "INTERNAL", False)
+
+
 def get_reports(configured_reports):
     """
     Returns dictionary with list of valid, enabled reports (listed in `configured_reports` set of str).
     If `configured_reports` contains `all` then all default reports are enabled.
     """
     reports = load_reports()
     enabled_reports = OrderedDict()
@@ -92,20 +104,36 @@
         elif report not in reports:
             raise robocop.exceptions.InvalidReportName(report, reports)
         elif report not in enabled_reports:
             enabled_reports[report] = reports[report]
     return enabled_reports
 
 
-def list_reports(reports):
-    """Returns description of enabled reports."""
-    sorted_by_name = sorted(reports.values(), key=lambda x: x.name)
-    available_reports = "Available reports:\n"
-    available_reports += "\n".join(f"{report.name:20} - {report.description}" for report in sorted_by_name) + "\n"
-    available_reports += "all" + " " * 18 + "- Turns on all default reports"
+def list_reports(reports, list_reports_with_status):
+    """Returns description of reports.
+
+    The reports list is filtered and only public reports are provided. If the report is enabled in current
+    configuration it will have (enabled) suffix (and (disabled) if it is disabled).
+    """
+    all_public_reports = [report for report in load_reports().values() if not is_report_internal(report)]
+    all_public_reports = sorted(all_public_reports, key=lambda x: x.name)
+    configured_reports = {x.name for x in reports.values()}
+    available_reports = "Available reports:"
+    for report in all_public_reports:
+        status = "enabled" if report.name in configured_reports else "disabled"
+        if list_reports_with_status != "default" and list_reports_with_status != status.upper():
+            continue
+        if not is_report_default(report):
+            status += " - non-default"
+        available_reports += f"\n{report.name:20} - {report.description} ({status})"
+    available_reports += (
+        "\n\nEnable report by passing report name using --reports option. "
+        "Use `all` to enable all default reports. "
+        "Non-default reports can be only enabled using report name."
+    )
     return available_reports
 
 
 class RulesByIdReport(Report):
     """
     Report name: ``rules_by_id``
 
@@ -178,14 +206,16 @@
     Report name: ``return_status``
 
     This report is always enabled.
     Report that checks if number of returned rules messages for given severity value does not exceed preset threshold.
     That information is later used as a return status from Robocop.
     """
 
+    INTERNAL = True
+
     def __init__(self):
         self.name = "return_status"
         self.description = "Checks if number of specific issues exceed quality gate limits"
         self.return_status = 0
         self.counter = RulesBySeverityReport()
         self.quality_gate = {"E": 0, "W": 0, "I": -1}
 
@@ -235,14 +265,15 @@
     """
     Report name: ``json_report``
 
     Report that returns list of found issues in JSON format.
     """
 
     DEFAULT = False
+    INTERNAL = True
 
     def __init__(self):
         self.name = "json_report"
         self.description = "Accumulates found issues in JSON format"
         self.issues = []
 
     def add_message(self, message: Message):
```

### Comparing `robotframework-robocop-3.1.1/robocop/rules.py` & `robotframework-robocop-3.2.0/robocop/rules.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-3.1.1/robocop/run.py` & `robotframework-robocop-3.2.0/robocop/run.py`

 * *Files 1% similar despite different names*

```diff
@@ -204,15 +204,15 @@
         )
         print("Visit https://robocop.readthedocs.io/en/stable/rules.html page for detailed documentation.")
         sys.exit()
 
     def load_reports(self):
         self.reports = reports.get_reports(self.config.reports)
         if self.config.list_reports:
-            available_reports = reports.list_reports(self.reports)
+            available_reports = reports.list_reports(self.reports, self.config.list_reports)
             print(available_reports)
             sys.exit()
 
     def register_checker(self, checker):
         for rule_name, rule in checker.rules.items():
             self.rules[rule_name] = rule
             self.rules[rule.rule_id] = rule
```

### Comparing `robotframework-robocop-3.1.1/robocop/utils/__init__.py` & `robotframework-robocop-3.2.0/robocop/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-3.1.1/robocop/utils/disablers.py` & `robotframework-robocop-3.2.0/robocop/utils/disablers.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-3.1.1/robocop/utils/file_types.py` & `robotframework-robocop-3.2.0/robocop/utils/file_types.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-3.1.1/robocop/utils/misc.py` & `robotframework-robocop-3.2.0/robocop/utils/misc.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 import ast
 import difflib
 import importlib.util
 import re
+import token
+import tokenize
 from collections import Counter, defaultdict
 from importlib import import_module
+from io import StringIO
 from pathlib import Path
+from tokenize import generate_tokens
 from typing import Dict, List, Optional, Pattern, Tuple
 
 from robot.api import Token
 
 try:
     from robot.api.parsing import Variable
 except ImportError:
@@ -342,7 +346,28 @@
     return ""
 
 
 def get_errors(node):
     if ROBOT_VERSION.major == 3:
         return [node.error] if node.error else []
     return node.errors
+
+
+def find_escaped_variables(string):
+    """Return list of $escaped or \${escaped} variables from the string.
+
+    We are tokenizing the string using Python ast modules. This allows us to find valid Python-like names and check
+    if they are escaped Robot Framework variables.
+    """
+    variable_started = False
+    variables = []
+    try:
+        for toknum, tokval, _, _, _ in generate_tokens(StringIO(string).readline):
+            if variable_started:
+                if toknum == token.NAME:
+                    variables.append(tokval)
+                variable_started = False
+            if toknum == token.ERRORTOKEN and tokval == "$":
+                variable_started = True
+    except tokenize.TokenError:
+        pass
+    return variables
```

### Comparing `robotframework-robocop-3.1.1/robocop/utils/run_keywords.py` & `robotframework-robocop-3.2.0/robocop/utils/run_keywords.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-3.1.1/robocop/utils/version_matching.py` & `robotframework-robocop-3.2.0/robocop/utils/version_matching.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-3.1.1/robotframework_robocop.egg-info/PKG-INFO` & `robotframework-robocop-3.2.0/robotframework_robocop.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-robocop
-Version: 3.1.1
+Version: 3.2.0
 Summary: Static code analysis tool (linter) for Robot Framework
 Home-page: https://github.com/MarketSquare/robotframework-robocop
 Download-URL: https://pypi.org/project/robotframework-robocop
 Author: Bartlomiej Hirsz, Mateusz Nojek
 Author-email: bartek.hirsz@gmail.com, matnojek@gmail.com
 License: Apache License 2.0
 Project-URL: Documentation, https://robocop.readthedocs.io/en/stable
```

### Comparing `robotframework-robocop-3.1.1/robotframework_robocop.egg-info/SOURCES.txt` & `robotframework-robocop-3.2.0/robotframework_robocop.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-3.1.1/setup.py` & `robotframework-robocop-3.2.0/setup.py`

 * *Files identical despite different names*

