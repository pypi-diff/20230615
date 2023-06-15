# Comparing `tmp/parsita-1.8.0b1.tar.gz` & `tmp/parsita-2.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parsita-1.8.0b1.tar", max compression
+gzip compressed data, was "parsita-2.0.0b1.tar", max compression
```

## Comparing `parsita-1.8.0b1.tar` & `parsita-2.0.0b1.tar`

### file list

```diff
@@ -1,10 +1,29 @@
--rw-r--r--   0        0        0     1062 2023-05-10 01:19:05.730334 parsita-1.8.0b1/LICENSE
--rw-r--r--   0        0        0     2647 2023-06-13 23:50:22.081287 parsita-1.8.0b1/README.md
--rw-r--r--   0        0        0     1828 2023-06-14 11:49:21.160625 parsita-1.8.0b1/pyproject.toml
--rw-r--r--   0        0        0      418 2023-06-14 00:03:19.042328 parsita-1.8.0b1/src/parsita/__init__.py
--rw-r--r--   0        0        0     6812 2023-06-14 10:34:20.127804 parsita-1.8.0b1/src/parsita/metaclasses.py
--rw-r--r--   0        0        0     1234 2023-06-13 23:50:22.081287 parsita-1.8.0b1/src/parsita/options.py
--rw-r--r--   0        0        0    37487 2023-06-13 23:50:22.081287 parsita-1.8.0b1/src/parsita/parsers.py
--rw-r--r--   0        0        0    14118 2023-06-14 10:26:34.544360 parsita-1.8.0b1/src/parsita/state.py
--rw-r--r--   0        0        0     1689 2023-06-13 23:50:22.085287 parsita-1.8.0b1/src/parsita/util.py
--rw-r--r--   0        0        0     3740 1970-01-01 00:00:00.000000 parsita-1.8.0b1/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-05-10 01:19:05.730334 parsita-2.0.0b1/LICENSE
+-rw-r--r--   0        0        0     2649 2023-06-15 01:24:20.089115 parsita-2.0.0b1/README.md
+-rw-r--r--   0        0        0     2115 2023-06-15 01:24:49.805056 parsita-2.0.0b1/pyproject.toml
+-rw-r--r--   0        0        0      363 2023-06-15 01:24:20.093115 parsita-2.0.0b1/src/parsita/__init__.py
+-rw-r--r--   0        0        0     5488 2023-06-15 01:24:20.093115 parsita-2.0.0b1/src/parsita/metaclasses.py
+-rw-r--r--   0        0        0      165 2023-06-15 01:24:20.093115 parsita-2.0.0b1/src/parsita/options.py
+-rw-r--r--   0        0        0      833 2023-06-15 01:24:20.093115 parsita-2.0.0b1/src/parsita/parsers/__init__.py
+-rw-r--r--   0        0        0     3845 2023-06-15 01:24:20.093115 parsita-2.0.0b1/src/parsita/parsers/_alternative.py
+-rw-r--r--   0        0        0      940 2023-06-15 01:24:20.093115 parsita-2.0.0b1/src/parsita/parsers/_any.py
+-rw-r--r--   0        0        0     7859 2023-06-15 01:24:20.093115 parsita-2.0.0b1/src/parsita/parsers/_base.py
+-rw-r--r--   0        0        0     1532 2023-06-15 01:24:20.093115 parsita-2.0.0b1/src/parsita/parsers/_conversion.py
+-rw-r--r--   0        0        0     2345 2023-06-15 01:24:20.093115 parsita-2.0.0b1/src/parsita/parsers/_debug.py
+-rw-r--r--   0        0        0      640 2023-06-15 01:24:20.093115 parsita-2.0.0b1/src/parsita/parsers/_end_of_source.py
+-rw-r--r--   0        0        0     2576 2023-06-15 01:24:20.093115 parsita-2.0.0b1/src/parsita/parsers/_literal.py
+-rw-r--r--   0        0        0     1266 2023-06-15 01:24:20.093115 parsita-2.0.0b1/src/parsita/parsers/_optional.py
+-rw-r--r--   0        0        0     1509 2023-06-15 01:24:20.093115 parsita-2.0.0b1/src/parsita/parsers/_predicate.py
+-rw-r--r--   0        0        0     1809 2023-06-15 01:24:20.093115 parsita-2.0.0b1/src/parsita/parsers/_regex.py
+-rw-r--r--   0        0        0     3863 2023-06-15 01:24:20.093115 parsita-2.0.0b1/src/parsita/parsers/_repeated.py
+-rw-r--r--   0        0        0     6112 2023-06-15 01:24:20.093115 parsita-2.0.0b1/src/parsita/parsers/_repeated_seperated.py
+-rw-r--r--   0        0        0     2512 2023-06-15 01:24:20.093115 parsita-2.0.0b1/src/parsita/parsers/_sequential.py
+-rw-r--r--   0        0        0     1817 2023-06-15 01:24:20.093115 parsita-2.0.0b1/src/parsita/parsers/_success.py
+-rw-r--r--   0        0        0     1298 2023-06-15 01:24:20.093115 parsita-2.0.0b1/src/parsita/parsers/_until.py
+-rw-r--r--   0        0        0      207 2023-06-15 01:24:20.093115 parsita-2.0.0b1/src/parsita/state/__init__.py
+-rw-r--r--   0        0        0      807 2023-06-15 01:24:20.093115 parsita-2.0.0b1/src/parsita/state/_exceptions.py
+-rw-r--r--   0        0        0     8171 2023-06-15 01:24:20.093115 parsita-2.0.0b1/src/parsita/state/_reader.py
+-rw-r--r--   0        0        0      500 2023-06-15 01:24:20.093115 parsita-2.0.0b1/src/parsita/state/_result.py
+-rw-r--r--   0        0        0     1050 2023-06-15 01:24:20.093115 parsita-2.0.0b1/src/parsita/state/_state.py
+-rw-r--r--   0        0        0     1688 2023-06-15 01:24:20.093115 parsita-2.0.0b1/src/parsita/util.py
+-rw-r--r--   0        0        0     3653 1970-01-01 00:00:00.000000 parsita-2.0.0b1/PKG-INFO
```

### Comparing `parsita-1.8.0b1/LICENSE` & `parsita-2.0.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `parsita-1.8.0b1/README.md` & `parsita-2.0.0b1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -26,23 +26,23 @@
 ## Hello world
 
 The following is a very basic parser for extracting the name from a `Hello, {name}!` string.
 
 ```python
 from parsita import *
 
