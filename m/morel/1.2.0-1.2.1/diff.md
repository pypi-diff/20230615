# Comparing `tmp/morel-1.2.0.tar.gz` & `tmp/morel-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "morel-1.2.0.tar", last modified: Tue Jun 13 10:10:30 2023, max compression
+gzip compressed data, was "morel-1.2.1.tar", last modified: Thu Jun 15 20:49:04 2023, max compression
```

## Comparing `morel-1.2.0.tar` & `morel-1.2.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 basilef   (1000) basilef   (1000)        0 2023-06-13 10:10:30.103531 morel-1.2.0/
--rw-r--r--   0 basilef   (1000) basilef   (1000)    35148 2023-06-11 10:50:26.000000 morel-1.2.0/LICENSE
--rw-r--r--   0 basilef   (1000) basilef   (1000)      695 2023-06-13 10:10:30.102531 morel-1.2.0/PKG-INFO
--rw-r--r--   0 basilef   (1000) basilef   (1000)      101 2023-06-11 11:30:40.000000 morel-1.2.0/README.md
--rw-r--r--   0 basilef   (1000) basilef   (1000)      794 2023-06-13 10:10:14.000000 morel-1.2.0/pyproject.toml
--rw-r--r--   0 basilef   (1000) basilef   (1000)       38 2023-06-13 10:10:30.103531 morel-1.2.0/setup.cfg
-drwxr-xr-x   0 basilef   (1000) basilef   (1000)        0 2023-06-13 10:10:30.099531 morel-1.2.0/src/
-drwxr-xr-x   0 basilef   (1000) basilef   (1000)        0 2023-06-13 10:10:30.101531 morel-1.2.0/src/morel/
--rw-r--r--   0 basilef   (1000) basilef   (1000)       76 2023-06-13 07:59:42.000000 morel-1.2.0/src/morel/__init__.py
--rw-r--r--   0 basilef   (1000) basilef   (1000)     2951 2023-06-13 08:20:52.000000 morel-1.2.0/src/morel/app.py
--rw-r--r--   0 basilef   (1000) basilef   (1000)      693 2023-06-13 08:50:20.000000 morel-1.2.0/src/morel/exploit_template.py
--rw-r--r--   0 basilef   (1000) basilef   (1000)     1013 2023-06-11 14:52:10.000000 morel-1.2.0/src/morel/exploits.py
--rw-r--r--   0 basilef   (1000) basilef   (1000)      406 2023-06-11 14:53:08.000000 morel-1.2.0/src/morel/logger.py
--rw-r--r--   0 basilef   (1000) basilef   (1000)     1525 2023-05-24 09:29:29.000000 morel-1.2.0/src/morel/singleton.py
--rw-r--r--   0 basilef   (1000) basilef   (1000)     2551 2023-06-13 09:59:19.000000 morel-1.2.0/src/morel/target.py
--rw-r--r--   0 basilef   (1000) basilef   (1000)      304 2023-06-13 08:11:32.000000 morel-1.2.0/src/morel/target_template.py
-drwxr-xr-x   0 basilef   (1000) basilef   (1000)        0 2023-06-13 10:10:30.102531 morel-1.2.0/src/morel.egg-info/
--rw-r--r--   0 basilef   (1000) basilef   (1000)      695 2023-06-13 10:10:30.000000 morel-1.2.0/src/morel.egg-info/PKG-INFO
--rw-r--r--   0 basilef   (1000) basilef   (1000)      415 2023-06-13 10:10:30.000000 morel-1.2.0/src/morel.egg-info/SOURCES.txt
--rw-r--r--   0 basilef   (1000) basilef   (1000)        1 2023-06-13 10:10:30.000000 morel-1.2.0/src/morel.egg-info/dependency_links.txt
--rw-r--r--   0 basilef   (1000) basilef   (1000)       36 2023-06-13 10:10:30.000000 morel-1.2.0/src/morel.egg-info/entry_points.txt
--rw-r--r--   0 basilef   (1000) basilef   (1000)       13 2023-06-13 10:10:30.000000 morel-1.2.0/src/morel.egg-info/requires.txt
--rw-r--r--   0 basilef   (1000) basilef   (1000)        6 2023-06-13 10:10:30.000000 morel-1.2.0/src/morel.egg-info/top_level.txt
+drwxr-xr-x   0 basilef   (1000) basilef   (1000)        0 2023-06-15 20:49:04.140593 morel-1.2.1/
+-rw-r--r--   0 basilef   (1000) basilef   (1000)    35148 2023-06-11 10:50:26.000000 morel-1.2.1/LICENSE
+-rw-r--r--   0 basilef   (1000) basilef   (1000)      695 2023-06-15 20:49:04.139593 morel-1.2.1/PKG-INFO
+-rw-r--r--   0 basilef   (1000) basilef   (1000)      101 2023-06-11 11:30:40.000000 morel-1.2.1/README.md
+-rw-r--r--   0 basilef   (1000) basilef   (1000)      794 2023-06-15 20:48:27.000000 morel-1.2.1/pyproject.toml
+-rw-r--r--   0 basilef   (1000) basilef   (1000)       38 2023-06-15 20:49:04.140593 morel-1.2.1/setup.cfg
+drwxr-xr-x   0 basilef   (1000) basilef   (1000)        0 2023-06-15 20:49:04.137593 morel-1.2.1/src/
+drwxr-xr-x   0 basilef   (1000) basilef   (1000)        0 2023-06-15 20:49:04.138593 morel-1.2.1/src/morel/
+-rw-r--r--   0 basilef   (1000) basilef   (1000)       76 2023-06-13 07:59:42.000000 morel-1.2.1/src/morel/__init__.py
+-rw-r--r--   0 basilef   (1000) basilef   (1000)     3725 2023-06-13 10:51:58.000000 morel-1.2.1/src/morel/app.py
+-rw-r--r--   0 basilef   (1000) basilef   (1000)      693 2023-06-13 08:50:20.000000 morel-1.2.1/src/morel/exploit_template.py
+-rw-r--r--   0 basilef   (1000) basilef   (1000)     1057 2023-06-15 13:11:55.000000 morel-1.2.1/src/morel/exploits.py
+-rw-r--r--   0 basilef   (1000) basilef   (1000)      406 2023-06-11 14:53:08.000000 morel-1.2.1/src/morel/logger.py
+-rw-r--r--   0 basilef   (1000) basilef   (1000)     1525 2023-05-24 09:29:29.000000 morel-1.2.1/src/morel/singleton.py
+-rw-r--r--   0 basilef   (1000) basilef   (1000)     2750 2023-06-15 20:36:09.000000 morel-1.2.1/src/morel/target.py
+-rw-r--r--   0 basilef   (1000) basilef   (1000)      304 2023-06-13 08:11:32.000000 morel-1.2.1/src/morel/target_template.py
+drwxr-xr-x   0 basilef   (1000) basilef   (1000)        0 2023-06-15 20:49:04.139593 morel-1.2.1/src/morel.egg-info/
+-rw-r--r--   0 basilef   (1000) basilef   (1000)      695 2023-06-15 20:49:04.000000 morel-1.2.1/src/morel.egg-info/PKG-INFO
+-rw-r--r--   0 basilef   (1000) basilef   (1000)      415 2023-06-15 20:49:04.000000 morel-1.2.1/src/morel.egg-info/SOURCES.txt
+-rw-r--r--   0 basilef   (1000) basilef   (1000)        1 2023-06-15 20:49:04.000000 morel-1.2.1/src/morel.egg-info/dependency_links.txt
+-rw-r--r--   0 basilef   (1000) basilef   (1000)       36 2023-06-15 20:49:04.000000 morel-1.2.1/src/morel.egg-info/entry_points.txt
+-rw-r--r--   0 basilef   (1000) basilef   (1000)       13 2023-06-15 20:49:04.000000 morel-1.2.1/src/morel.egg-info/requires.txt
+-rw-r--r--   0 basilef   (1000) basilef   (1000)        6 2023-06-15 20:49:04.000000 morel-1.2.1/src/morel.egg-info/top_level.txt
```

### Comparing `morel-1.2.0/LICENSE` & `morel-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `morel-1.2.0/PKG-INFO` & `morel-1.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morel
-Version: 1.2.0
+Version: 1.2.1
 Summary: morel helps you write and test your A/D exploits, built with Milkman compatibility in mind
 Author-email: Francesco Basile <basile1fr@gmail.com>
 Project-URL: Homepage, https://github.com/parmigggiana/morel
 Project-URL: Bug Tracker, https://github.com/parmigggiana/morel/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `morel-1.2.0/pyproject.toml` & `morel-1.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "morel"
