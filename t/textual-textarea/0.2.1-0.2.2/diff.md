# Comparing `tmp/textual_textarea-0.2.1.tar.gz` & `tmp/textual_textarea-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textual_textarea-0.2.1.tar", max compression
+gzip compressed data, was "textual_textarea-0.2.2.tar", max compression
```

## Comparing `textual_textarea-0.2.1.tar` & `textual_textarea-0.2.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1068 2023-06-15 16:37:30.880553 textual_textarea-0.2.1/LICENSE
--rw-r--r--   0        0        0     3615 2023-06-15 16:37:30.880553 textual_textarea-0.2.1/README.md
--rw-r--r--   0        0        0     1551 2023-06-15 16:37:30.880553 textual_textarea-0.2.1/pyproject.toml
--rw-r--r--   0        0        0       71 2023-06-15 16:37:30.880553 textual_textarea-0.2.1/src/textual_textarea/__init__.py
--rw-r--r--   0        0        0      491 2023-06-15 16:37:30.880553 textual_textarea-0.2.1/src/textual_textarea/__main__.py
--rw-r--r--   0        0        0      175 2023-06-15 16:37:30.880553 textual_textarea-0.2.1/src/textual_textarea/cancellable_input.py
--rw-r--r--   0        0        0     1028 2023-06-15 16:37:30.880553 textual_textarea-0.2.1/src/textual_textarea/colors.py
--rw-r--r--   0        0        0     1091 2023-06-15 16:37:30.880553 textual_textarea-0.2.1/src/textual_textarea/containers.py
--rw-r--r--   0        0        0     2021 2023-06-15 16:37:30.880553 textual_textarea-0.2.1/src/textual_textarea/error_modal.py
--rw-r--r--   0        0        0     3212 2023-06-15 16:37:30.880553 textual_textarea-0.2.1/src/textual_textarea/key_handlers.py
--rw-r--r--   0        0        0      681 2023-06-15 16:37:30.880553 textual_textarea-0.2.1/src/textual_textarea/messages.py
--rw-r--r--   0        0        0        0 2023-06-15 16:37:30.880553 textual_textarea-0.2.1/src/textual_textarea/py.typed
--rw-r--r--   0        0        0      450 2023-06-15 16:37:30.880553 textual_textarea-0.2.1/src/textual_textarea/serde.py
--rw-r--r--   0        0        0    25778 2023-06-15 16:37:30.880553 textual_textarea-0.2.1/src/textual_textarea/textarea.py
--rw-r--r--   0        0        0     4532 1970-01-01 00:00:00.000000 textual_textarea-0.2.1/setup.py
--rw-r--r--   0        0        0     4413 1970-01-01 00:00:00.000000 textual_textarea-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-06-15 18:38:15.941105 textual_textarea-0.2.2/LICENSE
+-rw-r--r--   0        0        0     4020 2023-06-15 18:38:15.941105 textual_textarea-0.2.2/README.md
+-rw-r--r--   0        0        0     1555 2023-06-15 18:38:15.941105 textual_textarea-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0       71 2023-06-15 18:38:15.941105 textual_textarea-0.2.2/src/textual_textarea/__init__.py
+-rw-r--r--   0        0        0      491 2023-06-15 18:38:15.941105 textual_textarea-0.2.2/src/textual_textarea/__main__.py
+-rw-r--r--   0        0        0      175 2023-06-15 18:38:15.941105 textual_textarea-0.2.2/src/textual_textarea/cancellable_input.py
+-rw-r--r--   0        0        0     1028 2023-06-15 18:38:15.941105 textual_textarea-0.2.2/src/textual_textarea/colors.py
+-rw-r--r--   0        0        0     1091 2023-06-15 18:38:15.941105 textual_textarea-0.2.2/src/textual_textarea/containers.py
+-rw-r--r--   0        0        0     2021 2023-06-15 18:38:15.941105 textual_textarea-0.2.2/src/textual_textarea/error_modal.py
+-rw-r--r--   0        0        0     3212 2023-06-15 18:38:15.941105 textual_textarea-0.2.2/src/textual_textarea/key_handlers.py
+-rw-r--r--   0        0        0      681 2023-06-15 18:38:15.941105 textual_textarea-0.2.2/src/textual_textarea/messages.py
+-rw-r--r--   0        0        0        0 2023-06-15 18:38:15.941105 textual_textarea-0.2.2/src/textual_textarea/py.typed
+-rw-r--r--   0        0        0      450 2023-06-15 18:38:15.941105 textual_textarea-0.2.2/src/textual_textarea/serde.py
+-rw-r--r--   0        0        0    26349 2023-06-15 18:38:15.941105 textual_textarea-0.2.2/src/textual_textarea/textarea.py
+-rw-r--r--   0        0        0     4950 1970-01-01 00:00:00.000000 textual_textarea-0.2.2/setup.py
+-rw-r--r--   0        0        0     4818 1970-01-01 00:00:00.000000 textual_textarea-0.2.2/PKG-INFO
```

### Comparing `textual_textarea-0.2.1/LICENSE` & `textual_textarea-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `textual_textarea-0.2.1/README.md` & `textual_textarea-0.2.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -59,14 +59,27 @@
 
 ```python
 ta = self.query_one(TextArea)
 old_text = ta.text
 ta.text = "New Text!\n\nMany Lines!"
 ```
 
+
+#### Getting and Setting The Cursor Position
+
+The TextArea exposes a `cursor` property that returns a NamedTuple with the position of the cursor. The tuple is (line_number, x_pos):
+
+```python
+ta = self.query_one(TextArea)
+old_cursor = ta.cursor
+ta.cursor = (999, 0)  # the cursor will move as close to line 999, pos 0 as possible
+cursor_line_number = ta.cursor.lno
+cursor_x_position = ta.cursor.pos
+```
+
 #### Getting Theme Colors
 
 If you would like the rest of your app to match the colors from the TextArea's theme, they are exposed via the `theme_colors` property.
 
 ```python
 ta = self.query_one(TextArea)
 color = ta.theme_colors.contrast_text_color
