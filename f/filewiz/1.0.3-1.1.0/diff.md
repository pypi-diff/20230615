# Comparing `tmp/filewiz-1.0.3.tar.gz` & `tmp/filewiz-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "filewiz-1.0.3.tar", last modified: Sat Apr 22 17:32:43 2023, max compression
+gzip compressed data, was "filewiz-1.1.0.tar", last modified: Thu Jun 15 00:21:04 2023, max compression
```

## Comparing `filewiz-1.0.3.tar` & `filewiz-1.1.0.tar`

### file list

```diff
@@ -1,18 +1,21 @@
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-22 17:32:43.618800 filewiz-1.0.3/
--rw-r--r--   0 francispotter   (501) staff       (20)     1873 2023-04-22 17:32:43.618399 filewiz-1.0.3/PKG-INFO
--rw-r--r--   0 francispotter   (501) staff       (20)     1618 2023-04-10 05:40:23.000000 filewiz-1.0.3/README.md
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-22 17:32:43.614318 filewiz-1.0.3/filewiz/
--rw-r--r--   0 francispotter   (501) staff       (20)     1504 2023-04-22 17:30:41.000000 filewiz-1.0.3/filewiz/__init__.py
--rw-r--r--   0 francispotter   (501) staff       (20)       74 2023-04-10 05:20:07.000000 filewiz-1.0.3/filewiz/__main__.py
--rw-r--r--   0 francispotter   (501) staff       (20)      309 2023-04-22 05:29:13.000000 filewiz-1.0.3/filewiz/handler.py
--rw-r--r--   0 francispotter   (501) staff       (20)     1283 2023-04-05 00:32:38.000000 filewiz-1.0.3/filewiz/readline_util.py
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-22 17:32:43.617745 filewiz-1.0.3/filewiz.egg-info/
--rw-r--r--   0 francispotter   (501) staff       (20)     1873 2023-04-22 17:32:43.000000 filewiz-1.0.3/filewiz.egg-info/PKG-INFO
--rw-r--r--   0 francispotter   (501) staff       (20)      304 2023-04-22 17:32:43.000000 filewiz-1.0.3/filewiz.egg-info/SOURCES.txt
--rw-r--r--   0 francispotter   (501) staff       (20)        1 2023-04-22 17:32:43.000000 filewiz-1.0.3/filewiz.egg-info/dependency_links.txt
--rw-r--r--   0 francispotter   (501) staff       (20)       49 2023-04-22 17:32:43.000000 filewiz-1.0.3/filewiz.egg-info/entry_points.txt
--rw-r--r--   0 francispotter   (501) staff       (20)       14 2023-04-22 17:32:43.000000 filewiz-1.0.3/filewiz.egg-info/requires.txt
--rw-r--r--   0 francispotter   (501) staff       (20)        8 2023-04-22 17:32:43.000000 filewiz-1.0.3/filewiz.egg-info/top_level.txt
--rw-r--r--   0 francispotter   (501) staff       (20)      562 2023-04-22 17:30:53.000000 filewiz-1.0.3/pyproject.toml
--rw-r--r--   0 francispotter   (501) staff       (20)       38 2023-04-22 17:32:43.618934 filewiz-1.0.3/setup.cfg
--rw-r--r--   0 francispotter   (501) staff       (20)        5 2023-04-22 17:32:29.000000 filewiz-1.0.3/version
+drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-06-15 00:21:04.097095 filewiz-1.1.0/
+-rw-r--r--   0 francispotter   (501) staff       (20)     1873 2023-06-15 00:21:04.096248 filewiz-1.1.0/PKG-INFO
+-rw-r--r--   0 francispotter   (501) staff       (20)     1618 2023-04-10 05:40:23.000000 filewiz-1.1.0/README.md
+drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-06-15 00:21:03.956085 filewiz-1.1.0/filewiz/
+-rw-r--r--   0 francispotter   (501) staff       (20)        0 2023-06-15 00:15:58.000000 filewiz-1.1.0/filewiz/__init__.py
+-rw-r--r--   0 francispotter   (501) staff       (20)       74 2023-04-10 05:20:07.000000 filewiz-1.1.0/filewiz/__main__.py
+-rw-r--r--   0 francispotter   (501) staff       (20)      935 2023-06-15 00:15:58.000000 filewiz-1.1.0/filewiz/_watchdog.py
+-rw-r--r--   0 francispotter   (501) staff       (20)      725 2023-06-15 00:15:58.000000 filewiz-1.1.0/filewiz/directory_scanner.py
+-rw-r--r--   0 francispotter   (501) staff       (20)     2365 2023-06-15 00:15:58.000000 filewiz-1.1.0/filewiz/file_mover.py
+-rw-r--r--   0 francispotter   (501) staff       (20)      522 2023-06-15 00:15:58.000000 filewiz-1.1.0/filewiz/handler.py
+-rw-r--r--   0 francispotter   (501) staff       (20)     1283 2023-04-05 00:32:38.000000 filewiz-1.1.0/filewiz/readline_util.py
+drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-06-15 00:21:04.095389 filewiz-1.1.0/filewiz.egg-info/
+-rw-r--r--   0 francispotter   (501) staff       (20)     1873 2023-06-15 00:21:03.000000 filewiz-1.1.0/filewiz.egg-info/PKG-INFO
+-rw-r--r--   0 francispotter   (501) staff       (20)      376 2023-06-15 00:21:03.000000 filewiz-1.1.0/filewiz.egg-info/SOURCES.txt
+-rw-r--r--   0 francispotter   (501) staff       (20)        1 2023-06-15 00:21:03.000000 filewiz-1.1.0/filewiz.egg-info/dependency_links.txt
+-rw-r--r--   0 francispotter   (501) staff       (20)       49 2023-06-15 00:21:03.000000 filewiz-1.1.0/filewiz.egg-info/entry_points.txt
+-rw-r--r--   0 francispotter   (501) staff       (20)       14 2023-06-15 00:21:03.000000 filewiz-1.1.0/filewiz.egg-info/requires.txt
+-rw-r--r--   0 francispotter   (501) staff       (20)        8 2023-06-15 00:21:03.000000 filewiz-1.1.0/filewiz.egg-info/top_level.txt
+-rw-r--r--   0 francispotter   (501) staff       (20)      562 2023-04-22 17:30:53.000000 filewiz-1.1.0/pyproject.toml
+-rw-r--r--   0 francispotter   (501) staff       (20)       38 2023-06-15 00:21:04.097300 filewiz-1.1.0/setup.cfg
+-rw-r--r--   0 francispotter   (501) staff       (20)        5 2023-06-15 00:20:15.000000 filewiz-1.1.0/version
```

### Comparing `filewiz-1.0.3/PKG-INFO` & `filewiz-1.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: filewiz
-Version: 1.0.3
+Version: 1.1.0
 Summary: Quickly rename and move new files into structured folders
 Author-email: Francis Potter <filewiz@steampunkwizard.ca>
 License: MIT
 Requires-Python: >=3.6.5
 Description-Content-Type: text/markdown
 
 # FileWiz
