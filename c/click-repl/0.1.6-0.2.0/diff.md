# Comparing `tmp/click-repl-0.1.6.tar.gz` & `tmp/click-repl-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/click-repl-0.1.6.tar", last modified: Mon Oct 15 16:53:49 2018, max compression
+gzip compressed data, was "dist/click-repl-0.2.0.tar", last modified: Sun May 30 20:20:07 2021, max compression
```

## Comparing `click-repl-0.1.6.tar` & `click-repl-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 untitaker   (501) staff       (20)        0 2018-10-15 16:53:49.000000 click-repl-0.1.6/
--rw-r--r--   0 untitaker   (501) staff       (20)     1084 2018-07-29 11:59:42.000000 click-repl-0.1.6/LICENSE
--rw-r--r--   0 untitaker   (501) staff       (20)       64 2018-08-04 15:10:37.000000 click-repl-0.1.6/MANIFEST.in
--rw-r--r--   0 untitaker   (501) staff       (20)      256 2018-10-15 16:53:49.000000 click-repl-0.1.6/PKG-INFO
--rw-r--r--   0 untitaker   (501) staff       (20)     2142 2018-07-29 12:14:49.000000 click-repl-0.1.6/README.rst
-drwxr-xr-x   0 untitaker   (501) staff       (20)        0 2018-10-15 16:53:49.000000 click-repl-0.1.6/click_repl/
--rw-r--r--   0 untitaker   (501) staff       (20)     8564 2018-10-15 16:53:25.000000 click-repl-0.1.6/click_repl/__init__.py
--rw-r--r--   0 untitaker   (501) staff       (20)      114 2018-07-29 11:59:42.000000 click-repl-0.1.6/click_repl/exceptions.py
-drwxr-xr-x   0 untitaker   (501) staff       (20)        0 2018-10-15 16:53:49.000000 click-repl-0.1.6/click_repl.egg-info/
--rw-r--r--   0 untitaker   (501) staff       (20)      256 2018-10-15 16:53:49.000000 click-repl-0.1.6/click_repl.egg-info/PKG-INFO
--rw-r--r--   0 untitaker   (501) staff       (20)      256 2018-10-15 16:53:49.000000 click-repl-0.1.6/click_repl.egg-info/SOURCES.txt
--rw-r--r--   0 untitaker   (501) staff       (20)        1 2018-10-15 16:53:49.000000 click-repl-0.1.6/click_repl.egg-info/dependency_links.txt
--rw-r--r--   0 untitaker   (501) staff       (20)       25 2018-10-15 16:53:49.000000 click-repl-0.1.6/click_repl.egg-info/requires.txt
--rw-r--r--   0 untitaker   (501) staff       (20)       11 2018-10-15 16:53:49.000000 click-repl-0.1.6/click_repl.egg-info/top_level.txt
--rw-r--r--   0 untitaker   (501) staff       (20)       38 2018-10-15 16:53:49.000000 click-repl-0.1.6/setup.cfg
--rw-r--r--   0 untitaker   (501) staff       (20)      614 2018-07-29 12:25:06.000000 click-repl-0.1.6/setup.py
+drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2021-05-30 20:20:07.438345 click-repl-0.2.0/
+-rw-rw-r--   0 markus    (1000) markus    (1000)     1084 2021-05-30 20:17:13.000000 click-repl-0.2.0/LICENSE
+-rw-rw-r--   0 markus    (1000) markus    (1000)       64 2021-05-30 20:17:13.000000 click-repl-0.2.0/MANIFEST.in
+-rw-rw-r--   0 markus    (1000) markus    (1000)      256 2021-05-30 20:20:07.438345 click-repl-0.2.0/PKG-INFO
+-rw-rw-r--   0 markus    (1000) markus    (1000)     2238 2021-05-30 20:17:13.000000 click-repl-0.2.0/README.rst
+drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2021-05-30 20:20:07.438345 click-repl-0.2.0/click_repl/
+-rw-rw-r--   0 markus    (1000) markus    (1000)     8906 2021-05-30 20:19:41.000000 click-repl-0.2.0/click_repl/__init__.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)      114 2021-05-30 20:17:13.000000 click-repl-0.2.0/click_repl/exceptions.py
+drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2021-05-30 20:20:07.438345 click-repl-0.2.0/click_repl.egg-info/
+-rw-rw-r--   0 markus    (1000) markus    (1000)      256 2021-05-30 20:20:07.000000 click-repl-0.2.0/click_repl.egg-info/PKG-INFO
+-rw-rw-r--   0 markus    (1000) markus    (1000)      256 2021-05-30 20:20:07.000000 click-repl-0.2.0/click_repl.egg-info/SOURCES.txt
+-rw-rw-r--   0 markus    (1000) markus    (1000)        1 2021-05-30 20:20:07.000000 click-repl-0.2.0/click_repl.egg-info/dependency_links.txt
+-rw-rw-r--   0 markus    (1000) markus    (1000)       25 2021-05-30 20:20:07.000000 click-repl-0.2.0/click_repl.egg-info/requires.txt
+-rw-rw-r--   0 markus    (1000) markus    (1000)       11 2021-05-30 20:20:07.000000 click-repl-0.2.0/click_repl.egg-info/top_level.txt
+-rw-rw-r--   0 markus    (1000) markus    (1000)       38 2021-05-30 20:20:07.438345 click-repl-0.2.0/setup.cfg
+-rw-rw-r--   0 markus    (1000) markus    (1000)      614 2021-05-30 20:17:13.000000 click-repl-0.2.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `click-repl-0.1.6/LICENSE` & `click-repl-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `click-repl-0.1.6/README.rst` & `click-repl-0.2.0/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -43,14 +43,24 @@
 
 You can use the internal ``:help`` command to explain usage.
 
 PyPI: `<https://pypi.python.org/pypi/click-repl>`_
 
 .. _click: http://click.pocoo.org/
 