-class HelloWorldParsers(TextParsers, whitespace=r'[ ]*'):
+class HelloWorldParsers(ParserContext, whitespace=r'[ ]*'):
     hello_world = lit('Hello') >> ',' >> reg(r'[A-Z][a-z]*') << '!'
 
 # A successful parse produces the parsed value
-name = HelloWorldParsers.hello_world.parse('Hello, David!').or_die()
+name = HelloWorldParsers.hello_world.parse('Hello, David!').unwrap()
 assert name == 'David'
 
 # A parsing failure produces a useful error message
-name = HelloWorldParsers.hello_world.parse('Hello David!').or_die()
+name = HelloWorldParsers.hello_world.parse('Hello David!').unwrap()
 # parsita.state.ParseError: Expected ',' but found 'David'
 # Line 1, character 7
 #
 # Hello David!
 #       ^
 ```
```

### Comparing `parsita-1.8.0b1/src/parsita/metaclasses.py` & `parsita-2.0.0b1/src/parsita/metaclasses.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,20 @@
+__all__ = ["ForwardDeclaration", "fwd", "ParserContext"]
+
 import builtins
 import inspect
 import re
-import warnings
+from re import Pattern
+from typing import Any, Union
 
 from . import options
-from .parsers import Parser, RegexParser
+from .parsers import LiteralParser, Parser, RegexParser
+from .state import Input
+
+missing = object()
 
 
 class ParsersDict(dict):
     def __init__(self, old_options: dict):
         super().__init__()
         self.old_options = old_options  # Holds state of options at start of definition
         self.forward_declarations = {}  # Stores forward declarations as they are discovered
