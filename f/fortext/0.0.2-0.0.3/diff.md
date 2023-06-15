# Comparing `tmp/fortext-0.0.2.tar.gz` & `tmp/fortext-0.0.3.tar.gz`

## Comparing `fortext-0.0.2.tar` & `fortext-0.0.3.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 fortext-0.0.2/requirements.txt
--rw-r--r--   0        0        0     4427 2020-02-02 00:00:00.000000 fortext-0.0.2/img/syntax_highlighting.png
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 fortext-0.0.2/src/fortext/__init__.py
--rw-r--r--   0        0        0     3223 2020-02-02 00:00:00.000000 fortext-0.0.2/src/fortext/ansi.py
--rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 fortext-0.0.2/src/fortext/style.py
--rw-r--r--   0        0        0     5878 2020-02-02 00:00:00.000000 fortext-0.0.2/src/fortext/syntax.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 fortext-0.0.2/.gitignore
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 fortext-0.0.2/LICENSE
--rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 fortext-0.0.2/README.md
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 fortext-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     3392 2020-02-02 00:00:00.000000 fortext-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 fortext-0.0.3/requirements.txt
+-rw-r--r--   0        0        0     4427 2020-02-02 00:00:00.000000 fortext-0.0.3/img/syntax_highlighting.png
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 fortext-0.0.3/src/fortext/__init__.py
+-rw-r--r--   0        0        0     3642 2020-02-02 00:00:00.000000 fortext-0.0.3/src/fortext/ansi.py
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 fortext-0.0.3/src/fortext/permutation.py
+-rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 fortext-0.0.3/src/fortext/style.py
+-rw-r--r--   0        0        0     5878 2020-02-02 00:00:00.000000 fortext-0.0.3/src/fortext/syntax.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 fortext-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 fortext-0.0.3/LICENSE
+-rw-r--r--   0        0        0     1963 2020-02-02 00:00:00.000000 fortext-0.0.3/README.md
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 fortext-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     3578 2020-02-02 00:00:00.000000 fortext-0.0.3/PKG-INFO
```

### Comparing `fortext-0.0.2/img/syntax_highlighting.png` & `fortext-0.0.3/img/syntax_highlighting.png`

 * *Files identical despite different names*

### Comparing `fortext-0.0.2/src/fortext/ansi.py` & `fortext-0.0.3/src/fortext/ansi.py`

 * *Files 6% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     DEFAULT = 0
     BOLD = 1
     FAINT = 2
     ITALIC = 3
     UNDERLINE = 4
     BLINK_SLOW = 5
     BLINK_FAST = 6
-    REVERSE = 7
+    INVERT = 7
     HIDE = 8
     STRIKETHROUGH = 9
     DOUBLE_UNDERLINE = 21
     OVERLINE = 53
 
 
 def fg_rgb(rgb_color: Tuple[int, int, int]) -> str:
@@ -139,7 +139,25 @@
         hex_color = hex_color[1:]
 
     r = hex2dec(hex_color[0:2])
     g = hex2dec(hex_color[2:4])
     b = hex2dec(hex_color[4:6])
 
     return (r, g, b)
+
+
+def print_styles(ansi_type: Fg | Bg | Frmt) -> None:
+    """Prints all common ANSI escape codes for a given type.
+    """
+
+    for style in ansi_type:
+        print(f'{ESC}{style.value}mExample Text\t{RESET}({style.name}) ')
+
+
+def print_styles_all() -> None:
+    """Prints all common ANSI escape codes.
+    """
+    print_styles(Fg)
+    print()
+    print_styles(Bg)
+    print()
+    print_styles(Frmt)
```

### Comparing `fortext-0.0.2/src/fortext/style.py` & `fortext-0.0.3/src/fortext/style.py`

 * *Files identical despite different names*

### Comparing `fortext-0.0.2/src/fortext/syntax.py` & `fortext-0.0.3/src/fortext/syntax.py`

 * *Files identical despite different names*

### Comparing `fortext-0.0.2/.gitignore` & `fortext-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `fortext-0.0.2/LICENSE` & `fortext-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fortext-0.0.2/README.md` & `fortext-0.0.3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 * [Table of Contents](#table-of-contents)
 * [Getting Started](#getting-started)
   * [Prerequisites](#prerequisites)
   * [Installation](#installation)
 * [Usage](#usage)
   * [Text styling](#text-styling)
   * [Syntax highlighting](#syntax-highlighting)
+  * [Permutations](#permutations)
 
 
 
 ## Getting Started
 
 ### Prerequisites
 * Install or update the [pip](https://pip.pypa.io/en/stable/) package manager.
@@ -66,7 +67,31 @@
 
 ```python
 print(highlight({'somekey': 'somevalue', 'anotherkey': [12.4, True, 23]}))
 ```
 Output:
 
 ![syntax highlighting example output](./img/syntax_highlighting.png)
+
+### Permutations
+```python
+for perm in string_permutations('abc'):
+    print(perm)
+```
+Output:
+```
+a
+b
+c
+ab
+ac
+ba
+bc
+ca
+cb
+abc
+acb
+bac
+bca
+cab
+cba
+```
```

### Comparing `fortext-0.0.2/pyproject.toml` & `fortext-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "fortext"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="4MBL" },
 ]
 description = "Text stylizer for Python. Mainly useful for CLI output."
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.11"
```

### Comparing `fortext-0.0.2/PKG-INFO` & `fortext-0.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fortext
-Version: 0.0.2
+Version: 0.0.3
 Summary: Text stylizer for Python. Mainly useful for CLI output.
 Project-URL: Homepage, https://github.com/4MBL/fortext
 Project-URL: Bug Tracker, https://github.com/4MBL/fortext/issues
 Author: 4MBL
 License: MIT License
         
         Copyright (c) 2023 4MBL
@@ -41,14 +41,15 @@
 * [Table of Contents](#table-of-contents)
 * [Getting Started](#getting-started)
   * [Prerequisites](#prerequisites)
   * [Installation](#installation)
 * [Usage](#usage)
   * [Text styling](#text-styling)
   * [Syntax highlighting](#syntax-highlighting)
+  * [Permutations](#permutations)
 
 
 
 ## Getting Started
 
 ### Prerequisites
 * Install or update the [pip](https://pip.pypa.io/en/stable/) package manager.
@@ -101,7 +102,31 @@
 
 ```python
 print(highlight({'somekey': 'somevalue', 'anotherkey': [12.4, True, 23]}))
 ```
 Output:
 
 ![syntax highlighting example output](./img/syntax_highlighting.png)
+
+### Permutations
+```python
+for perm in string_permutations('abc'):
+    print(perm)
+```
+Output:
+```
+a
+b
+c
+ab
+ac
+ba
+bc
+ca
+cb
+abc
+acb
+bac
+bca
+cab
+cba
+```
```

