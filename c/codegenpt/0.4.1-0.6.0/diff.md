# Comparing `tmp/codegenpt-0.4.1.tar.gz` & `tmp/codegenpt-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codegenpt-0.4.1.tar", max compression
+gzip compressed data, was "codegenpt-0.6.0.tar", max compression
```

## Comparing `codegenpt-0.4.1.tar` & `codegenpt-0.6.0.tar`

### file list

```diff
@@ -1,17 +1,20 @@
--rw-r--r--   0        0        0     1071 2023-06-14 02:09:48.042343 codegenpt-0.4.1/LICENSE
--rw-r--r--   0        0        0     2323 2023-06-14 02:09:48.042507 codegenpt-0.4.1/README.md
--rw-r--r--   0        0        0        0 2023-06-12 16:35:22.162725 codegenpt-0.4.1/codegenpt/__init__.py
--rw-r--r--   0        0        0     1577 2023-06-14 03:48:47.790152 codegenpt-0.4.1/codegenpt/cli.py
--rw-r--r--   0        0        0     1634 2023-06-14 02:09:48.042663 codegenpt-0.4.1/codegenpt/codegenpt_file.py
--rw-r--r--   0        0        0        0 2023-06-13 06:34:45.151317 codegenpt-0.4.1/codegenpt/commands/__init__.py
--rw-r--r--   0        0        0      248 2023-06-13 06:34:45.151452 codegenpt-0.4.1/codegenpt/commands/command.py
--rw-r--r--   0        0        0      572 2023-06-13 06:34:45.151534 codegenpt-0.4.1/codegenpt/commands/commands.py
--rw-r--r--   0        0        0     1592 2023-06-13 07:10:11.778638 codegenpt-0.4.1/codegenpt/commands/include.py
--rw-r--r--   0        0        0        0 2023-06-12 16:42:59.544293 codegenpt-0.4.1/codegenpt/filesystem/__init__.py
--rw-r--r--   0        0        0      337 2023-06-12 20:14:11.285545 codegenpt-0.4.1/codegenpt/filesystem/file_discovery.py
--rw-r--r--   0        0        0        0 2023-06-12 18:24:09.945595 codegenpt-0.4.1/codegenpt/generators/__init__.py
--rw-r--r--   0        0        0     1417 2023-06-13 06:34:45.151764 codegenpt-0.4.1/codegenpt/generators/file_generator.py
--rw-r--r--   0        0        0        0 2023-06-12 18:24:19.273140 codegenpt-0.4.1/codegenpt/llm/__init__.py
--rw-r--r--   0        0        0      415 2023-06-13 05:01:08.504508 codegenpt-0.4.1/codegenpt/llm/llm.py
--rw-r--r--   0        0        0      578 2023-06-14 04:09:44.521338 codegenpt-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     2895 1970-01-01 00:00:00.000000 codegenpt-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-14 02:09:48.042343 codegenpt-0.6.0/LICENSE
+-rw-r--r--   0        0        0     2636 2023-06-15 05:04:45.202904 codegenpt-0.6.0/README.md
+-rw-r--r--   0        0        0        0 2023-06-12 16:35:22.162725 codegenpt-0.6.0/codegenpt/__init__.py
+-rw-r--r--   0        0        0     3584 2023-06-14 22:22:28.675402 codegenpt-0.6.0/codegenpt/cli.py
+-rw-r--r--   0        0        0     2234 2023-06-15 02:58:09.578938 codegenpt-0.6.0/codegenpt/codegenpt_directory.py
+-rw-r--r--   0        0        0      558 2023-06-14 05:25:26.194231 codegenpt-0.6.0/codegenpt/codegenpt_file.py
+-rw-r--r--   0        0        0     1558 2023-06-14 21:25:13.619217 codegenpt-0.6.0/codegenpt/codegenpt_instructions.py
+-rw-r--r--   0        0        0        0 2023-06-13 06:34:45.151317 codegenpt-0.6.0/codegenpt/commands/__init__.py
+-rw-r--r--   0        0        0      248 2023-06-13 06:34:45.151452 codegenpt-0.6.0/codegenpt/commands/command.py
+-rw-r--r--   0        0        0      612 2023-06-14 06:02:51.279908 codegenpt-0.6.0/codegenpt/commands/commands.py
+-rw-r--r--   0        0        0     1672 2023-06-14 06:03:15.242782 codegenpt-0.6.0/codegenpt/commands/include.py
+-rw-r--r--   0        0        0        0 2023-06-12 16:42:59.544293 codegenpt-0.6.0/codegenpt/filesystem/__init__.py
+-rw-r--r--   0        0        0      778 2023-06-14 04:59:00.374025 codegenpt-0.6.0/codegenpt/filesystem/file_discovery.py
+-rw-r--r--   0        0        0        0 2023-06-12 18:24:09.945595 codegenpt-0.6.0/codegenpt/generators/__init__.py
+-rw-r--r--   0        0        0     3352 2023-06-14 22:43:05.464421 codegenpt-0.6.0/codegenpt/generators/directory_generator.py
+-rw-r--r--   0        0        0     1532 2023-06-14 21:57:11.609802 codegenpt-0.6.0/codegenpt/generators/file_generator.py
+-rw-r--r--   0        0        0        0 2023-06-12 18:24:19.273140 codegenpt-0.6.0/codegenpt/llm/__init__.py
+-rw-r--r--   0        0        0      707 2023-06-14 06:58:12.077684 codegenpt-0.6.0/codegenpt/llm/llm.py
+-rw-r--r--   0        0        0      578 2023-06-15 05:04:46.608673 codegenpt-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     3208 1970-01-01 00:00:00.000000 codegenpt-0.6.0/PKG-INFO
```

### Comparing `codegenpt-0.4.1/LICENSE` & `codegenpt-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `codegenpt-0.4.1/README.md` & `codegenpt-0.6.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 # CodeGenPT
 ![Version](https://img.shields.io/pypi/v/codegenpt)
 ![Python Version Support](https://img.shields.io/pypi/pyversions/codegenpt)
 
-Autogenerate files using ChatGPT API.
+Autogenerate files or entire projects using ChatGPT API.
 
 ## Installation
 ```
 pip install codegenpt
 ```
 
 ## Usage
-CodeGenPT looks for `.codegenpt` files within the source tree and generate files using its instructions.
+CodeGenPT looks for `.codegenpt` files and generate files using its instructions.
+
+### Generating individual files
 
 Example: `hello_world.py.codegenpt`
 ```
 Create a hello world program
 ```
 
 Then:
@@ -26,29 +28,36 @@
 ```
 
 Will generate a file named `helloworld.py`:
 ```python
 print("hello world");
 ```
 
