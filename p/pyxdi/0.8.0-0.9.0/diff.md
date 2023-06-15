# Comparing `tmp/pyxdi-0.8.0.tar.gz` & `tmp/pyxdi-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyxdi-0.8.0.tar", max compression
+gzip compressed data, was "pyxdi-0.9.0.tar", max compression
```

## Comparing `pyxdi-0.8.0.tar` & `pyxdi-0.9.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1069 2023-02-14 18:16:50.284355 pyxdi-0.8.0/LICENSE
--rw-r--r--   0        0        0     1547 2023-05-18 06:53:42.467888 pyxdi-0.8.0/README.md
--rw-r--r--   0        0        0     1593 2023-05-18 06:54:49.408916 pyxdi-0.8.0/pyproject.toml
--rw-r--r--   0        0        0      261 2023-05-18 06:53:42.470025 pyxdi-0.8.0/pyxdi/__init__.py
--rw-r--r--   0        0        0    30693 2023-05-18 06:53:42.470484 pyxdi-0.8.0/pyxdi/core.py
--rw-r--r--   0        0        0     2324 2023-05-18 06:53:42.470811 pyxdi-0.8.0/pyxdi/decorators.py
--rw-r--r--   0        0        0      263 2023-05-16 11:55:56.050387 pyxdi-0.8.0/pyxdi/exceptions.py
--rw-r--r--   0        0        0        0 2023-03-24 15:06:03.633484 pyxdi-0.8.0/pyxdi/ext/__init__.py
--rw-r--r--   0        0        0     2768 2023-05-16 11:55:56.050777 pyxdi-0.8.0/pyxdi/ext/fastapi.py
--rw-r--r--   0        0        0        0 2023-03-24 15:06:03.633846 pyxdi-0.8.0/pyxdi/ext/starlette/__init__.py
--rw-r--r--   0        0        0      629 2023-05-18 06:53:42.471309 pyxdi-0.8.0/pyxdi/ext/starlette/middleware.py
--rw-r--r--   0        0        0        0 2023-02-14 18:16:50.285713 pyxdi-0.8.0/pyxdi/py.typed
--rw-r--r--   0        0        0     1487 2023-05-18 06:53:42.471733 pyxdi-0.8.0/pyxdi/utils.py
--rw-r--r--   0        0        0     2485 1970-01-01 00:00:00.000000 pyxdi-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-02-14 18:16:50.284355 pyxdi-0.9.0/LICENSE
+-rw-r--r--   0        0        0     1547 2023-05-18 06:53:42.467888 pyxdi-0.9.0/README.md
+-rw-r--r--   0        0        0     1593 2023-05-20 07:30:10.212363 pyxdi-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0      261 2023-05-18 06:53:42.470025 pyxdi-0.9.0/pyxdi/__init__.py
+-rw-r--r--   0        0        0    32635 2023-05-20 07:29:53.700877 pyxdi-0.9.0/pyxdi/core.py
+-rw-r--r--   0        0        0     2217 2023-05-20 07:29:53.701102 pyxdi-0.9.0/pyxdi/decorators.py
+-rw-r--r--   0        0        0      278 2023-05-20 07:29:53.701235 pyxdi-0.9.0/pyxdi/exceptions.py
+-rw-r--r--   0        0        0        0 2023-03-24 15:06:03.633484 pyxdi-0.9.0/pyxdi/ext/__init__.py
+-rw-r--r--   0        0        0     2543 2023-05-20 07:29:53.701525 pyxdi-0.9.0/pyxdi/ext/fastapi.py
+-rw-r--r--   0        0        0        0 2023-03-24 15:06:03.633846 pyxdi-0.9.0/pyxdi/ext/starlette/__init__.py
+-rw-r--r--   0        0        0      629 2023-05-18 06:53:42.471309 pyxdi-0.9.0/pyxdi/ext/starlette/middleware.py
+-rw-r--r--   0        0        0        0 2023-02-14 18:16:50.285713 pyxdi-0.9.0/pyxdi/py.typed
+-rw-r--r--   0        0        0     1487 2023-05-18 06:53:42.471733 pyxdi-0.9.0/pyxdi/utils.py
+-rw-r--r--   0        0        0     2485 1970-01-01 00:00:00.000000 pyxdi-0.9.0/PKG-INFO
```

### Comparing `pyxdi-0.8.0/LICENSE` & `pyxdi-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyxdi-0.8.0/README.md` & `pyxdi-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `pyxdi-0.8.0/pyproject.toml` & `pyxdi-0.9.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyxdi"
-version = "0.8.0"
+version = "0.9.0"
 description = "Dependency Injection library"
 authors = ["Anton Ruhlov <antonruhlov@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/antonrh/pyxdi"
 keywords = ["dependency injection", "dependencies", "di", "async", "asyncio", "application"]
 packages = [
```

