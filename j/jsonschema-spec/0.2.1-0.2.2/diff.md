# Comparing `tmp/jsonschema_spec-0.2.1.tar.gz` & `tmp/jsonschema_spec-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsonschema_spec-0.2.1.tar", max compression
+gzip compressed data, was "jsonschema_spec-0.2.2.tar", max compression
```

## Comparing `jsonschema_spec-0.2.1.tar` & `jsonschema_spec-0.2.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0    11357 2023-06-12 17:39:03.948618 jsonschema_spec-0.2.1/LICENSE
--rw-r--r--   0        0        0     3121 2023-06-12 17:39:03.948618 jsonschema_spec-0.2.1/README.rst
--rw-r--r--   0        0        0      360 2023-06-12 17:39:03.952618 jsonschema_spec-0.2.1/jsonschema_spec/__init__.py
--rw-r--r--   0        0        0     2477 2023-06-12 17:39:03.952618 jsonschema_spec-0.2.1/jsonschema_spec/accessors.py
--rw-r--r--   0        0        0      761 2023-06-12 17:39:03.952618 jsonschema_spec-0.2.1/jsonschema_spec/handlers/__init__.py
--rw-r--r--   0        0        0     1557 2023-06-12 17:39:03.952618 jsonschema_spec-0.2.1/jsonschema_spec/handlers/file.py
--rw-r--r--   0        0        0      210 2023-06-12 17:39:03.952618 jsonschema_spec-0.2.1/jsonschema_spec/handlers/protocols.py
--rw-r--r--   0        0        0      747 2023-06-12 17:39:03.952618 jsonschema_spec-0.2.1/jsonschema_spec/handlers/requests.py
--rw-r--r--   0        0        0      587 2023-06-12 17:39:03.952618 jsonschema_spec-0.2.1/jsonschema_spec/handlers/urllib.py
--rw-r--r--   0        0        0      361 2023-06-12 17:39:03.952618 jsonschema_spec-0.2.1/jsonschema_spec/handlers/utils.py
--rw-r--r--   0        0        0     1392 2023-06-12 17:39:03.952618 jsonschema_spec-0.2.1/jsonschema_spec/loaders.py
--rw-r--r--   0        0        0     3271 2023-06-12 17:39:03.952618 jsonschema_spec-0.2.1/jsonschema_spec/paths.py
--rw-r--r--   0        0        0        0 2023-06-12 17:39:03.952618 jsonschema_spec-0.2.1/jsonschema_spec/py.typed
--rw-r--r--   0        0        0     1116 2023-06-12 17:39:03.952618 jsonschema_spec-0.2.1/jsonschema_spec/readers.py
--rw-r--r--   0        0        0     1551 2023-06-12 17:39:03.952618 jsonschema_spec-0.2.1/jsonschema_spec/retrievers.py
--rw-r--r--   0        0        0      148 2023-06-12 17:39:03.952618 jsonschema_spec-0.2.1/jsonschema_spec/typing.py
--rw-r--r--   0        0        0      247 2023-06-12 17:39:03.952618 jsonschema_spec-0.2.1/jsonschema_spec/utils.py
--rw-r--r--   0        0        0     1906 2023-06-12 17:39:03.952618 jsonschema_spec-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     4331 1970-01-01 00:00:00.000000 jsonschema_spec-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-15 07:44:42.482506 jsonschema_spec-0.2.2/LICENSE
+-rw-r--r--   0        0        0     3121 2023-06-15 07:44:42.482506 jsonschema_spec-0.2.2/README.rst
+-rw-r--r--   0        0        0      431 2023-06-15 07:44:42.486507 jsonschema_spec-0.2.2/jsonschema_spec/__init__.py
+-rw-r--r--   0        0        0     2918 2023-06-15 07:44:42.486507 jsonschema_spec-0.2.2/jsonschema_spec/accessors.py
+-rw-r--r--   0        0        0      761 2023-06-15 07:44:42.486507 jsonschema_spec-0.2.2/jsonschema_spec/handlers/__init__.py
+-rw-r--r--   0        0        0     1557 2023-06-15 07:44:42.486507 jsonschema_spec-0.2.2/jsonschema_spec/handlers/file.py
+-rw-r--r--   0        0        0      210 2023-06-15 07:44:42.486507 jsonschema_spec-0.2.2/jsonschema_spec/handlers/protocols.py
+-rw-r--r--   0        0        0      747 2023-06-15 07:44:42.486507 jsonschema_spec-0.2.2/jsonschema_spec/handlers/requests.py
+-rw-r--r--   0        0        0      587 2023-06-15 07:44:42.486507 jsonschema_spec-0.2.2/jsonschema_spec/handlers/urllib.py
+-rw-r--r--   0        0        0      361 2023-06-15 07:44:42.486507 jsonschema_spec-0.2.2/jsonschema_spec/handlers/utils.py
+-rw-r--r--   0        0        0     1392 2023-06-15 07:44:42.486507 jsonschema_spec-0.2.2/jsonschema_spec/loaders.py
+-rw-r--r--   0        0        0     3985 2023-06-15 07:44:42.486507 jsonschema_spec-0.2.2/jsonschema_spec/paths.py
+-rw-r--r--   0        0        0        0 2023-06-15 07:44:42.486507 jsonschema_spec-0.2.2/jsonschema_spec/py.typed
+-rw-r--r--   0        0        0     1116 2023-06-15 07:44:42.486507 jsonschema_spec-0.2.2/jsonschema_spec/readers.py
+-rw-r--r--   0        0        0     1471 2023-06-15 07:44:42.486507 jsonschema_spec-0.2.2/jsonschema_spec/retrievers.py
+-rw-r--r--   0        0        0      181 2023-06-15 07:44:42.486507 jsonschema_spec-0.2.2/jsonschema_spec/typing.py
+-rw-r--r--   0        0        0      247 2023-06-15 07:44:42.486507 jsonschema_spec-0.2.2/jsonschema_spec/utils.py
+-rw-r--r--   0        0        0     1867 2023-06-15 07:44:42.486507 jsonschema_spec-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     4267 1970-01-01 00:00:00.000000 jsonschema_spec-0.2.2/PKG-INFO
```

### Comparing `jsonschema_spec-0.2.1/LICENSE` & `jsonschema_spec-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jsonschema_spec-0.2.1/README.rst` & `jsonschema_spec-0.2.2/README.rst`

 * *Files identical despite different names*

### Comparing `jsonschema_spec-0.2.1/jsonschema_spec/accessors.py` & `jsonschema_spec-0.2.2/jsonschema_spec/accessors.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,75 +2,87 @@
 from collections import deque
 from contextlib import contextmanager
 from typing import Any
 from typing import Deque
 from typing import Hashable
 from typing import Iterator
 from typing import List
