# Comparing `tmp/sphinx-autodoc-typehints-1.8.0.tar.gz` & `tmp/sphinx-autodoc-typehints-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sphinx-autodoc-typehints-1.8.0.tar", last modified: Thu Sep 12 06:34:19 2019, max compression
+gzip compressed data, was "dist/sphinx-autodoc-typehints-1.9.0.tar", last modified: Fri Oct 25 10:35:57 2019, max compression
```

## Comparing `sphinx-autodoc-typehints-1.8.0.tar` & `sphinx-autodoc-typehints-1.9.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-09-12 06:34:19.000000 sphinx-autodoc-typehints-1.8.0/
--rw-rw-r--   0 travis    (2000) travis    (2000)     4395 2019-09-12 06:34:03.000000 sphinx-autodoc-typehints-1.8.0/CHANGELOG.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     6402 2019-09-12 06:34:19.000000 sphinx-autodoc-typehints-1.8.0/PKG-INFO
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-09-12 06:34:19.000000 sphinx-autodoc-typehints-1.8.0/sphinx_autodoc_typehints.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     6402 2019-09-12 06:34:19.000000 sphinx-autodoc-typehints-1.8.0/sphinx_autodoc_typehints.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-09-12 06:34:19.000000 sphinx-autodoc-typehints-1.8.0/sphinx_autodoc_typehints.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       25 2019-09-12 06:34:19.000000 sphinx-autodoc-typehints-1.8.0/sphinx_autodoc_typehints.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      524 2019-09-12 06:34:19.000000 sphinx-autodoc-typehints-1.8.0/sphinx_autodoc_typehints.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      175 2019-09-12 06:34:19.000000 sphinx-autodoc-typehints-1.8.0/sphinx_autodoc_typehints.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      303 2019-09-12 06:34:03.000000 sphinx-autodoc-typehints-1.8.0/tox.ini
--rw-rw-r--   0 travis    (2000) travis    (2000)      102 2019-09-12 06:34:03.000000 sphinx-autodoc-typehints-1.8.0/.gitignore
--rw-rw-r--   0 travis    (2000) travis    (2000)     1337 2019-09-12 06:34:19.000000 sphinx-autodoc-typehints-1.8.0/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     1648 2019-09-12 06:34:03.000000 sphinx-autodoc-typehints-1.8.0/.travis.yml
--rw-rw-r--   0 travis    (2000) travis    (2000)     1130 2019-09-12 06:34:03.000000 sphinx-autodoc-typehints-1.8.0/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)     4178 2019-09-12 06:34:03.000000 sphinx-autodoc-typehints-1.8.0/README.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      152 2019-09-12 06:34:03.000000 sphinx-autodoc-typehints-1.8.0/pyproject.toml
--rw-rw-r--   0 travis    (2000) travis    (2000)      239 2019-09-12 06:34:03.000000 sphinx-autodoc-typehints-1.8.0/setup.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    14658 2019-09-12 06:34:03.000000 sphinx-autodoc-typehints-1.8.0/sphinx_autodoc_typehints.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-09-12 06:34:19.000000 sphinx-autodoc-typehints-1.8.0/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)    16841 2019-09-12 06:34:03.000000 sphinx-autodoc-typehints-1.8.0/tests/test_sphinx_autodoc_typehints.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      778 2019-09-12 06:34:03.000000 sphinx-autodoc-typehints-1.8.0/tests/conftest.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-09-12 06:34:19.000000 sphinx-autodoc-typehints-1.8.0/tests/roots/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-09-12 06:34:19.000000 sphinx-autodoc-typehints-1.8.0/tests/roots/test-dummy/
--rw-rw-r--   0 travis    (2000) travis    (2000)      259 2019-09-12 06:34:03.000000 sphinx-autodoc-typehints-1.8.0/tests/roots/test-dummy/conf.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4211 2019-09-12 06:34:03.000000 sphinx-autodoc-typehints-1.8.0/tests/roots/test-dummy/dummy_module.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      824 2019-09-12 06:34:03.000000 sphinx-autodoc-typehints-1.8.0/tests/roots/test-dummy/index.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-25 10:35:57.000000 sphinx-autodoc-typehints-1.9.0/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4869 2019-10-25 10:35:41.000000 sphinx-autodoc-typehints-1.9.0/CHANGELOG.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6602 2019-10-25 10:35:57.000000 sphinx-autodoc-typehints-1.9.0/PKG-INFO
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-25 10:35:57.000000 sphinx-autodoc-typehints-1.9.0/sphinx_autodoc_typehints.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6602 2019-10-25 10:35:56.000000 sphinx-autodoc-typehints-1.9.0/sphinx_autodoc_typehints.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-10-25 10:35:56.000000 sphinx-autodoc-typehints-1.9.0/sphinx_autodoc_typehints.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       25 2019-10-25 10:35:56.000000 sphinx-autodoc-typehints-1.9.0/sphinx_autodoc_typehints.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      524 2019-10-25 10:35:56.000000 sphinx-autodoc-typehints-1.9.0/sphinx_autodoc_typehints.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      190 2019-10-25 10:35:56.000000 sphinx-autodoc-typehints-1.9.0/sphinx_autodoc_typehints.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      303 2019-10-25 10:35:41.000000 sphinx-autodoc-typehints-1.9.0/tox.ini
+-rw-rw-r--   0 travis    (2000) travis    (2000)      111 2019-10-25 10:35:41.000000 sphinx-autodoc-typehints-1.9.0/.gitignore
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1381 2019-10-25 10:35:57.000000 sphinx-autodoc-typehints-1.9.0/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1644 2019-10-25 10:35:41.000000 sphinx-autodoc-typehints-1.9.0/.travis.yml
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1130 2019-10-25 10:35:41.000000 sphinx-autodoc-typehints-1.9.0/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4362 2019-10-25 10:35:41.000000 sphinx-autodoc-typehints-1.9.0/README.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      152 2019-10-25 10:35:41.000000 sphinx-autodoc-typehints-1.9.0/pyproject.toml
+-rw-rw-r--   0 travis    (2000) travis    (2000)      239 2019-10-25 10:35:41.000000 sphinx-autodoc-typehints-1.9.0/setup.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15004 2019-10-25 10:35:41.000000 sphinx-autodoc-typehints-1.9.0/sphinx_autodoc_typehints.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-25 10:35:57.000000 sphinx-autodoc-typehints-1.9.0/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14714 2019-10-25 10:35:41.000000 sphinx-autodoc-typehints-1.9.0/tests/test_sphinx_autodoc_typehints.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1251 2019-10-25 10:35:41.000000 sphinx-autodoc-typehints-1.9.0/tests/conftest.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-25 10:35:57.000000 sphinx-autodoc-typehints-1.9.0/tests/roots/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-25 10:35:57.000000 sphinx-autodoc-typehints-1.9.0/tests/roots/test-dummy/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      259 2019-10-25 10:35:41.000000 sphinx-autodoc-typehints-1.9.0/tests/roots/test-dummy/conf.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4211 2019-10-25 10:35:41.000000 sphinx-autodoc-typehints-1.9.0/tests/roots/test-dummy/dummy_module.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      824 2019-10-25 10:35:41.000000 sphinx-autodoc-typehints-1.9.0/tests/roots/test-dummy/index.rst
```

### Comparing `sphinx-autodoc-typehints-1.8.0/CHANGELOG.rst` & `sphinx-autodoc-typehints-1.9.0/CHANGELOG.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+1.9.0
+=====
+
+* Added support for typing_extensions_
+* Added the ``typehints_document_rtype`` option (PR by Simon-Martin Schröder)
+* Fixed metaclasses as annotations causing ``TypeError``
+* Fixed rendering of ``typing.Literal``
+* Fixed OSError when generating docs for SQLAlchemy mapped classes
+* Fixed unparametrized generic classes being rendered with their type parameters
+  (e.g. ``Dict[~KT, ~VT]``)
+
+.. _typing_extensions: https://pypi.org/project/typing-extensions/
+
+
 1.8.0
 =====
 
 * Fixed regression which caused ``TypeError`` or ``OSError`` when trying to set annotations due to
   PR #87
 * Fixed unintentional mangling of annotation type names
 * Added proper ``:py:data`` targets for ``NoReturn``, ``ClassVar`` and ``Tuple``
