# Comparing `tmp/pytextcon-0.1.tar.gz` & `tmp/pytextcon-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytextcon-0.1.tar", last modified: Thu Jun 15 02:45:28 2023, max compression
+gzip compressed data, was "pytextcon-0.1.1.tar", last modified: Thu Jun 15 02:54:42 2023, max compression
```

## Comparing `pytextcon-0.1.tar` & `pytextcon-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 02:45:28.095395 pytextcon-0.1/
--rw-rw-rw-   0        0        0     1069 2023-06-04 20:53:32.000000 pytextcon-0.1/LICENSE
--rw-rw-rw-   0        0        0     2021 2023-06-15 02:45:28.094258 pytextcon-0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1343 2023-06-15 01:14:37.000000 pytextcon-0.1/README.md
--rw-rw-rw-   0        0        0      693 2023-06-15 02:44:58.000000 pytextcon-0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-15 02:45:28.095714 pytextcon-0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-15 02:45:28.051707 pytextcon-0.1/src/
-drwxrwxrwx   0        0        0        0 2023-06-15 02:45:28.069522 pytextcon-0.1/src/pytextcon/
--rw-rw-rw-   0        0        0        0 2023-06-15 01:18:50.000000 pytextcon-0.1/src/pytextcon/__init__.py
--rw-rw-rw-   0        0        0     3119 2023-06-15 01:32:39.000000 pytextcon-0.1/src/pytextcon/pytextcon.py
-drwxrwxrwx   0        0        0        0 2023-06-15 02:45:28.092199 pytextcon-0.1/src/pytextcon.egg-info/
--rw-rw-rw-   0        0        0     2021 2023-06-15 02:45:28.000000 pytextcon-0.1/src/pytextcon.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      233 2023-06-15 02:45:28.000000 pytextcon-0.1/src/pytextcon.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 02:45:28.000000 pytextcon-0.1/src/pytextcon.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-06-15 02:45:28.000000 pytextcon-0.1/src/pytextcon.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-15 02:54:42.638018 pytextcon-0.1.1/
+-rw-rw-rw-   0        0        0     1069 2023-06-04 20:53:32.000000 pytextcon-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     1997 2023-06-15 02:54:42.635826 pytextcon-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1318 2023-06-15 02:54:10.000000 pytextcon-0.1.1/README.md
+-rw-rw-rw-   0        0        0      695 2023-06-15 02:54:10.000000 pytextcon-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-15 02:54:42.638531 pytextcon-0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-15 02:54:42.603493 pytextcon-0.1.1/src/
+drwxrwxrwx   0        0        0        0 2023-06-15 02:54:42.613738 pytextcon-0.1.1/src/pytextcon/
+-rw-rw-rw-   0        0        0        0 2023-06-15 01:18:50.000000 pytextcon-0.1.1/src/pytextcon/__init__.py
+-rw-rw-rw-   0        0        0     3119 2023-06-15 01:32:39.000000 pytextcon-0.1.1/src/pytextcon/pytextcon.py
+drwxrwxrwx   0        0        0        0 2023-06-15 02:54:42.633767 pytextcon-0.1.1/src/pytextcon.egg-info/
+-rw-rw-rw-   0        0        0     1997 2023-06-15 02:54:42.000000 pytextcon-0.1.1/src/pytextcon.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      233 2023-06-15 02:54:42.000000 pytextcon-0.1.1/src/pytextcon.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 02:54:42.000000 pytextcon-0.1.1/src/pytextcon.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-06-15 02:54:42.000000 pytextcon-0.1.1/src/pytextcon.egg-info/top_level.txt
```

### Comparing `pytextcon-0.1/LICENSE` & `pytextcon-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytextcon-0.1/PKG-INFO` & `pytextcon-0.1.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,43 +1,42 @@
 Metadata-Version: 2.1
 Name: pytextcon
-Version: 0.1
+Version: 0.1.1
 Summary: Simple package to change the text color, text emphasis, and background color of print statements to the console.
 Author-email: Michael <michael.lokrosh@gmail.com>
 Project-URL: GitHub, https://github.com/Lokrosh/pycon_text
 Keywords: print,color,console,text,formatting,emphasis,underline,bright
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# pycon_text
+# pytextcon
 
-PyCon_Text is a lightweight, simple package designed to make basic changes to the text color, text emphasis, and background color of print statements to the console simple.
+pytextcon is a lightweight, simple package designed to make basic changes to the text color, text emphasis, and background color of print statements to the console simple.
 ## Getting Started
