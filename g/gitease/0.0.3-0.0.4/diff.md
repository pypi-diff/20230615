# Comparing `tmp/gitease-0.0.3.tar.gz` & `tmp/gitease-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitease-0.0.3.tar", last modified: Tue Jun 13 12:57:15 2023, max compression
+gzip compressed data, was "gitease-0.0.4.tar", last modified: Thu Jun 15 11:23:54 2023, max compression
```

## Comparing `gitease-0.0.3.tar` & `gitease-0.0.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 yonatanalexander   (501) staff       (20)        0 2023-06-13 12:57:15.015609 gitease-0.0.3/
--rw-r--r--   0 yonatanalexander   (501) staff       (20)       79 2023-06-07 11:21:02.000000 gitease-0.0.3/.gitattributes
--rw-r--r--   0 yonatanalexander   (501) staff       (20)     4118 2023-06-12 19:42:29.000000 gitease-0.0.3/.gitignore
--rw-r--r--   0 yonatanalexander   (501) staff       (20)     2743 2023-06-13 12:57:15.015276 gitease-0.0.3/PKG-INFO
--rw-r--r--   0 yonatanalexander   (501) staff       (20)     1491 2023-06-13 12:56:44.000000 gitease-0.0.3/README.md
--rw-r--r--   0 yonatanalexander   (501) staff       (20)       98 2023-06-13 12:41:22.000000 gitease-0.0.3/config.py
-drwxr-xr-x   0 yonatanalexander   (501) staff       (20)        0 2023-06-13 12:57:15.012797 gitease-0.0.3/gitease/
--rw-r--r--   0 yonatanalexander   (501) staff       (20)       35 2023-06-13 12:41:22.000000 gitease-0.0.3/gitease/__init__.py
--rw-r--r--   0 yonatanalexander   (501) staff       (20)     4628 2023-06-13 12:41:22.000000 gitease-0.0.3/gitease/automations.py
--rw-r--r--   0 yonatanalexander   (501) staff       (20)     4621 2023-06-13 12:49:26.000000 gitease-0.0.3/gitease/cli.py
--rw-r--r--   0 yonatanalexander   (501) staff       (20)     2421 2023-06-13 12:47:11.000000 gitease-0.0.3/gitease/git.py
-drwxr-xr-x   0 yonatanalexander   (501) staff       (20)        0 2023-06-13 12:57:15.014706 gitease-0.0.3/gitease/prompts/
--rw-r--r--   0 yonatanalexander   (501) staff       (20)      947 2023-06-13 08:49:13.000000 gitease-0.0.3/gitease/prompts/prompt_template.txt
--rw-r--r--   0 yonatanalexander   (501) staff       (20)      823 2023-06-13 08:49:13.000000 gitease-0.0.3/gitease/prompts/refine_template.txt
--rw-r--r--   0 yonatanalexander   (501) staff       (20)     1340 2023-06-13 12:41:22.000000 gitease-0.0.3/gitease/summrizer.py
-drwxr-xr-x   0 yonatanalexander   (501) staff       (20)        0 2023-06-13 12:57:15.014320 gitease-0.0.3/gitease.egg-info/
--rw-r--r--   0 yonatanalexander   (501) staff       (20)     2743 2023-06-13 12:57:11.000000 gitease-0.0.3/gitease.egg-info/PKG-INFO
--rw-r--r--   0 yonatanalexander   (501) staff       (20)      449 2023-06-13 12:57:15.000000 gitease-0.0.3/gitease.egg-info/SOURCES.txt
--rw-r--r--   0 yonatanalexander   (501) staff       (20)        1 2023-06-13 12:57:11.000000 gitease-0.0.3/gitease.egg-info/dependency_links.txt
--rw-r--r--   0 yonatanalexander   (501) staff       (20)       39 2023-06-13 12:57:11.000000 gitease-0.0.3/gitease.egg-info/entry_points.txt
--rw-r--r--   0 yonatanalexander   (501) staff       (20)       94 2023-06-13 12:57:11.000000 gitease-0.0.3/gitease.egg-info/requires.txt
--rw-r--r--   0 yonatanalexander   (501) staff       (20)        8 2023-06-13 12:57:11.000000 gitease-0.0.3/gitease.egg-info/top_level.txt
--rw-r--r--   0 yonatanalexander   (501) staff       (20)     1592 2023-06-13 12:56:56.000000 gitease-0.0.3/pyproject.toml
--rw-r--r--   0 yonatanalexander   (501) staff       (20)       64 2023-06-12 19:37:45.000000 gitease-0.0.3/requirements.txt
--rw-r--r--   0 yonatanalexander   (501) staff       (20)       38 2023-06-13 12:57:15.015689 gitease-0.0.3/setup.cfg
-drwxr-xr-x   0 yonatanalexander   (501) staff       (20)        0 2023-06-13 12:57:15.014900 gitease-0.0.3/tests/
--rw-r--r--   0 yonatanalexander   (501) staff       (20)        0 2023-06-07 11:21:27.000000 gitease-0.0.3/tests/__init__.py
+drwxr-xr-x   0 yonatanalexander   (501) staff       (20)        0 2023-06-15 11:23:54.354775 gitease-0.0.4/
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)       79 2023-06-07 11:21:02.000000 gitease-0.0.4/.gitattributes
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)     4118 2023-06-12 19:42:29.000000 gitease-0.0.4/.gitignore
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)     3063 2023-06-15 11:23:54.354433 gitease-0.0.4/PKG-INFO
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)     1809 2023-06-15 11:21:54.000000 gitease-0.0.4/README.md
+drwxr-xr-x   0 yonatanalexander   (501) staff       (20)        0 2023-06-15 11:23:54.351741 gitease-0.0.4/gitease/
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)        2 2023-06-14 15:01:01.000000 gitease-0.0.4/gitease/__init__.py
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)     4628 2023-06-13 12:41:22.000000 gitease-0.0.4/gitease/automations.py
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)     5385 2023-06-15 11:21:54.000000 gitease-0.0.4/gitease/cli.py
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)     3697 2023-06-15 11:21:54.000000 gitease-0.0.4/gitease/git_helper.py
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)     2996 2023-06-15 11:21:54.000000 gitease-0.0.4/gitease/llm_helper.py
+drwxr-xr-x   0 yonatanalexander   (501) staff       (20)        0 2023-06-15 11:23:54.353851 gitease-0.0.4/gitease/prompts/
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)      947 2023-06-13 08:49:13.000000 gitease-0.0.4/gitease/prompts/prompt_template.txt
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)      823 2023-06-13 08:49:13.000000 gitease-0.0.4/gitease/prompts/refine_template.txt
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)      157 2023-06-15 11:21:54.000000 gitease-0.0.4/gitease/prompts/undo_template.txt
+drwxr-xr-x   0 yonatanalexander   (501) staff       (20)        0 2023-06-15 11:23:54.353013 gitease-0.0.4/gitease.egg-info/
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)     3063 2023-06-15 11:23:50.000000 gitease-0.0.4/gitease.egg-info/PKG-INFO
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)      481 2023-06-15 11:23:54.000000 gitease-0.0.4/gitease.egg-info/SOURCES.txt
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)        1 2023-06-15 11:23:50.000000 gitease-0.0.4/gitease.egg-info/dependency_links.txt
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)       39 2023-06-15 11:23:50.000000 gitease-0.0.4/gitease.egg-info/entry_points.txt
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)       94 2023-06-15 11:23:50.000000 gitease-0.0.4/gitease.egg-info/requires.txt
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)        8 2023-06-15 11:23:50.000000 gitease-0.0.4/gitease.egg-info/top_level.txt
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)     1602 2023-06-15 11:22:12.000000 gitease-0.0.4/pyproject.toml
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)       64 2023-06-12 19:37:45.000000 gitease-0.0.4/requirements.txt
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)       38 2023-06-15 11:23:54.354853 gitease-0.0.4/setup.cfg
+drwxr-xr-x   0 yonatanalexander   (501) staff       (20)        0 2023-06-15 11:23:54.354072 gitease-0.0.4/tests/
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)        0 2023-06-07 11:21:27.000000 gitease-0.0.4/tests/__init__.py
```

### Comparing `gitease-0.0.3/.gitignore` & `gitease-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `gitease-0.0.3/PKG-INFO` & `gitease-0.0.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: gitease
-Version: 0.0.3
+Version: 0.0.4
 Summary: A tool to simplfy git operations
 Maintainer-email: XetHub <contact@xethub.com>
 License: BSD-3-Clause
-Project-URL: Homepage, https://xethub.com/xdssio/gitlm
+Project-URL: Homepage, https://xethub.com/xdssio/gitease
 Keywords: ai,llm,openai,developer-tools,git,nlp
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -40,33 +40,35 @@
 
 * Get an [openai api key](https://platform.openai.com/account/api-keys)
 
 ```bash
 $ export OPENAI_API_KEY=...
 $ pip install gitease
 ```
+
 * If OPENAI_API_KEY is not set, you will be prompted to enter a commit message manually.
 
 ## Usage
 
 Within a repo, run:
 
 ```bash 
