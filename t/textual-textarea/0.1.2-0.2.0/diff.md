# Comparing `tmp/textual_textarea-0.1.2.tar.gz` & `tmp/textual_textarea-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textual_textarea-0.1.2.tar", max compression
+gzip compressed data, was "textual_textarea-0.2.0.tar", max compression
```

## Comparing `textual_textarea-0.1.2.tar` & `textual_textarea-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,16 @@
--rw-r--r--   0        0        0     1068 2023-06-01 15:55:25.580012 textual_textarea-0.1.2/LICENSE
--rw-r--r--   0        0        0     2058 2023-06-01 15:55:25.580012 textual_textarea-0.1.2/README.md
--rw-r--r--   0        0        0     1510 2023-06-01 15:55:25.584012 textual_textarea-0.1.2/pyproject.toml
--rw-r--r--   0        0        0       71 2023-06-01 15:55:25.584012 textual_textarea-0.1.2/src/textual_textarea/__init__.py
--rw-r--r--   0        0        0      175 2023-06-01 15:55:25.584012 textual_textarea-0.1.2/src/textual_textarea/cancellable_input.py
--rw-r--r--   0        0        0     1028 2023-06-01 15:55:25.584012 textual_textarea-0.1.2/src/textual_textarea/colors.py
--rw-r--r--   0        0        0     1091 2023-06-01 15:55:25.584012 textual_textarea-0.1.2/src/textual_textarea/containers.py
--rw-r--r--   0        0        0     2021 2023-06-01 15:55:25.584012 textual_textarea-0.1.2/src/textual_textarea/error_modal.py
--rw-r--r--   0        0        0     3212 2023-06-01 15:55:25.584012 textual_textarea-0.1.2/src/textual_textarea/key_handlers.py
--rw-r--r--   0        0        0      681 2023-06-01 15:55:25.584012 textual_textarea-0.1.2/src/textual_textarea/messages.py
--rw-r--r--   0        0        0        0 2023-06-01 15:55:25.584012 textual_textarea-0.1.2/src/textual_textarea/py.typed
--rw-r--r--   0        0        0    25314 2023-06-01 15:55:25.584012 textual_textarea-0.1.2/src/textual_textarea/textarea.py
--rw-r--r--   0        0        0     2911 1970-01-01 00:00:00.000000 textual_textarea-0.1.2/setup.py
--rw-r--r--   0        0        0     2814 1970-01-01 00:00:00.000000 textual_textarea-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-06-14 23:08:58.058305 textual_textarea-0.2.0/LICENSE
+-rw-r--r--   0        0        0     3615 2023-06-14 23:08:58.058305 textual_textarea-0.2.0/README.md
+-rw-r--r--   0        0        0     1551 2023-06-14 23:08:58.058305 textual_textarea-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       71 2023-06-14 23:08:58.058305 textual_textarea-0.2.0/src/textual_textarea/__init__.py
+-rw-r--r--   0        0        0      491 2023-06-14 23:08:58.058305 textual_textarea-0.2.0/src/textual_textarea/__main__.py
+-rw-r--r--   0        0        0      175 2023-06-14 23:08:58.058305 textual_textarea-0.2.0/src/textual_textarea/cancellable_input.py
+-rw-r--r--   0        0        0     1028 2023-06-14 23:08:58.058305 textual_textarea-0.2.0/src/textual_textarea/colors.py
+-rw-r--r--   0        0        0     1091 2023-06-14 23:08:58.058305 textual_textarea-0.2.0/src/textual_textarea/containers.py
+-rw-r--r--   0        0        0     2021 2023-06-14 23:08:58.058305 textual_textarea-0.2.0/src/textual_textarea/error_modal.py
+-rw-r--r--   0        0        0     3212 2023-06-14 23:08:58.062305 textual_textarea-0.2.0/src/textual_textarea/key_handlers.py
+-rw-r--r--   0        0        0      681 2023-06-14 23:08:58.062305 textual_textarea-0.2.0/src/textual_textarea/messages.py
+-rw-r--r--   0        0        0        0 2023-06-14 23:08:58.062305 textual_textarea-0.2.0/src/textual_textarea/py.typed
+-rw-r--r--   0        0        0      449 2023-06-14 23:08:58.066305 textual_textarea-0.2.0/src/textual_textarea/serde.py
+-rw-r--r--   0        0        0    25677 2023-06-14 23:08:58.066305 textual_textarea-0.2.0/src/textual_textarea/textarea.py
+-rw-r--r--   0        0        0     4532 1970-01-01 00:00:00.000000 textual_textarea-0.2.0/setup.py
+-rw-r--r--   0        0        0     4413 1970-01-01 00:00:00.000000 textual_textarea-0.2.0/PKG-INFO
```

### Comparing `textual_textarea-0.1.2/LICENSE` & `textual_textarea-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `textual_textarea-0.1.2/pyproject.toml` & `textual_textarea-0.2.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "textual-textarea"
-version = "0.1.2"
+version = "0.2.0"
 description = "A text area (multi-line input) with syntax highlighting for Textual"
 authors = ["Ted Conbeer <tconbeer@users.noreply.github.com>"]
 license = "MIT"
 homepage = "https://github.com/tconbeer/textual-textarea"
 repository = "https://github.com/tconbeer/textual-textarea"
 readme = "README.md"
 packages = [{ include = "textual_textarea", from = "src" }]
@@ -12,22 +12,23 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 textual = ">=0.21.0, <1.0.0"
+pyperclip = "^1.8.2"
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.3.1"
 textual = {version="0.21.0", extras=["dev"]}
 
 [tool.poetry.group.static.dependencies]
 black = "^23.3.0"
-ruff = ">=0.0.264,<0.0.271"
+ruff = ">=0.0.264,<0.0.273"
 mypy = "^1.2.0"
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.3.1"
 pytest-asyncio = "^0.21.0"
 
 [tool.ruff]
@@ -35,14 +36,15 @@
 
 [tool.mypy]
 python_version = "3.11"
 files = [
     "src/textual_textarea/**/*.py",
     "tests/**/*.py",
 ]
+mypy_path = "stubs"
 
 show_column_numbers = true
 
 # show error messages from unrelated files
 follow_imports = "normal"
 
 # be strict
```