```

### Comparing `textual_textarea-0.2.1/pyproject.toml` & `textual_textarea-0.2.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "textual-textarea"
-version = "0.2.1"
+version = "0.2.2"
 description = "A text area (multi-line input) with syntax highlighting for Textual"
 authors = ["Ted Conbeer <tconbeer@users.noreply.github.com>"]
 license = "MIT"
 homepage = "https://github.com/tconbeer/textual-textarea"
 repository = "https://github.com/tconbeer/textual-textarea"
 readme = "README.md"
 packages = [{ include = "textual_textarea", from = "src" }]
@@ -36,15 +36,15 @@
 
 [tool.mypy]
 python_version = "3.11"
 files = [
     "src/textual_textarea/**/*.py",
     "tests/**/*.py",
 ]
-mypy_path = "stubs"
+mypy_path = "src:stubs"
 
 show_column_numbers = true
 
 # show error messages from unrelated files
 follow_imports = "normal"
 
 # be strict
```

### Comparing `textual_textarea-0.2.1/src/textual_textarea/colors.py` & `textual_textarea-0.2.2/src/textual_textarea/colors.py`

 * *Files identical despite different names*

### Comparing `textual_textarea-0.2.1/src/textual_textarea/containers.py` & `textual_textarea-0.2.2/src/textual_textarea/containers.py`

 * *Files identical despite different names*

### Comparing `textual_textarea-0.2.1/src/textual_textarea/error_modal.py` & `textual_textarea-0.2.2/src/textual_textarea/error_modal.py`

 * *Files identical despite different names*

### Comparing `textual_textarea-0.2.1/src/textual_textarea/key_handlers.py` & `textual_textarea-0.2.2/src/textual_textarea/key_handlers.py`

 * *Files identical despite different names*

### Comparing `textual_textarea-0.2.1/src/textual_textarea/messages.py` & `textual_textarea-0.2.2/src/textual_textarea/messages.py`

 * *Files identical despite different names*

### Comparing `textual_textarea-0.2.1/src/textual_textarea/textarea.py` & `textual_textarea-0.2.2/src/textual_textarea/textarea.py`

 * *Files 2% similar despite different names*

```diff
@@ -522,76 +522,91 @@
 
     @property
     def text(self) -> str:
         """
         Returns:
             (str) The contents of the TextArea.
         """