-(.venv) $ ge --help
+$ ge --help
 ```
 
 ```bash
 Commands:
   --help:  Show this message and exit.        
     save <message>: Add and commit files to git. Massage is genereated if not provided         
     share <message>: Share to remote - Add, commit and push changes to git. Massage is genereated if not provided
     load :  Pull recent updates from git
     message: Generate commit message from diff using AI.
+    undo: Undo last git action - only works using AI
 
-## Basic Example
+## Examples
 ```bash
 ge save
 
 > Entering new StuffDocumentsChain chain...
 
 
 > Entering new LLMChain chain...
@@ -74,11 +76,23 @@
 Write a concise summary of the following:
 ...
 > Finished chain.
 Automated commit - 4 files:
  writing README.md new instructions.
 gitease/__init__.py
 gitease/cli.py
-gitease/git.py
+gitease/git_helper.py
 pyproject.toml
 ```
 
+```bash
+$ ge undo
+
+Welcome to GitEase
+Last git action is: Update README and CLI files
+A revert command is: git reset HEAD@{0}
+Shell I run the command for you? [y/n]: 
+Running: git reset HEAD@{0}
+Unstaged changes after reset:
+M       README.md
+M       gitease/cli.py
+```
```

### Comparing `gitease-0.0.3/README.md` & `gitease-0.0.4/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -12,33 +12,35 @@
 
 * Get an [openai api key](https://platform.openai.com/account/api-keys)
 
 ```bash
 $ export OPENAI_API_KEY=...
 $ pip install gitease
 ```
+
 * If OPENAI_API_KEY is not set, you will be prompted to enter a commit message manually.
 
 ## Usage
 
 Within a repo, run:
 
 ```bash 
-(.venv) $ ge --help
+$ ge --help
 ```
 
 ```bash
 Commands:
   --help:  Show this message and exit.        
     save <message>: Add and commit files to git. Massage is genereated if not provided         
     share <message>: Share to remote - Add, commit and push changes to git. Massage is genereated if not provided
     load :  Pull recent updates from git
     message: Generate commit message from diff using AI.
+    undo: Undo last git action - only works using AI
 
-## Basic Example
+## Examples
 ```bash
 ge save
 
 > Entering new StuffDocumentsChain chain...
 
 
 > Entering new LLMChain chain...
@@ -46,11 +48,23 @@
 Write a concise summary of the following:
 ...
 > Finished chain.
 Automated commit - 4 files:
  writing README.md new instructions.
 gitease/__init__.py
 gitease/cli.py
-gitease/git.py
+gitease/git_helper.py
 pyproject.toml
 ```
 
+```bash
+$ ge undo
+
+Welcome to GitEase
+Last git action is: Update README and CLI files
+A revert command is: git reset HEAD@{0}
+Shell I run the command for you? [y/n]: 
+Running: git reset HEAD@{0}
+Unstaged changes after reset:
+M       README.md
+M       gitease/cli.py
+```
```

### Comparing `gitease-0.0.3/gitease/automations.py` & `gitease-0.0.4/gitease/automations.py`

 * *Files identical despite different names*

### Comparing `gitease-0.0.3/gitease/cli.py` & `gitease-0.0.4/gitease/cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 import typer
+import os
+import subprocess
 from typing import List
 from rich.style import Style
 from rich.console import Console
 from rich.prompt import Prompt
 from typing_extensions import Annotated
-from gitease import GitHelper
-from gitease.summrizer import Summarizer
-from config import OPENAI_API_KEY_NAME, OPENAI_API_KEY
+from gitease.git_helper import GitHelper
+from gitease.llm_helper import LanguageModel
 
+OPENAI_API_KEY = os.getenv('OPENAI_API_KEY')
 cli = typer.Typer(add_completion=False)
-
 console = Console()
 console.print("Welcome to GitEase", style=Style(color="green", blink=True, bold=True))
 
 add_annotation = Annotated[List[str], typer.Option("--add", "-a", help="Files to add. All of not provided")]
 message_annotation = Annotated[str, typer.Option("--message", "-m",
-                                                 help=f"commit message - If not provided, Generate by AI (given {OPENAI_API_KEY_NAME} is set)")]
+                                                 help=f"commit message - If not provided, Generate by AI (given OPENAI_API_KEY is set)")]
 quiet_annotation = Annotated[
     bool, typer.Option("--quiet", "-q", help="If True - Quiet the the LLM thoughts and other messages")]
 y_annotation = Annotated[bool, typer.Option("--yes", "-y", help="If True - Skips confirmation message")]
 
 
 def _join_files(files):
     return '\n'.join(files)