+
+
+How to install
+==============
+
+Installation is done with pip:
+
+    $ pip install click-repl
+
+
 Advanced Usage
 ==============
 
 For more flexibility over how your REPL works you can use the ``repl`` function
 directly instead of ``register_repl``. For example, in your app:
 
 .. code:: python
```

### Comparing `click-repl-0.1.6/click_repl/__init__.py` & `click-repl-0.2.0/click_repl/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,27 @@
 from collections import defaultdict
 from prompt_toolkit.completion import Completer, Completion
 from prompt_toolkit.history import InMemoryHistory
 from prompt_toolkit.shortcuts import prompt
 import click
-import click._bashcomplete
 import click.parser
 import os
 import shlex
 import sys
 import six
 from .exceptions import InternalCommandException, ExitReplException  # noqa
 
+# Handle backwards compatibility between Click 7.0 and 8.0
+try: 
+    import click.shell_completion
+    HAS_C8 = True
+except ImportError:
+    import click._bashcomplete
+    HAS_C8 = False
+
 # Handle click.exceptions.Exit introduced in Click 7.0
 try:
     from click.exceptions import Exit as ClickExit
 except ImportError:
     class ClickExit(RuntimeError):
         pass
 
@@ -22,15 +29,15 @@
 
 if PY2:
     text_type = unicode  # noqa
 else:
     text_type = str  # noqa
 
 
-__version__ = "0.1.6"
+__version__ = "0.2.0"
 
 _internal_commands = dict()
 
 
 def _register_internal_command(names, target, description=None):
     if not hasattr(target, "__call__"):
         raise ValueError("Internal command must be a callable")
@@ -103,16 +110,20 @@
             # We've entered some text and no space, give completions for the
             # current word.
             incomplete = args.pop()
         else:
             # We've not entered anything, either at all or for the current
             # command, so give all relevant completions for this context.
             incomplete = ""
-
-        ctx = click._bashcomplete.resolve_ctx(self.cli, "", args)
+        # Resolve context based on click version
+        if HAS_C8:
+            ctx = click.shell_completion._resolve_context(self.cli, {}, "", args)
+        else: 
+            ctx = click._bashcomplete.resolve_ctx(self.cli, "", args)
+            
         if ctx is None:
             return
 
         choices = []
         for param in ctx.command.params:
             if isinstance(param, click.Option):
                 for options in (param.opts, param.secondary_opts):
```

### Comparing `click-repl-0.1.6/setup.py` & `click-repl-0.2.0/setup.py`

 * *Files identical despite different names*

