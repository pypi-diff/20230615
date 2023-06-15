# Comparing `tmp/conventional-commits-check-1.0.3.tar.gz` & `tmp/conventional-commits-check-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conventional-commits-check-1.0.3.tar", last modified: Tue Mar 28 15:52:56 2023, max compression
+gzip compressed data, was "conventional-commits-check-1.0.4.tar", last modified: Thu Jun 15 11:04:43 2023, max compression
```

## Comparing `conventional-commits-check-1.0.3.tar` & `conventional-commits-check-1.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 aliyaman   (501) staff       (20)        0 2023-03-28 15:52:56.837159 conventional-commits-check-1.0.3/
--rw-r--r--   0 aliyaman   (501) staff       (20)     1066 2023-03-26 21:03:56.000000 conventional-commits-check-1.0.3/LICENSE
--rw-r--r--   0 aliyaman   (501) staff       (20)     4083 2023-03-28 15:52:56.836983 conventional-commits-check-1.0.3/PKG-INFO
--rw-r--r--   0 aliyaman   (501) staff       (20)     2880 2023-03-28 15:52:41.000000 conventional-commits-check-1.0.3/README.md
-drwxr-xr-x   0 aliyaman   (501) staff       (20)        0 2023-03-28 15:52:56.835853 conventional-commits-check-1.0.3/conventional_commits_check/
--rw-r--r--   0 aliyaman   (501) staff       (20)        0 2023-03-27 22:33:22.000000 conventional-commits-check-1.0.3/conventional_commits_check/__init__.py
--rw-r--r--   0 aliyaman   (501) staff       (20)     2151 2023-03-28 15:30:51.000000 conventional-commits-check-1.0.3/conventional_commits_check/main.py
-drwxr-xr-x   0 aliyaman   (501) staff       (20)        0 2023-03-28 15:52:56.836752 conventional-commits-check-1.0.3/conventional_commits_check.egg-info/
--rw-r--r--   0 aliyaman   (501) staff       (20)     4083 2023-03-28 15:52:56.000000 conventional-commits-check-1.0.3/conventional_commits_check.egg-info/PKG-INFO
--rw-r--r--   0 aliyaman   (501) staff       (20)      402 2023-03-28 15:52:56.000000 conventional-commits-check-1.0.3/conventional_commits_check.egg-info/SOURCES.txt
--rw-r--r--   0 aliyaman   (501) staff       (20)        1 2023-03-28 15:52:56.000000 conventional-commits-check-1.0.3/conventional_commits_check.egg-info/dependency_links.txt
--rw-r--r--   0 aliyaman   (501) staff       (20)       84 2023-03-28 15:52:56.000000 conventional-commits-check-1.0.3/conventional_commits_check.egg-info/entry_points.txt
--rw-r--r--   0 aliyaman   (501) staff       (20)       11 2023-03-28 15:52:56.000000 conventional-commits-check-1.0.3/conventional_commits_check.egg-info/requires.txt
--rw-r--r--   0 aliyaman   (501) staff       (20)       27 2023-03-28 15:52:56.000000 conventional-commits-check-1.0.3/conventional_commits_check.egg-info/top_level.txt
--rw-r--r--   0 aliyaman   (501) staff       (20)       38 2023-03-28 15:52:56.837289 conventional-commits-check-1.0.3/setup.cfg
--rw-r--r--   0 aliyaman   (501) staff       (20)     1640 2023-03-28 15:52:49.000000 conventional-commits-check-1.0.3/setup.py
+drwxr-xr-x   0 aliyaman   (501) staff       (20)        0 2023-06-15 11:04:43.724404 conventional-commits-check-1.0.4/
+-rw-r--r--   0 aliyaman   (501) staff       (20)     1066 2023-03-26 21:03:56.000000 conventional-commits-check-1.0.4/LICENSE
+-rw-r--r--   0 aliyaman   (501) staff       (20)     4064 2023-06-15 11:04:43.724263 conventional-commits-check-1.0.4/PKG-INFO
+-rw-r--r--   0 aliyaman   (501) staff       (20)     2880 2023-06-15 11:03:59.000000 conventional-commits-check-1.0.4/README.md
+drwxr-xr-x   0 aliyaman   (501) staff       (20)        0 2023-06-15 11:04:43.723145 conventional-commits-check-1.0.4/conventional_commits_check/
+-rw-r--r--   0 aliyaman   (501) staff       (20)        0 2023-03-27 22:33:22.000000 conventional-commits-check-1.0.4/conventional_commits_check/__init__.py
+-rw-r--r--   0 aliyaman   (501) staff       (20)     2352 2023-06-15 11:01:14.000000 conventional-commits-check-1.0.4/conventional_commits_check/main.py
+drwxr-xr-x   0 aliyaman   (501) staff       (20)        0 2023-06-15 11:04:43.724083 conventional-commits-check-1.0.4/conventional_commits_check.egg-info/
+-rw-r--r--   0 aliyaman   (501) staff       (20)     4064 2023-06-15 11:04:43.000000 conventional-commits-check-1.0.4/conventional_commits_check.egg-info/PKG-INFO
+-rw-r--r--   0 aliyaman   (501) staff       (20)      402 2023-06-15 11:04:43.000000 conventional-commits-check-1.0.4/conventional_commits_check.egg-info/SOURCES.txt
+-rw-r--r--   0 aliyaman   (501) staff       (20)        1 2023-06-15 11:04:43.000000 conventional-commits-check-1.0.4/conventional_commits_check.egg-info/dependency_links.txt
+-rw-r--r--   0 aliyaman   (501) staff       (20)       84 2023-06-15 11:04:43.000000 conventional-commits-check-1.0.4/conventional_commits_check.egg-info/entry_points.txt
+-rw-r--r--   0 aliyaman   (501) staff       (20)       11 2023-06-15 11:04:43.000000 conventional-commits-check-1.0.4/conventional_commits_check.egg-info/requires.txt
+-rw-r--r--   0 aliyaman   (501) staff       (20)       27 2023-06-15 11:04:43.000000 conventional-commits-check-1.0.4/conventional_commits_check.egg-info/top_level.txt
+-rw-r--r--   0 aliyaman   (501) staff       (20)       38 2023-06-15 11:04:43.724447 conventional-commits-check-1.0.4/setup.cfg
+-rw-r--r--   0 aliyaman   (501) staff       (20)     1640 2023-06-15 11:04:08.000000 conventional-commits-check-1.0.4/setup.py
```

### Comparing `conventional-commits-check-1.0.3/LICENSE` & `conventional-commits-check-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `conventional-commits-check-1.0.3/PKG-INFO` & `conventional-commits-check-1.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: conventional-commits-check
-Version: 1.0.3
+Version: 1.0.4
 Summary: A pre-commit hook to check Conventional Commits and add emojis.
 Home-page: https://github.com/AliYmn/conventional-commits-check
 Author: Ali Yaman
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.0
 Classifier: Programming Language :: Python :: 3.1
@@ -129,8 +128,7 @@
 ```bash
 pre-commit autoupdate
 ```
 
 # Usage
 
 Once the hook is added to your project, it will automatically run every time you create a commit. The hook will check the commit messages according to the Conventional Commits rules and add the corresponding emojis. If a commit message does not follow the rules, the commit will be blocked.
-
```