-from typing import Mapping
 from typing import Optional
 from typing import Union
 
 from pathable.accessors import LookupAccessor
 from referencing import Registry
 from referencing import Specification
+from referencing._core import Resolved
 from referencing._core import Resolver
 from referencing.jsonschema import DRAFT202012
 
 from jsonschema_spec.handlers import default_handlers
-from jsonschema_spec.retrievers import HandlersRetriever
+from jsonschema_spec.retrievers import SchemaRetriever
+from jsonschema_spec.typing import Lookup
 from jsonschema_spec.typing import ResolverHandlers
 from jsonschema_spec.typing import Schema
 from jsonschema_spec.utils import is_ref
 
 
 class ResolverAccessor(LookupAccessor):
-    def __init__(self, schema: Schema, resolver: Resolver[Schema]):
-        super().__init__(schema)
+    def __init__(self, lookup: Lookup, resolver: Resolver[Lookup]):
+        super().__init__(lookup)
         self.resolver = resolver
 
+
+class SchemaAccessor(ResolverAccessor):
     @classmethod
     def from_schema(
         cls,
         schema: Schema,
         specification: Specification[Schema] = DRAFT202012,
         base_uri: str = "",
         handlers: ResolverHandlers = default_handlers,
-    ) -> "ResolverAccessor":
-        retriever = HandlersRetriever(handlers, specification)
+    ) -> "SchemaAccessor":
+        retriever = SchemaRetriever(handlers, specification)
         base_resource = specification.create_resource(schema)
         registry: Registry[Schema] = Registry(
             retrieve=retriever,  # type: ignore
         )
         registry = registry.with_resource(base_uri, base_resource)
         resolver = registry.resolver(base_uri=base_uri)
         return cls(schema, resolver)
 
     @contextmanager
     def open(self, parts: List[Hashable]) -> Iterator[Union[Schema, Any]]:
         parts_deque = deque(parts)
         try:
-            yield self._open(self.lookup, parts_deque)
+            resolved = self._resolve(self.lookup, parts_deque)
+            yield resolved.contents
+        finally:
+            pass
+
+    @contextmanager
+    def resolve(self, parts: List[Hashable]) -> Iterator[Resolved[Any]]:
+        parts_deque = deque(parts)
+        try:
+            yield self._resolve(self.lookup, parts_deque)
         finally:
             pass
 
