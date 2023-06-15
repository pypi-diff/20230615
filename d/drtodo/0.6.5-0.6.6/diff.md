# Comparing `tmp/drtodo-0.6.5.tar.gz` & `tmp/drtodo-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drtodo-0.6.5.tar", max compression
+gzip compressed data, was "drtodo-0.6.6.tar", max compression
```

## Comparing `drtodo-0.6.5.tar` & `drtodo-0.6.6.tar`

### file list

```diff
@@ -1,13 +1,19 @@
--rw-r--r--   0        0        0     1064 2023-05-31 19:03:43.606591 drtodo-0.6.5/LICENSE
--rw-r--r--   0        0        0     9777 2023-05-31 19:03:43.610591 drtodo-0.6.5/drtodo/README.md
--rw-r--r--   0        0        0      224 2023-05-31 19:03:43.610591 drtodo-0.6.5/drtodo/__init__.py
--rw-r--r--   0        0        0       46 2023-05-31 19:03:43.610591 drtodo-0.6.5/drtodo/__main__.py
--rw-r--r--   0        0        0    12223 2023-05-31 19:03:43.610591 drtodo-0.6.5/drtodo/main.py
--rw-r--r--   0        0        0     4977 2023-05-31 19:03:43.610591 drtodo-0.6.5/drtodo/man_command.py
--rw-r--r--   0        0        0     4784 2023-05-31 19:03:43.610591 drtodo-0.6.5/drtodo/mdparser.py
--rw-r--r--   0        0        0     1406 2023-05-31 19:03:43.610591 drtodo-0.6.5/drtodo/mistuneplugin.py
--rw-r--r--   0        0        0      618 2023-05-31 19:03:43.610591 drtodo-0.6.5/drtodo/rich_display.py
--rw-r--r--   0        0        0     7061 2023-05-31 19:03:43.610591 drtodo-0.6.5/drtodo/settings.py
--rw-r--r--   0        0        0       11 2023-05-31 19:03:43.610591 drtodo-0.6.5/drtodo/util.py
--rw-r--r--   0        0        0      808 2023-05-31 19:03:59.298785 drtodo-0.6.5/pyproject.toml
--rw-r--r--   0        0        0    10671 1970-01-01 00:00:00.000000 drtodo-0.6.5/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-15 15:30:01.641876 drtodo-0.6.6/LICENSE
+-rw-r--r--   0        0        0     9777 2023-06-15 15:30:01.641876 drtodo-0.6.6/drtodo/README.md
+-rw-r--r--   0        0        0      224 2023-06-15 15:30:01.641876 drtodo-0.6.6/drtodo/__init__.py
+-rw-r--r--   0        0        0       46 2023-06-15 15:30:01.641876 drtodo-0.6.6/drtodo/__main__.py
+-rw-r--r--   0        0        0     4385 2023-06-15 15:30:01.641876 drtodo-0.6.6/drtodo/backup_command.py
+-rw-r--r--   0        0        0    12994 2023-06-15 15:30:01.641876 drtodo-0.6.6/drtodo/main.py
+-rw-r--r--   0        0        0      419 2023-06-15 15:30:01.641876 drtodo-0.6.6/drtodo/man/README.md
+-rw-r--r--   0        0        0        0 2023-06-15 15:30:01.641876 drtodo-0.6.6/drtodo/man/__init__.py
+-rw-r--r--   0        0        0     2872 2023-06-15 15:30:01.641876 drtodo-0.6.6/drtodo/man/config.md
+-rw-r--r--   0        0        0      874 2023-06-15 15:30:01.641876 drtodo-0.6.6/drtodo/man/mdfiles.md
+-rw-r--r--   0        0        0     1271 2023-06-15 15:30:01.641876 drtodo-0.6.6/drtodo/man_command.py
+-rw-r--r--   0        0        0     6793 2023-06-15 15:30:01.641876 drtodo-0.6.6/drtodo/mdparser.py
+-rw-r--r--   0        0        0     1406 2023-06-15 15:30:01.641876 drtodo-0.6.6/drtodo/mistuneplugin.py
+-rw-r--r--   0        0        0      719 2023-06-15 15:30:01.641876 drtodo-0.6.6/drtodo/rich_display.py
+-rw-r--r--   0        0        0     7211 2023-06-15 15:30:01.641876 drtodo-0.6.6/drtodo/settings.py
+-rw-r--r--   0        0        0     2771 2023-06-15 15:30:01.641876 drtodo-0.6.6/drtodo/taskitems.py
+-rw-r--r--   0        0        0      256 2023-06-15 15:30:01.641876 drtodo-0.6.6/drtodo/util.py
+-rw-r--r--   0        0        0      808 2023-06-15 15:30:14.241861 drtodo-0.6.6/pyproject.toml
+-rw-r--r--   0        0        0    10671 1970-01-01 00:00:00.000000 drtodo-0.6.6/PKG-INFO
```

### Comparing `drtodo-0.6.5/LICENSE` & `drtodo-0.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `drtodo-0.6.5/drtodo/README.md` & `drtodo-0.6.6/drtodo/README.md`

 * *Files identical despite different names*