@@ -64,130 +70,80 @@
     Normally, forward declarations are created automatically by the contexts.
     But they can be created manually if not in a context or if the user wants
     to avoid confusing the IDE.
     """
     return ForwardDeclaration()
 
 
-# The Deprecated package does not work on __init_subclass__
-deprecation_text = "{} is deprecated; use ParserContext instead. -- Deprecated since 1.8.0."
+class ParserContextMeta(type):
+    default_whitespace: Union[Parser[Input, Any], Pattern, str, None] = None
 
-
-class GeneralParsersMeta(type):
     @classmethod
-    def __prepare__(mcs, name, bases, **_):  # noqa: N804
+    def __prepare__(
+        mcs, name, bases, *, whitespace: Union[Parser[Input, Any], Pattern, str, None] = missing  # noqa: N804
+    ):
+        if whitespace is missing:
+            whitespace = mcs.default_whitespace
+
+        if isinstance(whitespace, (str, bytes)):
+            whitespace = re.compile(whitespace)
+
+        if isinstance(whitespace, Pattern):
+            whitespace = RegexParser(whitespace)
+
         old_options = {
-            "handle_literal": options.handle_literal,
-            "parse_method": options.parse_method,
+            "whitespace": options.whitespace,
         }
 
-        options.handle_literal = options.wrap_literal
-        options.parse_method = options.basic_parse
-
+        # Store whitespace in global location
+        options.whitespace = whitespace
         return ParsersDict(old_options)
 
     def __init__(cls, name, bases, dct, **_):
         old_options = dct.old_options
 
         super().__init__(name, bases, dct)
 
         # Resolve forward declarations, will raise if name not found
         for name, forward_declaration in dct.forward_declarations.items():
             obj = dct[name]
             if not isinstance(obj, Parser):
-                obj = options.handle_literal(obj)
+                obj = LiteralParser(obj, options.whitespace)
             forward_declaration._definition = obj
 
         # Reset global variables
         for key, value in old_options.items():
             setattr(options, key, value)
 
+    def __new__(mcs, name, bases, dct, **_):  # noqa: N804
+        return super().__new__(mcs, name, bases, dct)
+
     def __call__(cls, *args, **kwargs):
         raise TypeError(
             "Parsers cannot be instantiated. They use class bodies purely as contexts for managing defaults and "
             "allowing forward declarations. Access the individual parsers as static attributes."
         )
 
 
-class GeneralParsers(metaclass=GeneralParsersMeta):
-    """Context for parsing general sequences.
-
-    This is not a real class. Don't instantiate it. This is used by inheriting
-    from it and defining parsers as class attributes in the body of the child
-    class.
-
-    In Parsita 2.0, this context will be removed, use ``ParserContext`` instead.
-    """
-
-    def __init_subclass__(cls, **kwargs) -> None:
-        warnings.warn(DeprecationWarning(deprecation_text.format("GeneralParsers")), stacklevel=1)
-        super().__init_subclass__(**kwargs)
-
-
-class TextParsersMeta(GeneralParsersMeta):
-    @classmethod
-    def __prepare__(mcs, name, bases, whitespace: str = options.default_whitespace):  # noqa: N804
-        old_options = {
-            "whitespace": options.whitespace,
-            "handle_literal": options.handle_literal,
-            "parse_method": options.parse_method,
-        }
-
-        # Store whitespace in global location so regex parsers can see it
-        if isinstance(whitespace, str):
-            whitespace = re.compile(whitespace)
-
-        if whitespace is None:
-            options.whitespace = None
-        else:
-            options.whitespace = RegexParser(whitespace)
-
-        options.handle_literal = options.default_handle_literal
-        options.parse_method = options.default_parse_method
-
-        return ParsersDict(old_options)
-
-    def __new__(mcs, name, bases, dct, **_):  # noqa: N804
-        return super().__new__(mcs, name, bases, dct)
-
-
-class TextParsers(metaclass=TextParsersMeta):
-    r"""Context for parsing text.
-
-    This is not a real class. Don't instantiate it. This is used by inheriting
-    from it and defining parsers as class attributes in the body of the child
-    class.
-
-    There is a keyword argument for the metaclass ``whitespace``. This is a
-    regular expression defining the whitespace to be ignored. The default is
-    r"\s*".
-
-    In Parsita 2.0, this context will be removed, use ``ParserContext`` instead.
-    """
-
-    def __init_subclass__(cls, **kwargs) -> None:
-        warnings.warn(DeprecationWarning(deprecation_text.format("TextParsers")), stacklevel=1)
-        super().__init_subclass__(**kwargs)
-
-
-class ParserContextMeta(TextParsersMeta):
-    @classmethod
-    def __prepare__(mcs, name, bases, whitespace: str = None):  # noqa: N804
-        return super().__prepare__(name, bases, whitespace=whitespace)
-
-
 class ParserContext(metaclass=ParserContextMeta):
     """Context for parsing.
 
     This is not a real class. Don't instantiate it. This is used by inheriting
     from it and defining parsers as class attributes in the body of the child
     class.
 