-version = "1.2.0"
+version = "1.2.1"
 authors = [
   { name="Francesco Basile", email="basile1fr@gmail.com" },
 ]
 description = "morel helps you write and test your A/D exploits, built with Milkman compatibility in mind"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `morel-1.2.0/src/morel/app.py` & `morel-1.2.1/src/morel/app.py`

 * *Files 20% similar despite different names*

```diff
@@ -93,7 +93,34 @@
             exploitfun,
             target,
         ),
         name=f"{exploitfun.__module__}_{target}",
     )
     t.start()
     t.join()
+
+
+@app.command()
+@click.argument("shell", type=click.Choice(["bash", "zsh", "fish"]))
+def complete(shell):
+    match shell:
+        case "fish":
+            cmdstring = "_MOREL_COMPLETE=fish_source morel > ~/.config/fish/completions/morel.fish"
+
+        case "bash":
+            cmdstring = (
+                r"echo eval \"\$\(_MOREL_COMPLETE=bash_source morel\)\" >> ~/.bashrc"
+            )
+
+        case "zsh":
+            cmdstring = (
+                r"echo eval \"\$\(_MOREL_COMPLETE=zsh_source morel\)\" >> ~/.zshrc"
+            )
+
+        case _:
+            click.echo("Error! How did you input this?")
+    try:
+        confirm = click.confirm(f"Executing `{cmdstring}`")
+    except click.Abort:
+        confirm = False
+    if confirm:
+        os.system(cmdstring)
```