```

### Comparing `sphinx-autodoc-typehints-1.8.0/PKG-INFO` & `sphinx-autodoc-typehints-1.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-autodoc-typehints
-Version: 1.8.0
+Version: 1.9.0
 Summary: Type hints (PEP 484) support for the Sphinx autodoc extension
 Home-page: UNKNOWN
 Author: Alex Grönholm
 Author-email: alex.gronholm@nextday.fi
 License: MIT
 Project-URL: Change log, https://github.com/agronholm/sphinx-autodoc-typehints/blob/master/CHANGELOG.rst
 Project-URL: Source code, https://github.com/agronholm/sphinx-autodoc-typehints
@@ -70,14 +70,16 @@
           ``True`` to enable "expensive" typing imports
         * ``typehints_fully_qualified`` (default: ``False``): if ``True``, class names are always fully
           qualified (e.g. ``module.for.Class``). If ``False``, just the class name displays (e.g.
           ``Class``)
         * ``always_document_param_types`` (default: ``False``): If ``False``, do not add type info for
           undocumented parameters.  If ``True``, add stub documentation for undocumented parameters to
           be able to add type info.
+        * ``typehints_document_rtype`` (default: ``True``): If ``False``, never add an ``:rtype:`` directive.
+          If ``True``, add the ``:rtype:`` directive if no existing ``:rtype:`` is found.
         
         
         How it works
         ------------
         
         The extension listens to the ``autodoc-process-signature`` and ``autodoc-process-docstring``
         Sphinx events. In the former, it strips the annotations from the function signature. In the latter,
