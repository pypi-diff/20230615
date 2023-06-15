# Comparing `tmp/git_timemachine-1.3.0.tar.gz` & `tmp/git_timemachine-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git_timemachine-1.3.0.tar", max compression
+gzip compressed data, was "git_timemachine-1.3.1.tar", max compression
```

## Comparing `git_timemachine-1.3.0.tar` & `git_timemachine-1.3.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rwxr-xr-x   0        0        0    35147 2023-05-02 06:28:21.000000 git_timemachine-1.3.0/LICENSE
--rwxr-xr-x   0        0        0      408 2023-06-02 10:58:19.377074 git_timemachine-1.3.0/README.md
--rw-r--r--   0        0        0     1024 2023-06-02 17:06:24.277346 git_timemachine-1.3.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-02 02:05:43.427329 git_timemachine-1.3.0/src/git_timemachine/__init__.py
--rw-r--r--   0        0        0      747 2023-06-02 10:46:36.247096 git_timemachine-1.3.0/src/git_timemachine/__main__.py
--rw-r--r--   0        0        0      231 2023-06-02 16:41:44.873985 git_timemachine-1.3.0/src/git_timemachine/commands/__init__.py
--rw-r--r--   0        0        0     3273 2023-06-02 17:05:53.787345 git_timemachine-1.3.0/src/git_timemachine/commands/commit.py
--rw-r--r--   0        0        0     1176 2023-06-02 02:23:15.307335 git_timemachine-1.3.0/src/git_timemachine/commands/log.py
--rwxr-xr-x   0        0        0     2832 2023-06-02 16:43:00.203987 git_timemachine-1.3.0/src/git_timemachine/commands/migrate.py
--rw-r--r--   0        0        0      641 2023-06-02 16:31:24.703974 git_timemachine-1.3.0/src/git_timemachine/commands/switch_date.py
--rw-r--r--   0        0        0     1125 2023-06-02 10:31:13.707125 git_timemachine-1.3.0/src/git_timemachine/state.py
--rw-r--r--   0        0        0      951 2023-06-02 17:02:12.764008 git_timemachine-1.3.0/src/git_timemachine/utils.py
--rw-r--r--   0        0        0     1209 1970-01-01 00:00:00.000000 git_timemachine-1.3.0/PKG-INFO
+-rwxr-xr-x   0        0        0    35147 2023-06-15 17:39:29.797642 git_timemachine-1.3.1/LICENSE
+-rwxr-xr-x   0        0        0      408 2023-06-15 17:39:29.798637 git_timemachine-1.3.1/README.md
+-rwxr-xr-x   0        0        0     1024 2023-06-15 17:39:29.800604 git_timemachine-1.3.1/pyproject.toml
+-rwxr-xr-x   0        0        0       87 2023-06-15 17:39:29.801629 git_timemachine-1.3.1/src/git_timemachine/__init__.py
+-rwxr-xr-x   0        0        0     1033 2023-06-15 17:39:29.801629 git_timemachine-1.3.1/src/git_timemachine/__main__.py
+-rwxr-xr-x   0        0        0      231 2023-06-15 17:39:29.802626 git_timemachine-1.3.1/src/git_timemachine/commands/__init__.py
+-rwxr-xr-x   0        0        0     3273 2023-06-15 17:39:29.803627 git_timemachine-1.3.1/src/git_timemachine/commands/commit.py
+-rwxr-xr-x   0        0        0     1176 2023-06-15 17:39:29.803627 git_timemachine-1.3.1/src/git_timemachine/commands/log.py
+-rwxr-xr-x   0        0        0     2832 2023-06-15 17:39:29.804621 git_timemachine-1.3.1/src/git_timemachine/commands/migrate.py
+-rwxr-xr-x   0        0        0      641 2023-06-15 17:39:29.804621 git_timemachine-1.3.1/src/git_timemachine/commands/switch_date.py
+-rwxr-xr-x   0        0        0     1125 2023-06-15 17:39:29.805591 git_timemachine-1.3.1/src/git_timemachine/state.py
+-rwxr-xr-x   0        0        0      951 2023-06-15 17:39:29.805591 git_timemachine-1.3.1/src/git_timemachine/utils.py
+-rw-r--r--   0        0        0     1209 1970-01-01 00:00:00.000000 git_timemachine-1.3.1/PKG-INFO
```

### Comparing `git_timemachine-1.3.0/LICENSE` & `git_timemachine-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `git_timemachine-1.3.0/pyproject.toml` & `git_timemachine-1.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "git-timemachine"
-version = "1.3.0"
+version = "1.3.1"
 description = "A command-line tool that helps you record commits on Git repositories at any time node."
 authors = ["HE Yaowen <he.yaowen@hotmail.com>"]
 license = "GPL-3.0"
 readme = "README.md"
 homepage = "https://github.com/he-yaowen/git-timemachine"
 packages = [{include = "git_timemachine", from = "src"}]
```