-    def _open(
+    def _resolve(
         self,
-        content: Schema,
+        contents: Schema,
         parts_deque: Deque[Hashable],
         resolver: Optional[Resolver[Schema]] = None,
-    ) -> Any:
-        if is_ref(content):
-            ref = content["$ref"]
-            resolver = resolver or self.resolver
+    ) -> Resolved[Any]:
+        resolver = resolver or self.resolver
+        if is_ref(contents):
+            ref = contents["$ref"]
             resolved = resolver.lookup(ref)
-            return self._open(
+            return self._resolve(
                 resolved.contents, parts_deque, resolver=resolved.resolver
             )
 
         try:
             part = parts_deque.popleft()
         except IndexError:
-            return content
+            return Resolved(contents=contents, resolver=resolver)  # type: ignore
         else:
-            target = content[part]
-            return self._open(target, parts_deque, resolver=resolver)
+            target = contents[part]
+            return self._resolve(target, parts_deque, resolver=resolver)
```

### Comparing `jsonschema_spec-0.2.1/jsonschema_spec/handlers/__init__.py` & `jsonschema_spec-0.2.2/jsonschema_spec/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `jsonschema_spec-0.2.1/jsonschema_spec/handlers/file.py` & `jsonschema_spec-0.2.2/jsonschema_spec/handlers/file.py`

 * *Files identical despite different names*

### Comparing `jsonschema_spec-0.2.1/jsonschema_spec/handlers/requests.py` & `jsonschema_spec-0.2.2/jsonschema_spec/handlers/requests.py`

 * *Files identical despite different names*

### Comparing `jsonschema_spec-0.2.1/jsonschema_spec/handlers/urllib.py` & `jsonschema_spec-0.2.2/jsonschema_spec/handlers/urllib.py`

 * *Files identical despite different names*

### Comparing `jsonschema_spec-0.2.1/jsonschema_spec/loaders.py` & `jsonschema_spec-0.2.2/jsonschema_spec/loaders.py`

 * *Files identical despite different names*

### Comparing `jsonschema_spec-0.2.1/jsonschema_spec/readers.py` & `jsonschema_spec-0.2.2/jsonschema_spec/readers.py`

 * *Files identical despite different names*

### Comparing `jsonschema_spec-0.2.1/pyproject.toml` & `jsonschema_spec-0.2.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 [[tool.mypy.overrides]]
 module = "jsonschema_specifications"
 ignore_missing_imports = true
 
 [tool.poetry]
 name = "jsonschema-spec"
-version = "0.2.1"
+version = "0.2.2"
 description = "JSONSchema Spec with object-oriented paths"
 authors = ["Artur Maciag <maciag.artur@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.rst"
 repository = "https://github.com/p1c2u/jsonschema-spec"
 keywords = ["jsonschema", "swagger", "spec"]
 classifiers = [
@@ -41,27 +41,26 @@
 
 [tool.poetry.dependencies]
 pathable = "^0.4.1"
 python = "^3.8.0"
 PyYAML = ">=5.1"
 requests = {version = "^2.31.0", optional = true}
 referencing = ">=0.28.0,<0.30.0"
-jsonschema-specifications = "^2023.5.1"
 
 [tool.poetry.dev-dependencies]
 pre-commit = "*"
 pytest = "^7.3.1"
 pytest-flake8 = "=1.1.0"
 pytest-cov = "^4.1.0"
-isort = "^5.0.0"
+isort = "^5.12.0"
 black = "^23.3.0"
-flynt = "0.76"
-mypy = "^0.971"
+flynt = "0.78"
+mypy = "^1.3.0"
 types-PyYAML = "^6.0.11"
-types-requests = "^2.28.9"
+types-requests = "^2.31.0"
 responses = "^0.23.1"
 deptry = "^0.11.0"
 
 [tool.pytest.ini_options]
 addopts = """
 --capture=no
 --verbose
```

### Comparing `jsonschema_spec-0.2.1/PKG-INFO` & `jsonschema_spec-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonschema-spec
-Version: 0.2.1
+Version: 0.2.2
 Summary: JSONSchema Spec with object-oriented paths
 Home-page: https://github.com/p1c2u/jsonschema-spec
 License: Apache-2.0
 Keywords: jsonschema,swagger,spec
 Author: Artur Maciag
 Author-email: maciag.artur@gmail.com
 Requires-Python: >=3.8.0,<4.0.0
@@ -16,15 +16,14 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: PyYAML (>=5.1)
-Requires-Dist: jsonschema-specifications (>=2023.5.1,<2024.0.0)
 Requires-Dist: pathable (>=0.4.1,<0.5.0)
 Requires-Dist: referencing (>=0.28.0,<0.30.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Project-URL: Repository, https://github.com/p1c2u/jsonschema-spec
 Description-Content-Type: text/x-rst
 
 ***************
```

