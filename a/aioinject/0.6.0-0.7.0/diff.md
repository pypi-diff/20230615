# Comparing `tmp/aioinject-0.6.0.tar.gz` & `tmp/aioinject-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioinject-0.6.0.tar", last modified: Fri Jun  9 04:36:37 2023, max compression
+gzip compressed data, was "aioinject-0.7.0.tar", last modified: Thu Jun 15 08:41:58 2023, max compression
```

## Comparing `aioinject-0.6.0.tar` & `aioinject-0.7.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0      429 2023-06-09 04:36:24.553667 aioinject-0.6.0/aioinject/__init__.py
--rw-r--r--   0        0        0     2701 2023-06-09 04:28:13.918025 aioinject-0.6.0/aioinject/containers.py
--rw-r--r--   0        0        0     6734 2023-06-09 04:31:32.178144 aioinject-0.6.0/aioinject/context.py
--rw-r--r--   0        0        0     3198 2023-02-19 10:45:20.646472 aioinject-0.6.0/aioinject/decorators.py
--rw-r--r--   0        0        0        0 2022-06-21 12:45:09.224983 aioinject-0.6.0/aioinject/ext/__init__.py
--rw-r--r--   0        0        0     1142 2023-02-19 10:46:32.417782 aioinject-0.6.0/aioinject/ext/fastapi.py
--rw-r--r--   0        0        0      866 2023-03-25 23:51:07.879400 aioinject-0.6.0/aioinject/ext/strawberry.py
--rw-r--r--   0        0        0      154 2022-02-14 23:34:38.786956 aioinject-0.6.0/aioinject/markers.py
--rw-r--r--   0        0        0     5852 2023-02-19 10:37:32.040086 aioinject-0.6.0/aioinject/providers.py
--rw-r--r--   0        0        0     1063 2023-02-19 10:45:09.937041 aioinject-0.6.0/aioinject/utils.py
--rw-r--r--   0        0        0     1063 2022-02-10 14:33:31.888253 aioinject-0.6.0/LICENSE
--rw-r--r--   0        0        0     1966 2023-06-09 04:36:24.617667 aioinject-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     5266 2022-05-25 14:51:11.254512 aioinject-0.6.0/readme.md
--rw-r--r--   0        0        0        0 2022-02-10 14:33:31.896255 aioinject-0.6.0/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-02-19 10:38:23.524000 aioinject-0.6.0/tests/container/__init__.py
--rw-r--r--   0        0        0     3271 2023-06-09 04:28:11.487983 aioinject-0.6.0/tests/container/test_container.py
--rw-r--r--   0        0        0      489 2023-02-18 10:15:01.863109 aioinject-0.6.0/tests/container/test_override.py
--rw-r--r--   0        0        0        0 2022-02-14 23:35:15.649789 aioinject-0.6.0/tests/context/__init__.py
--rw-r--r--   0        0        0      500 2023-02-18 10:10:22.057657 aioinject-0.6.0/tests/context/conftest.py
--rw-r--r--   0        0        0     2022 2023-02-18 10:10:14.586441 aioinject-0.6.0/tests/context/test_context.py
--rw-r--r--   0        0        0     4256 2023-06-09 04:35:11.554281 aioinject-0.6.0/tests/context/test_context_managers.py
--rw-r--r--   0        0        0     2060 2023-02-18 11:02:03.522559 aioinject-0.6.0/tests/context/test_execute.py
--rw-r--r--   0        0        0        0 2023-02-19 10:38:23.524000 aioinject-0.6.0/tests/ext/__init__.py
--rw-r--r--   0        0        0        0 2023-02-19 10:38:23.524000 aioinject-0.6.0/tests/ext/strawberry/__init__.py
--rw-r--r--   0        0        0      818 2023-02-18 11:06:42.742442 aioinject-0.6.0/tests/ext/strawberry/test_inject_decorator.py
--rw-r--r--   0        0        0        0 2022-02-10 14:33:31.897254 aioinject-0.6.0/tests/providers/__init__.py
--rw-r--r--   0        0        0     4257 2023-02-19 10:29:06.577098 aioinject-0.6.0/tests/providers/test_callable.py
--rw-r--r--   0        0        0     1139 2023-02-18 11:02:25.628622 aioinject-0.6.0/tests/providers/test_object.py
--rw-r--r--   0        0        0      686 2023-02-18 09:50:26.751944 aioinject-0.6.0/tests/providers/test_singleton.py
--rw-r--r--   0        0        0     3845 2023-02-19 10:03:00.125198 aioinject-0.6.0/tests/test_inject.py
--rw-r--r--   0        0        0       39 2022-08-16 11:16:21.152175 aioinject-0.6.0/tests/utils/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2022-08-16 11:16:21.153175 aioinject-0.6.0/tests/utils/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      310 2022-08-16 11:16:21.152175 aioinject-0.6.0/tests/utils/.pytest_cache/README.md
--rw-r--r--   0        0        0       43 2022-08-16 11:16:21.153175 aioinject-0.6.0/tests/utils/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2022-08-16 11:16:21.154175 aioinject-0.6.0/tests/utils/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0        0 2023-02-19 10:38:23.524819 aioinject-0.6.0/tests/utils/__init__.py
--rw-r--r--   0        0        0     1502 2023-02-19 10:35:54.331885 aioinject-0.6.0/tests/utils/test_guess_impl.py
--rw-r--r--   0        0        0      520 2023-02-18 11:01:50.087958 aioinject-0.6.0/tests/utils/test_utils.py
--rw-r--r--   0        0        0     5443 1970-01-01 00:00:00.000000 aioinject-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0      429 2023-06-15 08:41:37.030861 aioinject-0.7.0/aioinject/__init__.py
+-rw-r--r--   0        0        0     2701 2023-06-09 04:28:13.918025 aioinject-0.7.0/aioinject/containers.py
+-rw-r--r--   0        0        0     7191 2023-06-15 08:38:21.343298 aioinject-0.7.0/aioinject/context.py
+-rw-r--r--   0        0        0     3198 2023-02-19 10:45:20.646472 aioinject-0.7.0/aioinject/decorators.py
+-rw-r--r--   0        0        0        0 2022-06-21 12:45:09.224983 aioinject-0.7.0/aioinject/ext/__init__.py
+-rw-r--r--   0        0        0     1142 2023-02-19 10:46:32.417782 aioinject-0.7.0/aioinject/ext/fastapi.py
+-rw-r--r--   0        0        0      866 2023-03-25 23:51:07.879400 aioinject-0.7.0/aioinject/ext/strawberry.py
+-rw-r--r--   0        0        0      154 2022-02-14 23:34:38.786956 aioinject-0.7.0/aioinject/markers.py
+-rw-r--r--   0        0        0     6152 2023-06-15 08:40:09.657942 aioinject-0.7.0/aioinject/providers.py
+-rw-r--r--   0        0        0     1078 2023-06-15 08:09:15.419129 aioinject-0.7.0/aioinject/utils.py
+-rw-r--r--   0        0        0     1063 2022-02-10 14:33:31.888253 aioinject-0.7.0/LICENSE
+-rw-r--r--   0        0        0     1966 2023-06-15 08:41:37.095859 aioinject-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     5266 2022-05-25 14:51:11.254512 aioinject-0.7.0/readme.md
+-rw-r--r--   0        0        0        0 2022-02-10 14:33:31.896255 aioinject-0.7.0/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-19 10:38:23.524000 aioinject-0.7.0/tests/container/__init__.py
+-rw-r--r--   0        0        0     3302 2023-06-15 07:30:36.661079 aioinject-0.7.0/tests/container/test_container.py
+-rw-r--r--   0        0        0      489 2023-02-18 10:15:01.863109 aioinject-0.7.0/tests/container/test_override.py
+-rw-r--r--   0        0        0        0 2022-02-14 23:35:15.649789 aioinject-0.7.0/tests/context/__init__.py
+-rw-r--r--   0        0        0      500 2023-02-18 10:10:22.057657 aioinject-0.7.0/tests/context/conftest.py
+-rw-r--r--   0        0        0     2022 2023-02-18 10:10:14.586441 aioinject-0.7.0/tests/context/test_context.py
+-rw-r--r--   0        0        0     4256 2023-06-15 08:37:09.906573 aioinject-0.7.0/tests/context/test_context_managers.py
+-rw-r--r--   0        0        0     2060 2023-02-18 11:02:03.522559 aioinject-0.7.0/tests/context/test_execute.py
+-rw-r--r--   0        0        0        0 2023-02-19 10:38:23.524000 aioinject-0.7.0/tests/ext/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-19 10:38:23.524000 aioinject-0.7.0/tests/ext/strawberry/__init__.py
+-rw-r--r--   0        0        0      818 2023-02-18 11:06:42.742442 aioinject-0.7.0/tests/ext/strawberry/test_inject_decorator.py
+-rw-r--r--   0        0        0        0 2022-02-10 14:33:31.897254 aioinject-0.7.0/tests/providers/__init__.py
+-rw-r--r--   0        0        0     4257 2023-06-15 08:40:10.535168 aioinject-0.7.0/tests/providers/test_callable.py
+-rw-r--r--   0        0        0     1139 2023-02-18 11:02:25.628622 aioinject-0.7.0/tests/providers/test_object.py
+-rw-r--r--   0        0        0      686 2023-02-18 09:50:26.751944 aioinject-0.7.0/tests/providers/test_singleton.py
+-rw-r--r--   0        0        0     3845 2023-02-19 10:03:00.125198 aioinject-0.7.0/tests/test_inject.py
+-rw-r--r--   0        0        0       39 2022-08-16 11:16:21.152175 aioinject-0.7.0/tests/utils/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2022-08-16 11:16:21.153175 aioinject-0.7.0/tests/utils/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      310 2022-08-16 11:16:21.152175 aioinject-0.7.0/tests/utils/.pytest_cache/README.md
+-rw-r--r--   0        0        0       43 2022-08-16 11:16:21.153175 aioinject-0.7.0/tests/utils/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2022-08-16 11:16:21.154175 aioinject-0.7.0/tests/utils/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0        0 2023-02-19 10:38:23.524819 aioinject-0.7.0/tests/utils/__init__.py
+-rw-r--r--   0        0        0     1562 2023-06-15 08:40:10.557168 aioinject-0.7.0/tests/utils/test_guess_impl.py
+-rw-r--r--   0        0        0      520 2023-02-18 11:01:50.087958 aioinject-0.7.0/tests/utils/test_utils.py
+-rw-r--r--   0        0        0     5443 1970-01-01 00:00:00.000000 aioinject-0.7.0/PKG-INFO
```

### Comparing `aioinject-0.6.0/aioinject/containers.py` & `aioinject-0.7.0/aioinject/containers.py`

 * *Files identical despite different names*

### Comparing `aioinject-0.6.0/aioinject/context.py` & `aioinject-0.7.0/aioinject/context.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 container_var: ContextVar[Container] = ContextVar("aioinject_container")
 
 TypeAndImpl = tuple[type[_T], _T | None]
 TExitStack = TypeVar("TExitStack")
 
 