-    There is a keyword argument for the metaclass ``whitespace``. This is a
-    regular expression defining the whitespace to be ignored. The default is
-    ``None``.
+    The parser context uses various aspects of class bodies in Python to
+    perform a few kinds of magic:
 
-    In Parsita 2.0, this will become the only context.
+    1. Assign the metaclass argument ``whitespace`` to ``options.whitespace``
+       only while the class body is being executed so that it can be used by
+       terminal parsers.
+    2. For each class attribute that is a ``Parser``, assign the name of that
+       attribute to the ``name`` attribute of the parser so that names parsers
+       know their own name.
+    3. For each class attribute that is a ``Parser``, set the ``protected``
+       attribute of the parser to ``True`` so that parsers know when they are
+       in a chain of `a | b | c` or `a & b & c` and when they are not.
+    4. Create a ``ForwardDeclaration`` as a new class attribute every time a
+       name is accessed that does not exist and then resolve those forward
+       declarations at the end of the class body.
     """
-
-
-__all__ = ["ForwardDeclaration", "fwd", "GeneralParsers", "TextParsers", "ParserContext"]
```

### Comparing `parsita-1.8.0b1/src/parsita/util.py` & `parsita-2.0.0b1/src/parsita/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+__all__ = ["constant", "splat", "unsplat"]
+
 from typing import Callable, Iterable, TypeVar
 
 A = TypeVar("A")
 
 
 def constant(x: A) -> Callable[..., A]:
     """Produce a function that always returns a supplied value.
@@ -63,10 +65,7 @@
         $ g(1, 2, 3)  # 6
     """
 
     def unsplatted(*args):
         return f(args)
 
     return unsplatted
-
-
-__all__ = ["constant", "splat", "unsplat"]
```

### Comparing `parsita-1.8.0b1/PKG-INFO` & `parsita-2.0.0b1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 Metadata-Version: 2.1
 Name: parsita
-Version: 1.8.0b1
+Version: 2.0.0b1
 Summary: Parser combinator library for Python
 Home-page: https://github.com/drhagen/parsita
 License: MIT
 Keywords: text,parsing,parser,combinator
 Author: David Hagen
 Author-email: david@drhagen.com
-Requires-Python: >=3.7.0,<4.0.0
+Requires-Python: >=3.8.0,<4.0.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: deprecated (>=1.2,<2.0)
-Requires-Dist: returns (>=0.19.0,<0.20.0)
+Requires-Dist: returns (>=0.20.0,<0.21.0)
 Project-URL: Documentation, https://parsita.drhagen.com
 Project-URL: Repository, https://github.com/drhagen/parsita
 Description-Content-Type: text/markdown
 
 # Parsita
 
 [![Build status][build-image]][build-link]
@@ -53,23 +51,23 @@
 ## Hello world
 
 The following is a very basic parser for extracting the name from a `Hello, {name}!` string.
 
 ```python
 from parsita import *
 
-class HelloWorldParsers(TextParsers, whitespace=r'[ ]*'):
+class HelloWorldParsers(ParserContext, whitespace=r'[ ]*'):
     hello_world = lit('Hello') >> ',' >> reg(r'[A-Z][a-z]*') << '!'
 
 # A successful parse produces the parsed value
-name = HelloWorldParsers.hello_world.parse('Hello, David!').or_die()
+name = HelloWorldParsers.hello_world.parse('Hello, David!').unwrap()
 assert name == 'David'
 
 # A parsing failure produces a useful error message
-name = HelloWorldParsers.hello_world.parse('Hello David!').or_die()
+name = HelloWorldParsers.hello_world.parse('Hello David!').unwrap()
 # parsita.state.ParseError: Expected ',' but found 'David'
 # Line 1, character 7
 #
 # Hello David!
 #       ^
 ```
```