@@ -64,15 +65,15 @@
     if message is None:
         diff = helper.get_diff(staged=True)
         if not diff:
             console.print("No message provided, skipping commit", style=Style(color="red", blink=True, bold=True))
             return
         response = None
         if OPENAI_API_KEY:
-            message = Summarizer(verbose=not quiet).summarize(diff).lstrip()
+            message = LanguageModel(verbose=not quiet).summarize(diff).lstrip()
             message = message + f"\n{_join_files(add)}"
             if not y:
                 response = confirm_message(message)
             if response and len(response) > 0:  # new user commit message
                 message = response
         else:
             message = get_user_message(diff)
@@ -101,21 +102,37 @@
 
 
 @cli.command()
 def message(quiet: quiet_annotation = False,
             copy: Annotated[bool, typer.Option("--copy", "-c", help="Copy to clipboard")] = False):
     """Generate commit message from diff using AI"""
     if not OPENAI_API_KEY:
-        console.print(f"{OPENAI_API_KEY_NAME} not set", style=Style(color="red", blink=True, bold=True))
+        console.print(f"OPENAI_API_KEY not set", style=Style(color="red", blink=True, bold=True))
         return False
     diff = GitHelper(verbose=not quiet).get_diff(staged=True)
-    message = Summarizer(verbose=not quiet).summarize(diff).lstrip()
+    message = LanguageModel(verbose=not quiet).summarize(diff).lstrip()
     console.print("Commit message:\n", style=Style(color="red", blink=True, bold=True))
     console.print(message)
     if copy:
         try:
             import clipboard
             console.print("Copied to clipboard", style=Style(color="green"))
             clipboard.copy(message)
         except ImportError:
             console.print("Install clipboard to copy to clipboard: 'pip install clipboard'",
                           style=Style(color="red", blink=True, bold=True))