-class DiCache(Protocol):
+class DICache(Protocol):
     def __setitem__(self, key: TypeAndImpl[_T], value: _T) -> None:
         ...  # pragma: no cover
 
     def __getitem__(self, item: TypeAndImpl[_T]) -> _T:
         ...  # pragma: no cover
 
     def __contains__(self, item: TypeAndImpl) -> bool:
@@ -45,15 +45,15 @@
         self,
         container: Container,
         singleton_exit_stack: AsyncExitStack,
     ) -> None:
         self.container = container
         self.singleton_exit_stack = singleton_exit_stack
         self.exit_stack = self._exit_stack_type()
-        self.cache: DiCache = {}
+        self.cache: DICache = {}
         self._token = None
 
     def __class_getitem__(
         cls,
         item: type[TExitStack],
     ) -> _BaseInjectionContext[TExitStack]:
         return type(  # type: ignore[return-value]
@@ -66,14 +66,23 @@
         self,
         provider: Provider,
     ) -> TExitStack | AsyncExitStack:
         if isinstance(provider, Singleton):
             return self.singleton_exit_stack
         return self.exit_stack
 
+    def _update_singleton_cache(
+        self,
+        provider: Provider,
+        resolved_value: Any,
+    ) -> None:
+        if not isinstance(provider, Singleton):
+            return
+        provider.cache = resolved_value
+
 
 class InjectionContext(_BaseInjectionContext[AsyncExitStack]):
     async def resolve(
         self,
         type_: type[_T],
         impl: Any | None = None,
         *,
@@ -98,15 +107,18 @@
         if isinstance(resolved, contextlib.ContextDecorator):
             resolved = stack.enter_context(resolved)  # type: ignore[arg-type]
 
         if isinstance(resolved, contextlib.AsyncContextDecorator):
             resolved = await stack.enter_async_context(
                 resolved,  # type: ignore[arg-type]
             )
-
+        self._update_singleton_cache(
+            provider=provider,
+            resolved_value=resolved,
+        )
         if use_cache:
             self.cache[type_, impl] = resolved
         return resolved
 
     @typing.overload
     async def execute(
         self,
@@ -181,15 +193,18 @@
             )
             for dep in provider.dependencies
         }
 
         resolved = provider.provide_sync(**dependencies)
         if isinstance(resolved, contextlib.ContextDecorator):
             resolved = self.exit_stack.enter_context(resolved)  # type: ignore[arg-type]