### Comparing `git_timemachine-1.3.0/src/git_timemachine/__main__.py` & `git_timemachine-1.3.1/src/git_timemachine/__main__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,18 +1,26 @@
 from os import PathLike
 from pathlib import Path
 
 import click
 
+from git_timemachine import __version__
 from git_timemachine.commands import command_group
 from git_timemachine.state import StateFile
 
 
+def print_version(ctx: click.Context, _, value: str):
+    if not value or ctx.resilient_parsing:
+        return
+    click.echo(__version__)
+    ctx.exit()
+
+
 @click.group(commands=command_group)
-@click.version_option(message='%(version)s')
+@click.option('--version', help='Show version information.', is_flag=True, callback=print_version, expose_value=False, is_eager=True)
 @click.option('--state-file', help='Path of state file.', type=click.Path(dir_okay=False, exists=False), is_eager=True, default=Path.home().joinpath('.git-timemachine.state'))
 @click.pass_context
 def cli(ctx: click.Context, state_file: PathLike):
     """A command-line tool that helps you record commits on Git repositories at any time node."""
 
     ctx.ensure_object(dict)
     ctx.obj['states'] = StateFile(state_file)
```

### Comparing `git_timemachine-1.3.0/src/git_timemachine/commands/commit.py` & `git_timemachine-1.3.1/src/git_timemachine/commands/commit.py`

 * *Files identical despite different names*

### Comparing `git_timemachine-1.3.0/src/git_timemachine/commands/log.py` & `git_timemachine-1.3.1/src/git_timemachine/commands/log.py`

 * *Files identical despite different names*

### Comparing `git_timemachine-1.3.0/src/git_timemachine/commands/migrate.py` & `git_timemachine-1.3.1/src/git_timemachine/commands/migrate.py`

 * *Files identical despite different names*

### Comparing `git_timemachine-1.3.0/src/git_timemachine/commands/switch_date.py` & `git_timemachine-1.3.1/src/git_timemachine/commands/switch_date.py`

 * *Files identical despite different names*

### Comparing `git_timemachine-1.3.0/src/git_timemachine/state.py` & `git_timemachine-1.3.1/src/git_timemachine/state.py`

 * *Files identical despite different names*

### Comparing `git_timemachine-1.3.0/src/git_timemachine/utils.py` & `git_timemachine-1.3.1/src/git_timemachine/utils.py`

 * *Files identical despite different names*

### Comparing `git_timemachine-1.3.0/PKG-INFO` & `git_timemachine-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git-timemachine
-Version: 1.3.0
+Version: 1.3.1
 Summary: A command-line tool that helps you record commits on Git repositories at any time node.
 Home-page: https://github.com/he-yaowen/git-timemachine
 License: GPL-3.0
 Author: HE Yaowen
 Author-email: he.yaowen@hotmail.com
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