+
+
+@cli.command()
+def undo():
+    """Undo last git action"""
+    llm = LanguageModel()
+    reflog = "\n".join(GitHelper().reflog().split("\n")[0])
+    last_action = llm.get_git_undo(reflog)
+    console.print(f"Last git action is: [purple]{last_action.action}[/purple]", style=Style(color="yellow"))
+    console.print(f"A revert command is: [red]{last_action.revert_command}[/red]", style=Style(color="yellow"))
+    response = Prompt.ask("Shell I run the command for you?", choices=["y", "n"])
+    if response == "y":
+        console.print(f"Running: '{last_action.revert_command}'", style=Style(color="red"))
+        os.system(last_action.revert_command)
+    if response == "n":
+        console.print("Ok, Bye!", style=Style(color="green"))
```

### Comparing `gitease-0.0.3/gitease/prompts/prompt_template.txt` & `gitease-0.0.4/gitease/prompts/prompt_template.txt`

 * *Files identical despite different names*

### Comparing `gitease-0.0.3/gitease/prompts/refine_template.txt` & `gitease-0.0.4/gitease/prompts/refine_template.txt`

 * *Files identical despite different names*

### Comparing `gitease-0.0.3/gitease.egg-info/PKG-INFO` & `gitease-0.0.4/gitease.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: gitease
-Version: 0.0.3
+Version: 0.0.4
 Summary: A tool to simplfy git operations
 Maintainer-email: XetHub <contact@xethub.com>
 License: BSD-3-Clause