@@ -149,9 +151,9 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.5.2
-Provides-Extra: type_comments
 Provides-Extra: test
+Provides-Extra: type_comments
```

### Comparing `sphinx-autodoc-typehints-1.8.0/sphinx_autodoc_typehints.egg-info/PKG-INFO` & `sphinx-autodoc-typehints-1.9.0/sphinx_autodoc_typehints.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-autodoc-typehints
-Version: 1.8.0
+Version: 1.9.0
 Summary: Type hints (PEP 484) support for the Sphinx autodoc extension
 Home-page: UNKNOWN
 Author: Alex Grönholm
 Author-email: alex.gronholm@nextday.fi
 License: MIT
 Project-URL: Change log, https://github.com/agronholm/sphinx-autodoc-typehints/blob/master/CHANGELOG.rst
 Project-URL: Source code, https://github.com/agronholm/sphinx-autodoc-typehints
@@ -70,14 +70,16 @@
           ``True`` to enable "expensive" typing imports
         * ``typehints_fully_qualified`` (default: ``False``): if ``True``, class names are always fully
           qualified (e.g. ``module.for.Class``). If ``False``, just the class name displays (e.g.
           ``Class``)
         * ``always_document_param_types`` (default: ``False``): If ``False``, do not add type info for
           undocumented parameters.  If ``True``, add stub documentation for undocumented parameters to
           be able to add type info.
+        * ``typehints_document_rtype`` (default: ``True``): If ``False``, never add an ``:rtype:`` directive.
+          If ``True``, add the ``:rtype:`` directive if no existing ``:rtype:`` is found.
         
         
         How it works
         ------------
         
         The extension listens to the ``autodoc-process-signature`` and ``autodoc-process-docstring``
         Sphinx events. In the former, it strips the annotations from the function signature. In the latter,
@@ -149,9 +151,9 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.5.2
-Provides-Extra: type_comments
 Provides-Extra: test
+Provides-Extra: type_comments
```

### Comparing `sphinx-autodoc-typehints-1.8.0/sphinx_autodoc_typehints.egg-info/SOURCES.txt` & `sphinx-autodoc-typehints-1.9.0/sphinx_autodoc_typehints.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sphinx-autodoc-typehints-1.8.0/setup.cfg` & `sphinx-autodoc-typehints-1.9.0/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -29,20 +29,22 @@
 install_requires = Sphinx >= 2.1
 
 [options.extras_require]
 test = 
 	pytest >= 3.1.0
 	typing_extensions >= 3.5
 	dataclasses; python_version == "3.6"
+	sphobjinv >= 2.0
 type_comments = 
 	typed_ast >= 1.4.0; python_version < "3.8"
 
 [flake8]
 max-line-length = 99
 
 [tool:pytest]
+addopts = -rsx --tb=short
 testpaths = tests
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `sphinx-autodoc-typehints-1.8.0/.travis.yml` & `sphinx-autodoc-typehints-1.9.0/.travis.yml`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     - stage: test
       env: TOXENV=py37
       python: "3.7"
       after_success: *after_success
 
     - stage: test
       env: TOXENV=py38
-      python: "3.8-dev"
+      python: "3.8"
       after_success: *after_success
 
     - stage: deploy to pypi
       install: skip
       script: skip
       deploy:
         provider: pypi
```

### Comparing `sphinx-autodoc-typehints-1.8.0/LICENSE` & `sphinx-autodoc-typehints-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinx-autodoc-typehints-1.8.0/README.rst` & `sphinx-autodoc-typehints-1.9.0/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -59,14 +59,16 @@
   ``True`` to enable "expensive" typing imports
 * ``typehints_fully_qualified`` (default: ``False``): if ``True``, class names are always fully
   qualified (e.g. ``module.for.Class``). If ``False``, just the class name displays (e.g.
   ``Class``)
 * ``always_document_param_types`` (default: ``False``): If ``False``, do not add type info for
   undocumented parameters.  If ``True``, add stub documentation for undocumented parameters to
   be able to add type info.