-The actual content of the file will be generated by ChatGPT, so it will vary at each run.
+The actual content of the file will be generated by ChatGPT, so it will vary at each run. You can use `codegenpt -R .` to recursively look for all `.codegenpt` files and generate them.
+
+### Generate entire directories or projects
+
+You can create entire directories or projects using a `.dir.codegenpt` file.
+Example: `tictactoe.dir.codegenpt`
+```
+Create a tic-tac-toe game using html, js and css.
+```
 
-You can also recursevily generate all files within a directory:
+Then:
 ```bash
-$ codegenpt -R .
-🔎 Searching files...
-⏳ Generating file: helloworld.py
-🍺 File generated: helloworld.py
-⏳ Generating file: README.md
-🍺 File generated: README.md
-⏳ Generating file: tests/tests.py
-🍺 File generated: tests/tests.py
+$ codegenpt tic-tac-toe.dir.codegenpt
+⏳ Generating directory: tic-tac-toe
+🍺 File generated: tic-tac-toe/style.css
+🍺 File generated: tic-tac-toe/index.html
+🍺 File generated: tic-tac-toe/game.js
 🍻 Success
 ```
 
+Will create a folder called tic-tac-toe and generate all needed files.
+
 ## Setup
 CodeGenPT expects an environment variable called `OPEN_API_KEY`.
 
 1. Get an [Open AI API Key](https://github.com/Significant-Gravitas/Auto-GPT#:~:text=Get%20an%20OpenAI-,API%20Key,-Download%20the%20latest)
 2. Add the key to your `OPEN_API_KEY` environment variable:
   - If you use `bash`:
     ```bash
```

### Comparing `codegenpt-0.4.1/codegenpt/codegenpt_file.py` & `codegenpt-0.6.0/codegenpt/codegenpt_instructions.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,59 +1,54 @@
+from abc import ABC, abstractmethod
 from os import path
+import os
 import shlex
-
 from codegenpt.commands.command import Command
 
-class CodeGenPTFile:
+class CodeGenPTInstructions(ABC):
+    
+    @property
+    def suffix(self):
+        return '.codegenpt'
 
     @property
-    def filename(self):
-        return '.'.join(self.__filename.split('.')[:-1])
-    
+    def basename(self):
+        return path.basename(self.fullPath)
+      
     @property
-    def extension(self):
-        return self.filename.split('.')[-1]
-    
+    def fullPath(self):
+        return self.instructions_filename.replace(self.suffix, '')
+
     @property
     def prompt(self):
-        with open(self.__filename, 'r') as file:
+        with open(self.instructions_filename, 'r') as file:
             prompt_lines = list(filter(lambda line: not line.startswith('@'), file.readlines()))
             # Filter first lines if they are empty or whitespace
             while prompt_lines[0].strip() == '':
                 prompt_lines.pop(0)
 
         return ''.join(prompt_lines)
 
     @property
     def commands(self):
-        with open(self.__filename, 'r') as file:
+        with open(self.instructions_filename, 'r') as file:
             commands = list(map(
                 lambda line: Command(
                     name = line.strip().split(' ')[0].replace('@', ''),
                     arguments = shlex.split(line.strip())[1:]
                 ),
                 list(filter(lambda line: line.startswith('@'), file.readlines()))
             ))
         return commands
         
     @property
     def path(self):
-        return self.filename.split('/')[:-1]
-    
-    @property
-    def basename(self):
-        return path.basename(self.filename)
+        return self.instructions_filename.split(os.sep)[:-1]
         
     @property
+    @abstractmethod
     def context(self):
-        return {
-            'basename': self.basename,
-            'extension': self.extension,
-            'path': self.path,
-        }
-
-    def __init__(self, filename):
-        self.__filename = filename
-
-    def write(self, content):
-        with open(self.filename, "w+") as file:
-            file.write(content)
+        pass
+
+    def __init__(self, filename, parent = None):
+        self.instructions_filename = filename
+        self.parent = parent
```

### Comparing `codegenpt-0.4.1/codegenpt/commands/commands.py` & `codegenpt-0.6.0/codegenpt/commands/commands.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-from codegenpt.codegenpt_file import CodeGenPTFile
+from codegenpt.codegenpt_instructions import CodeGenPTInstructions
 from codegenpt.commands.include import include
 from codegenpt.commands.command import Command
 
 
 class Commands:
     commandRunners = {}
 
     def registerCommandRunner(name, commandRunner):
         Commands.commandRunners[name] = commandRunner
 
-    def run(command: Command, file: CodeGenPTFile,  messages):
+    def run(command: Command, instructions: CodeGenPTInstructions,  messages):
         if command.name in Commands.commandRunners:
-            return Commands.commandRunners[command.name](command, file, messages)
+            return Commands.commandRunners[command.name](command, instructions, messages)
         return messages
     
 
 Commands.registerCommandRunner('include', include)
```

### Comparing `codegenpt-0.4.1/codegenpt/commands/include.py` & `codegenpt-0.6.0/codegenpt/commands/include.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from codegenpt.codegenpt_file import CodeGenPTFile
+from codegenpt.codegenpt_instructions import CodeGenPTInstructions
 from codegenpt.commands.command import Command
 
 command_message = '''\
 @command
 If the message starts with @include, I'll send the content of files
 that can be included in future instructions, and you should respond with OK.
 
@@ -31,29 +31,32 @@
 {file_content}\
 '''
 
 assistant_message = '''\
 OK\
 '''
 
-def include(command: Command, file: CodeGenPTFile, messages):
-    command_messages = [{
-        "role": "user",
-        "content": command_message,
-    },
-    {
-        "role": "assistant",
-        "content": assistant_message
-    }
+
+def include(command: Command, instructions: CodeGenPTInstructions, messages):
+    command_messages = [
+        {
+            "role": "user",
+            "content": command_message,
+        },
+        {
+            "role": "assistant",
+            "content": assistant_message
+        }
     ]
+
     for filename in command.arguments:
         if filename.startswith('/'):
             path = filename[1:].split('/')
         else:
-            path = file.path + filename.split('/')
+            path = instructions.path + filename.split('/')
 
         with open('/'.join(path), 'r') as file:
             file_content = file.read()
             command_messages.append({
                 "role": "user",
                 "content": user_message.format(
                     file_name = filename,
@@ -62,8 +65,8 @@
             })
 
         command_messages.append({
             "role": "assistant",
             "content": assistant_message
         })
 
-    return [messages[0]] + command_messages + messages[1:]
+    return [messages[0]] + command_messages + messages[1:]
```

### Comparing `codegenpt-0.4.1/codegenpt/generators/file_generator.py` & `codegenpt-0.6.0/codegenpt/generators/file_generator.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from codegenpt.llm.llm import askLLM
 
 system_message = """\
 You are a file generator that follows strict commands. 
 
 If the input starts with @generate, I'll provide instructions for the creation of \
 a single file and you will output only the raw file content, without any instructions or comments.
+If this file is part of a directory described by a codegenpt.json, consider its role within the directory.
 
 If the input starts with @command, you should learn the new command and respond with OK.
 
 Example input:
 @command
 Respond with "Hello!"
 
@@ -52,13 +53,13 @@
         {
             "role": "user",
             "content": user_message,
         }
     ]
 
     for command in file.commands:
-        messages = Commands.run(command=command, file=file, messages=messages)
+        messages = Commands.run(command=command, instructions=file, messages=messages)
 
     response = askLLM(messages=messages)
 
     return response
```

### Comparing `codegenpt-0.4.1/pyproject.toml` & `codegenpt-0.6.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "codegenpt"
-version = "0.4.1"
+version = "0.6.0"
 description = "Autogenerate files and folders using ChatGPT API"
 authors = ["Diego Quinteiro <diegoquinteiro@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [project.urls]
 homepage = "https://github.com/diegoquinteiro/codegenpt"
```