### Comparing `textual_textarea-0.1.2/src/textual_textarea/colors.py` & `textual_textarea-0.2.0/src/textual_textarea/colors.py`

 * *Files identical despite different names*

### Comparing `textual_textarea-0.1.2/src/textual_textarea/containers.py` & `textual_textarea-0.2.0/src/textual_textarea/containers.py`

 * *Files identical despite different names*

### Comparing `textual_textarea-0.1.2/src/textual_textarea/error_modal.py` & `textual_textarea-0.2.0/src/textual_textarea/error_modal.py`

 * *Files identical despite different names*

### Comparing `textual_textarea-0.1.2/src/textual_textarea/key_handlers.py` & `textual_textarea-0.2.0/src/textual_textarea/key_handlers.py`

 * *Files identical despite different names*

### Comparing `textual_textarea-0.1.2/src/textual_textarea/messages.py` & `textual_textarea-0.2.0/src/textual_textarea/messages.py`

 * *Files identical despite different names*

### Comparing `textual_textarea-0.1.2/src/textual_textarea/textarea.py` & `textual_textarea-0.2.0/src/textual_textarea/textarea.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from math import ceil, floor
 from typing import List, Tuple, Union
 
+import pyperclip
 from rich.console import RenderableType
 from rich.style import Style
 from rich.syntax import Syntax
 from textual import events
 from textual.app import ComposeResult
 from textual.binding import Binding
 from textual.reactive import reactive
@@ -13,14 +14,15 @@
 
 from textual_textarea.cancellable_input import CancellableInput
 from textual_textarea.colors import WidgetColors
 from textual_textarea.containers import FooterContainer, TextContainer
 from textual_textarea.error_modal import ErrorModal
 from textual_textarea.key_handlers import Cursor, handle_arrow
 from textual_textarea.messages import TextAreaCursorMoved, TextAreaScrollOne
+from textual_textarea.serde import deserialize_lines, serialize_lines
 
 BRACKETS = {
     "(": ")",
     "[": "]",
     "{": "}",
 }
 CLOSERS = {'"': '"', "'": "'", **BRACKETS}