-        editor = self.query_one(TextInput)
-        return serialize_lines(editor.lines)
+        return serialize_lines(self.text_input.lines)
 
     @text.setter
     def text(self, contents: str) -> None:
         """
         Args:
             contents (str): A string (optionally containing newlines) to
                 set the contents of the TextArea equal to.
         """
-        editor = self.query_one(TextInput)
-        editor.move_cursor(0, 0)
-        editor.lines = deserialize_lines(contents)
+        self.text_input.move_cursor(0, 0)
+        self.text_input.lines = deserialize_lines(contents)
+
+    @property
+    def cursor(self) -> Cursor:
+        """
+        Returns
+            Cursor: The location of the cursor in the TextInput
+        """
+        return self.text_input.cursor
+
+    @cursor.setter
+    def cursor(self, cursor: Union[Cursor, Tuple[int, int]]) -> None:
+        """
+        Args:
+            cursor (Union[Cursor, Tuple[int, int]]): The position (line number, pos)
+            to move the cursor to
+        """
+        self.text_input.move_cursor(cursor[1], cursor[0])
 
     def compose(self) -> ComposeResult:
         with TextContainer():
             yield TextInput(
                 language=self.language, theme=self.theme, theme_colors=self.theme_colors
             )
         yield FooterContainer(theme_colors=self.theme_colors)
 
     def on_mount(self) -> None:
         self.styles.background = self.theme_colors.bgcolor
+        self.text_container = self.query_one(TextContainer)
+        self.text_input = self.query_one(TextInput)
+        self.footer = self.query_one(FooterContainer)
 
     def on_focus(self) -> None:
-        input = self.query_one(TextInput)
-        input.focus()
+        self.text_input.focus()
 
     def action_save(self) -> None:
         self._mount_footer_input("save")
 
     def action_load(self) -> None:
         self._mount_footer_input("open")
 
     def _mount_footer_input(self, name: str) -> None:
-        footer = self.query_one(FooterContainer)
         input = CancellableInput(
             id=f"textarea__{name}_input",
             placeholder=f"{name.capitalize()}: Enter file path OR press ESC to cancel",
         )
         input.styles.background = self.theme_colors.bgcolor
         input.styles.border = "round", self.theme_colors.contrast_text_color
         input.styles.color = self.theme_colors.contrast_text_color
-        footer.mount(input)
+        self.footer.mount(input)
         input.focus()
 
     def on_click(self, event: events.Click) -> None:
         """
         Moves the cursor to the click.
         """
-        input = self.query_one(TextInput)
-        input.cursor_visible = True
-        input.blink_timer.reset()
-        input.move_cursor(event.x - 1, event.y)
-        input.focus()
+        self.text_input.cursor_visible = True
+        self.text_input.blink_timer.reset()
+        self.text_input.move_cursor(event.x - 1, event.y)
+        self.text_input.focus()
 
-    def on_cursor_moved(self, event: TextAreaCursorMoved) -> None:
+    def on_text_area_cursor_moved(self, event: TextAreaCursorMoved) -> None:
         """
         Scrolls the container so the cursor is visible.
         """
         event.stop()
-        container = self.query_one(TextContainer)
+        container = self.text_container
         x_buffer = container.window_region.width // 4
         y_buffer = container.window_region.height // 4
         if event.cursor_x < container.window_region.x + x_buffer:  # scroll left
             container.scroll_to(event.cursor_x - x_buffer, container.window_region.y)
         elif (
             event.cursor_x
             >= container.window_region.x + container.window_region.width - x_buffer
@@ -606,21 +621,22 @@
             event.cursor_y
             >= container.window_region.y + container.window_region.height - y_buffer
         ):  # scroll down
             container.scroll_to(
                 container.window_region.x,
                 event.cursor_y - container.window_region.height + y_buffer,
             )
