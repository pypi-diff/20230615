# Comparing `tmp/textual_textarea-0.1.1.tar.gz` & `tmp/textual_textarea-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textual_textarea-0.1.1.tar", max compression
+gzip compressed data, was "textual_textarea-0.1.2.tar", max compression
```

## Comparing `textual_textarea-0.1.1.tar` & `textual_textarea-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0     1068 2023-06-01 15:08:20.139341 textual_textarea-0.1.1/LICENSE
--rw-r--r--   0        0        0     2058 2023-06-01 15:08:20.139341 textual_textarea-0.1.1/README.md
--rw-r--r--   0        0        0     1496 2023-06-01 15:08:20.143341 textual_textarea-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       71 2023-06-01 15:08:20.143341 textual_textarea-0.1.1/src/textual_textarea/__init__.py
--rw-r--r--   0        0        0      175 2023-06-01 15:08:20.143341 textual_textarea-0.1.1/src/textual_textarea/cancellable_input.py
--rw-r--r--   0        0        0     1028 2023-06-01 15:08:20.143341 textual_textarea-0.1.1/src/textual_textarea/colors.py
--rw-r--r--   0        0        0     1114 2023-06-01 15:08:20.143341 textual_textarea-0.1.1/src/textual_textarea/containers.py
--rw-r--r--   0        0        0     2021 2023-06-01 15:08:20.143341 textual_textarea-0.1.1/src/textual_textarea/error_modal.py
--rw-r--r--   0        0        0     3212 2023-06-01 15:08:20.143341 textual_textarea-0.1.1/src/textual_textarea/key_handlers.py
--rw-r--r--   0        0        0      681 2023-06-01 15:08:20.143341 textual_textarea-0.1.1/src/textual_textarea/messages.py
--rw-r--r--   0        0        0    25158 2023-06-01 15:08:20.143341 textual_textarea-0.1.1/src/textual_textarea/textarea.py
--rw-r--r--   0        0        0     2912 1970-01-01 00:00:00.000000 textual_textarea-0.1.1/setup.py
--rw-r--r--   0        0        0     2815 1970-01-01 00:00:00.000000 textual_textarea-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-06-01 15:55:25.580012 textual_textarea-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2058 2023-06-01 15:55:25.580012 textual_textarea-0.1.2/README.md
+-rw-r--r--   0        0        0     1510 2023-06-01 15:55:25.584012 textual_textarea-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       71 2023-06-01 15:55:25.584012 textual_textarea-0.1.2/src/textual_textarea/__init__.py
+-rw-r--r--   0        0        0      175 2023-06-01 15:55:25.584012 textual_textarea-0.1.2/src/textual_textarea/cancellable_input.py
+-rw-r--r--   0        0        0     1028 2023-06-01 15:55:25.584012 textual_textarea-0.1.2/src/textual_textarea/colors.py
+-rw-r--r--   0        0        0     1091 2023-06-01 15:55:25.584012 textual_textarea-0.1.2/src/textual_textarea/containers.py
+-rw-r--r--   0        0        0     2021 2023-06-01 15:55:25.584012 textual_textarea-0.1.2/src/textual_textarea/error_modal.py
+-rw-r--r--   0        0        0     3212 2023-06-01 15:55:25.584012 textual_textarea-0.1.2/src/textual_textarea/key_handlers.py
+-rw-r--r--   0        0        0      681 2023-06-01 15:55:25.584012 textual_textarea-0.1.2/src/textual_textarea/messages.py
+-rw-r--r--   0        0        0        0 2023-06-01 15:55:25.584012 textual_textarea-0.1.2/src/textual_textarea/py.typed
+-rw-r--r--   0        0        0    25314 2023-06-01 15:55:25.584012 textual_textarea-0.1.2/src/textual_textarea/textarea.py
+-rw-r--r--   0        0        0     2911 1970-01-01 00:00:00.000000 textual_textarea-0.1.2/setup.py
+-rw-r--r--   0        0        0     2814 1970-01-01 00:00:00.000000 textual_textarea-0.1.2/PKG-INFO
```

### Comparing `textual_textarea-0.1.1/LICENSE` & `textual_textarea-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `textual_textarea-0.1.1/README.md` & `textual_textarea-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `textual_textarea-0.1.1/pyproject.toml` & `textual_textarea-0.1.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 [tool.poetry]
 name = "textual-textarea"