+* ``typehints_document_rtype`` (default: ``True``): If ``False``, never add an ``:rtype:`` directive.
+  If ``True``, add the ``:rtype:`` directive if no existing ``:rtype:`` is found.
 
 
 How it works
 ------------
 
 The extension listens to the ``autodoc-process-signature`` and ``autodoc-process-docstring``
 Sphinx events. In the former, it strips the annotations from the function signature. In the latter,
```

### Comparing `sphinx-autodoc-typehints-1.8.0/sphinx_autodoc_typehints.py` & `sphinx-autodoc-typehints-1.9.0/sphinx_autodoc_typehints.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 import inspect
 import sys
 import textwrap
 import typing
-from typing import get_type_hints, TypeVar, Any, AnyStr, Generic, Union
+from typing import get_type_hints, TypeVar, Generic
 
 from sphinx.util import logging
 from sphinx.util.inspect import Signature
 
 try:
     from typing_extensions import Protocol
 except ImportError:
     Protocol = None
 
 logger = logging.getLogger(__name__)
-pydata_annotations = {'Any', 'AnyStr', 'Callable', 'ClassVar', 'NoReturn', 'Optional', 'Tuple',
-                      'Union'}
+pydata_annotations = {'Any', 'AnyStr', 'Callable', 'ClassVar', 'Literal', 'NoReturn', 'Optional',
+                      'Tuple', 'Union'}
 
 
 def format_annotation(annotation, fully_qualified=False):
     if inspect.isclass(annotation) and annotation.__module__ == 'builtins':
         if annotation.__qualname__ == 'NoneType':
             return '``None``'
         else:
             return ':py:class:`{}`'.format(annotation.__qualname__)
 
     annotation_cls = annotation if inspect.isclass(annotation) else type(annotation)
-    if annotation_cls.__module__ == 'typing':
+    if annotation_cls.__module__ in ('typing', 'typing_extensions'):
         class_name = str(annotation).split('[')[0].split('.')[-1]
         params = None
         module = 'typing'
         extra = ''
 
         origin = getattr(annotation, '__origin__', None)
         if inspect.isclass(origin):
@@ -37,36 +37,35 @@
             try:
                 mro = annotation_cls.mro()
                 if Generic in mro or (Protocol and Protocol in mro):
                     module = annotation_cls.__module__
             except TypeError:
                 pass  # annotation_cls was either the "type" object or typing.Type
 
-        if annotation is Any:
+        if class_name == 'Any':
             return ':py:data:`{}typing.Any`'.format("" if fully_qualified else "~")
-        elif annotation is AnyStr:
+        elif class_name == '~AnyStr':
             return ':py:data:`{}typing.AnyStr`'.format("" if fully_qualified else "~")
         elif isinstance(annotation, TypeVar):
             return '\\%r' % annotation
-        elif (annotation is Union or getattr(annotation, '__origin__', None) is Union or
-              hasattr(annotation, '__union_params__')):
+        elif class_name == 'Union':
             if hasattr(annotation, '__union_params__'):
                 params = annotation.__union_params__
             elif hasattr(annotation, '__args__'):
                 params = annotation.__args__
 
             if params and len(params) == 2 and (hasattr(params[1], '__qualname__') and
                                                 params[1].__qualname__ == 'NoneType'):
                 class_name = 'Optional'
                 params = (params[0],)
-        elif annotation_cls.__qualname__ == 'Tuple' and hasattr(annotation, '__tuple_params__'):
+        elif class_name == 'Tuple' and hasattr(annotation, '__tuple_params__'):
             params = annotation.__tuple_params__
             if annotation.__tuple_use_ellipsis__:
                 params += (Ellipsis,)
-        elif annotation_cls.__qualname__ == 'Callable':
+        elif class_name == 'Callable':
             arg_annotations = result_annotation = None
             if hasattr(annotation, '__result__'):
                 arg_annotations = annotation.__args__
                 result_annotation = annotation.__result__
             elif getattr(annotation, '__args__', None):
                 arg_annotations = annotation.__args__[:-1]
                 result_annotation = annotation.__args__[-1]
@@ -77,27 +76,30 @@
                 params = [
                     '\\[{}]'.format(
                         ', '.join(
                             format_annotation(param, fully_qualified)
                             for param in arg_annotations)),
                     result_annotation
                 ]
