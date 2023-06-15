# Comparing `tmp/codegenpt-0.6.2.tar.gz` & `tmp/codegenpt-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codegenpt-0.6.2.tar", max compression
+gzip compressed data, was "codegenpt-0.8.0.tar", max compression
```

## Comparing `codegenpt-0.6.2.tar` & `codegenpt-0.8.0.tar`

### file list

```diff
@@ -1,21 +1,23 @@
--rw-r--r--   0        0        0     1071 2023-06-14 02:09:48.042343 codegenpt-0.6.2/LICENSE
--rw-r--r--   0        0        0     2636 2023-06-15 05:04:45.202904 codegenpt-0.6.2/README.md
--rw-r--r--   0        0        0        0 2023-06-12 16:35:22.162725 codegenpt-0.6.2/codegenpt/__init__.py
--rw-r--r--   0        0        0     3584 2023-06-15 05:29:28.226734 codegenpt-0.6.2/codegenpt/cli.py
--rw-r--r--   0        0        0     2234 2023-06-15 05:33:36.376126 codegenpt-0.6.2/codegenpt/codegenpt_directory.py
--rw-r--r--   0        0        0      558 2023-06-14 05:25:26.194231 codegenpt-0.6.2/codegenpt/codegenpt_file.py
--rw-r--r--   0        0        0     1558 2023-06-15 05:29:28.227116 codegenpt-0.6.2/codegenpt/codegenpt_instructions.py
--rw-r--r--   0        0        0        0 2023-06-13 06:34:45.151317 codegenpt-0.6.2/codegenpt/commands/__init__.py
--rw-r--r--   0        0        0      248 2023-06-13 06:34:45.151452 codegenpt-0.6.2/codegenpt/commands/command.py
--rw-r--r--   0        0        0      612 2023-06-14 06:02:51.279908 codegenpt-0.6.2/codegenpt/commands/commands.py
--rw-r--r--   0        0        0     1672 2023-06-14 06:03:15.242782 codegenpt-0.6.2/codegenpt/commands/include.py
--rw-r--r--   0        0        0      377 2023-06-15 05:24:10.521616 codegenpt-0.6.2/codegenpt/dependency_batch.py.codegenpt
--rw-r--r--   0        0        0        0 2023-06-12 16:42:59.544293 codegenpt-0.6.2/codegenpt/filesystem/__init__.py
--rw-r--r--   0        0        0      778 2023-06-14 04:59:00.374025 codegenpt-0.6.2/codegenpt/filesystem/file_discovery.py
--rw-r--r--   0        0        0        0 2023-06-12 18:24:09.945595 codegenpt-0.6.2/codegenpt/generators/__init__.py
--rw-r--r--   0        0        0     3352 2023-06-15 05:29:28.227327 codegenpt-0.6.2/codegenpt/generators/directory_generator.py
--rw-r--r--   0        0        0     1532 2023-06-14 21:57:11.609802 codegenpt-0.6.2/codegenpt/generators/file_generator.py
--rw-r--r--   0        0        0        0 2023-06-12 18:24:19.273140 codegenpt-0.6.2/codegenpt/llm/__init__.py
--rw-r--r--   0        0        0      707 2023-06-14 06:58:12.077684 codegenpt-0.6.2/codegenpt/llm/llm.py
--rw-r--r--   0        0        0      597 2023-06-15 05:46:16.173971 codegenpt-0.6.2/pyproject.toml
--rw-r--r--   0        0        0     3249 1970-01-01 00:00:00.000000 codegenpt-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-14 02:09:48.042343 codegenpt-0.8.0/LICENSE
+-rw-r--r--   0        0        0     2636 2023-06-15 05:04:45.202904 codegenpt-0.8.0/README.md
+-rw-r--r--   0        0        0        0 2023-06-12 16:35:22.162725 codegenpt-0.8.0/codegenpt/__init__.py
+-rw-r--r--   0        0        0     4076 2023-06-15 10:21:14.381398 codegenpt-0.8.0/codegenpt/cli.py
+-rw-r--r--   0        0        0     2020 2023-06-15 07:19:48.367628 codegenpt-0.8.0/codegenpt/codegenpt_directory.py
+-rw-r--r--   0        0        0      558 2023-06-14 05:25:26.194231 codegenpt-0.8.0/codegenpt/codegenpt_file.py
+-rw-r--r--   0        0        0     1938 2023-06-15 09:38:29.001720 codegenpt-0.8.0/codegenpt/codegenpt_instructions.py
+-rw-r--r--   0        0        0        0 2023-06-13 06:34:45.151317 codegenpt-0.8.0/codegenpt/commands/__init__.py
+-rw-r--r--   0        0        0      248 2023-06-13 06:34:45.151452 codegenpt-0.8.0/codegenpt/commands/command.py
+-rw-r--r--   0        0        0      612 2023-06-14 06:02:51.279908 codegenpt-0.8.0/codegenpt/commands/commands.py
+-rw-r--r--   0        0        0     1672 2023-06-14 06:03:15.242782 codegenpt-0.8.0/codegenpt/commands/include.py
+-rw-r--r--   0        0        0     1635 2023-06-15 08:24:12.106287 codegenpt-0.8.0/codegenpt/dependency_batch-old copy.py
+-rw-r--r--   0        0        0     2038 2023-06-15 10:11:53.433347 codegenpt-0.8.0/codegenpt/dependency_batch.py
+-rw-r--r--   0        0        0      876 2023-06-15 08:39:57.106197 codegenpt-0.8.0/codegenpt/dependency_batch.py.codegenpt
+-rw-r--r--   0        0        0        0 2023-06-12 16:42:59.544293 codegenpt-0.8.0/codegenpt/filesystem/__init__.py
+-rw-r--r--   0        0        0      846 2023-06-15 06:23:20.951010 codegenpt-0.8.0/codegenpt/filesystem/file_discovery.py
+-rw-r--r--   0        0        0        0 2023-06-12 18:24:09.945595 codegenpt-0.8.0/codegenpt/generators/__init__.py
+-rw-r--r--   0        0        0     4801 2023-06-15 07:49:05.613004 codegenpt-0.8.0/codegenpt/generators/directory_generator.py
+-rw-r--r--   0        0        0     1532 2023-06-14 21:57:11.609802 codegenpt-0.8.0/codegenpt/generators/file_generator.py
+-rw-r--r--   0        0        0        0 2023-06-12 18:24:19.273140 codegenpt-0.8.0/codegenpt/llm/__init__.py
+-rw-r--r--   0        0        0      707 2023-06-14 06:58:12.077684 codegenpt-0.8.0/codegenpt/llm/llm.py
+-rw-r--r--   0        0        0      597 2023-06-15 10:26:43.469838 codegenpt-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     3249 1970-01-01 00:00:00.000000 codegenpt-0.8.0/PKG-INFO
```

### Comparing `codegenpt-0.6.2/LICENSE` & `codegenpt-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `codegenpt-0.6.2/README.md` & `codegenpt-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `codegenpt-0.6.2/codegenpt/cli.py` & `codegenpt-0.8.0/codegenpt/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import os
 from threading import Thread
 import click
 from codegenpt.codegenpt_directory import CodeGenPTDirectory
 from codegenpt.codegenpt_file import CodeGenPTFile