-
+        self._update_singleton_cache(
+            provider=provider,
+            resolved_value=resolved,
+        )
         if use_cache:
             self.cache[type_, impl] = resolved
         return resolved
 
     def execute(
         self,
         function: Callable[..., _T],
```

### Comparing `aioinject-0.6.0/aioinject/decorators.py` & `aioinject-0.7.0/aioinject/decorators.py`

 * *Files identical despite different names*

### Comparing `aioinject-0.6.0/aioinject/ext/fastapi.py` & `aioinject-0.7.0/aioinject/ext/fastapi.py`

 * *Files identical despite different names*

### Comparing `aioinject-0.6.0/aioinject/ext/strawberry.py` & `aioinject-0.7.0/aioinject/ext/strawberry.py`

 * *Files identical despite different names*

### Comparing `aioinject-0.6.0/aioinject/providers.py` & `aioinject-0.7.0/aioinject/providers.py`

 * *Files 6% similar despite different names*

```diff
@@ -84,21 +84,21 @@
                 break
         else:
             type_hints[key] = Annotated[value, Inject]
 
     return type_hints
 
 
-_ITERABLES = {
+_GENERATORS = {
     collections.abc.Generator,
-    collections.abc.AsyncGenerator,
     collections.abc.Iterator,
+}
+_ASYNC_GENERATORS = {
+    collections.abc.AsyncGenerator,
     collections.abc.AsyncIterator,
-    collections.abc.Iterable,
-    collections.abc.AsyncIterable,
 }
 
 
 def _guess_impl(factory: t.Callable[..., Any]) -> type:
     if isclass(factory):
         return factory
     type_hints = typing.get_type_hints(factory)
@@ -108,15 +108,27 @@
         err_msg = (
             f"factory {factory.__qualname__} does not specify return type."
         )
         raise ValueError(err_msg) from e
 
     if origin := typing.get_origin(return_type):
         args = typing.get_args(return_type)
-        if origin in _ITERABLES:
+
+        maybe_wrapped = getattr(  # @functools.wraps
+            factory,
+            "__wrapped__",
+            factory,
+        )
+        if origin in _ASYNC_GENERATORS and inspect.isasyncgenfunction(
+            maybe_wrapped,
+        ):
+            return args[0]
+        if origin in _GENERATORS and inspect.isgeneratorfunction(
+            maybe_wrapped,
+        ):
             return args[0]
     return return_type
 
 
 class Provider(t.Generic[_T], abc.ABC):
     def __init__(self, type_: type[_T], impl: Any) -> None:
         self.type = type_
```

### Comparing `aioinject-0.6.0/aioinject/utils.py` & `aioinject-0.7.0/aioinject/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,17 @@
     inject_annotations = get_inject_annotations(wrapper)
     signature = inspect.signature(wrapper)
     new_params = tuple(
         p
         for p in signature.parameters.values()
         if p.name not in inject_annotations
     )
-    wrapper.__signature__ = signature.replace(parameters=new_params)  # type: ignore[attr-defined]
+    wrapper.__signature__ = signature.replace(  # type: ignore[attr-defined]
+        parameters=new_params,
+    )
     for name in inject_annotations:
         del wrapper.__annotations__[name]
     return wrapper
 
 
 def get_inject_annotations(function: Callable[..., Any]) -> dict[str, Any]:
     return {
```

### Comparing `aioinject-0.6.0/LICENSE` & `aioinject-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aioinject-0.6.0/pyproject.toml` & `aioinject-0.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 composite = [
     "coverage run",
     "coverage report",
 ]
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.6.0"
+version = "0.7.0"
 version_files = [
     "aioinject/__init__.py",
     "pyproject.toml:version",
 ]
 
 [tool.coverage.run]
 source = [
@@ -108,15 +108,15 @@
 ]
 staticmethod-decorators = [
     "staticmethod",
 ]
 
 [project]
 name = "aioinject"
-version = "0.6.0"
+version = "0.7.0"
 description = ""
 authors = [
     { name = "Doctor", email = "thirvondukr@gmail.com" },
 ]
 dependencies = []
 requires-python = ">=3.10"
 readme = "readme.md"
```

### Comparing `aioinject-0.6.0/readme.md` & `aioinject-0.7.0/readme.md`

 * *Files identical despite different names*

### Comparing `aioinject-0.6.0/tests/container/test_container.py` & `aioinject-0.7.0/tests/container/test_container.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,13 +108,14 @@
         yield 42
         shutdown = True
 
     provider = Singleton(dependency)
 
     container = Container()
     container.register(provider)
-    async with container.context() as ctx:
-        assert await ctx.resolve(int) == 42  # noqa: PLR2004
+    for _ in range(2):
+        async with container.context() as ctx:
+            assert await ctx.resolve(int) == 42  # noqa: PLR2004
     assert shutdown is False
 
     await container.aclose()
     assert shutdown is True
```

### Comparing `aioinject-0.6.0/tests/context/test_context.py` & `aioinject-0.7.0/tests/context/test_context.py`

 * *Files identical despite different names*

### Comparing `aioinject-0.6.0/tests/context/test_context_managers.py` & `aioinject-0.7.0/tests/context/test_context_managers.py`

 * *Files identical despite different names*

### Comparing `aioinject-0.6.0/tests/context/test_execute.py` & `aioinject-0.7.0/tests/context/test_execute.py`

 * *Files identical despite different names*

### Comparing `aioinject-0.6.0/tests/ext/strawberry/test_inject_decorator.py` & `aioinject-0.7.0/tests/ext/strawberry/test_inject_decorator.py`

 * *Files identical despite different names*

### Comparing `aioinject-0.6.0/tests/providers/test_callable.py` & `aioinject-0.7.0/tests/providers/test_callable.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from collections import defaultdict
-from collections.abc import AsyncGenerator, AsyncIterable, Generator, Iterable
+from collections.abc import AsyncGenerator, AsyncIterator, Generator, Iterator
 from typing import Annotated
 from unittest.mock import patch
 
 import pytest
 
 from aioinject import Inject, Provider, providers
 from aioinject.providers import Dependency
@@ -149,21 +149,21 @@
             use_cache=False,
         ),
     )
     assert provider.dependencies == expected
 
 
 def test_generator_return_types() -> None:
-    def iterable() -> Iterable[int]:
+    def iterable() -> Iterator[int]:
         yield 42
 
     def gen() -> Generator[int, None, None]:
         yield 42
 
-    async def async_iterable() -> AsyncIterable[int]:
+    async def async_iterable() -> AsyncIterator[int]:
         yield 42
 
     async def async_gen() -> AsyncGenerator[int, None]:
         yield 42
 
     factories = [iterable, gen, async_iterable, async_gen]
     for factory in factories:
```

### Comparing `aioinject-0.6.0/tests/providers/test_object.py` & `aioinject-0.7.0/tests/providers/test_object.py`

 * *Files identical despite different names*

### Comparing `aioinject-0.6.0/tests/providers/test_singleton.py` & `aioinject-0.7.0/tests/providers/test_singleton.py`

 * *Files identical despite different names*

### Comparing `aioinject-0.6.0/tests/test_inject.py` & `aioinject-0.7.0/tests/test_inject.py`

 * *Files identical despite different names*

### Comparing `aioinject-0.6.0/tests/utils/test_guess_impl.py` & `aioinject-0.7.0/tests/utils/test_guess_impl.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,9 @@
-from collections.abc import (
-    AsyncGenerator,
-    AsyncIterable,
-    AsyncIterator,
-    Generator,
-    Iterable,
-    Iterator,
-)
+import contextlib
+from collections.abc import AsyncGenerator, AsyncIterator, Generator, Iterator
 from typing import TypeAlias
 
 import pytest
 
 from aioinject.providers import _guess_impl
 
 
@@ -41,32 +35,32 @@
     msg = f"factory {factory.__qualname__} does not specify return type."
     assert str(exc_info.value) == msg
 
 
 @pytest.mark.parametrize(
     "return_type",
     [
-        Iterable[int],
         Iterator[int],
         Generator[int, None, None],
     ],
 )
 def test_sync_iterables(return_type: TypeAlias) -> None:
     def iterable() -> return_type:
-        ...
+        yield None
 
     assert _guess_impl(iterable) is int
+    assert _guess_impl(contextlib.contextmanager(iterable)) is int
 
 
 @pytest.mark.parametrize(
     "return_type",
     [
-        AsyncIterable[int],
         AsyncIterator[int],
         AsyncGenerator[int, None],
     ],
 )
 def test_async_iterables(return_type: TypeAlias) -> None:
     async def iterable() -> return_type:
-        ...
+        yield None
 
     assert _guess_impl(iterable) is int
+    assert _guess_impl(contextlib.asynccontextmanager(iterable)) is int
```

### Comparing `aioinject-0.6.0/tests/utils/test_utils.py` & `aioinject-0.7.0/tests/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `aioinject-0.6.0/PKG-INFO` & `aioinject-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioinject
-Version: 0.6.0
+Version: 0.7.0
 License: MIT
 Author-email: Doctor <thirvondukr@gmail.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 Async-first dependency injection library based on python type hints
```