-        elif str(annotation).startswith('typing.ClassVar[') and hasattr(annotation, '__type__'):
+        elif class_name == 'Literal':
+            annotation_args = getattr(annotation, '__args__', ()) or annotation.__values__
+            extra = '\\[{}]'.format(', '.join(repr(arg) for arg in annotation_args))
+        elif class_name == 'ClassVar' and hasattr(annotation, '__type__'):
             # < py3.7
             params = (annotation.__type__,)
         elif hasattr(annotation, 'type_var'):
             # Type alias
             class_name = annotation.name
             params = (annotation.type_var,)
         elif getattr(annotation, '__args__', None) is not None:
             params = annotation.__args__
         elif hasattr(annotation, '__parameters__'):
             params = annotation.__parameters__
 
-        if params:
+        if params and annotation is not getattr(sys.modules[module], class_name):
             extra = '\\[{}]'.format(', '.join(
                 format_annotation(param, fully_qualified) for param in params))
 
         return '{prefix}`{qualify}{module}.{name}`{extra}'.format(
             prefix=':py:data:' if class_name in pydata_annotations else ':py:class:',
             qualify="" if fully_qualified else "~",
             module=module,
@@ -114,21 +116,25 @@
             extra=format_annotation(annotation.__supertype__, fully_qualified),
         )
     elif inspect.isclass(annotation) or inspect.isclass(getattr(annotation, '__origin__', None)):
         if not inspect.isclass(annotation):
             annotation_cls = annotation.__origin__
 
         extra = ''
-        mro = annotation_cls.mro()
-        if Generic in mro or (Protocol and Protocol in mro):
-            params = (getattr(annotation, '__parameters__', None) or
-                      getattr(annotation, '__args__', None))
-            if params:
-                extra = '\\[{}]'.format(', '.join(
-                    format_annotation(param, fully_qualified) for param in params))
+        try:
+            mro = annotation_cls.mro()
+        except TypeError:
+            pass
+        else:
+            if Generic in mro or (Protocol and Protocol in mro):
+                params = (getattr(annotation, '__parameters__', None) or
+                          getattr(annotation, '__args__', None))
+                if params:
+                    extra = '\\[{}]'.format(', '.join(
+                        format_annotation(param, fully_qualified) for param in params))
 
         return ':py:class:`{qualify}{module}.{name}`{extra}'.format(
             qualify="" if fully_qualified else "~",
             module=annotation.__module__,
             name=annotation_cls.__qualname__,
             extra=extra
         )
@@ -241,15 +247,15 @@
                 'Did not get exactly one node from AST for "%s", got %s', name, len(children))
             return
 
         return children[0]
 
     try:
         obj_ast = ast.parse(textwrap.dedent(inspect.getsource(obj)), **parse_kwargs)
-    except TypeError:
+    except (OSError, TypeError):
         return {}
 
     obj_ast = _one_child(obj_ast)
     if obj_ast is None:
         return {}
 
     try:
@@ -384,15 +390,15 @@
             for i, line in enumerate(lines):
                 if line.startswith(':rtype:'):
                     insert_index = None
                     break
                 elif line.startswith(':return:') or line.startswith(':returns:'):
                     insert_index = i
 
-            if insert_index is not None:
+            if insert_index is not None and app.config.typehints_document_rtype:
                 if insert_index == len(lines):
                     # Ensure that :rtype: doesn't get joined with a paragraph of text, which
                     # prevents it being interpreted.
                     lines.append('')
                     insert_index += 1
 
                 lines.insert(insert_index, ':rtype: {}'.format(formatted_annotation))
@@ -403,11 +409,12 @@
         typing.TYPE_CHECKING = True
 
 
 def setup(app):
     app.add_config_value('set_type_checking_flag', False, 'html')
     app.add_config_value('always_document_param_types', False, 'html')
     app.add_config_value('typehints_fully_qualified', False, 'env')
+    app.add_config_value('typehints_document_rtype', True, 'env')
     app.connect('builder-inited', builder_ready)
     app.connect('autodoc-process-signature', process_signature)
     app.connect('autodoc-process-docstring', process_docstring)
     return dict(parallel_read_safe=True)
```

### Comparing `sphinx-autodoc-typehints-1.8.0/tests/test_sphinx_autodoc_typehints.py` & `sphinx-autodoc-typehints-1.9.0/tests/test_sphinx_autodoc_typehints.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,37 @@
 import pathlib
-import pytest
+import re
 import sys
 import textwrap
+import typing
+from collections import defaultdict
 from typing import (
     Any, AnyStr, Callable, Dict, Generic, Mapping, NewType, Optional, Pattern,
     Tuple, TypeVar, Union, Type)
 