### Comparing `drtodo-0.6.5/drtodo/main.py` & `drtodo-0.6.6/drtodo/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-import re
 from pathlib import Path
 from typing import Optional
 
 import rich.markdown
 import typer
-from typer_aliases import Typer
 from git.repo import Repo
-from rich import print
 
+from typer_aliases import Typer
+
+from . import backup_command, util
 from .man_command import manapp
 from .mdparser import TaskListTraverser, TodoListParser
-from .rich_display import console
-from .settings import constants, globals, settings, Style
-
+from .rich_display import console, error_console
+from .settings import Style, constants, globals, make_pretty_path, settings
+from . import taskitems
 
 
 app = Typer(
     no_args_is_help=True,
     rich_markup_mode="markdown",
     help=f"**{constants.appname}, MD**: *a straightforward todo list manager for markdown files in git repos.*",
     epilog=f"DrTodo can manage items in a global todo list ({globals.global_todofile_pretty})"
@@ -28,15 +28,15 @@
 def version_string() -> str:
     return f"{constants.appname} v{constants.version}"
 
 
 def ensure_appdir(may_create: bool = False) -> None:
     if not constants.appdir.exists():
         if not may_create:
-            print(f"DrTodo folder {constants.appdir} does not exist. Use [bold]todo init[/bold] to create it.")
+            error_console().print(f"DrTodo folder {constants.appdir} does not exist. Use [bold]todo init[/bold] to create it.")
         else:
             constants.appdir.mkdir(parents=False, exist_ok=False)
             assert globals.global_todofile and not globals.global_todofile.exists()
             globals.global_todofile.touch()
             repo = Repo.init(constants.appdir)
             repo.index.add([globals.global_todofile])
 
@@ -72,35 +72,42 @@
     if dim:
         mdtext_part.style = "dim"
     if strike:
         mdtext_part.style = "strike"
     console().print(index_part + hash_part + checkmark_part, mdtext_part, end='')
 
 
-def print_todo_items(items: list):
-    for item in items:
-        print_todo_item(item)
-
-
 @app.command(name="list")
 @app.command(name="ls", hidden=True)
-def list_command():
+def list_command(
+    spec: str = typer.Argument(None, help="ID, index, range or regular expression to match item text"),
+    id: str = typer.Option(None, "--id", "-i", help="ID of the item to list"),
+    index: int = typer.Option(None, "--index", "-n", help="Index of the item to list"),
+    range: str = typer.Option(None, "--range", "-r", help="Range of item indices to list, e.g, 2:5, 2:, :5"),
+    match: str = typer.Option(None, "--match", "-m", help="Regular expression to match item text"),
+    # TODO: add more filter options, done/undone, priority, due, owner, etc.
+):
     """
     List todo items in the list
     """
     if globals.global_todofile and globals.global_todofile.exists():
         console().print(f"[header]{globals.global_todofile_pretty}[text]")
         todo = TodoListParser()
         todo.parse(globals.global_todofile)
-        print_todo_items(todo.items)
+        for item in taskitems.task_iterator(todo.items, omit_means_all=True,
+                                            spec=spec, id=id, index=index, range=range, match=match):
+            print_todo_item(item)
+
     if globals.local_todofile and globals.local_todofile.exists():
         console().print(f"[header]{globals.local_todofile_pretty}[text]")
         todo = TodoListParser()
         todo.parse(globals.local_todofile)
-        print_todo_items(todo.items)
+        for item in taskitems.task_iterator(todo.items, omit_means_all=True,
+                                            spec=spec, id=id, index=index, range=range, match=match):
+            print_todo_item(item)
 
 
 @app.command(name="debug")
 @app.command(name="dbg", hidden=True)
 def debug_command():
     """
     List configuration, settings, version and other debug info.
@@ -113,17 +120,17 @@
 
 def _add_item(todo_item: dict, todofile_path: Path):
     if todofile_path and todofile_path.exists():
         todo = TodoListParser()
         todo.parse(todofile_path)
         # TODO: need to append in the MD file in the right place (once we support sections, etc.)
         todo.add_item_after(add=todo_item, after=todo.items[-1])
-        save_todo_backups(todofile_path, todo)
+        backup_command.save_with_backups(todofile_path, todo)
     else:
-        print(f"Cannot add item to {todofile_path} because it does not exist")
+        error_console().print(f"Cannot add item to {todofile_path} because it does not exist")
         raise typer.Exit(2)
 
 
 # add [--priority <priority>] [--due <due>] [--owner <owner>] [--done] <item description>
 @app.command()
 def add(
     description: str,
@@ -147,163 +154,144 @@
         _add_item(todo_item, globals.local_todofile)
     else:
         assert globals.global_todofile
         console().print(f"[header]{globals.global_todofile_pretty}[text]")
         _add_item(todo_item, globals.global_todofile)
     print_todo_item(todo_item)
 
-
-def save_todo_backups(pathname: Path, todo):
-    def make_backup_path(i: int) -> Path:
-        assert isinstance(i, int) and i > 0
-        # files are hidden and have a '.bak-1' extension for the most recent backup, '.bak-2' for the next, etc.
-        return pathname.with_name(f".{pathname.name.removeprefix('.')}.bak-{i}")
-
-    # first write to a temp file with a '.tmp' extension
-    tmpfilepath = pathname.with_suffix(pathname.suffix + '.tmp')
-    todo.write(tmpfilepath)
-
-    # if file write worked, then we can perform the rename dance
-    n = settings.keep_backups
-    if n > 0:
-        # we keep n backups named as '.bak-1' (for the most recent n-1 backup), '.bak-2', etc.)
-        # first delete the oldest backup
-        make_backup_path(n).unlink(missing_ok=True)
-        for i in range(n - 1, 0, -1):
-            bakfilepath = make_backup_path(i)
-            if bakfilepath.exists():
-                bakfilepath.rename(make_backup_path(i + 1))
-        # rename the original file to '.bak-1'
-        pathname.rename(make_backup_path(1))
-    # finally, rename the temp file to the original filename
-    tmpfilepath.rename(pathname)
-
-
-def _done_undone_marker(done: bool, spec, id, index, match, all):
+def _done_undone_marker(done: bool, spec, id, index, range, match, all):
     """
     Mark one or more todo items as done or undone.
     """
     # ensure exactly one of spec, id, index, match or all is not None
-    if sum([spec is not None, id is not None, index is not None, match is not None, all]) != 1:
-        # console().print("[error]ERROR:[/error] Exactly one of --id, --index, --match or --all must be provided")
-        raise typer.BadParameter("Exactly one of --id, --index, --match or --all must be provided")
-
-    if spec is not None:
-        # heuristics:
-        # if spec is a small integer, assume it's an index
-        # if spec is a a pure hex string assume it's an ID
-        # otherwise assume it's a regular expression
-        try:
-            index = int(spec)
-            if index >= 1000:
-                raise ValueError
-        except ValueError:
-            if re.match(r'^[0-9a-f]+$', spec):
-                id = spec
-            else:
-                match = spec
-
-    def matching_items_iter(items, id, index, match, all):
-        if all:
-            for item in items:
-                yield item
-        elif id is not None:
-            for item in items:
-                if item['id'].startswith(id):
-                    yield item
-        elif index is not None:
-            for item in items:
-                if item['index'] == index:
-                    yield item
-        elif match is not None:
-            for item in items:
-                if re.search(match, item['text']):
-                    yield item
+    if sum([spec is not None, id is not None, index is not None, range is not None, match is not None, all]) != 1:
+        raise typer.BadParameter("Exactly one of --id, --index, --range, --match or --all must be provided")
 
     if globals.global_todofile and globals.global_todofile.exists():
         console().print(f"[header]{globals.global_todofile}[text] changes:")
         todo = TodoListParser()
         todo.parse(globals.global_todofile)
-        for item in matching_items_iter(todo.items, id, index, match, all):
+        items = taskitems.task_iterator(todo.items, id=id, index=index, range=range, match=match) if not all else todo.items
+        for item in items:
             item['checked'] = done
             print_todo_item(item)
         # write back to file
-        save_todo_backups(globals.global_todofile, todo)
+        backup_command.save_with_backups(globals.global_todofile, todo)
 
     if globals.local_todofile and globals.local_todofile.exists():
         console().print(f"[header]{globals.local_todofile}[text] changes:")
         todo = TodoListParser()
         todo.parse(globals.local_todofile)
-        for item in matching_items_iter(todo.items, id, index, match, all):
+        items = taskitems.task_iterator(todo.items, id=id, index=index, range=range, match=match) if not all else todo.items
+        for item in items:
             item['checked'] = done
             print_todo_item(item)
         # write back to file
-        save_todo_backups(globals.local_todofile, todo)
+        backup_command.save_with_backups(globals.local_todofile, todo)
 
 
 # done [--id <id> | --index <index> | --all | --match <regular expression> | <specification>]
 # (exactly one option must be provided)
 @app.command()
 def done(
-    spec: str = typer.Argument(None, help="ID, index or regular expression to match item text"),
-    id: str = typer.Option(None, "--id", "-i", help="ID of the item to mark as done"),
-    index: int = typer.Option(None, "--index", "-n", help="Index of the item to mark as done"),
+    spec: str = typer.Argument(None, help="ID, index, range or regular expression to match item text"),
+    id: str = typer.Option(None, "--id", "-i", help="ID of the item to mark"),
+    index: int = typer.Option(None, "--index", "-n", help="Index of the item to mark"),
+    range: str = typer.Option(None, "--range", "-r", help="Range of item indices to mark, e.g, 2:5, 2:, :5"),
     match: str = typer.Option(None, "--match", "-m", help="Regular expression to match item text"),
-    all: bool = typer.Option(False, "--all", "-a", help="Mark all items as done"),
+    all: bool = typer.Option(False, "--all", "-a", help="Mark all items"),
 ):
     """
     Mark one or more todo items as done
     """
-    _done_undone_marker(True, spec, id, index, match, all)
+    _done_undone_marker(True, spec, id, index, range, match, all)
 
 
 # undone [--id <id> | --index <index> | --all | --match <regular expression> | <specification>]
 # (exactly one option must be provided)
 @app.command()
 def undone(
-    spec: str = typer.Argument(None, help="ID, index or regular expression to match item text"),
-    id: str = typer.Option(None, "--id", "-i", help="ID of the item to mark as done"),
-    index: int = typer.Option(None, "--index", "-n", help="Index of the item to mark as done"),
+    spec: str = typer.Argument(None, help="ID, index, range or regular expression to match item text"),
+    id: str = typer.Option(None, "--id", "-i", help="ID of the item to mark"),
+    index: int = typer.Option(None, "--index", "-n", help="Index of the item to mark"),
+    range: str = typer.Option(None, "--range", "-r", help="Range of item indices to mark,e.g, 2:5, 2:, :5"),
     match: str = typer.Option(None, "--match", "-m", help="Regular expression to match item text"),
-    all: bool = typer.Option(False, "--all", "-a", help="Mark all items as done"),
+    all: bool = typer.Option(False, "--all", "-a", help="Mark all items"),
 ):
     """
     Mark one or more todo items as NOT done (undone)
     """
-    _done_undone_marker(False, spec, id, index, match, all)
+    _done_undone_marker(False, spec, id, index, range, match, all)
+
+
+@app.command()
+def show(files: Optional[list[Path]] = typer.Argument(None, help="override which markdown files to show"),
+         raw: bool = typer.Option(False, "--raw", help="Print the raw markdown man content")
+        ):
+    """
+    Show markdown file(s) with rich rendering. Defaults to the active, configured files.
+    """
+    md_print = util.print_md_as_raw if raw else util.print_md_pretty
+    if not files:
+        files = [globals.global_todofile, globals.local_todofile]
+    for file in files:
+        if file and file.exists():
+            if len(files) > 1:
+                console().print(f"[header]{make_pretty_path(file)}[text]")
+            with file.open() as f:
+                mdstring = f.read()
+                md_print(mdstring)
 
 
 app.add_typer(manapp,
               name="man",
               help="Show detailed help and context for settings, file format and heuristics",
               no_args_is_help=True)
 
 
+app.add_typer(backup_command.app,
+              name="backup",
+              help="Manage backups of markdown files",
+              no_args_is_help=True)
+
+
 def _version_callback(value: bool) -> None:
     if value:
         console().print(f"{version_string()}", highlight=False)
         raise typer.Exit()
 
 
 panel_GLOBAL = "Global Options"
 panel_FILESELECTION = "File Selection Options"
 
 
 # Typer callback handles global options like --mdfile and --verbose
 @app.callback()
 def main_callback(
-    settings: Optional[Path] = typer.Option(constants.appdir, "--settings", "-s", help="Settings file to use",
-                                            rich_help_panel=panel_GLOBAL),
-    verbose: Optional[bool] = typer.Option(False, "--verbose", "-v", help="Verbose output",
+    settings_file: Optional[Path] = typer.Option(constants.appdir, "--settings", "-s", help="Settings file to use",
+                                                 rich_help_panel=panel_GLOBAL),
+    verbose: Optional[bool] = typer.Option(settings.verbose, "--verbose", "-v", help="Verbose output",
                                            rich_help_panel=panel_GLOBAL),
     mdfile: Optional[Path] = typer.Option(settings.mdfile, help="Markdown file to use for todo list",
                                           rich_help_panel=panel_FILESELECTION),
+    section: Optional[str] = typer.Option(settings.section,
+                                          help="Section name in markdown file to use for todo list, with optional "\
+                                          "heading level, e.g. '## TODO'",
+                                          rich_help_panel=panel_FILESELECTION),
+    reverse_order: Optional[bool] = typer.Option(settings.reverse_order, "--reverse-order/--normal-order",
+                                                 help="Whether todo items should be in reverse order (latest first)",
+                                                 rich_help_panel=panel_FILESELECTION),
     version: Optional[bool] = typer.Option(False, "--version", "-V", help="Show version and exit",
                                            callback=_version_callback, is_eager=True, rich_help_panel=panel_GLOBAL),
 ):
+    settings.mdfile = mdfile
+    settings.verbose = verbose
+    settings.section = section
+    settings.reverse_order = reverse_order
+
     # BUG: this is called even when the command is init, so it prints a warning about the appdir not existing
     ensure_appdir()
 
 def main(*args, **kwargs):
     # typer_aliases(app=app)
     app(*args, **kwargs)
```

### Comparing `drtodo-0.6.5/drtodo/mistuneplugin.py` & `drtodo-0.6.6/drtodo/mistuneplugin.py`

 * *Files identical despite different names*

### Comparing `drtodo-0.6.5/drtodo/settings.py` & `drtodo-0.6.6/drtodo/settings.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,15 +51,17 @@
     'boxed': Style(checked='☑', unchecked='☐'),
     'dark': Style(checked='✅', unchecked='🔳'),
     'light': Style(checked='✅', unchecked='🔲'),
 }
 
 
 class Settings(BaseSettings):
-    mdfile: str = Field("TODO.md", env=constants.env_prefix + "MDFILE")
+    mdfile: str = Field('TODO.md', env=constants.env_prefix + 'MDFILE')
+    section: str = Field('', env=constants.env_prefix + 'SECTION')
+    reverse_order: bool = Field(False, env=constants.env_prefix + 'REVERSE_ORDER')
     verbose: bool = False
     keep_backups: int = 3   # number of backups to keep
     hide_hash: bool = False
     style: Union[Style, str] = ''
 
     # def __init__(self, **kwargs):
     #     super().__init__(**kwargs)
```

### Comparing `drtodo-0.6.5/pyproject.toml` & `drtodo-0.6.6/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "DrTodo"
-version = "0.6.5"
+version = "0.6.6"
 description = "DrTodo, MD: todo list manager using markdown files and git"
 authors = ["exilium <info@exilium.com>"]
 readme = "drtodo/README.md"
 license = "MIT"
 repository = "https://github.com/exilium-com/DrTodo"
 keywords = ["utilities", "todo", "markdown"]
```

### Comparing `drtodo-0.6.5/PKG-INFO` & `drtodo-0.6.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drtodo
-Version: 0.6.5
+Version: 0.6.6
 Summary: DrTodo, MD: todo list manager using markdown files and git
 Home-page: https://github.com/exilium-com/DrTodo
 License: MIT
 Keywords: utilities,todo,markdown
 Author: exilium
 Author-email: info@exilium.com
 Requires-Python: >=3.9,<4.0
```