### Comparing `pyxdi-0.8.0/pyxdi/core.py` & `pyxdi-0.9.0/pyxdi/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 from __future__ import annotations
 
 import contextlib
 import importlib
 import inspect
-import logging
 import pkgutil
 import types
 import typing as t
 import uuid
 from collections import defaultdict
 from contextvars import ContextVar
 from dataclasses import dataclass
 from functools import cached_property, wraps
 
-from typing_extensions import Annotated, ParamSpec
+from typing_extensions import Annotated, ParamSpec, Self
 
 try:
     from types import NoneType
 except ImportError:
     NoneType = type(None)  # type: ignore[assignment,misc]
 
 
 from .exceptions import (
     AnnotationError,
-    InvalidScope,
+    InvalidScopeError,
     ProviderError,
-    ScopeMismatch,
-    UnknownDependency,
+    ScopeMismatchError,
+    UnknownDependencyError,
 )
 from .utils import (
     get_full_qualname,
     get_signature,
     is_builtin_type,
     make_lazy,
     run_async,
@@ -42,16 +41,14 @@
 
 ALLOWED_SCOPES: t.Dict[Scope, t.List[Scope]] = {
     "singleton": ["singleton"],
     "request": ["request", "singleton"],
     "transient": ["transient", "singleton", "request"],
 }
 
-logger = logging.getLogger(__name__)
-
 
 @dataclass(frozen=True)
 class Provider:
     obj: t.Callable[..., t.Any]
     scope: Scope
 
     def __str__(self) -> str:
@@ -68,14 +65,18 @@
     @cached_property
     def is_function(self) -> bool:
         return (inspect.isfunction(self.obj) or inspect.ismethod(self.obj)) and not (
             self.is_resource or self.is_async_resource
         )
 
     @cached_property
+    def is_coroutine(self) -> bool:
+        return inspect.iscoroutinefunction(self.obj)
+
+    @cached_property
     def is_resource(self) -> bool:
         return inspect.isgeneratorfunction(self.obj)
 
     @cached_property
     def is_async_resource(self) -> bool:
         return inspect.isasyncgenfunction(self.obj)
 
@@ -87,15 +88,14 @@
     provider: Provider
 
 
 @dataclass(frozen=True)
 class ScannedDependency:
     member: t.Any
     module: types.ModuleType
-    lazy: t.Optional[bool] = None
 
 
 class DependencyMark:
     __slots__ = ()
 
 
 # Dependency mark with Any type
@@ -111,31 +111,30 @@
 
 @dataclass(frozen=True)
 class UnresolvedDependency:
     parameter_name: str
     obj: t.Callable[..., t.Any]
 
 
+@t.final
 class PyxDI:
     def __init__(
         self,
         *,
         default_scope: Scope = "singleton",
         auto_register: bool = False,
-        lazy_inject: bool = False,
         modules: t.Optional[
-            t.Sequence[t.Union[Module, t.Type[Module], t.Callable[["PyxDI"], None]]],
+            t.Sequence[t.Union[Module, t.Type[Module], t.Callable[[PyxDI], None]]],
         ] = None,
     ) -> None:
         self._default_scope = default_scope
         self._auto_register = auto_register
-        self._lazy_inject = lazy_inject
         self._providers: t.Dict[t.Type[t.Any], Provider] = {}
-        self._singleton_context = ScopedContext("singleton", self)
-        self._request_context_var: ContextVar[t.Optional[ScopedContext]] = ContextVar(
+        self._singleton_context = SingletonContext(self)
+        self._request_context_var: ContextVar[t.Optional[RequestContext]] = ContextVar(
             "request_context", default=None
         )
         self._unresolved_providers: t.Dict[
             t.Type[t.Any], t.List[UnresolvedProvider]
         ] = defaultdict(list)
         self._unresolved_dependencies: t.Dict[t.Type[t.Any], UnresolvedDependency] = {}
 
@@ -149,18 +148,14 @@
         return self._default_scope
 
     @property
     def auto_register(self) -> bool:
         return self._auto_register
 
     @property
-    def lazy_inject(self) -> bool:
-        return self._lazy_inject
-
-    @property
     def providers(self) -> t.Dict[t.Type[t.Any], Provider]:
         return self._providers
 
     # Provider
 
     def has_provider(self, interface: t.Type[t.Any]) -> bool:
         return interface in self._providers
@@ -171,33 +166,31 @@
         obj: t.Callable[..., t.Any],
         *,
         scope: t.Optional[Scope] = None,
         override: bool = False,
     ) -> Provider:
         provider = Provider(obj=obj, scope=scope or self.default_scope)
 
+        # Create Event type
         if (provider.is_resource or provider.is_async_resource) and (
             interface is NoneType or interface is None
         ):
-            interface = type(f"EventResource_{uuid.uuid4()}", (), {})
+            interface = type(f"Event{uuid.uuid4().hex}", (), {})
 
-        try:
-            self.get_provider(interface)
-        except ProviderError:
-            pass
-        else:
+        if interface in self._providers:
             if override:
                 self._providers[interface] = provider
                 return provider
 
             raise ProviderError(
                 f"The provider interface `{get_full_qualname(interface)}` "
                 "already registered."
             )
 
+        # Validate provider
         self._validate_provider_scope(provider)
         self._validate_provider_type(provider)
         self._validate_provider_match_scopes(interface, provider)
 
         self._providers[interface] = provider
         return provider
 
@@ -230,34 +223,42 @@
     def get_provider(self, interface: t.Type[t.Any]) -> Provider:
         """
         Get provider by interface.
         """
         try:
             return self._providers[interface]
         except KeyError as exc:
+            # Try to auto register instance class, or raise ProviderError
+            if (
+                self.auto_register
+                and inspect.isclass(interface)
+                and not is_builtin_type(interface)
+            ):
+                scope = getattr(interface, "__pyxdi_scope__", self.default_scope)
+                return self.register_provider(interface, interface, scope=scope)
             raise ProviderError(
                 f"The provider interface for `{get_full_qualname(interface)}` has "
                 "not been registered. Please ensure that the provider interface is "
                 "properly registered before attempting to use it."
             ) from exc
 
     def singleton(
-        self, interface: t.Type[T], instance: t.Any, *, override: bool = False
+        self, interface: t.Type[t.Any], instance: t.Any, *, override: bool = False
     ) -> Provider:
         """
         Register singleton instance provider.
         """
         return self.register_provider(
             interface, lambda: instance, scope="singleton", override=override
         )
 
     # Validators
     def _validate_provider_scope(self, provider: Provider) -> None:
         if provider.scope not in t.get_args(Scope):
-            raise InvalidScope(
+            raise InvalidScopeError(
                 "The scope provided is invalid. Only the following scopes are "
                 f"supported: {', '.join(t.get_args(Scope))}. Please use one of the "
                 "supported scopes when registering a provider."
             )
 
     def _validate_provider_type(self, provider: Provider) -> None:
         if provider.is_function or provider.is_class:
@@ -310,15 +311,15 @@
         for related_provider, direct in related_providers:
             if direct:
                 left_scope, right_scope = related_provider.scope, scope
             else:
                 left_scope, right_scope = scope, related_provider.scope
             allowed_scopes = ALLOWED_SCOPES.get(right_scope) or []
             if left_scope not in allowed_scopes:
-                raise ScopeMismatch(
+                raise ScopeMismatchError(
                     f"The provider `{get_full_qualname(obj)}` with a {scope} scope was "
                     f"attempted to be registered with the provider "
                     f"`{related_provider}` with a `{related_provider.scope}` scope, "
                     f"which is not allowed. Please ensure that all providers are "
                     f"registered with matching scopes."
                 )
 
@@ -333,15 +334,15 @@
                     parameter_name = unresolved_provider.parameter_name
                     provider_name = get_full_qualname(unresolved_provider.provider.obj)
                     errors.append(
                         f"- `{provider_name}` has unknown `{parameter_name}: "
                         f"{get_full_qualname(unresolved_interface)}` parameter"
                     )
             message = "\n".join(errors)
-            raise UnknownDependency(
+            raise UnknownDependencyError(
                 "The following unknown provided dependencies were detected:"
                 f"\n{message}."
             )
         if self._unresolved_dependencies:
             errors = []
             for (
                 unresolved_interface,
@@ -354,22 +355,22 @@
                     f"- `{get_full_qualname(dependency.obj)}` has unknown "
                     f"`{parameter_name}: {get_full_qualname(unresolved_interface)}` "
                     f"injected parameter"
                 )
             if not errors:
                 return
             message = "\n".join(errors)
-            raise UnknownDependency(
+            raise UnknownDependencyError(
                 "The following unknown injected dependencies were detected:"
                 f"\n{message}."
             )
 
     # Modules
     def register_module(
-        self, module: t.Union[Module, t.Type[Module], t.Callable[["PyxDI"], None]]
+        self, module: t.Union[Module, t.Type[Module], t.Callable[[PyxDI], None]]
     ) -> None:
         """
         Register module as callable, Module type or Module instance.
         """
         # Callable Module
         if inspect.isfunction(module):
             module(self)
@@ -394,47 +395,46 @@
         self._singleton_context.start()
 
     def close(self) -> None:
         self._singleton_context.close()
 
     def request_context(
         self,
-    ) -> t.ContextManager["ScopedContext"]:
+    ) -> t.ContextManager[RequestContext]:
         return contextlib.contextmanager(self._request_context)()
 
-    def _request_context(self) -> t.Iterator["ScopedContext"]:
-        with self._create_request_context() as context:
-            token = self._request_context_var.set(context)
+    def _request_context(self) -> t.Iterator[RequestContext]:
+        context = RequestContext(self)
+        token = self._request_context_var.set(context)
+        with context:
             yield context
             self._request_context_var.reset(token)
 
     # Asynchronous lifespan
 
     async def astart(self) -> None:
         self.validate()
         await self._singleton_context.astart()
 
     async def aclose(self) -> None:
         await self._singleton_context.aclose()
 
     def arequest_context(
         self,
-    ) -> t.AsyncContextManager["ScopedContext"]:
+    ) -> t.AsyncContextManager[RequestContext]:
         return contextlib.asynccontextmanager(self._arequest_context)()
 
-    async def _arequest_context(self) -> t.AsyncIterator["ScopedContext"]:
-        async with self._create_request_context() as context:
-            token = self._request_context_var.set(context)
+    async def _arequest_context(self) -> t.AsyncIterator[RequestContext]:
+        context = RequestContext(self)
+        token = self._request_context_var.set(context)
+        async with context:
             yield context
             self._request_context_var.reset(token)
 
-    def _create_request_context(self) -> "ScopedContext":
-        return ScopedContext("request", self)
-
-    def _get_request_context(self) -> "ScopedContext":
+    def _get_request_context(self) -> RequestContext:
         request_context = self._request_context_var.get()
         if request_context is None:
             raise LookupError(
                 "The request context has not been started. Please ensure that "
                 "the request context is properly initialized before attempting "
                 "to use it."
             )
@@ -442,47 +442,48 @@
 
     # Instance
 
     def get(self, interface: t.Type[T]) -> T:
         """
         Get instance by interface.
         """
-        try:
-            provider = self.get_provider(interface)
-        except ProviderError:
-            if (
-                self.auto_register
-                and inspect.isclass(interface)
-                and not is_builtin_type(interface)
-            ):
-                scope = getattr(interface, "__pyxdi_scope__", self._default_scope)
-                provider = self.register_provider(interface, interface, scope=scope)
-            else:
-                raise
+        provider = self.get_provider(interface)
 
         scoped_context = self._get_scoped_context(provider.scope)
         if scoped_context:
             return scoped_context.get(interface)
 
         return t.cast(T, self.create_instance(provider))
 
+    async def aget(self, interface: t.Type[T]) -> T:
+        """
+        Get instance by interface.
+        """
+        provider = self.get_provider(interface)
+
+        scoped_context = self._get_scoped_context(provider.scope)
+        if scoped_context:
+            return await scoped_context.aget(interface)
+
+        return t.cast(T, await self.acreate_instance(provider))
+
     def has(self, interface: t.Type[T]) -> bool:
         """
         Check that container contains instance by interface.
         """
         try:
             provider = self.get_provider(interface)
         except ProviderError:
             return False
         scoped_context = self._get_scoped_context(provider.scope)
         if scoped_context:
             return scoped_context.has(interface)
         return True
 
-    def _get_scoped_context(self, scope: Scope) -> t.Optional["ScopedContext"]:
+    def _get_scoped_context(self, scope: Scope) -> t.Optional[ScopedContext]:
         if scope == "singleton":
             return self._singleton_context
         elif scope == "request":
             request_context = self._get_request_context()
             return request_context
         return None
 
@@ -531,27 +532,42 @@
 
     async def acreate_resource(
         self,
         provider: Provider,
         *,
         stack: contextlib.AsyncExitStack,
     ) -> t.Any:
-        args, kwargs = self._get_provider_arguments(provider)
+        args, kwargs = await self._aget_provider_arguments(provider)
         cm = contextlib.asynccontextmanager(provider.obj)(*args, **kwargs)
         return await stack.enter_async_context(cm)
 
     def create_instance(self, provider: Provider) -> t.Any:
+        self._validate_instance_is_not_resource(provider)
+        if provider.is_coroutine:
+            raise ProviderError(
+                f"The instance for the coroutine provider `{provider}` cannot be "
+                "created in synchronous mode."
+            )
+        args, kwargs = self._get_provider_arguments(provider)
+        return provider.obj(*args, **kwargs)
+
+    async def acreate_instance(self, provider: Provider) -> t.Any:
+        self._validate_instance_is_not_resource(provider)
+        args, kwargs = await self._aget_provider_arguments(provider)
+        if provider.is_coroutine:
+            return await provider.obj(*args, **kwargs)
+        return provider.obj(*args, **kwargs)
+
+    def _validate_instance_is_not_resource(self, provider: Provider) -> None:
         if provider.is_resource or provider.is_async_resource:
             raise ProviderError(
                 f"The instance for the resource provider `{provider}` cannot be "
                 "created until the scope context has been started. Please ensure "
                 "that the scope context is started."
             )
-        args, kwargs = self._get_provider_arguments(provider)
-        return provider.obj(*args, **kwargs)
 
     # Decorators
 
     @t.overload
     def provider(self, func: t.Callable[P, T]) -> t.Callable[P, T]:
         ...
 
@@ -588,58 +604,51 @@
     def inject(
         self, obj: t.Callable[P, t.Awaitable[T]]
     ) -> t.Callable[P, t.Awaitable[T]]:
         ...
 
     @t.overload
     def inject(
-        self, *, lazy: t.Optional[bool] = None
+        self,
     ) -> t.Callable[
         [t.Callable[P, t.Union[T, t.Awaitable[T]]]],
         t.Callable[P, t.Union[T, t.Awaitable[T]]],
     ]:
         ...
 
     def inject(
         self,
         obj: t.Union[t.Callable[P, t.Union[T, t.Awaitable[T]]], None] = None,
-        lazy: t.Optional[bool] = None,
     ) -> t.Union[
         t.Callable[
             [t.Callable[P, t.Union[T, t.Awaitable[T]]]],
             t.Callable[P, t.Union[T, t.Awaitable[T]]],
         ],
         t.Callable[P, t.Union[T, t.Awaitable[T]]],
     ]:
-        lazy = self.lazy_inject if lazy is None else lazy
-
         def decorator(
             obj: t.Callable[P, t.Union[T, t.Awaitable[T]]]
         ) -> t.Callable[P, t.Union[T, t.Awaitable[T]]]:
-            injected_params = self._get_injectable_params(obj)
-
-            def _inject_kwargs(**kwargs: P.kwargs) -> t.Dict[str, t.Any]:
-                for name, annotation in injected_params.items():
-                    if lazy:
-                        kwargs[name] = make_lazy(self.get, annotation)
-                    else:
-                        kwargs[name] = self.get(annotation)
-                return kwargs
+            injected_params = self._get_injected_params(obj)
 
             if inspect.iscoroutinefunction(obj):
 
                 @wraps(obj)
                 async def awrapped(*args: P.args, **kwargs: P.kwargs) -> T:
-                    return t.cast(T, await obj(*args, **_inject_kwargs(**kwargs)))
+                    for name, annotation in injected_params.items():
+                        kwargs[name] = await self.aget(annotation)
+                    return t.cast(T, await obj(*args, **kwargs))
 
                 return awrapped
 
             @wraps(obj)
             def wrapped(*args: P.args, **kwargs: P.kwargs) -> T:
-                return t.cast(T, obj(*args, **_inject_kwargs(**kwargs)))
+                for name, annotation in injected_params.items():
+                    kwargs[name] = make_lazy(self.get, annotation)
+                return t.cast(T, obj(*args, **kwargs))
 
             return wrapped
 
         if obj is None:
             return decorator
         return decorator(obj)
 
@@ -664,15 +673,15 @@
                 t.Iterable[t.Union[types.ModuleType, str]], [packages]
             )
 
         for package in scan_packages:
             dependencies.extend(self._scan_package(package, tags=tags))
 
         for dependency in dependencies:
-            decorator = self.inject(lazy=dependency.lazy)(dependency.member)
+            decorator = self.inject()(dependency.member)
             setattr(dependency.module, dependency.member.__name__, decorator)
 
     def _scan_package(
         self,
         package: t.Union[types.ModuleType, str],
         *,
         tags: t.Optional[t.Iterable[str]] = None,
@@ -716,19 +725,16 @@
                 and not set(member_tags).intersection(tags)
                 or not member_tags
             ):
                 continue
 
             injected = getattr(member, "__pyxdi_inject__", None)
             if injected:
-                lazy = injected["lazy"]
                 dependencies.append(
-                    self._create_scanned_dependency(
-                        member=member, module=module, lazy=lazy
-                    )
+                    self._create_scanned_dependency(member=member, module=module)
                 )
                 continue
 
             # Get by pyxdi.dep mark
             if inspect.isclass(member):
                 signature = get_signature(member.__init__)
             else:
@@ -739,19 +745,19 @@
                         self._create_scanned_dependency(member=member, module=module)
                     )
                     continue
 
         return dependencies
 
     def _create_scanned_dependency(
-        self, member: t.Any, module: types.ModuleType, lazy: t.Optional[bool] = None
+        self, member: t.Any, module: types.ModuleType
     ) -> ScannedDependency:
         if hasattr(member, "__wrapped__"):
             member = member.__wrapped__
-        return ScannedDependency(member=member, module=module, lazy=lazy)
+        return ScannedDependency(member=member, module=module)
 
     # Inspection
 
     def _get_provider_annotation(self, obj: t.Callable[..., t.Any]) -> t.Any:
         annotation = get_signature(obj).return_annotation
 
         if annotation is inspect._empty:  # noqa
@@ -778,25 +784,37 @@
             return annotation
 
     def _get_provider_arguments(
         self, provider: Provider
     ) -> t.Tuple[t.List[t.Any], t.Dict[str, t.Any]]:
         args = []
         kwargs = {}
-        signature = get_signature(provider.obj)
-        for parameter in signature.parameters.values():
-            instance = self.get(parameter.annotation)
+        for parameter in get_signature(provider.obj).parameters.values():
+            instance = make_lazy(self.get, parameter.annotation)
+            if parameter.kind == parameter.POSITIONAL_ONLY:
+                args.append(instance)
+            else:
+                kwargs[parameter.name] = instance
+        return args, kwargs
+
+    async def _aget_provider_arguments(
+        self, provider: Provider
+    ) -> t.Tuple[t.List[t.Any], t.Dict[str, t.Any]]:
+        args = []
+        kwargs = {}
+        for parameter in get_signature(provider.obj).parameters.values():
+            instance = await self.aget(parameter.annotation)
             if parameter.kind == parameter.POSITIONAL_ONLY:
                 args.append(instance)
             else:
                 kwargs[parameter.name] = instance
         return args, kwargs
 
-    def _get_injectable_params(self, obj: t.Callable[..., t.Any]) -> t.Dict[str, t.Any]:
-        injectable_params = {}
+    def _get_injected_params(self, obj: t.Callable[..., t.Any]) -> t.Dict[str, t.Any]:
+        injected_params = {}
         for parameter in get_signature(obj).parameters.values():
             if not isinstance(parameter.default, DependencyMark):
                 continue
 
             annotation = parameter.annotation
             if annotation is inspect._empty:  # noqa
                 raise AnnotationError(
@@ -808,16 +826,16 @@
                 and annotation not in self._unresolved_providers
                 and annotation not in self._unresolved_dependencies
             ):
                 self._unresolved_dependencies[annotation] = UnresolvedDependency(
                     parameter_name=parameter.name, obj=obj
                 )
 
-            injectable_params[parameter.name] = annotation
-        return injectable_params
+            injected_params[parameter.name] = annotation
+        return injected_params
 
 
 class ScopedContext:
     def __init__(self, scope: Scope, root: PyxDI) -> None:
         self._scope = scope
         self._root = root
         self._instances: t.Dict[t.Type[t.Any], t.Any] = {}
@@ -831,90 +849,124 @@
             if provider.is_resource:
                 instance = self._root.create_resource(provider, stack=self._stack)
             else:
                 instance = self._root.create_instance(provider)
             self._instances[interface] = instance
         return t.cast(T, instance)
 
+    async def aget(self, interface: t.Type[T]) -> T:
+        instance = self._instances.get(interface)
+        if instance is None:
+            provider = self._root.get_provider(interface)
+            if provider.is_resource:
+                instance = await run_async(
+                    self._root.create_resource, provider, stack=self._stack
+                )
+            elif provider.is_async_resource:
+                instance = await self._root.acreate_resource(
+                    provider, stack=self._async_stack
+                )
+            else:
+                instance = await self._root.acreate_instance(provider)
+            self._instances[interface] = instance
+        return t.cast(T, instance)
+
     def set(self, interface: t.Type[t.Any], instance: t.Any) -> None:
         self._instances[interface] = instance
         self._root.register_provider(
             interface, lambda: interface, scope=self._scope, override=True
         )
 
     def has(self, interface: t.Type[t.Any]) -> bool:
         return interface in self._instances
 
     def delete(self, interface: t.Type[t.Any]) -> None:
         self._instances.pop(interface, None)
 
     def start(self) -> None:
-        for interface, provider in self._iter_providers():
-            if provider.is_resource:
-                instance = self._root.create_resource(provider, stack=self._stack)
-                self.set(interface, instance)
-            elif provider.is_async_resource:
-                raise ProviderError(
-                    f"The provider `{provider}` cannot be started in synchronous mode "
-                    "because it is an asynchronous provider. Please start the provider "
-                    "in asynchronous mode before using it."
-                )
+        """Scope Context start event."""
 
     def close(self) -> None:
         self._stack.close()
 
     async def astart(self) -> None:
-        for interface, provider in self._iter_providers():
-            if provider.is_resource:
-                instance = await run_async(
-                    self._root.create_resource, provider, stack=self._stack
-                )
-                self.set(interface, instance)
-            elif provider.is_async_resource:
-                instance = await self._root.acreate_resource(
-                    provider, stack=self._async_stack
-                )
-                self.set(interface, instance)
+        """Scope Context start asynchronous event."""
 
     async def aclose(self) -> None:
-        await self._async_stack.aclose()
         await run_async(self._stack.close)
+        await self._async_stack.aclose()
 
-    def __enter__(self) -> ScopedContext:
+    def __enter__(self) -> Self:
         self.start()
         return self
 
     def __exit__(
         self,
         exc_type: t.Type[BaseException] | None,
         exc_val: BaseException | None,
         exc_tb: types.TracebackType | None,
     ) -> None:
         self.close()
         return
 
-    async def __aenter__(self) -> ScopedContext:
+    async def __aenter__(self) -> Self:
         await self.astart()
         return self
 
     async def __aexit__(
         self,
         exc_type: t.Type[BaseException] | None,
         exc_val: BaseException | None,
         exc_tb: types.TracebackType | None,
     ) -> None:
         await self.aclose()
         return
 
+
+@t.final
+class SingletonContext(ScopedContext):
+    def __init__(self, root: PyxDI):
+        super().__init__("singleton", root)
+
+    def start(self) -> None:
+        for interface, provider in self._iter_providers():
+            if provider.is_resource:
+                self._instances[interface] = self._root.create_resource(
+                    provider, stack=self._stack
+                )
+            elif provider.is_async_resource:
+                raise ProviderError(
+                    f"The provider `{provider}` cannot be started in synchronous mode "
+                    "because it is an asynchronous provider. Please start the provider "
+                    "in asynchronous mode before using it."
+                )
+
+    async def astart(self) -> None:
+        for interface, provider in self._iter_providers():
+            if provider.is_resource:
+                self._instances[interface] = await run_async(
+                    self._root.create_resource, provider, stack=self._stack
+                )
+            elif provider.is_async_resource:
+                self._instances[interface] = await self._root.acreate_resource(
+                    provider, stack=self._async_stack
+                )
+
     def _iter_providers(self) -> t.Iterator[t.Tuple[t.Type[t.Any], Provider]]:
         for interface, provider in self._root.providers.items():
             if provider.scope == self._scope:
                 yield interface, provider
 
 
+@t.final
+class RequestContext(ScopedContext):
+    def __init__(self, root: PyxDI):
+        super().__init__("request", root)
+
+
 class Module:
     """
     Module base class.
     """
 
     def configure(self, di: PyxDI) -> None:
         ...
```

### Comparing `pyxdi-0.8.0/pyxdi/decorators.py` & `pyxdi-0.9.0/pyxdi/decorators.py`

 * *Files 3% similar despite different names*

```diff
@@ -64,42 +64,39 @@
 @t.overload
 def inject(obj: t.Callable[P, t.Awaitable[T]]) -> t.Callable[P, t.Awaitable[T]]:
     ...
 
 
 @t.overload
 def inject(
-    *, lazy: t.Optional[bool] = None, tags: t.Optional[t.Iterable[str]] = None
+    *, tags: t.Optional[t.Iterable[str]] = None
 ) -> t.Callable[
     [t.Callable[P, t.Union[T, t.Awaitable[T]]]],
     t.Callable[P, t.Union[T, t.Awaitable[T]]],
 ]:
     ...
 
 
 def inject(
     obj: t.Union[t.Callable[P, t.Union[T, t.Awaitable[T]]], None] = None,
-    lazy: t.Optional[bool] = None,
     tags: t.Optional[t.Iterable[str]] = None,
 ) -> t.Union[
     t.Callable[
         [t.Callable[P, t.Union[T, t.Awaitable[T]]]],
         t.Callable[P, t.Union[T, t.Awaitable[T]]],
     ],
     t.Callable[P, t.Union[T, t.Awaitable[T]]],
 ]:
     def decorator(
         obj: t.Callable[P, t.Union[T, t.Awaitable[T]]]
     ) -> t.Callable[P, t.Union[T, t.Awaitable[T]]]:
         setattr(
             obj,
             "__pyxdi_inject__",
-            {
-                "lazy": lazy,
-            },
+            True,
         )
         setattr(obj, "__pyxdi_tags__", tags)
         return obj
 
     if obj is None:
         return decorator
```

### Comparing `pyxdi-0.8.0/pyxdi/ext/fastapi.py` & `pyxdi-0.9.0/pyxdi/ext/fastapi.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,38 +42,34 @@
 
 
 def get_di(request: Request) -> pyxdi.PyxDI:
     return t.cast(pyxdi.PyxDI, request.app.state.di)
 
 
 class InjectParam(params.Depends):
-    def __init__(self, lazy: t.Optional[bool] = None) -> None:
+    def __init__(self) -> None:
         super().__init__(dependency=self._dependency, use_cache=True)
         self._interface: t.Any = None
-        self._lazy = lazy
 
     @property
     def interface(self) -> t.Any:
         if self._interface is None:
             raise TypeError("Interface is not set.")
         return self._interface
 
     @interface.setter
     def interface(self, val: t.Any) -> None:
         self._interface = val
 
     def _dependency(self, di: pyxdi.PyxDI = fastapi.Depends(get_di)) -> t.Any:
-        lazy = di.lazy_inject if self._lazy is None else self._lazy
-        if lazy:
-            return make_lazy(di.get, self.interface)
-        return di.get(self.interface)
+        return make_lazy(di.get, self.interface)
 
 
-def Inject(*, lazy: t.Optional[bool] = None) -> t.Any:  # noqa
-    return InjectParam(lazy=lazy)
+def Inject() -> t.Any:  # noqa
+    return InjectParam()
 
 
 def iter_dependencies(dependant: Dependant) -> t.Iterator[Dependant]:
     yield dependant
     if dependant.dependencies:
         for sub_dependant in dependant.dependencies:
             yield from iter_dependencies(sub_dependant)
```

### Comparing `pyxdi-0.8.0/pyxdi/ext/starlette/middleware.py` & `pyxdi-0.9.0/pyxdi/ext/starlette/middleware.py`

 * *Files identical despite different names*

### Comparing `pyxdi-0.8.0/pyxdi/utils.py` & `pyxdi-0.9.0/pyxdi/utils.py`

 * *Files identical despite different names*

### Comparing `pyxdi-0.8.0/PKG-INFO` & `pyxdi-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyxdi
-Version: 0.8.0
+Version: 0.9.0
 Summary: Dependency Injection library
 Home-page: https://github.com/antonrh/pyxdi
 License: MIT
 Keywords: dependency injection,dependencies,di,async,asyncio,application
 Author: Anton Ruhlov
 Author-email: antonruhlov@gmail.com
 Requires-Python: >=3.8,<3.12
```

