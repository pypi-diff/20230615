# Comparing `tmp/codegenpt-0.6.1.tar.gz` & `tmp/codegenpt-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codegenpt-0.6.1.tar", max compression
+gzip compressed data, was "codegenpt-0.6.2.tar", max compression
```

## Comparing `codegenpt-0.6.1.tar` & `codegenpt-0.6.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1071 2023-06-14 02:09:48.042343 codegenpt-0.6.1/LICENSE
--rw-r--r--   0        0        0     2636 2023-06-15 05:04:45.202904 codegenpt-0.6.1/README.md
--rw-r--r--   0        0        0        0 2023-06-12 16:35:22.162725 codegenpt-0.6.1/codegenpt/__init__.py
--rw-r--r--   0        0        0     3584 2023-06-15 05:29:28.226734 codegenpt-0.6.1/codegenpt/cli.py
--rw-r--r--   0        0        0     2234 2023-06-15 05:29:28.226943 codegenpt-0.6.1/codegenpt/codegenpt_directory.py
--rw-r--r--   0        0        0      558 2023-06-14 05:25:26.194231 codegenpt-0.6.1/codegenpt/codegenpt_file.py
--rw-r--r--   0        0        0     1558 2023-06-15 05:29:28.227116 codegenpt-0.6.1/codegenpt/codegenpt_instructions.py
--rw-r--r--   0        0        0        0 2023-06-13 06:34:45.151317 codegenpt-0.6.1/codegenpt/commands/__init__.py
--rw-r--r--   0        0        0      248 2023-06-13 06:34:45.151452 codegenpt-0.6.1/codegenpt/commands/command.py
--rw-r--r--   0        0        0      612 2023-06-14 06:02:51.279908 codegenpt-0.6.1/codegenpt/commands/commands.py
--rw-r--r--   0        0        0     1672 2023-06-14 06:03:15.242782 codegenpt-0.6.1/codegenpt/commands/include.py
--rw-r--r--   0        0        0      377 2023-06-15 05:24:10.521616 codegenpt-0.6.1/codegenpt/dependency_batch.py.codegenpt
--rw-r--r--   0        0        0        0 2023-06-12 16:42:59.544293 codegenpt-0.6.1/codegenpt/filesystem/__init__.py
--rw-r--r--   0        0        0      778 2023-06-14 04:59:00.374025 codegenpt-0.6.1/codegenpt/filesystem/file_discovery.py
--rw-r--r--   0        0        0        0 2023-06-12 18:24:09.945595 codegenpt-0.6.1/codegenpt/generators/__init__.py
--rw-r--r--   0        0        0     3352 2023-06-15 05:29:28.227327 codegenpt-0.6.1/codegenpt/generators/directory_generator.py
--rw-r--r--   0        0        0     1532 2023-06-14 21:57:11.609802 codegenpt-0.6.1/codegenpt/generators/file_generator.py
--rw-r--r--   0        0        0        0 2023-06-12 18:24:19.273140 codegenpt-0.6.1/codegenpt/llm/__init__.py
--rw-r--r--   0        0        0      707 2023-06-14 06:58:12.077684 codegenpt-0.6.1/codegenpt/llm/llm.py
--rw-r--r--   0        0        0      578 2023-06-15 05:31:26.083236 codegenpt-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     3208 1970-01-01 00:00:00.000000 codegenpt-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-14 02:09:48.042343 codegenpt-0.6.2/LICENSE
+-rw-r--r--   0        0        0     2636 2023-06-15 05:04:45.202904 codegenpt-0.6.2/README.md
+-rw-r--r--   0        0        0        0 2023-06-12 16:35:22.162725 codegenpt-0.6.2/codegenpt/__init__.py
+-rw-r--r--   0        0        0     3584 2023-06-15 05:29:28.226734 codegenpt-0.6.2/codegenpt/cli.py
+-rw-r--r--   0        0        0     2234 2023-06-15 05:33:36.376126 codegenpt-0.6.2/codegenpt/codegenpt_directory.py
+-rw-r--r--   0        0        0      558 2023-06-14 05:25:26.194231 codegenpt-0.6.2/codegenpt/codegenpt_file.py
+-rw-r--r--   0        0        0     1558 2023-06-15 05:29:28.227116 codegenpt-0.6.2/codegenpt/codegenpt_instructions.py
+-rw-r--r--   0        0        0        0 2023-06-13 06:34:45.151317 codegenpt-0.6.2/codegenpt/commands/__init__.py
+-rw-r--r--   0        0        0      248 2023-06-13 06:34:45.151452 codegenpt-0.6.2/codegenpt/commands/command.py
+-rw-r--r--   0        0        0      612 2023-06-14 06:02:51.279908 codegenpt-0.6.2/codegenpt/commands/commands.py
+-rw-r--r--   0        0        0     1672 2023-06-14 06:03:15.242782 codegenpt-0.6.2/codegenpt/commands/include.py
+-rw-r--r--   0        0        0      377 2023-06-15 05:24:10.521616 codegenpt-0.6.2/codegenpt/dependency_batch.py.codegenpt
+-rw-r--r--   0        0        0        0 2023-06-12 16:42:59.544293 codegenpt-0.6.2/codegenpt/filesystem/__init__.py
+-rw-r--r--   0        0        0      778 2023-06-14 04:59:00.374025 codegenpt-0.6.2/codegenpt/filesystem/file_discovery.py
+-rw-r--r--   0        0        0        0 2023-06-12 18:24:09.945595 codegenpt-0.6.2/codegenpt/generators/__init__.py
+-rw-r--r--   0        0        0     3352 2023-06-15 05:29:28.227327 codegenpt-0.6.2/codegenpt/generators/directory_generator.py
+-rw-r--r--   0        0        0     1532 2023-06-14 21:57:11.609802 codegenpt-0.6.2/codegenpt/generators/file_generator.py
+-rw-r--r--   0        0        0        0 2023-06-12 18:24:19.273140 codegenpt-0.6.2/codegenpt/llm/__init__.py
+-rw-r--r--   0        0        0      707 2023-06-14 06:58:12.077684 codegenpt-0.6.2/codegenpt/llm/llm.py
+-rw-r--r--   0        0        0      597 2023-06-15 05:46:16.173971 codegenpt-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0     3249 1970-01-01 00:00:00.000000 codegenpt-0.6.2/PKG-INFO
```

### Comparing `codegenpt-0.6.1/LICENSE` & `codegenpt-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `codegenpt-0.6.1/README.md` & `codegenpt-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `codegenpt-0.6.1/codegenpt/cli.py` & `codegenpt-0.6.2/codegenpt/cli.py`

 * *Files identical despite different names*

### Comparing `codegenpt-0.6.1/codegenpt/codegenpt_directory.py` & `codegenpt-0.6.2/codegenpt/codegenpt_directory.py`

 * *Files identical despite different names*

### Comparing `codegenpt-0.6.1/codegenpt/codegenpt_file.py` & `codegenpt-0.6.2/codegenpt/codegenpt_file.py`

 * *Files identical despite different names*

### Comparing `codegenpt-0.6.1/codegenpt/codegenpt_instructions.py` & `codegenpt-0.6.2/codegenpt/codegenpt_instructions.py`

 * *Files identical despite different names*

### Comparing `codegenpt-0.6.1/codegenpt/commands/commands.py` & `codegenpt-0.6.2/codegenpt/commands/commands.py`

 * *Files identical despite different names*

### Comparing `codegenpt-0.6.1/codegenpt/commands/include.py` & `codegenpt-0.6.2/codegenpt/commands/include.py`

 * *Files identical despite different names*

### Comparing `codegenpt-0.6.1/codegenpt/filesystem/file_discovery.py` & `codegenpt-0.6.2/codegenpt/filesystem/file_discovery.py`

 * *Files identical despite different names*

### Comparing `codegenpt-0.6.1/codegenpt/generators/directory_generator.py` & `codegenpt-0.6.2/codegenpt/generators/directory_generator.py`

 * *Files identical despite different names*

### Comparing `codegenpt-0.6.1/codegenpt/generators/file_generator.py` & `codegenpt-0.6.2/codegenpt/generators/file_generator.py`

 * *Files identical despite different names*

### Comparing `codegenpt-0.6.1/codegenpt/llm/llm.py` & `codegenpt-0.6.2/codegenpt/llm/llm.py`

 * *Files identical despite different names*

### Comparing `codegenpt-0.6.1/pyproject.toml` & `codegenpt-0.6.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "codegenpt"
-version = "0.6.1"
+version = "0.6.2"
 description = "Autogenerate files and folders using ChatGPT API"
 authors = ["Diego Quinteiro <diegoquinteiro@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [project.urls]
 homepage = "https://github.com/diegoquinteiro/codegenpt"
 source = "https://github.com/diegoquinteiro/codegenpt"
 
 [tool.poetry.dependencies]
 python = ">=3.10"
 openai = "^0.27.8"
 pytest = "^7.3.2"
 click = "^8.1.3"
-
+demjson3 = "^3.0.6"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 codegenpt = "codegenpt.cli:cli"
```

### Comparing `codegenpt-0.6.1/PKG-INFO` & `codegenpt-0.6.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: codegenpt
-Version: 0.6.1
+Version: 0.6.2
 Summary: Autogenerate files and folders using ChatGPT API
 License: MIT
 Author: Diego Quinteiro
 Author-email: diegoquinteiro@gmail.com
 Requires-Python: >=3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
+Requires-Dist: demjson3 (>=3.0.6,<4.0.0)
 Requires-Dist: openai (>=0.27.8,<0.28.0)
 Requires-Dist: pytest (>=7.3.2,<8.0.0)
 Description-Content-Type: text/markdown
 
 # CodeGenPT
 ![Version](https://img.shields.io/pypi/v/codegenpt)
 ![Python Version Support](https://img.shields.io/pypi/pyversions/codegenpt)
```

