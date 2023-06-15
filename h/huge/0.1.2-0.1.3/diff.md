# Comparing `tmp/huge-0.1.2.tar.gz` & `tmp/huge-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huge-0.1.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "huge-0.1.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `huge-0.1.2.tar` & `huge-0.1.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      775 2023-06-13 18:44:24.521849 huge-0.1.2/.github/workflows/package.yml
--rw-r--r--   0        0        0       13 2023-06-13 18:44:24.521849 huge-0.1.2/.gitignore
--rw-r--r--   0        0        0     1069 2023-06-13 18:44:24.521849 huge-0.1.2/LICENSE
--rw-r--r--   0        0        0     3334 2023-06-13 18:44:24.521849 huge-0.1.2/README.md
--rw-r--r--   0        0        0     2008 2023-06-13 18:44:24.521849 huge-0.1.2/huge.py
--rw-r--r--   0        0        0      434 2023-06-13 18:44:24.521849 huge-0.1.2/pyproject.toml
--rw-r--r--   0        0        0       11 2023-06-13 18:44:24.521849 huge-0.1.2/requirements.txt
--rw-r--r--   0        0        0     3708 1970-01-01 00:00:00.000000 huge-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      775 2023-06-15 12:43:44.765052 huge-0.1.3/.github/workflows/package.yml
+-rw-r--r--   0        0        0       13 2023-06-15 12:43:44.765052 huge-0.1.3/.gitignore
+-rw-r--r--   0        0        0     1069 2023-06-15 12:43:44.765052 huge-0.1.3/LICENSE
+-rw-r--r--   0        0        0     3418 2023-06-15 12:43:44.765052 huge-0.1.3/README.md
+-rw-r--r--   0        0        0     2462 2023-06-15 12:43:44.765052 huge-0.1.3/huge.py
+-rw-r--r--   0        0        0      434 2023-06-15 12:43:44.765052 huge-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0       11 2023-06-15 12:43:44.765052 huge-0.1.3/requirements.txt
+-rw-r--r--   0        0        0     3792 1970-01-01 00:00:00.000000 huge-0.1.3/PKG-INFO
```

### Comparing `huge-0.1.2/.github/workflows/package.yml` & `huge-0.1.3/.github/workflows/package.yml`

 * *Files identical despite different names*

### Comparing `huge-0.1.2/LICENSE` & `huge-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `huge-0.1.2/README.md` & `huge-0.1.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -12,25 +12,25 @@
 ```
 $ pip install huge
 ```
 
 
 ### Command line options
 
-```
+```console
 $ huge --help
 
 Usage: huge [OPTIONS]
 
 Options:
-  --branch TEXT          Which branch to scan.  [default: main]
+  --branch TEXT          Which branch to scan. By default it will scan the
+                         currently active branch.  [default: HEAD]
   --num-entries INTEGER  How many top entries to show.  [default: 20]
   --cutoff INTEGER       Cutoff (bytes) below which to ignore entries.
                          [default: 1000000]
-
   --help                 Show this message and exit.
 ```
 
 
 ### Example output
 
 ```
```

### Comparing `huge-0.1.2/huge.py` & `huge-0.1.3/huge.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,29 @@
 """Find huge additions in Git history."""
 
-__version__ = "0.1.2"
+__version__ = "0.1.3"
 
 
 import subprocess
+import sys
 import itertools
 from tqdm import tqdm
 import click
 from tabulate import tabulate
 
 
+def branch_exists(branch) -> bool:
+    """Check if a branch exists."""
+    try:
+        subprocess.check_output(f"git rev-parse --quiet --verify {branch}", shell=True)
+        return True
+    except subprocess.CalledProcessError:
+        return False
+
+
 def get_all_commits_on_branch(branch):
     return (
         subprocess.check_output(f"git rev-list {branch}", shell=True)
         .decode("utf8")
         .splitlines()
     )
 
@@ -24,15 +34,18 @@
         .decode("utf8")
         .splitlines()
     )
 
 
 @click.command()
 @click.option(
-    "--branch", default="main", show_default=True, help="Which branch to scan."
+    "--branch",
+    default="HEAD",
+    show_default=True,
+    help="Which branch to scan. By default it will scan the currently active branch.",
 )
 @click.option(
     "--num-entries",
     default=20,
     type=int,
     show_default=True,
     help="How many top entries to show.",
@@ -41,14 +54,18 @@
     "--cutoff",
     default=1000000,
     type=int,
     show_default=True,
     help="Cutoff (bytes) below which to ignore entries.",
 )
 def main(branch, num_entries, cutoff):
+    if not branch_exists(branch):
+        sys.stderr.write(f"ERROR: branch {branch} does not exist\n")
+        sys.exit(1)
+
     commits = get_all_commits_on_branch(branch)
 
     print("scanning the history ...")
     additions_dict = {}
     for commit in tqdm(commits):
         entries = get_file_entries(commit)
         for line in entries:
```

### Comparing `huge-0.1.2/PKG-INFO` & `huge-0.1.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: huge
-Version: 0.1.2
+Version: 0.1.3
 Summary: Find huge additions in Git history.
 Home-page: https://github.com/bast/huge
 Author: Radovan Bast
 Author-email: radovan.bast@uit.no
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: tqdm>=4.65,<5
@@ -25,25 +25,25 @@
 ```
 $ pip install huge
 ```
 
 
 ### Command line options
 
-```
+```console
 $ huge --help
 
 Usage: huge [OPTIONS]
 
 Options:
-  --branch TEXT          Which branch to scan.  [default: main]
+  --branch TEXT          Which branch to scan. By default it will scan the
+                         currently active branch.  [default: HEAD]
   --num-entries INTEGER  How many top entries to show.  [default: 20]
   --cutoff INTEGER       Cutoff (bytes) below which to ignore entries.
                          [default: 1000000]
-
   --help                 Show this message and exit.
 ```
 
 
 ### Example output
 
 ```
```