-version = "0.1.1"
+version = "0.1.2"
 description = "A text area (multi-line input) with syntax highlighting for Textual"
 authors = ["Ted Conbeer <tconbeer@users.noreply.github.com>"]
 license = "MIT"
 homepage = "https://github.com/tconbeer/textual-textarea"
 repository = "https://github.com/tconbeer/textual-textarea"
 readme = "README.md"
 packages = [{ include = "textual_textarea", from = "src" }]
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-textual = "^0.27.0"
+textual = ">=0.21.0, <1.0.0"
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.3.1"
-textual = {version="*", extras=["dev"]}
+textual = {version="0.21.0", extras=["dev"]}
 
 [tool.poetry.group.static.dependencies]
 black = "^23.3.0"
 ruff = ">=0.0.264,<0.0.271"
 mypy = "^1.2.0"
 
 [tool.poetry.group.test.dependencies]
```

### Comparing `textual_textarea-0.1.1/src/textual_textarea/colors.py` & `textual_textarea-0.1.2/src/textual_textarea/colors.py`

 * *Files identical despite different names*

### Comparing `textual_textarea-0.1.1/src/textual_textarea/containers.py` & `textual_textarea-0.1.2/src/textual_textarea/containers.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,15 +10,14 @@
     ScrollableContainer,
     inherit_bindings=False,
     can_focus=False,
     can_focus_children=True,
 ):
     DEFAULT_CSS = """
         TextContainer {
-            dock: top;
             height: 1fr;
             width: 100%
         }
     """
 
 
 class FooterContainer(
```

### Comparing `textual_textarea-0.1.1/src/textual_textarea/error_modal.py` & `textual_textarea-0.1.2/src/textual_textarea/error_modal.py`

 * *Files identical despite different names*

### Comparing `textual_textarea-0.1.1/src/textual_textarea/key_handlers.py` & `textual_textarea-0.1.2/src/textual_textarea/key_handlers.py`

 * *Files identical despite different names*

### Comparing `textual_textarea-0.1.1/src/textual_textarea/messages.py` & `textual_textarea-0.1.2/src/textual_textarea/messages.py`

 * *Files identical despite different names*

### Comparing `textual_textarea-0.1.1/src/textual_textarea/textarea.py` & `textual_textarea-0.1.2/src/textual_textarea/textarea.py`

 * *Files 0% similar despite different names*

```diff
@@ -449,15 +449,15 @@
         safe_y = min(max_y, y)
         max_x = len(self.lines[safe_y]) - 1
         safe_x = min(max_x, x)
         self.cursor = Cursor(lno=max(0, safe_y), pos=max(0, safe_x))
         self.update(self._content)
 
 
-class TextArea(Widget, can_focus=False, can_focus_children=True):
+class TextArea(Widget, can_focus=True, can_focus_children=False):
     """
     A Widget that presents a feature-rich, multiline text editor interface.
 
     Attributes:
         text (str): The contents of the TextArea
         language (str): Must be the short name of a Pygments lexer
             (https://pygments.org/docs/lexers/), e.g., "python", "sql", "as3".
@@ -528,14 +528,18 @@
                 language=self.language, theme=self.theme, theme_colors=self.theme_colors
             )
         yield FooterContainer(theme_colors=self.theme_colors)
 
     def on_mount(self) -> None:
         self.styles.background = self.theme_colors.bgcolor
 
+    def on_focus(self) -> None:
+        input = self.query_one(TextInput)
+        input.focus()
+
     def action_save(self) -> None:
         self._mount_footer_input("save")
 
     def action_load(self) -> None:
         self._mount_footer_input("open")
 
     def _mount_footer_input(self, name: str) -> None:
@@ -636,14 +640,15 @@
 
 if __name__ == "__main__":
     from textual.app import App, ComposeResult
 
     class TextApp(App, inherit_bindings=False):
         def compose(self) -> ComposeResult:
             yield TextArea(language="python", theme="github-dark")
+            yield TextArea(language="sql", theme="monokai")
 
         def on_mount(self) -> None:
-            ta = self.query_one(TextArea)
+            ta = self.query(TextArea)[0]
             ta.focus()
 
     app = TextApp()
     app.run()
```

### Comparing `textual_textarea-0.1.1/setup.py` & `textual_textarea-0.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,19 +7,19 @@
 packages = \
 ['textual_textarea']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['textual>=0.27.0,<0.28.0']
+['textual>=0.21.0,<1.0.0']
 
 setup_kwargs = {
     'name': 'textual-textarea',
-    'version': '0.1.1',
+    'version': '0.1.2',
     'description': 'A text area (multi-line input) with syntax highlighting for Textual',
     'long_description': '# Textual Textarea\n\n# Installation\n\n```\npip install textual-textarea\n```\n\n# Usage\n\n## Initializing the Widget\n\nThe TextArea is a Textual Widget. You can add it to a Textual\napp using `compose` or `mount`:\n\n```python\nfrom textual_textarea import TextArea\nfrom textual.app import App, ComposeResult\n\nclass TextApp(App, inherit_bindings=False):\n    def compose(self) -> ComposeResult:\n        yield TextArea(language="python", theme="solarized-dark")\n\n    def on_mount(self) -> None:\n        ta = self.query_one(TextArea)\n        ta.focus()\n\napp = TextApp()\napp.run()\n```\n\nIn addition to the standard Widget arguments, TextArea accepts two additional, optional arguments when initializing the widget:\n\n- language: Must be `None` or the short name of a [Pygments lexer](https://pygments.org/docs/lexers/), e.g., `python`, `sql`, `as3`. Defaults to None.\n- theme: Must be name of a [Pygments style](https://pygments.org/styles/), e.g., `bw`, `github-dark`, `solarized-light`. Defaults to `monokai`.\n\nThe TextArea supports many actions and key bindings. **For proper binding of `ctrl+c` to the COPY action,\nyou must initialize your App with `inherit_bindings=False`** (as shown above), so that `ctrl+c` does not quit the app. The TextArea implements `ctrl+q` as quit; you way wish to mimic that in your app so that other in-focus widgets use the same behavior.\n\n## Interacting with the Widget\n\n### Getting and Setting Text\n\nThe TextArea exposes a `text` property that contains the full text contained in the widget. You can retrieve or set the text by interacting with this property:\n\n```python\nta = self.query_one(TextArea)\nold_text = ta.text\nta.text = "New Text!\\n\\nMany Lines!"\n```\n\n### Getting Theme Colors\n\nIf you would like the rest of your app to match the colors from the TextArea\'s theme, they are exposed via the `theme_colors` property.\n\n```python\nta = self.query_one(TextArea)\ncolor = ta.theme_colors.contrast_text_color\nbgcolor = ta.theme_colors.bgcolor\nhighlight = ta.theme_colors.selection_bgcolor\n```\n\nYou cannot set these colors this way, however.',
     'author': 'Ted Conbeer',
     'author_email': 'tconbeer@users.noreply.github.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/tconbeer/textual-textarea',
```

### Comparing `textual_textarea-0.1.1/PKG-INFO` & `textual_textarea-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: textual-textarea
-Version: 0.1.1
+Version: 0.1.2
 Summary: A text area (multi-line input) with syntax highlighting for Textual
 Home-page: https://github.com/tconbeer/textual-textarea
 License: MIT
 Author: Ted Conbeer
 Author-email: tconbeer@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: textual (>=0.27.0,<0.28.0)
+Requires-Dist: textual (>=0.21.0,<1.0.0)
 Project-URL: Repository, https://github.com/tconbeer/textual-textarea
 Description-Content-Type: text/markdown
 
 # Textual Textarea
 
 # Installation
```