### Comparing `morel-1.2.0/src/morel/exploit_template.py` & `morel-1.2.1/src/morel/exploit_template.py`

 * *Files identical despite different names*

### Comparing `morel-1.2.0/src/morel/exploits.py` & `morel-1.2.1/src/morel/exploits.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,30 +6,31 @@
 
 
 def launchAttack(exploit, target_ip: str):
     start = time.time()
     flags_iterable = exploit(target_ip)
     if isinstance(flags_iterable, str):
         flags_iterable: list[str] = [flags_iterable]
-    for flag in flags_iterable:
-        find_flags(flag)
+    # for flag in flags_iterable:
+    find_flags(flags_iterable)
 
     elapsed = time.time() - start
 
     logger.info(f"{exploit.__module__} took {elapsed:.2f} seconds")
     return
 
 
 def find_flags(flags: list[str]):
     valid_flags = []
 
     if isinstance(flags, str):
         flags = [
             flags,
         ]
+    print(os.environ["FLAG_REGEX"])
     if os.environ["FLAG_REGEX"] != "None":
         for flag in flags:
             m = re.finditer(pattern=os.environ["FLAG_REGEX"], string=flag)
             if m:
                 for f in m:
                     valid_flags.append(f.group())
```

### Comparing `morel-1.2.0/src/morel/singleton.py` & `morel-1.2.1/src/morel/singleton.py`

 * *Files identical despite different names*

### Comparing `morel-1.2.0/src/morel/target.py` & `morel-1.2.1/src/morel/target.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,16 +3,14 @@
 from multiprocessing import Lock
 import sys
 
 from pathlib import Path
 from typing import Iterable
 from morel.singleton import SingletonMeta
 
-p = Path("/home/basilef/Documents/Repos/morel/tests/targets")
-
 
 class _restrictedDict(dict):
     def __init__(self):
         return super().__init__()
 
     def __init__(self, initialD):
         return super().__init__(initialD)
@@ -41,36 +39,48 @@
             if k not in self:
                 self[k] = v
                 continue
 
             if isinstance(self[k], dict) and not isinstance(self[k], _restrictedDict):
                 self[k] = _restrictedDict(self[k])
 
+            if isinstance(self[k], list):
+                self[k] = set(self[k])
+
+            if not isinstance(self[k], Iterable):
+                self[k] = {
+                    self[k],
+                }
+
             if isinstance(self[k], _restrictedDict):
                 self[k].append(dict2[k])
 
-            elif isinstance(self[k], list):
-                tmp = self[k]
-                tmp.append(v)
-                self[k] = tmp
+            elif isinstance(self[k], set):
+                self[k] |= {
+                    v,
+                }
 
             # print(self)
 
 
-class _Target(_restrictedDict, metaclass=SingletonMeta):
+class Targets(_restrictedDict, metaclass=SingletonMeta):
     def __init__(self):
         self._lock = Lock()
-        self.populate()
+        self.p = Path(".")
+        self.update()
+
+    def setBaseDir(self, dir):
+        self.p = Path(dir)
 
     def add_targets(self, targets):
         with self._lock:
             self.append(targets)
 
-    def populate(self):
-        files = p.glob("**/*.py")
+    def update(self):
+        files = list(self.p.glob("**/[!_]*.py"))
         targets_functions = []
 
         for targ in files:
             name = targ.stem
 
             try:
                 spec = importlib.util.spec_from_file_location(name, targ.resolve())
@@ -83,12 +93,9 @@
                 print(e)
 
         # print(targets_functions)
         for function in targets_functions:
             self.add_targets(function())
 
 
-Targets = _Target()
-
-
 if __name__ == "__main__":
     json.dump(Targets, sys.stdout, indent=2)
```

### Comparing `morel-1.2.0/src/morel.egg-info/PKG-INFO` & `morel-1.2.1/src/morel.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morel
-Version: 1.2.0
+Version: 1.2.1
 Summary: morel helps you write and test your A/D exploits, built with Milkman compatibility in mind
 Author-email: Francesco Basile <basile1fr@gmail.com>
 Project-URL: Homepage, https://github.com/parmigggiana/morel
 Project-URL: Bug Tracker, https://github.com/parmigggiana/morel/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