```

### Comparing `filewiz-1.0.3/README.md` & `filewiz-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `filewiz-1.0.3/filewiz/__init__.py` & `filewiz-1.1.0/filewiz/file_mover.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,45 +1,63 @@
 from pathlib import Path
 import re
 import sys
+from dataclasses import dataclass
+from subprocess import run
 
 from wizlib.rlinput import rlinput
 
 PATTERN = re.compile(r'\d{8}\-([a-zA-Z0-9-]+)\.(\w+)')
 
-def get_parts(root:Path, sub:str):
-    """Return a set of past filename parts"""
-    parts = set()
-    for year in root.iterdir():
-        if year.name.isdigit():
-            subdir = year / sub
-            if subdir.is_dir():
-                for file in subdir.iterdir():
-                    match = re.match(PATTERN, file.name)
-                    if match:
-                        parts.add(match.groups()[0])
-    return parts
-
-def move_file(source, root_dir:str):
-    """Ask the user some questions then move the file"""
-    root = Path(root_dir).expanduser()
-    sourcepath = Path(source).expanduser()
-    assert sourcepath.is_file()
-    extension = sourcepath.suffix
-    print("Only handling accounts")
-    date = input("Date: ")
-    account = input("Account: ")
-    parts = get_parts(root, account)
-    part = rlinput("Part: ", options=parts)
-    year = date[:4]
-    dirpath = root / year / account
-    if not dirpath.exists():
-        confirm = rlinput(f"Create {dirpath}? ", default="yes")
-        if confirm.startswith('y'):
-            dirpath.mkdir(parents=True)
-    targetpath = dirpath / f"{date}-{part}{extension}"
-    if targetpath.exists():
-        print(f"File exists at {targetpath}")
-    else:
-        confirm = rlinput(f"Move file to {targetpath}? ", default="yes")
-        if confirm.startswith('y'):
-            sourcepath.rename(targetpath)
+class FileMover:
+
+    def __init__(self, target_root):
+        if isinstance(target_root, str):
+            self.target_root_path = Path(target_root).expanduser()
+        elif isinstance(target_root, Path):
+            self.target_root_path = target_root.expanduser()
+        else:
+            raise RuntimeError(f"Invalid target root {target_root}")
+
+    def get_parts(self, sub:str) -> set:
+        """Return a set of past filename parts"""
+        parts = set()
+        for year in self.target_root_path.iterdir():
+            if year.name.isdigit():
+                subdir = year / sub
+                if subdir.is_dir():
+                    for file in subdir.iterdir():
+                        match = re.match(PATTERN, file.name)
+                        if match:
+                            parts.add(match.groups()[0])
+        return parts
+
+    def handle_file(self, source_file_path:Path):
+        print()
+        assert source_file_path.is_file()
+        confirm1 = rlinput(f"Open {source_file_path}? ", default="yes")
+        if confirm1.startswith('y'):
+            run(['open', source_file_path])
+        confirm2 = rlinput(f"Move {source_file_path}? ", default="yes")
+        if confirm2.startswith('y'):
+            self.move_file(source_file_path)
+
+    def move_file(self, source_file_path:Path):
+        """Ask the user some questions then move the file"""
+        extension = source_file_path.suffix
+        date = input("Date: ")
+        account = input("Account: ")
+        parts = self.get_parts(account)
+        part = rlinput("Part: ", options=parts)
+        year = date[:4]
+        dirpath = self.target_root_path / year / account
+        if not dirpath.exists():
+            confirm = rlinput(f"Create {dirpath}? ", default="yes")
+            if confirm.startswith('y'):
+                dirpath.mkdir(parents=True)
+        targetpath = dirpath / f"{date}-{part}{extension}"
+        if targetpath.exists():
+            print(f"File exists at {targetpath}")
+        else:
+            confirm = rlinput(f"Move file to {targetpath}? ", default="yes")
+            if confirm.startswith('y'):
+                source_file_path.rename(targetpath)
```

### Comparing `filewiz-1.0.3/filewiz/readline_util.py` & `filewiz-1.1.0/filewiz/readline_util.py`

 * *Files identical despite different names*

### Comparing `filewiz-1.0.3/filewiz.egg-info/PKG-INFO` & `filewiz-1.1.0/filewiz.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: filewiz
-Version: 1.0.3
+Version: 1.1.0
 Summary: Quickly rename and move new files into structured folders
 Author-email: Francis Potter <filewiz@steampunkwizard.ca>
 License: MIT
 Requires-Python: >=3.6.5
 Description-Content-Type: text/markdown
 
 # FileWiz
```

### Comparing `filewiz-1.0.3/pyproject.toml` & `filewiz-1.1.0/pyproject.toml`

 * *Files identical despite different names*