+from codegenpt.codegenpt_instructions import CodeGenPTInstructions
+from codegenpt.dependency_batch import batch_instructions_by_dependencies
 
 from codegenpt.filesystem.file_discovery import find_codegenpt_directories, find_codegenpt_files
 from codegenpt.generators.directory_generator import generate_directory
 from codegenpt.generators.file_generator import generate_file
 
 
 @click.command()
@@ -18,52 +20,54 @@
 def cli(recursive=False, iterations=3, force=False, path='.'):
     codegenpt(recursive=recursive, iterations=iterations, force=force, path=path)
 
 
 def codegenpt(recursive=True, iterations=1, force=True, path='.'):
     if os.path.isdir(path):
         click.echo(f"🔎 Searching files...")
-        files = find_codegenpt_files(recursive=recursive, path=path)
-        directories = find_codegenpt_directories(
+        instructions = find_codegenpt_files(recursive=recursive, path=path) + find_codegenpt_directories(
             recursive=recursive, path=path)
     else:
-        files = []
-        directories = []
-        if path.endswith('.dir.codegenpt'):
-            directories = [CodeGenPTDirectory(path)]
+        if path.endswith(".dir.codegenpt"):
+            instructions = [CodeGenPTDirectory(path)]
+        elif path.endswith(".codegenpt"):
+            instructions = [CodeGenPTFile(path)]
         else:
-            files = [CodeGenPTFile(path)]
+            raise Exception("Path must be a directory or a .codegenpt file.")
 
-    file_generation_threads = [Thread(target=generate_file_async, args=(file, force)) for file in files]
-    directory_generation_threads = []
-    recursion_threads = []
-    thread_to_directory_mapping = {}
-    for directory in directories:
-        thread = Thread(target=generate_directory_async, args=(directory, force))
-        directory_generation_threads.append(thread)
-        thread_to_directory_mapping[thread.name] = directory
-
-    for thread in file_generation_threads:
-        thread.start()
-    
-    for thread in directory_generation_threads:
-        thread.start()
-
-    for thread in directory_generation_threads:
-        thread.join()
-        if iterations > 1:
-            recursion_thread = Thread(target = codegenpt, kwargs={"recursive": True, "iterations": iterations -1, "force": force, "path": thread_to_directory_mapping[thread.name].fullPath})
-            recursion_thread.start()
-            recursion_threads.append(recursion_thread)
+    batches = batch_instructions_by_dependencies(instructions)
 
-    for thread in file_generation_threads:
-        thread.join()
+    for batch in batches:
+        file_generation_threads = [Thread(target=generate_file_async, args=(file, force)) for file in batch if isinstance(file, CodeGenPTFile)]
+        directory_generation_threads = []
+        recursion_threads = []
+        thread_to_directory_mapping = {}
+        for directory in filter(lambda directory: isinstance(directory, CodeGenPTDirectory), batch):
+            thread = Thread(target=generate_directory_async, args=(directory, force))
+            directory_generation_threads.append(thread)
+            thread_to_directory_mapping[thread.name] = directory
+
+        for thread in file_generation_threads:
+            thread.start()
+        
+        for thread in directory_generation_threads:
+            thread.start()
+
+        for thread in directory_generation_threads:
+            thread.join()
+            if iterations > 1:
+                recursion_thread = Thread(target = codegenpt, kwargs={"recursive": True, "iterations": iterations -1, "force": force, "path": thread_to_directory_mapping[thread.name].fullPath})
+                recursion_thread.start()
+                recursion_threads.append(recursion_thread)
 
-    for thread in recursion_threads:
-        thread.join()
+        for thread in file_generation_threads:
+            thread.join()
+
+        for thread in recursion_threads:
+            thread.join()
 
     click.echo(f"🍻 Success")
 
 
 def generate_file_async(file: CodeGenPTFile, force=True):
     if os.path.exists(file.fullPath) and not force:
         click.echo(
```

### Comparing `codegenpt-0.6.2/codegenpt/codegenpt_directory.py` & `codegenpt-0.8.0/codegenpt/codegenpt_directory.py`

 * *Files 24% similar despite different names*

```diff
@@ -15,37 +15,35 @@
         return {
             'directory_name': self.basename,
             'path': self.path,
         }
 
     def create(self, content):
         if not path.exists(self.fullPath):
-            click.echo(f'📁 created directory: {self.fullPath}')
             os.mkdir(self.fullPath)
         with open(path.join(self.fullPath, '.codegenpt.json'), 'w') as file:
-            click.echo(f'📄 created file: {self.fullPath}.codegenpt.json')
             file.write(encode(content))
         if "children" in content:
-            click.echo(f'🗂️ creating files for: {self.fullPath}')
             
             # Create the include statements for the parent directories
             dir = self
             parent_dir = ''
-            includes = ['@include .codegenpt.json']
+            parent_includes = ['@include .codegenpt.json']
             while dir.parent is not None:
                 parent_dir = path.join('..', parent_dir)
-                includes.append(f'@include {parent_dir}.codegenpt.json')
+                parent_includes.append(f'@include {parent_dir}.codegenpt.json')
                 dir = dir.parent
-            includes = '\n'.join(includes) + '\n'
+            parent_includes = '\n'.join(parent_includes) + '\n'
 
             for children in content["children"]:
+                includes = parent_includes
+                if "dependencies" in children:
+                    includes = includes + '\n'.join([f"@include {dependency}" for dependency in children["dependencies"]]) + '\n'
                 if "filename" in children:
                     with open(path.join(self.fullPath, children["filename"] + ".codegenpt"), 'w+') as file:
-                        click.echo(f'📄 created file: {path.join(self.fullPath, children["filename"] + ".codegenpt")}')
                         file.write(includes + children["prompt"])
 
                 elif "dirname" in children:
                     with open(path.join(self.fullPath, children["dirname"] + ".dir.codegenpt"), 'w+') as file:
-                        click.echo(f'📄 created file: {path.join(self.fullPath, children["dirname"] + ".dir.codegenpt")}')
                         file.write(includes + children["prompt"])
                         if "children" in children:
                             CodeGenPTDirectory(self.fullPath + os.sep + children["dirname"], parent=self).create(children)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `codegenpt-0.6.2/codegenpt/codegenpt_file.py` & `codegenpt-0.8.0/codegenpt/codegenpt_file.py`

 * *Files identical despite different names*

### Comparing `codegenpt-0.6.2/codegenpt/codegenpt_instructions.py` & `codegenpt-0.8.0/codegenpt/codegenpt_instructions.py`

 * *Files 24% similar despite different names*

```diff
@@ -11,23 +11,24 @@
         return '.codegenpt'
 
     @property
     def basename(self):
         return path.basename(self.fullPath)
       
     @property
+    # The full path of the instructions file, without the suffix
     def fullPath(self):
         return self.instructions_filename.replace(self.suffix, '')
 
     @property
     def prompt(self):
         with open(self.instructions_filename, 'r') as file:
             prompt_lines = list(filter(lambda line: not line.startswith('@'), file.readlines()))
             # Filter first lines if they are empty or whitespace
-            while prompt_lines[0].strip() == '':
+            while prompt_lines and prompt_lines[0].strip() == '':
                 prompt_lines.pop(0)
 
         return ''.join(prompt_lines)
 
     @property
     def commands(self):
         with open(self.instructions_filename, 'r') as file:
@@ -35,14 +36,25 @@
                 lambda line: Command(
                     name = line.strip().split(' ')[0].replace('@', ''),
                     arguments = shlex.split(line.strip())[1:]
                 ),
                 list(filter(lambda line: line.startswith('@'), file.readlines()))
             ))
         return commands
+    
+    @property
+    def dependencies(self):
+        dependencies = list(map(
+            lambda command: command.arguments[0],
+            list(filter(
+                lambda command: command.name == 'include',
+                self.commands
+            ))
+        ))
+        return dependencies
         
     @property
     def path(self):
         return self.instructions_filename.split(os.sep)[:-1]
         
     @property
     @abstractmethod
```

### Comparing `codegenpt-0.6.2/codegenpt/commands/commands.py` & `codegenpt-0.8.0/codegenpt/commands/commands.py`

 * *Files identical despite different names*

### Comparing `codegenpt-0.6.2/codegenpt/commands/include.py` & `codegenpt-0.8.0/codegenpt/commands/include.py`

 * *Files identical despite different names*

### Comparing `codegenpt-0.6.2/codegenpt/filesystem/file_discovery.py` & `codegenpt-0.8.0/codegenpt/filesystem/file_discovery.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 
 # Find all codegenpt files in the given root directory
 def find_codegenpt_files(path='', recursive=True):
     return list(map(
         lambda filename: CodeGenPTFile(filename),
         filter(
             lambda filename: not filename.endswith('.dir.codegenpt'),
-            glob.glob(os.path.join(path, '**/*.codegenpt'), recursive=recursive)
+            glob.glob(os.path.join(path, '**/*.codegenpt' if recursive else '*.codegenpt'), recursive=recursive)
         )
     ))
 
 # Find all codegenpt directories in the given root directory
 def find_codegenpt_directories(path='', recursive=True):
     return list(map(
         lambda dirname: CodeGenPTDirectory(dirname),
-        glob.glob(os.path.join(path, '**/*.dir.codegenpt'), recursive=recursive)
+        glob.glob(os.path.join(path, '**/*.dir.codegenpt' if recursive else '*.dir.codegenpt'), recursive=recursive)
     ))
```

### Comparing `codegenpt-0.6.2/codegenpt/generators/file_generator.py` & `codegenpt-0.8.0/codegenpt/generators/file_generator.py`

 * *Files identical despite different names*

### Comparing `codegenpt-0.6.2/codegenpt/llm/llm.py` & `codegenpt-0.8.0/codegenpt/llm/llm.py`

 * *Files identical despite different names*

### Comparing `codegenpt-0.6.2/pyproject.toml` & `codegenpt-0.8.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "codegenpt"
-version = "0.6.2"
+version = "0.8.0"
 description = "Autogenerate files and folders using ChatGPT API"
 authors = ["Diego Quinteiro <diegoquinteiro@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [project.urls]
 homepage = "https://github.com/diegoquinteiro/codegenpt"
```

### Comparing `codegenpt-0.6.2/PKG-INFO` & `codegenpt-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codegenpt
-Version: 0.6.2
+Version: 0.8.0
 Summary: Autogenerate files and folders using ChatGPT API
 License: MIT
 Author: Diego Quinteiro
 Author-email: diegoquinteiro@gmail.com
 Requires-Python: >=3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