+        self.text_input.update(self.text_input._content)
 
-    def on_scroll_one(self, event: TextAreaScrollOne) -> None:
+    def on_text_area_scroll_one(self, event: TextAreaScrollOne) -> None:
         event.stop()
         offset = 1 if event.direction == "down" else -1
-        container = self.query_one(TextContainer)
-        container.scroll_to(
-            container.window_region.x, container.window_region.y + offset
+        self.text_container.scroll_to(
+            self.text_container.window_region.x,
+            self.text_container.window_region.y + offset,
         )
 
     def on_input_submitted(self, message: Input.Submitted) -> None:
         """
         Handle the submit event for the Save and Open modals.
         """
         if message.input.id == "textarea__save_input":
@@ -650,10 +666,9 @@
                         ),
                         error=e,
                     )
                 )
             else:
                 self.text = contents
         message.input.remove()
-        input = self.query_one(TextInput)
-        input.update(input._content)
-        input.focus()
+        self.text_input.update(self.text_input._content)
+        self.text_input.focus()
```

### Comparing `textual_textarea-0.2.1/setup.py` & `textual_textarea-0.2.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 {'': ['*']}
 
 install_requires = \
 ['pyperclip>=1.8.2,<2.0.0', 'textual>=0.21.0,<1.0.0']
 
 setup_kwargs = {
     'name': 'textual-textarea',
-    'version': '0.2.1',
+    'version': '0.2.2',
     'description': 'A text area (multi-line input) with syntax highlighting for Textual',
-    'long_description': '# Textual Textarea\n![Textual Textarea Screenshot](textarea.png)\n\n## Installation\n\n```\npip install textual-textarea\n```\n\n## Features\nFull-featured text editor experience with VS-Code-like bindings, in your Textual App:\n- Syntax highlighting and support for themes.\n- Move cursor and scroll with mouse or keys (including <kbd>ctrl+arrow</kbd>, <kbd>PgUp/Dn</kbd>,  <kbd>Home/End</kbd>).\n- Select text using <kbd>shift</kbd>.\n- Open (<kbd>ctrl+o</kbd>) and save (<kbd>ctrl+s</kbd>) files.\n- Cut (<kbd>ctrl+x</kbd>), copy (<kbd>ctrl+c</kbd>), paste (<kbd>ctrl+u/v</kbd>), optionally using the system clipboard.\n- Comment selections with <kbd>ctrl+/</kbd>.\n- Indent and dedent (optionally for a multiline selection) to tab stops with <kbd>Tab</kbd> and <kbd>shift+Tab</kbd>.\n- Automatic completions of quotes and brackets.\n- Quit with <kbd>ctrl+q</kbd>.\n\n## Usage\n\n### Initializing the Widget\n\nThe TextArea is a Textual Widget. You can add it to a Textual\napp using `compose` or `mount`:\n\n```python\nfrom textual_textarea import TextArea\nfrom textual.app import App, ComposeResult\n\nclass TextApp(App, inherit_bindings=False):\n    def compose(self) -> ComposeResult:\n        yield TextArea(language="python", theme="solarized-dark")\n\n    def on_mount(self) -> None:\n        ta = self.query_one(TextArea)\n        ta.focus()\n\napp = TextApp()\napp.run()\n```\n\nIn addition to the standard Widget arguments, TextArea accepts three additional, optional arguments when initializing the widget:\n\n- language (str): Must be `None` or the short name of a [Pygments lexer](https://pygments.org/docs/lexers/), e.g., `python`, `sql`, `as3`. Defaults to `None`.\n- theme (str): Must be name of a [Pygments style](https://pygments.org/styles/), e.g., `bw`, `github-dark`, `solarized-light`. Defaults to `monokai`.\n- use_system_clipboard (bool): Set to `False` to make the TextArea\'s copy and paste operations ignore the system clipboard. Defaults to `True`.\n\nThe TextArea supports many actions and key bindings. **For proper binding of `ctrl+c` to the COPY action,\nyou must initialize your App with `inherit_bindings=False`** (as shown above), so that `ctrl+c` does not quit the app. The TextArea implements `ctrl+q` as quit; you way wish to mimic that in your app so that other in-focus widgets use the same behavior.\n\n### Interacting with the Widget\n\n#### Getting and Setting Text\n\nThe TextArea exposes a `text` property that contains the full text contained in the widget. You can retrieve or set the text by interacting with this property:\n\n```python\nta = self.query_one(TextArea)\nold_text = ta.text\nta.text = "New Text!\\n\\nMany Lines!"\n```\n\n#### Getting Theme Colors\n\nIf you would like the rest of your app to match the colors from the TextArea\'s theme, they are exposed via the `theme_colors` property.\n\n```python\nta = self.query_one(TextArea)\ncolor = ta.theme_colors.contrast_text_color\nbgcolor = ta.theme_colors.bgcolor\nhighlight = ta.theme_colors.selection_bgcolor\n```\n\n\n#### Adding Bindings and other Behavior\n\nYou can subclass TextArea to add your own behavior. This snippet adds an action that posts a Submitted message containing the text of the TextArea when the user presses <kbd>ctrl+j</kbd>:\n\n```python\nfrom textual.message import Message\nfrom textual_textarea import TextArea\n\n\nclass CodeEditor(TextArea):\n    BINDINGS = [\n        ("ctrl+j", "submit", "Run Query"),\n    ]\n\n    class Submitted(Message, bubble=True):\n        def __init__(self, text: str) -> None:\n            super().__init__()\n            self.text = text\n\n    async def action_submit(self) -> None:\n        self.post_message(self.Submitted(self.text))\n```',
+    'long_description': '# Textual Textarea\n![Textual Textarea Screenshot](textarea.png)\n\n## Installation\n\n```\npip install textual-textarea\n```\n\n## Features\nFull-featured text editor experience with VS-Code-like bindings, in your Textual App:\n- Syntax highlighting and support for themes.\n- Move cursor and scroll with mouse or keys (including <kbd>ctrl+arrow</kbd>, <kbd>PgUp/Dn</kbd>,  <kbd>Home/End</kbd>).\n- Select text using <kbd>shift</kbd>.\n- Open (<kbd>ctrl+o</kbd>) and save (<kbd>ctrl+s</kbd>) files.\n- Cut (<kbd>ctrl+x</kbd>), copy (<kbd>ctrl+c</kbd>), paste (<kbd>ctrl+u/v</kbd>), optionally using the system clipboard.\n- Comment selections with <kbd>ctrl+/</kbd>.\n- Indent and dedent (optionally for a multiline selection) to tab stops with <kbd>Tab</kbd> and <kbd>shift+Tab</kbd>.\n- Automatic completions of quotes and brackets.\n- Quit with <kbd>ctrl+q</kbd>.\n\n## Usage\n\n### Initializing the Widget\n\nThe TextArea is a Textual Widget. You can add it to a Textual\napp using `compose` or `mount`:\n\n```python\nfrom textual_textarea import TextArea\nfrom textual.app import App, ComposeResult\n\nclass TextApp(App, inherit_bindings=False):\n    def compose(self) -> ComposeResult:\n        yield TextArea(language="python", theme="solarized-dark")\n\n    def on_mount(self) -> None:\n        ta = self.query_one(TextArea)\n        ta.focus()\n\napp = TextApp()\napp.run()\n```\n\nIn addition to the standard Widget arguments, TextArea accepts three additional, optional arguments when initializing the widget:\n\n- language (str): Must be `None` or the short name of a [Pygments lexer](https://pygments.org/docs/lexers/), e.g., `python`, `sql`, `as3`. Defaults to `None`.\n- theme (str): Must be name of a [Pygments style](https://pygments.org/styles/), e.g., `bw`, `github-dark`, `solarized-light`. Defaults to `monokai`.\n- use_system_clipboard (bool): Set to `False` to make the TextArea\'s copy and paste operations ignore the system clipboard. Defaults to `True`.\n\nThe TextArea supports many actions and key bindings. **For proper binding of `ctrl+c` to the COPY action,\nyou must initialize your App with `inherit_bindings=False`** (as shown above), so that `ctrl+c` does not quit the app. The TextArea implements `ctrl+q` as quit; you way wish to mimic that in your app so that other in-focus widgets use the same behavior.\n\n### Interacting with the Widget\n\n#### Getting and Setting Text\n\nThe TextArea exposes a `text` property that contains the full text contained in the widget. You can retrieve or set the text by interacting with this property:\n\n```python\nta = self.query_one(TextArea)\nold_text = ta.text\nta.text = "New Text!\\n\\nMany Lines!"\n```\n\n\n#### Getting and Setting The Cursor Position\n\nThe TextArea exposes a `cursor` property that returns a NamedTuple with the position of the cursor. The tuple is (line_number, x_pos):\n\n```python\nta = self.query_one(TextArea)\nold_cursor = ta.cursor\nta.cursor = (999, 0)  # the cursor will move as close to line 999, pos 0 as possible\ncursor_line_number = ta.cursor.lno\ncursor_x_position = ta.cursor.pos\n```\n\n#### Getting Theme Colors\n\nIf you would like the rest of your app to match the colors from the TextArea\'s theme, they are exposed via the `theme_colors` property.\n\n```python\nta = self.query_one(TextArea)\ncolor = ta.theme_colors.contrast_text_color\nbgcolor = ta.theme_colors.bgcolor\nhighlight = ta.theme_colors.selection_bgcolor\n```\n\n\n#### Adding Bindings and other Behavior\n\nYou can subclass TextArea to add your own behavior. This snippet adds an action that posts a Submitted message containing the text of the TextArea when the user presses <kbd>ctrl+j</kbd>:\n\n```python\nfrom textual.message import Message\nfrom textual_textarea import TextArea\n\n\nclass CodeEditor(TextArea):\n    BINDINGS = [\n        ("ctrl+j", "submit", "Run Query"),\n    ]\n\n    class Submitted(Message, bubble=True):\n        def __init__(self, text: str) -> None:\n            super().__init__()\n            self.text = text\n\n    async def action_submit(self) -> None:\n        self.post_message(self.Submitted(self.text))\n```',
     'author': 'Ted Conbeer',
     'author_email': 'tconbeer@users.noreply.github.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/tconbeer/textual-textarea',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `textual_textarea-0.2.1/PKG-INFO` & `textual_textarea-0.2.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textual-textarea
-Version: 0.2.1
+Version: 0.2.2
 Summary: A text area (multi-line input) with syntax highlighting for Textual
 Home-page: https://github.com/tconbeer/textual-textarea
 License: MIT
 Author: Ted Conbeer
 Author-email: tconbeer@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -79,14 +79,27 @@
 
 ```python
 ta = self.query_one(TextArea)
 old_text = ta.text
 ta.text = "New Text!\n\nMany Lines!"
 ```
 
+
+#### Getting and Setting The Cursor Position
+
+The TextArea exposes a `cursor` property that returns a NamedTuple with the position of the cursor. The tuple is (line_number, x_pos):
+
+```python
+ta = self.query_one(TextArea)
+old_cursor = ta.cursor
+ta.cursor = (999, 0)  # the cursor will move as close to line 999, pos 0 as possible
+cursor_line_number = ta.cursor.lno
+cursor_x_position = ta.cursor.pos
+```
+
 #### Getting Theme Colors
 
 If you would like the rest of your app to match the colors from the TextArea's theme, they are exposed via the `theme_colors` property.
 
 ```python
 ta = self.query_one(TextArea)
 color = ta.theme_colors.contrast_text_color
```