-Project-URL: Homepage, https://xethub.com/xdssio/gitlm
+Project-URL: Homepage, https://xethub.com/xdssio/gitease
 Keywords: ai,llm,openai,developer-tools,git,nlp
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -40,33 +40,35 @@
 
 * Get an [openai api key](https://platform.openai.com/account/api-keys)
 
 ```bash
 $ export OPENAI_API_KEY=...
 $ pip install gitease
 ```
+
 * If OPENAI_API_KEY is not set, you will be prompted to enter a commit message manually.
 
 ## Usage
 
 Within a repo, run:
 
 ```bash 
-(.venv) $ ge --help
+$ ge --help
 ```
 
 ```bash
 Commands:
   --help:  Show this message and exit.        
     save <message>: Add and commit files to git. Massage is genereated if not provided         
     share <message>: Share to remote - Add, commit and push changes to git. Massage is genereated if not provided
     load :  Pull recent updates from git
     message: Generate commit message from diff using AI.
+    undo: Undo last git action - only works using AI
 
-## Basic Example
+## Examples
 ```bash
 ge save
 
 > Entering new StuffDocumentsChain chain...
 
 
 > Entering new LLMChain chain...
@@ -74,11 +76,23 @@
 Write a concise summary of the following:
 ...
 > Finished chain.
 Automated commit - 4 files:
  writing README.md new instructions.
 gitease/__init__.py
 gitease/cli.py
-gitease/git.py
+gitease/git_helper.py
 pyproject.toml
 ```
 
+```bash
+$ ge undo
+
+Welcome to GitEase
+Last git action is: Update README and CLI files
+A revert command is: git reset HEAD@{0}
+Shell I run the command for you? [y/n]: 
+Running: git reset HEAD@{0}
+Unstaged changes after reset:
+M       README.md
+M       gitease/cli.py
+```
```

### Comparing `gitease-0.0.3/pyproject.toml` & `gitease-0.0.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gitease"
-version = "0.0.3"
+version = "0.0.4"
 description = "A tool to simplfy git operations"
 readme = "README.md"
 keywords = [
     "ai",
     "llm",
     "openai",
     "developer-tools",
@@ -43,14 +43,14 @@
     "rich>=13.4.2",
     "langchain>=0.0.191",
     "GitPython>=3.1.31",
     "tiktoken>=0.4.0"
 ]
 
 [project.urls]
-Homepage = "https://xethub.com/xdssio/gitlm"
+Homepage = "https://xethub.com/xdssio/gitease"
 
 
 [project.scripts]
 ge = "gitease.cli:cli"
-#bgitllm = "gitease.cli:backgroundcli"
+#bgitllm = "gitease.automations:backgroundcli"
```