-Download pycon_text:
+Download pytextcon:
 ```pycon
-pip install pycon_text
+pip install pytextcon
 ```
 ## Usage
 Use an f-string to include text formatting to print statements. Formatting will continue 
 until cleared. Use `RESET` to end all formatting. Use `DEFAULT` to clear text color only. 
 ### Example:
 ```Python
-import pycon_text as text
+import pytextcon as text
 
 print(f"{text.BOLD}{text.BLUE}Some text that will be bold and blue.{text.DEFAULT}\
 Some other text that will be bold but not blue")
 
 print(f"{text.UNDERLINE}{text.BLUE}Some text that will be bold, underlined, and blue.\
 {text.RESET}Some other text that will not be bold, underlined or blue")
 ```
-![img.png](img.png)
 
 
 ## Formatting Options
 ### Basic Colors:
 BLACK,
 RED,
 GREEN,
```

### Comparing `pytextcon-0.1/README.md` & `pytextcon-0.1.1/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,29 +1,28 @@
-# pycon_text
+# pytextcon
 
-PyCon_Text is a lightweight, simple package designed to make basic changes to the text color, text emphasis, and background color of print statements to the console simple.
+pytextcon is a lightweight, simple package designed to make basic changes to the text color, text emphasis, and background color of print statements to the console simple.
 ## Getting Started
-Download pycon_text:
+Download pytextcon:
 ```pycon
-pip install pycon_text
+pip install pytextcon
 ```
 ## Usage
 Use an f-string to include text formatting to print statements. Formatting will continue 
 until cleared. Use `RESET` to end all formatting. Use `DEFAULT` to clear text color only. 
 ### Example:
 ```Python
-import pycon_text as text
+import pytextcon as text
 
 print(f"{text.BOLD}{text.BLUE}Some text that will be bold and blue.{text.DEFAULT}\
 Some other text that will be bold but not blue")
 
 print(f"{text.UNDERLINE}{text.BLUE}Some text that will be bold, underlined, and blue.\
 {text.RESET}Some other text that will not be bold, underlined or blue")
 ```
-![img.png](img.png)
 
 
 ## Formatting Options
 ### Basic Colors:
 BLACK,
 RED,
 GREEN,
```

### Comparing `pytextcon-0.1/pyproject.toml` & `pytextcon-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pytextcon"
-version = "0.1"
+version = "0.1.1"
 authors = [
   { name="Michael", email="michael.lokrosh@gmail.com" },
 ]
 description = "Simple package to change the text color, text emphasis, and background color of print statements to the console."
 readme = "README.md"
 requires-python = ">=3.7"
 keywords = ["print", "color", "console", "text", "formatting", "emphasis", "underline", "bright"]
```

### Comparing `pytextcon-0.1/src/pytextcon/pytextcon.py` & `pytextcon-0.1.1/src/pytextcon/pytextcon.py`

 * *Files identical despite different names*

### Comparing `pytextcon-0.1/src/pytextcon.egg-info/PKG-INFO` & `pytextcon-0.1.1/src/pytextcon.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,43 +1,42 @@
 Metadata-Version: 2.1
 Name: pytextcon
-Version: 0.1
+Version: 0.1.1
 Summary: Simple package to change the text color, text emphasis, and background color of print statements to the console.
 Author-email: Michael <michael.lokrosh@gmail.com>
 Project-URL: GitHub, https://github.com/Lokrosh/pycon_text
 Keywords: print,color,console,text,formatting,emphasis,underline,bright
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# pycon_text
+# pytextcon
 
-PyCon_Text is a lightweight, simple package designed to make basic changes to the text color, text emphasis, and background color of print statements to the console simple.
+pytextcon is a lightweight, simple package designed to make basic changes to the text color, text emphasis, and background color of print statements to the console simple.
 ## Getting Started
-Download pycon_text:
+Download pytextcon:
 ```pycon
-pip install pycon_text
+pip install pytextcon
 ```
 ## Usage
 Use an f-string to include text formatting to print statements. Formatting will continue 
 until cleared. Use `RESET` to end all formatting. Use `DEFAULT` to clear text color only. 
 ### Example:
 ```Python
-import pycon_text as text
+import pytextcon as text
 
 print(f"{text.BOLD}{text.BLUE}Some text that will be bold and blue.{text.DEFAULT}\
 Some other text that will be bold but not blue")
 
 print(f"{text.UNDERLINE}{text.BLUE}Some text that will be bold, underlined, and blue.\
 {text.RESET}Some other text that will not be bold, underlined or blue")
 ```
-![img.png](img.png)
 
 
 ## Formatting Options
 ### Basic Colors:
 BLACK,
 RED,
 GREEN,
```