### Comparing `conventional-commits-check-1.0.3/README.md` & `conventional-commits-check-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `conventional-commits-check-1.0.3/conventional_commits_check/main.py` & `conventional-commits-check-1.0.4/conventional_commits_check/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #!/usr/bin/env python3
 import argparse
 import re
 import sys
 from typing import Dict
 import yaml
+import os
 
 COMMIT_TYPES = {
     "feat": "^feat(\(.+\))?:",
     "fix": "^fix(\(.+\))?:",
     "docs": "^docs(\(.+\))?:",
     "style": "^style(\(.+\))?:",
     "refactor": "^refactor(\(.+\))?:",
@@ -27,28 +28,31 @@
     "refactor": "🧹",
     "perf": "🚀",
     "test": "🧪",
     "build": "🏗️",
     "ci": "👷",
     "chore": "♻️",
     "revert": "⏪",
+    "merge": "🔀",
 }
 
 
-def load_custom_rules(config_file="conventional_commits_check_config.yaml"):
+def load_custom_rules(config_file="commits_check_config.yaml"):
+    config_path = os.path.join(os.getcwd(), config_file)
+
     try:
-        with open(config_file, "r") as file:
+        with open(config_path, "r") as file:
             config_data = yaml.safe_load(file)
 
         return config_data.get("additional_commands", {}), config_data.get("additional_emojis", {})
 
     except FileNotFoundError:
-        pass
-
-    return {}, {}
+        print(
+            f"No such file or directory: '{config_path}'. Please make sure the config file is in the correct directory.")
+        sys.exit(1)
 
 
 def main():
     additional_commands, additional_emojis = load_custom_rules()
 
     # Merge additional commands and emojis with the existing ones
     COMMIT_TYPES.update(additional_commands)
```

### Comparing `conventional-commits-check-1.0.3/conventional_commits_check.egg-info/PKG-INFO` & `conventional-commits-check-1.0.4/conventional_commits_check.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: conventional-commits-check
-Version: 1.0.3
+Version: 1.0.4
 Summary: A pre-commit hook to check Conventional Commits and add emojis.
 Home-page: https://github.com/AliYmn/conventional-commits-check
 Author: Ali Yaman
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.0
 Classifier: Programming Language :: Python :: 3.1
@@ -129,8 +128,7 @@
 ```bash
 pre-commit autoupdate
 ```
 
 # Usage
 
 Once the hook is added to your project, it will automatically run every time you create a commit. The hook will check the commit messages according to the Conventional Commits rules and add the corresponding emojis. If a commit message does not follow the rules, the commit will be blocked.
-
```

### Comparing `conventional-commits-check-1.0.3/setup.py` & `conventional-commits-check-1.0.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
         README = f.read()
 else:
     with open('README.md', encoding='utf-8') as f:
         README = f.read()
 
 setup(
     name="conventional-commits-check",
-    version="1.0.3",
+    version="1.0.4",
     description="A pre-commit hook to check Conventional Commits and add emojis.",
     author="Ali Yaman",
     packages=find_packages(),
     license="MIT",
     long_description_content_type="text/markdown",
     long_description=README,
     url="https://github.com/AliYmn/conventional-commits-check",
```