@@ -37,25 +39,28 @@
     """
 
     lines: reactive[List[str]] = reactive(lambda: list(" "))
     cursor: reactive[Cursor] = reactive(Cursor(0, 0))
     selection_anchor: reactive[Union[Cursor, None]] = reactive(None)
     clipboard: List[str] = list()
     cursor_visible: reactive[bool] = reactive(True)
+    use_system_clipboard: bool = True
 
     def __init__(
         self,
         theme_colors: WidgetColors,
         language: Union[str, None] = None,
         theme: str = "monokai",
+        use_system_clipboard: bool = True,
     ) -> None:
         super().__init__()
         self.theme_colors = theme_colors
         self.language = language
         self.theme = theme
+        self.use_system_clipboard = use_system_clipboard
 
     def on_mount(self) -> None:
         self.blink_timer = self.set_interval(
             0.5,
             self._toggle_cursor,
             pause=not self.has_focus,
         )
@@ -72,16 +77,16 @@
         self.update(self._content)
 
     def on_paste(self, event: events.Paste) -> None:
         """
         If the user hits ctrl+v, we don't get that keypress;
         we get a Paste event instead.
 
-        For now, ignore the system clipboard and mimic ctrl+u.
-        Todo: Use the system clipboard for copy/paste.
+        This ignores the contents of the Paste message and mimics the behavior of
+        ctrl+u.
         """
         event.stop()
         self.cursor_visible = True
         self.blink_timer.reset()
         self._insert_clipboard_at_selection(self.selection_anchor, self.cursor)
         self.selection_anchor = None
         self.update(self._content)
@@ -186,14 +191,20 @@
                     [self.lines[self.cursor.lno], ""],
                     Cursor(self.cursor.lno, 0),
                     Cursor(self.cursor.lno, len(self.lines[self.cursor.lno])),
                 )
             lines[-1] = lines[-1][: last.pos]
             lines[0] = lines[0][first.pos :]
             self.clipboard = lines.copy()
+            if self.use_system_clipboard:
+                try:
+                    pyperclip.copy(serialize_lines(self.clipboard))
+                except pyperclip.PyperclipException:
+                    # no system clipboard; common in CI runners
+                    pass
             self.log(f"copied to clipboard: {self.clipboard}")
             if event.key == "ctrl+x":
                 self._delete_selection(first, last)
                 new_lno = min(first.lno, len(self.lines) - 1)
                 self.cursor = Cursor(
                     new_lno, min(first.pos, len(self.lines[new_lno]) - 1)
                 )
@@ -416,14 +427,22 @@
             if cursor.pos == 0
             else Cursor(cursor.lno, cursor.pos + change_at_cursor)
         )
 
     def _insert_clipboard_at_selection(
         self, anchor: Union[Cursor, None], cursor: Cursor
     ) -> None:
+        if self.use_system_clipboard:
+            try:
+                sys_clipboard = pyperclip.paste()
+            except pyperclip.PyperclipException:
+                # no system clipboard; common in CI runners
+                pass
+            else:
+                self.clipboard = deserialize_lines(sys_clipboard, trim=True)
         if anchor:
             self._delete_selection(anchor, cursor)
             cursor = self.cursor
         head = self.lines[cursor.lno][: cursor.pos]
         tail = self.lines[cursor.lno][cursor.pos :]
         if (clip_len := len(self.clipboard)) != 0:
             new_lines = self.clipboard.copy()
@@ -477,14 +496,15 @@
         *children: Widget,
         name: Union[str, None] = None,
         id: Union[str, None] = None,
         classes: Union[str, None] = None,
         disabled: bool = False,
         language: Union[str, None] = None,
         theme: str = "monokai",
+        use_system_clipboard: bool = True,
     ) -> None:
         """
         Initializes an instance of a TextArea.
 
         Args:
             (see also textual.widget.Widget)
             language (str): Must be the short name of a Pygments lexer