-from typing_extensions import Protocol
+import pytest
+import typing_extensions
 
 from sphinx_autodoc_typehints import format_annotation, process_docstring
 
 try:
     from typing import ClassVar  # not available prior to Python 3.5.3
 except ImportError:
     ClassVar = None
 
 try:
     from typing import NoReturn  # not available prior to Python 3.6.5
 except ImportError:
     NoReturn = None
 
+try:
+    from typing import Literal
+except ImportError:
+    Literal = defaultdict(lambda: None)
+
 T = TypeVar('T')
 U = TypeVar('U', covariant=True)
 V = TypeVar('V', contravariant=True)
 W = NewType('W', str)
 
 
 class A:
@@ -35,46 +43,53 @@
     pass
 
 
 class C(B[str]):
     pass
 
 
-class D(Protocol):
+class D(typing_extensions.Protocol):
     pass
 
 
-class E(Protocol[T]):
+class E(typing_extensions.Protocol[T]):
     pass
 
 
 class Slotted:
     __slots__ = ()
 
 
+class Metaclass(type):
+    pass
+
+
 @pytest.mark.parametrize('annotation, expected_result', [
     (str,                           ':py:class:`str`'),
     (int,                           ':py:class:`int`'),
     (type(None),                    '``None``'),
+    (type,                          ':py:class:`type`'),
+    (Type,                          ':py:class:`~typing.Type`'),
+    (Type[A],                       ':py:class:`~typing.Type`\\[:py:class:`~%s.A`]' % __name__),
     pytest.param(NoReturn,          ':py:data:`~typing.NoReturn`',
                  marks=[pytest.mark.skipif(NoReturn is None,
                                            reason='typing.NoReturn is not available')]),
     pytest.param(ClassVar[str],      ':py:data:`~typing.ClassVar`\\[:py:class:`str`]',
                  marks=[pytest.mark.skipif(ClassVar is None,
                                            reason='typing.ClassVar is not available')]),
     (Any,                           ':py:data:`~typing.Any`'),
     (AnyStr,                        ':py:data:`~typing.AnyStr`'),
     (Generic[T],                    ':py:class:`~typing.Generic`\\[\\~T]'),
-    (Mapping,                       ':py:class:`~typing.Mapping`\\[\\~KT, \\+VT_co]'),
+    (Mapping,                       ':py:class:`~typing.Mapping`'),
     (Mapping[T, int],               ':py:class:`~typing.Mapping`\\[\\~T, :py:class:`int`]'),
     (Mapping[str, V],               ':py:class:`~typing.Mapping`\\[:py:class:`str`, \\-V]'),
     (Mapping[T, U],                 ':py:class:`~typing.Mapping`\\[\\~T, \\+U]'),
     (Mapping[str, bool],            ':py:class:`~typing.Mapping`\\[:py:class:`str`, '
                                     ':py:class:`bool`]'),
-    (Dict,                          ':py:class:`~typing.Dict`\\[\\~KT, \\~VT]'),
+    (Dict,                          ':py:class:`~typing.Dict`'),
     (Dict[T, int],                  ':py:class:`~typing.Dict`\\[\\~T, :py:class:`int`]'),
     (Dict[str, V],                  ':py:class:`~typing.Dict`\\[:py:class:`str`, \\-V]'),
     (Dict[T, U],                    ':py:class:`~typing.Dict`\\[\\~T, \\+U]'),
     (Dict[str, bool],               ':py:class:`~typing.Dict`\\[:py:class:`str`, '
                                     ':py:class:`bool`]'),
     (Tuple,                         ':py:data:`~typing.Tuple`'),
     (Tuple[str, bool],              ':py:data:`~typing.Tuple`\\[:py:class:`str`, '
@@ -95,98 +110,70 @@
     (Callable[[int], int],          ':py:data:`~typing.Callable`\\[\\[:py:class:`int`], '
                                     ':py:class:`int`]'),
     (Callable[[int, str], bool],    ':py:data:`~typing.Callable`\\[\\[:py:class:`int`, '
                                     ':py:class:`str`], :py:class:`bool`]'),
     (Callable[[int, str], None],    ':py:data:`~typing.Callable`\\[\\[:py:class:`int`, '
                                     ':py:class:`str`], ``None``]'),
     (Callable[[T], T],              ':py:data:`~typing.Callable`\\[\\[\\~T], \\~T]'),
-    (Pattern,                       ':py:class:`~typing.Pattern`\\[:py:data:`~typing.AnyStr`]'),
+    (Pattern,                       ':py:class:`~typing.Pattern`'),
     (Pattern[str],                  ':py:class:`~typing.Pattern`\\[:py:class:`str`]'),
+    pytest.param(Literal['a', 1],   ":py:data:`~typing.Literal`\\['a', 1]",
+                 marks=[pytest.mark.skipif(isinstance(Literal, defaultdict),
+                                           reason='Requires Python 3.8+')]),
+    (Metaclass,                     ':py:class:`~%s.Metaclass`' % __name__),
     (A,                             ':py:class:`~%s.A`' % __name__),
     (B,                             ':py:class:`~%s.B`\\[\\~T]' % __name__),
     (B[int],                        ':py:class:`~%s.B`\\[:py:class:`int`]' % __name__),
     (C,                             ':py:class:`~%s.C`' % __name__),
     (D,                             ':py:class:`~%s.D`' % __name__),
     (E,                             ':py:class:`~%s.E`\\[\\~T]' % __name__),
     (E[int],                        ':py:class:`~%s.E`\\[:py:class:`int`]' % __name__),
     (W,                             ':py:func:`~typing.NewType`\\(:py:data:`~W`, :py:class:`str`)')
 ])
-def test_format_annotation(annotation, expected_result):
+def test_format_annotation(inv, annotation, expected_result):
     result = format_annotation(annotation)
     assert result == expected_result
 
-
-@pytest.mark.parametrize('annotation, expected_result', [
-    (str,                           ':py:class:`str`'),
-    (int,                           ':py:class:`int`'),
-    (type(None),                    '``None``'),
-    pytest.param(NoReturn,          ':py:data:`typing.NoReturn`',
-                 marks=[pytest.mark.skipif(NoReturn is None,
-                                           reason='typing.NoReturn is not available')]),
-    pytest.param(ClassVar[str],      ':py:data:`typing.ClassVar`\\[:py:class:`str`]',
-                 marks=[pytest.mark.skipif(ClassVar is None,
-                                           reason='typing.ClassVar is not available')]),
-    (Any,                           ':py:data:`typing.Any`'),
-    (AnyStr,                        ':py:data:`typing.AnyStr`'),
-    (Generic[T],                    ':py:class:`typing.Generic`\\[\\~T]'),
-    (Mapping,                       ':py:class:`typing.Mapping`\\[\\~KT, \\+VT_co]'),
-    (Mapping[T, int],               ':py:class:`typing.Mapping`\\[\\~T, :py:class:`int`]'),
-    (Mapping[str, V],               ':py:class:`typing.Mapping`\\[:py:class:`str`, \\-V]'),
-    (Mapping[T, U],                 ':py:class:`typing.Mapping`\\[\\~T, \\+U]'),
-    (Mapping[str, bool],            ':py:class:`typing.Mapping`\\[:py:class:`str`, '
-                                    ':py:class:`bool`]'),
-    (Dict,                          ':py:class:`typing.Dict`\\[\\~KT, \\~VT]'),
-    (Dict[T, int],                  ':py:class:`typing.Dict`\\[\\~T, :py:class:`int`]'),
-    (Dict[str, V],                  ':py:class:`typing.Dict`\\[:py:class:`str`, \\-V]'),
-    (Dict[T, U],                    ':py:class:`typing.Dict`\\[\\~T, \\+U]'),
-    (Dict[str, bool],               ':py:class:`typing.Dict`\\[:py:class:`str`, '
-                                    ':py:class:`bool`]'),
-    (Tuple,                         ':py:data:`typing.Tuple`'),
-    (Tuple[str, bool],              ':py:data:`typing.Tuple`\\[:py:class:`str`, '
-                                    ':py:class:`bool`]'),
-    (Tuple[int, int, int],          ':py:data:`typing.Tuple`\\[:py:class:`int`, '
-                                    ':py:class:`int`, :py:class:`int`]'),
-    (Tuple[str, ...],               ':py:data:`typing.Tuple`\\[:py:class:`str`, ...]'),
-    (Union,                         ':py:data:`typing.Union`'),
-    (Union[str, bool],              ':py:data:`typing.Union`\\[:py:class:`str`, '
-                                    ':py:class:`bool`]'),
-    (Optional[str],                 ':py:data:`typing.Optional`\\[:py:class:`str`]'),
-    (Callable,                      ':py:data:`typing.Callable`'),
-    (Callable[..., int],            ':py:data:`typing.Callable`\\[..., :py:class:`int`]'),
-    (Callable[[int], int],          ':py:data:`typing.Callable`\\[\\[:py:class:`int`], '
-                                    ':py:class:`int`]'),
-    (Callable[[int, str], bool],    ':py:data:`typing.Callable`\\[\\[:py:class:`int`, '
-                                    ':py:class:`str`], :py:class:`bool`]'),
-    (Callable[[int, str], None],    ':py:data:`typing.Callable`\\[\\[:py:class:`int`, '
-                                    ':py:class:`str`], ``None``]'),
-    (Callable[[T], T],              ':py:data:`typing.Callable`\\[\\[\\~T], \\~T]'),
-    (Pattern,                       ':py:class:`typing.Pattern`\\[:py:data:`typing.AnyStr`]'),
-    (Pattern[str],                  ':py:class:`typing.Pattern`\\[:py:class:`str`]'),
-    (A,                             ':py:class:`%s.A`' % __name__),
-    (B,                             ':py:class:`%s.B`\\[\\~T]' % __name__),
-    (B[int],                        ':py:class:`%s.B`\\[:py:class:`int`]' % __name__),
-    (C,                             ':py:class:`%s.C`' % __name__),
-    (D,                             ':py:class:`%s.D`' % __name__),
-    (E,                             ':py:class:`%s.E`\\[\\~T]' % __name__),
-    (E[int],                        ':py:class:`%s.E`\\[:py:class:`int`]' % __name__),
-    (W,                             ':py:func:`typing.NewType`\\(:py:data:`~W`, :py:class:`str`)')
+    # Test with the "fully_qualified" flag turned on
+    if 'typing' in expected_result or __name__ in expected_result:
+        expected_result = expected_result.replace('~typing', 'typing')
+        expected_result = expected_result.replace('~' + __name__, __name__)
+        assert format_annotation(annotation, fully_qualified=True) == expected_result
+
+    # Test for the correct role (class vs data) using the official Sphinx inventory
+    if 'typing' in expected_result:
+        m = re.match('^:py:(?P<role>class|data|func):`~(?P<name>[^`]+)`', result)
+        assert m, 'No match'
+        name = m.group('name')
+        role = next((o.role for o in inv.objects if o.name == name), None)
+        if name in {'typing.Pattern', 'typing.Match', 'typing.NoReturn'}:
+            if sys.version_info < (3, 6):
+                assert role is None, 'No entry in Python 3.5’s objects.inv'
+                return
+
+        assert role is not None, 'Name {} not found'.format(name)
+        assert m.group('role') == ('func' if role == 'function' else role)
+
+
+@pytest.mark.parametrize('library', [typing, typing_extensions],
+                         ids=['typing', 'typing_extensions'])
+@pytest.mark.parametrize('annotation, params, expected_result', [
+    ('Literal', ('a', 1), ":py:data:`~typing.Literal`\\['a', 1]"),
+    ('Type', None, ':py:class:`~typing.Type`'),
+    ('Type', (A,), ':py:class:`~typing.Type`\\[:py:class:`~%s.A`]' % __name__)
 ])
-def test_format_annotation_fully_qualified(annotation, expected_result):
-    result = format_annotation(annotation, fully_qualified=True)
-    assert result == expected_result
-
+def test_format_annotation_both_libs(inv, library, annotation, params, expected_result):
+    try:
+        annotation_cls = getattr(library, annotation)
+    except AttributeError:
+        pytest.skip('{} not available in the {} module'.format(annotation, library.__name__))
 
-@pytest.mark.parametrize('type_param, expected_result', [
-    (None, ':py:class:`~typing.Type`\\[\\+CT'),
-    (A, ':py:class:`~typing.Type`\\[:py:class:`~%s.A`]' % __name__)
-])
-def test_format_annotation_type(type_param, expected_result):
-    annotation = Type[type_param] if type_param else Type
-    result = format_annotation(annotation)
-    assert result.startswith(expected_result)
+    ann = annotation_cls if params is None else annotation_cls[params]
+    result = format_annotation(ann)
+    assert result == expected_result
 
 
 def test_process_docstring_slot_wrapper():
     lines = []
     process_docstring(None, 'class', 'SlotWrapper', Slotted, None, lines)
     assert not lines
```

### Comparing `sphinx-autodoc-typehints-1.8.0/tests/roots/test-dummy/dummy_module.py` & `sphinx-autodoc-typehints-1.9.0/tests/roots/test-dummy/dummy_module.py`

 * *Files identical despite different names*

### Comparing `sphinx-autodoc-typehints-1.8.0/tests/roots/test-dummy/index.rst` & `sphinx-autodoc-typehints-1.9.0/tests/roots/test-dummy/index.rst`

 * *Files identical despite different names*