@@ -494,37 +514,35 @@
         """
         super().__init__(
             *children, name=name, id=id, classes=classes, disabled=disabled
         )
         self.language = language
         self.theme = theme
         self.theme_colors = WidgetColors.from_theme(self.theme)
+        self.use_system_clipboard = use_system_clipboard
 
     @property
     def text(self) -> str:
         """
         Returns:
             (str) The contents of the TextArea.
         """
         editor = self.query_one(TextInput)
-        return "\n".join([line.rstrip() for line in editor.lines])
+        return serialize_lines(editor.lines)
 
     @text.setter
     def text(self, contents: str) -> None:
         """
         Args:
             contents (str): A string (optionally containing newlines) to
                 set the contents of the TextArea equal to.
         """
         editor = self.query_one(TextInput)
         editor.move_cursor(0, 0)
-        if contents:
-            editor.lines = [f"{line} " for line in contents.splitlines()]
-        else:
-            editor.lines = [" "]
+        editor.lines = deserialize_lines(contents)
 
     def compose(self) -> ComposeResult:
         with TextContainer():
             yield TextInput(
                 language=self.language, theme=self.theme, theme_colors=self.theme_colors
             )
         yield FooterContainer(theme_colors=self.theme_colors)
@@ -632,23 +650,7 @@
                         ),
                         error=e,
                     )
                 )
             else:
                 self.text = contents
         message.input.remove()
-
-
-if __name__ == "__main__":
-    from textual.app import App, ComposeResult
-
-    class TextApp(App, inherit_bindings=False):
-        def compose(self) -> ComposeResult:
-            yield TextArea(language="python", theme="github-dark")
-            yield TextArea(language="sql", theme="monokai")
-
-        def on_mount(self) -> None:
-            ta = self.query(TextArea)[0]
-            ta.focus()
-
-    app = TextApp()
-    app.run()
```

### Comparing `textual_textarea-0.1.2/setup.py` & `textual_textarea-0.2.0/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 packages = \
 ['textual_textarea']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['textual>=0.21.0,<1.0.0']
+['pyperclip>=1.8.2,<2.0.0', 'textual>=0.21.0,<1.0.0']
 
 setup_kwargs = {
     'name': 'textual-textarea',
-    'version': '0.1.2',
+    'version': '0.2.0',
     'description': 'A text area (multi-line input) with syntax highlighting for Textual',
-    'long_description': '# Textual Textarea\n\n# Installation\n\n```\npip install textual-textarea\n```\n\n# Usage\n\n## Initializing the Widget\n\nThe TextArea is a Textual Widget. You can add it to a Textual\napp using `compose` or `mount`:\n\n```python\nfrom textual_textarea import TextArea\nfrom textual.app import App, ComposeResult\n\nclass TextApp(App, inherit_bindings=False):\n    def compose(self) -> ComposeResult:\n        yield TextArea(language="python", theme="solarized-dark")\n\n    def on_mount(self) -> None:\n        ta = self.query_one(TextArea)\n        ta.focus()\n\napp = TextApp()\napp.run()\n```\n\nIn addition to the standard Widget arguments, TextArea accepts two additional, optional arguments when initializing the widget:\n\n- language: Must be `None` or the short name of a [Pygments lexer](https://pygments.org/docs/lexers/), e.g., `python`, `sql`, `as3`. Defaults to None.\n- theme: Must be name of a [Pygments style](https://pygments.org/styles/), e.g., `bw`, `github-dark`, `solarized-light`. Defaults to `monokai`.\n\nThe TextArea supports many actions and key bindings. **For proper binding of `ctrl+c` to the COPY action,\nyou must initialize your App with `inherit_bindings=False`** (as shown above), so that `ctrl+c` does not quit the app. The TextArea implements `ctrl+q` as quit; you way wish to mimic that in your app so that other in-focus widgets use the same behavior.\n\n## Interacting with the Widget\n\n### Getting and Setting Text\n\nThe TextArea exposes a `text` property that contains the full text contained in the widget. You can retrieve or set the text by interacting with this property:\n\n```python\nta = self.query_one(TextArea)\nold_text = ta.text\nta.text = "New Text!\\n\\nMany Lines!"\n```\n\n### Getting Theme Colors\n\nIf you would like the rest of your app to match the colors from the TextArea\'s theme, they are exposed via the `theme_colors` property.\n\n```python\nta = self.query_one(TextArea)\ncolor = ta.theme_colors.contrast_text_color\nbgcolor = ta.theme_colors.bgcolor\nhighlight = ta.theme_colors.selection_bgcolor\n```\n\nYou cannot set these colors this way, however.',
+    'long_description': '# Textual Textarea\n![Textual Textarea Screenshot](textarea.png)\n\n## Installation\n\n```\npip install textual-textarea\n```\n\n## Features\nFull-featured text editor experience with VS-Code-like bindings, in your Textual App:\n- Syntax highlighting and support for themes.\n- Move cursor and scroll with mouse or keys (including <kbd>ctrl+arrow</kbd>, <kbd>PgUp/Dn</kbd>,  <kbd>Home/End</kbd>).\n- Select text using <kbd>shift</kbd>.\n- Open (<kbd>ctrl+o</kbd>) and save (<kbd>ctrl+s</kbd>) files.\n- Cut (<kbd>ctrl+x</kbd>), copy (<kbd>ctrl+c</kbd>), paste (<kbd>ctrl+u/v</kbd>), optionally using the system clipboard.\n- Comment selections with <kbd>ctrl+/</kbd>.\n- Indent and dedent (optionally for a multiline selection) to tab stops with <kbd>Tab</kbd> and <kbd>shift+Tab</kbd>.\n- Automatic completions of quotes and brackets.\n- Quit with <kbd>ctrl+q</kbd>.\n\n## Usage\n\n### Initializing the Widget\n\nThe TextArea is a Textual Widget. You can add it to a Textual\napp using `compose` or `mount`:\n\n```python\nfrom textual_textarea import TextArea\nfrom textual.app import App, ComposeResult\n\nclass TextApp(App, inherit_bindings=False):\n    def compose(self) -> ComposeResult:\n        yield TextArea(language="python", theme="solarized-dark")\n\n    def on_mount(self) -> None:\n        ta = self.query_one(TextArea)\n        ta.focus()\n\napp = TextApp()\napp.run()\n```\n\nIn addition to the standard Widget arguments, TextArea accepts three additional, optional arguments when initializing the widget:\n\n- language (str): Must be `None` or the short name of a [Pygments lexer](https://pygments.org/docs/lexers/), e.g., `python`, `sql`, `as3`. Defaults to `None`.\n- theme (str): Must be name of a [Pygments style](https://pygments.org/styles/), e.g., `bw`, `github-dark`, `solarized-light`. Defaults to `monokai`.\n- use_system_clipboard (bool): Set to `False` to make the TextArea\'s copy and paste operations ignore the system clipboard. Defaults to `True`.\n\nThe TextArea supports many actions and key bindings. **For proper binding of `ctrl+c` to the COPY action,\nyou must initialize your App with `inherit_bindings=False`** (as shown above), so that `ctrl+c` does not quit the app. The TextArea implements `ctrl+q` as quit; you way wish to mimic that in your app so that other in-focus widgets use the same behavior.\n\n### Interacting with the Widget\n\n#### Getting and Setting Text\n\nThe TextArea exposes a `text` property that contains the full text contained in the widget. You can retrieve or set the text by interacting with this property:\n\n```python\nta = self.query_one(TextArea)\nold_text = ta.text\nta.text = "New Text!\\n\\nMany Lines!"\n```\n\n#### Getting Theme Colors\n\nIf you would like the rest of your app to match the colors from the TextArea\'s theme, they are exposed via the `theme_colors` property.\n\n```python\nta = self.query_one(TextArea)\ncolor = ta.theme_colors.contrast_text_color\nbgcolor = ta.theme_colors.bgcolor\nhighlight = ta.theme_colors.selection_bgcolor\n```\n\n\n#### Adding Bindings and other Behavior\n\nYou can subclass TextArea to add your own behavior. This snippet adds an action that posts a Submitted message containing the text of the TextArea when the user presses <kbd>ctrl+j</kbd>:\n\n```python\nfrom textual.message import Message\nfrom textual_textarea import TextArea\n\n\nclass CodeEditor(TextArea):\n    BINDINGS = [\n        ("ctrl+j", "submit", "Run Query"),\n    ]\n\n    class Submitted(Message, bubble=True):\n        def __init__(self, text: str) -> None:\n            super().__init__()\n            self.text = text\n\n    async def action_submit(self) -> None:\n        self.post_message(self.Submitted(self.text))\n```',
     'author': 'Ted Conbeer',
     'author_email': 'tconbeer@users.noreply.github.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/tconbeer/textual-textarea',
     'package_dir': package_dir,
     'packages': packages,
```

