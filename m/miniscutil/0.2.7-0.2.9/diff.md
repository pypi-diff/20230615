# Comparing `tmp/miniscutil-0.2.7.tar.gz` & `tmp/miniscutil-0.2.9.tar.gz`

## Comparing `miniscutil-0.2.7.tar` & `miniscutil-0.2.9.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 miniscutil-0.2.7/miniscutil/__about__.py
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 miniscutil-0.2.7/miniscutil/__init__.py
--rw-r--r--   0        0        0     3148 2020-02-02 00:00:00.000000 miniscutil-0.2.7/miniscutil/adapt.py
--rw-r--r--   0        0        0     6171 2020-02-02 00:00:00.000000 miniscutil-0.2.7/miniscutil/asyncio_helpers.py
--rw-r--r--   0        0        0     8959 2020-02-02 00:00:00.000000 miniscutil-0.2.7/miniscutil/config.py
--rw-r--r--   0        0        0     1821 2020-02-02 00:00:00.000000 miniscutil-0.2.7/miniscutil/current.py
--rw-r--r--   0        0        0    11903 2020-02-02 00:00:00.000000 miniscutil-0.2.7/miniscutil/deep.py
--rw-r--r--   0        0        0     2154 2020-02-02 00:00:00.000000 miniscutil-0.2.7/miniscutil/deepeq.py
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 miniscutil-0.2.7/miniscutil/dictdiff.py
--rw-r--r--   0        0        0     3469 2020-02-02 00:00:00.000000 miniscutil-0.2.7/miniscutil/dispatch.py
--rw-r--r--   0        0        0     3422 2020-02-02 00:00:00.000000 miniscutil-0.2.7/miniscutil/misc.py
--rw-r--r--   0        0        0    13850 2020-02-02 00:00:00.000000 miniscutil-0.2.7/miniscutil/ofdict.py
--rw-r--r--   0        0        0     2860 2020-02-02 00:00:00.000000 miniscutil-0.2.7/miniscutil/sum.py
--rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 miniscutil-0.2.7/miniscutil/type_util.py
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 miniscutil-0.2.7/miniscutil/lsp/README.md
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 miniscutil-0.2.7/miniscutil/lsp/__init__.py
--rw-r--r--   0        0        0     7291 2020-02-02 00:00:00.000000 miniscutil-0.2.7/miniscutil/lsp/document.py
--rw-r--r--   0        0        0     5050 2020-02-02 00:00:00.000000 miniscutil-0.2.7/miniscutil/lsp/server.py
--rw-r--r--   0        0        0    12815 2020-02-02 00:00:00.000000 miniscutil-0.2.7/miniscutil/lsp/types.py
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 miniscutil-0.2.7/miniscutil/rpc/__init__.py
--rw-r--r--   0        0        0     5176 2020-02-02 00:00:00.000000 miniscutil-0.2.7/miniscutil/rpc/extrarpc.py
--rw-r--r--   0        0        0     2711 2020-02-02 00:00:00.000000 miniscutil-0.2.7/miniscutil/rpc/io_transport.py
--rw-r--r--   0        0        0    19268 2020-02-02 00:00:00.000000 miniscutil-0.2.7/miniscutil/rpc/jsonrpc.py
--rw-r--r--   0        0        0     1483 2020-02-02 00:00:00.000000 miniscutil-0.2.7/miniscutil/rpc/starlette_ws_transport.py
--rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 miniscutil-0.2.7/miniscutil/rpc/transport.py
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 miniscutil-0.2.7/miniscutil/rpc/websocket_transport.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 miniscutil-0.2.7/tests/__init__.py
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 miniscutil-0.2.7/tests/test_classdispatch.py
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 miniscutil-0.2.7/tests/test_config.py
--rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 miniscutil-0.2.7/tests/test_current.py
--rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 miniscutil-0.2.7/tests/test_deepeq.py
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 miniscutil-0.2.7/tests/test_humansize.py
--rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 miniscutil-0.2.7/tests/test_lsp.py
--rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 miniscutil-0.2.7/tests/test_ofdict.py
--rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 miniscutil-0.2.7/tests/test_typing.py
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 miniscutil-0.2.7/tests/test_util.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 miniscutil-0.2.7/tests/snapshots/test_humansize/test_human_size/bytes
--rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 miniscutil-0.2.7/.gitignore
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 miniscutil-0.2.7/LICENSE.txt
--rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 miniscutil-0.2.7/README.md
--rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 miniscutil-0.2.7/pyproject.toml
--rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 miniscutil-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 miniscutil-0.2.9/miniscutil/__about__.py
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 miniscutil-0.2.9/miniscutil/__init__.py
+-rw-r--r--   0        0        0     5091 2020-02-02 00:00:00.000000 miniscutil-0.2.9/miniscutil/adapt.py
+-rw-r--r--   0        0        0     6171 2020-02-02 00:00:00.000000 miniscutil-0.2.9/miniscutil/asyncio_helpers.py
+-rw-r--r--   0        0        0     9335 2020-02-02 00:00:00.000000 miniscutil-0.2.9/miniscutil/config.py
+-rw-r--r--   0        0        0     1821 2020-02-02 00:00:00.000000 miniscutil-0.2.9/miniscutil/current.py
+-rw-r--r--   0        0        0    11903 2020-02-02 00:00:00.000000 miniscutil-0.2.9/miniscutil/deep.py
+-rw-r--r--   0        0        0     2154 2020-02-02 00:00:00.000000 miniscutil-0.2.9/miniscutil/deepeq.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 miniscutil-0.2.9/miniscutil/dictdiff.py
+-rw-r--r--   0        0        0     3469 2020-02-02 00:00:00.000000 miniscutil-0.2.9/miniscutil/dispatch.py
+-rw-r--r--   0        0        0     4218 2020-02-02 00:00:00.000000 miniscutil-0.2.9/miniscutil/misc.py
+-rw-r--r--   0        0        0    13850 2020-02-02 00:00:00.000000 miniscutil-0.2.9/miniscutil/ofdict.py
+-rw-r--r--   0        0        0     2860 2020-02-02 00:00:00.000000 miniscutil-0.2.9/miniscutil/sum.py
+-rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 miniscutil-0.2.9/miniscutil/type_util.py
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 miniscutil-0.2.9/miniscutil/lsp/README.md
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 miniscutil-0.2.9/miniscutil/lsp/__init__.py
+-rw-r--r--   0        0        0     8301 2020-02-02 00:00:00.000000 miniscutil-0.2.9/miniscutil/lsp/document.py
+-rw-r--r--   0        0        0     5050 2020-02-02 00:00:00.000000 miniscutil-0.2.9/miniscutil/lsp/server.py
+-rw-r--r--   0        0        0    11978 2020-02-02 00:00:00.000000 miniscutil-0.2.9/miniscutil/lsp/types.py
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 miniscutil-0.2.9/miniscutil/rpc/__init__.py
+-rw-r--r--   0        0        0     5176 2020-02-02 00:00:00.000000 miniscutil-0.2.9/miniscutil/rpc/extrarpc.py
+-rw-r--r--   0        0        0     2711 2020-02-02 00:00:00.000000 miniscutil-0.2.9/miniscutil/rpc/io_transport.py
+-rw-r--r--   0        0        0    19516 2020-02-02 00:00:00.000000 miniscutil-0.2.9/miniscutil/rpc/jsonrpc.py
+-rw-r--r--   0        0        0     1483 2020-02-02 00:00:00.000000 miniscutil-0.2.9/miniscutil/rpc/starlette_ws_transport.py
+-rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 miniscutil-0.2.9/miniscutil/rpc/transport.py
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 miniscutil-0.2.9/miniscutil/rpc/websocket_transport.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 miniscutil-0.2.9/tests/__init__.py
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 miniscutil-0.2.9/tests/test_classdispatch.py
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 miniscutil-0.2.9/tests/test_config.py
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 miniscutil-0.2.9/tests/test_current.py
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 miniscutil-0.2.9/tests/test_deepeq.py
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 miniscutil-0.2.9/tests/test_humansize.py
+-rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 miniscutil-0.2.9/tests/test_lsp.py
+-rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 miniscutil-0.2.9/tests/test_ofdict.py
+-rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 miniscutil-0.2.9/tests/test_typing.py
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 miniscutil-0.2.9/tests/test_util.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 miniscutil-0.2.9/tests/snapshots/test_humansize/test_human_size/bytes
+-rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 miniscutil-0.2.9/.gitignore
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 miniscutil-0.2.9/LICENSE.txt
+-rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 miniscutil-0.2.9/README.md
+-rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 miniscutil-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 miniscutil-0.2.9/PKG-INFO
```

### Comparing `miniscutil-0.2.7/miniscutil/__init__.py` & `miniscutil-0.2.9/miniscutil/__init__.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.7/miniscutil/adapt.py` & `miniscutil-0.2.9/miniscutil/dispatch.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,124 +1,122 @@
-from collections import defaultdict
-from contextvars import ContextVar
-import datetime
-from enum import Enum
-from functools import singledispatch
-from typing import Any, Callable, NewType, Type, get_origin
-import uuid
-
-from .dispatch import Dispatcher, classdispatch
-from .type_util import as_newtype, as_optional
-
-""" Implementation of PEP-246 https://peps.python.org/pep-0246/#specification
-
-I'm not sure it quite captures the spirit of the PEP because adapt doesn't necessarily _wrap_ the input.
-"""
-
-
-class AdaptationError(TypeError):
-    pass
-
-
-class LiskovViolation(AdaptationError):
-    pass
-
-
-adapters: dict[Type, Dispatcher[Callable[[Any], Any]]] = defaultdict(Dispatcher)
-
-
-def register_adapter(T: Type, protocol: Type):
-    def core(f: Callable[[Any], Any]):
-        dispatcher = adapters[protocol]
-        dispatcher.register(T, f)
-        return f
-
-    return core
-
-
-def adapt(obj, protocol):
-    """Turn it into a compatible type."""
-    t = type(obj)
-    if t is protocol:
-        return obj
-    if protocol is None:
-        raise ValueError("No protocol specified")
-    try:
-        conform = getattr(obj, "__conform__", None)
-        if conform is not None:
-            r = conform(protocol)
-            if r is not NotImplemented:
-                return r
-        adapt = getattr(protocol, "__adapt__", None)
-        if adapt is not None:
-            r = adapt(obj)
-            if r is not NotImplemented:
-                return r
-    except LiskovViolation:
-        pass
-    else:
-        if isinstance(obj, protocol):
-            return obj
-    f = adapters[protocol].dispatch(t)
-    if f is not None:
-        r = f(obj)
-        if r is not NotImplemented:
-            return r
-    raise AdaptationError(f"No adapter found for {t} and {protocol}")
-
-
-@classdispatch
-def restore(X, x):
-    """Inverse of adapt.
-
-    Args:
-        X(type): The type to restore x to.
-        x(object): The object to restore.
-    """
-    # [todo] abstract this out into an adapter pattern. adapt(x, protocol = X)
+from abc import get_cache_token
+from typing import (
+    Any,
+    Callable,
+    Dict,
+    Generic,
+    Optional,
+    Type,
+    TypeVar,
+    Union,
+    get_origin,
+    NewType,
+)
+from functools import singledispatch, update_wrapper
+from functools import _find_impl  # type: ignore
+from weakref import WeakKeyDictionary
+
+F = TypeVar("F")
+
+
+class Dispatcher(Generic[F]):
+    """Reimplementation of the dispatching logic for functools.singledispatch."""
+
+    registry: Dict[Type, F]
+    cache: WeakKeyDictionary
+    cache_token: Optional[object]
+
+    def __init__(self):
+        self.registry = {}
+        self.cache = WeakKeyDictionary()
+        self.cache_token = None
+
+    def register(self, cls: Type, f: Optional[F] = None):
+        # [todo] method override
+        if f is not None:
+            self.registry[cls] = f
+        else:
+
+            def x(f):
+                self.registry[cls] = f
+                return f
 
-    Y = as_optional(X)
-    if Y is not None:
-        if x is None:
             return x
-        else:
-            return restore(Y, x)
 
-    S = as_newtype(X)
-    if S is not None:
-        r = restore(S, x)
-        return X(r)
-
-    if get_origin(X) is None and isinstance(x, X):
-        return x
-    adapt = getattr(X, "__adapt__", None)
-    if adapt is not None:
-        r = adapt(x)
-        if r is not NotImplemented:
-            return r
-
-    if issubclass(X, Enum):
-        return X(x)
-    if X is bool:
-        return bool(x)
-    raise NotImplementedError(f"Unsupported target type {X}")
-
-
-# [todo] use pydantic
-@restore.register(datetime.datetime)
-def _restore_datetime(T, d):
-    if isinstance(d, datetime.datetime):
-        return d
-    elif isinstance(d, str):
-        return datetime.datetime.fromisoformat(d)
-    else:
-        raise TypeError(f"Unsupported datetime type {type(d)}")
-
-
-@restore.register(uuid.UUID)
-def _restore_uuid(T, b):
-    if isinstance(b, uuid.UUID):
-        return b
-    elif isinstance(b, bytes):
-        return uuid.UUID(bytes=b)
-    else:
-        raise TypeError(f"Unsupported uuid type {type(b)}")
+    def update(self, cls: Type, modifier: Callable[[Optional[F]], F]) -> None:
+        r = self.get(cls)
+        r = modifier(r)
+        self.register(cls, r)
+        self.cache.clear()
+
+    def __contains__(self, cls):
+        return self.get(cls) is not None
+
+    def __getitem__(self, cls):
+        return self.get(cls)
+
+    def dispatch(self, cls) -> Optional[F]:
+        return self.get(cls)
+
+    def get(self, cls) -> Union[F, None]:
+        """generic_func.dispatch(cls) -> <function implementation>
+
+        Runs the dispatch algorithm to return the best available implementation
+        for the given *cls* registered on *generic_func*.
+
+        """
+        # [todo] also dispatch on generic aliases.
+        if self.cache_token is not None:
+            current_token = get_cache_token()
+            if self.cache_token != current_token:
+                self.cache.clear()
+                self.cache_token = current_token
+        try:
+            impl = self.cache[cls]
+        except KeyError:
+            try:
+                impl = self.registry[cls]
+            except KeyError:
+                try:
+                    impl = _find_impl(cls, self.registry)
+                except KeyError:
+                    impl = self.registry[Any]
+            self.cache[cls] = impl
+        return impl
+
+
+def classdispatch(func):
+    """Dynamic dispatch on a class.
+
+    Similar to ``functools.singledispatch``, except treats the first argument as a class to be dispatched on.
+    """
+    # [todo] switch to using dispatcher
+    # [todo] add support for register(Optional) and register(Union) and register(list[int]).
+    funcname = getattr(func, "__name__", "class dispatch function")
+    sdfunc = singledispatch(func)
+
+    def dispatch(cls):
+        g = sdfunc.registry.get(cls)
+        if g is not None:
+            return g
+        orig = get_origin(cls)
+        if orig is not None:
+            g = sdfunc.registry.get(orig)
+            if g is not None:
+                return g
+            cls = orig
+        try:
+            return sdfunc.dispatch(cls)
+        except Exception:
+            return sdfunc.dispatch(object)
+
+    def wrapper(*args, **kwargs):
+        if not args:
+            raise TypeError(f"{funcname} requires at leat one positional argument.")
+        cls = args[0]
+        return dispatch(cls)(*args, **kwargs)
+
+    for n in ["register", "registry"]:
+        setattr(wrapper, n, getattr(sdfunc, n))
+    setattr(wrapper, "dispatch", dispatch)
+    update_wrapper(wrapper, func)
+    return wrapper
```

### Comparing `miniscutil-0.2.7/miniscutil/asyncio_helpers.py` & `miniscutil-0.2.9/miniscutil/asyncio_helpers.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.7/miniscutil/config.py` & `miniscutil-0.2.9/miniscutil/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,23 @@
+import functools
 import json
 import logging
 import sys
 from typing import Any, Optional, Union
 from pathlib import Path
 import os
 import subprocess
 from subprocess import PIPE, CalledProcessError
 from miniscutil.type_util import is_subtype
 
 from pydantic import BaseSettings, Field, SecretStr
 
 """ Helpers for working with projects, config files etc. """
 
-logger = logging.getLogger("miniscutil.config")
+logger = logging.getLogger(__name__)
 
 
 def get_git_root(cwd: Optional[Path] = None) -> Optional[Path]:
     """
     Gets the git root for the current working directory.
 
     source: https://github.com/maxnoe/python-gitpath/blob/86973f112b976a87e2ffa734fa2e43cc76dfe90d/gitpath/__init__.py
@@ -71,14 +72,15 @@
         return Path(git_root)
     logger.debug(
         f"{cwd} is not in a git repository and no pyproject.toml could be found."
     )
     return None
 
 
+@functools.cache
 def get_app_config_dir(app_name: str) -> Path:
     """Get the path to the application directory.
 
     The implementation is based on https://click.palletsprojects.com/en/8.1.x/api/#click.get_app_dir
     """
     if sys.platform == "win32":
         p = Path(os.environ.get("APPDATA", "~/.config"))
@@ -86,33 +88,42 @@
         p = Path(os.environ.get("XDG_CONFIG_HOME", "~/.config"))
     elif sys.platform == "darwin":  # macos
         # [todo] "~/Library/Application Support" or "~/Library/Preferences"?
         p = Path("~") / "Library" / "Application Support"
     else:
         p = Path(os.environ.get("XDG_CONFIG_HOME", "~/.config"))
     p = p.expanduser().resolve() / app_name
-    p.mkdir(exist_ok=True)
+    # [todo] handle permissions errors
+    try:
+        p.mkdir(exist_ok=True)
+    except Exception:
+        logger.exception(f"Couldn't create app config dir {p}")
     return p
 
 
+@functools.cache
 def get_app_cache_dir(app_name: str) -> Path:
     """Returns the path that ths OS wants you to use to place application-specific caching files."""
     if sys.platform == "win32":
         p = Path(os.environ.get("LOCALAPPDATA", "~/.cache"))
     elif sys.platform == "linux":
         p = Path(os.environ.get("XDG_CACHE_HOME", "~/.cache"))
     elif sys.platform == "darwin":  # macos
         p = Path("~/Library/Caches")
     else:
         logger.warning(
             f"Unrecognised platform: {sys.platform}, user cache is defaulting to a tmpdir."
         )
         p = Path(tempfile.gettempdir())
     p = p.expanduser().resolve() / app_name
-    p.mkdir(exist_ok=True)
+    # [todo] handle permissions errors
+    try:
+        p.mkdir(exist_ok=True)
+    except Exception:
+        logger.exception(f"Couldn't create app cache dir {p}")
     return p
 
 
 def persist_config(p: Path, key: Union[str, tuple[str, ...]], value: Any):
     if p.exists():
         root = json.loads(p.read_text())
     else:
@@ -218,14 +229,15 @@
         field = fields[key]
         assert is_subtype(SecretStr, field.annotation)
         extra = field.field_info.extra
         assert extra.get(
             "is_secret", False
         ), "please add the 'is_secret=True' kwarg to Field constructor"
         cfg = getattr(self, "__config__")
+        # [todo] user might not have permissions to set file
         secrets_file = getattr(self, "secrets_file")
         secret_postfix = getattr(cfg, "secret_postfix", None)
         if secret_postfix is None:
             secret_postfix = "default"
         elif secret_postfix in fields:
             secret_postfix = getattr(self, secret_postfix)
             assert isinstance(secret_postfix, str)
```

### Comparing `miniscutil-0.2.7/miniscutil/current.py` & `miniscutil-0.2.9/miniscutil/current.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.7/miniscutil/deep.py` & `miniscutil-0.2.9/miniscutil/deep.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.7/miniscutil/deepeq.py` & `miniscutil-0.2.9/miniscutil/deepeq.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.7/miniscutil/misc.py` & `miniscutil-0.2.9/miniscutil/misc.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 from dataclasses import dataclass, is_dataclass, Field, fields
 from itertools import filterfalse, tee
 from datetime import datetime, timezone
+import contextvars
 from subprocess import check_output, CalledProcessError
+import contextlib
+from sys import _xoptions
+import itertools
 from typing import (
     IO,
     Callable,
     Dict,
     Generic,
     Iterable,
     Iterator,
@@ -14,14 +18,15 @@
     TypeVar,
 )
 from functools import partial
 import math
 import functools
 import contextvars
 import contextlib
+from typing_extensions import deprecated
 
 
 X = TypeVar("X")
 Y = TypeVar("Y")
 Z = TypeVar("Z")
 
 
@@ -105,14 +110,48 @@
     query.update(params)
     parts = parts._replace(query=urlencode(query))
     result = urlunparse(parts)
     assert isinstance(result, str)
     return result
 
 
+@contextlib.contextmanager
+def onectx(var: contextvars.ContextVar[X], mk: Callable[[], X]):
+    """If the context variable is not set, set it to the result of calling mk()."""
+    o = var.get(None)
+    if o is None:
+        x = mk()
+        token = var.set(x)
+        try:
+            yield x
+        finally:
+            var.reset(token)
+    else:
+        yield o
+
+
+def intercalate(
+    items: Iterable[X],
+    sep: X,
+):
+    xs = iter(items)
+    yield next(xs)
+    for x in xs:
+        yield sep
+        yield x
+
+
+def interlace(items: Iterable[X], seps: Iterable[X]):
+    xs = iter(items)
+    yield next(xs)
+    for s, x in zip(seps, xs):
+        yield s
+        yield x
+
+
 T = TypeVar("T")
 
 
 @contextlib.contextmanager
 def set_ctx(v: contextvars.ContextVar[T], t: T):
     x = v.set(t)
     try:
```

### Comparing `miniscutil-0.2.7/miniscutil/ofdict.py` & `miniscutil-0.2.9/miniscutil/ofdict.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.7/miniscutil/sum.py` & `miniscutil-0.2.9/miniscutil/sum.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.7/miniscutil/type_util.py` & `miniscutil-0.2.9/miniscutil/type_util.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import inspect
 from typing import (
     Any,
     NewType,
     get_origin,
     get_args,
     Type,
+    Literal,
     Optional,
     Union,
 )
 
 
 def is_optional(T: Type) -> bool:
     """Returns true if ``T == Union[NoneType, _] == Optional[_]``."""
@@ -31,14 +32,20 @@
             if len(ts) == 1:
                 return ts[0]
             else:
                 return Union[ts]  # type: ignore
     return None
 
 
+def as_literal(T: Type) -> Optional[tuple[str, ...]]:
+    if get_origin(T) is Literal:
+        return get_args(T)
+    return None
+
+
 def as_list(T: Type) -> Optional[Type]:
     """If `T = List[X]`, return `X`, otherwise return None."""
     if T == list:
         return Any
     o = get_origin(T)
     if o is None:
         return None
```

### Comparing `miniscutil-0.2.7/miniscutil/lsp/document.py` & `miniscutil-0.2.9/miniscutil/lsp/document.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import bisect
 import contextlib
 from contextvars import ContextVar
 from dataclasses import dataclass, replace
 from enum import Enum
 import functools
 import itertools
+from pathlib import Path
 from typing import Iterable, Optional, Union
+from urllib.parse import urlparse
 
 try:
     from typing import TypeAlias, TypeVar
 except:
     from typing_extensions import TypeAlias, TypeVar
 from miniscutil.misc import set_ctx
 
@@ -230,15 +232,46 @@
             self.position_to_offset(range.start),
             self.position_to_offset(range.end),
         )
 
     # [todo] enter, exit does setdoc
 
 
+def path_of_uri(uri: DocumentUri):
+    x = urlparse(uri)
+    assert x.netloc == ""
+    assert x.scheme == "file"
+    return Path(x.path)
+
+
+@dataclass
+class TextDocumentIdentifier:
+    """
+    References:
+    - https://microsoft.github.io/language-server-protocol/specifications/lsp/3.17/specification/#textDocumentIdentifier
+
+    """
+
+    uri: str
+    version: Optional[int]
+    """
+    The version number of a document will increase after each change, including undo/redo. The number doesn't need to be consecutive.
+    The server can send `null` to indicate that the version is known and the content on disk is the master (as specified with document content ownership).
+    """
+
+    def __fspath__(self):
+        # https://docs.python.org/3/library/os.html#os.PathLike.__fspath__
+        return str(path_of_uri(self.uri))
+
+
 @dataclass
 class TextDocumentItem(DocumentContext):
     uri: DocumentUri
     languageId: str
     version: int
 
     def __fspath__(self):
-        return self.uri
+        return str(path_of_uri(self.uri))
+
+    @property
+    def id(self):
+        return TextDocumentIdentifier(uri=self.uri, version=self.version)
```

### Comparing `miniscutil-0.2.7/miniscutil/lsp/server.py` & `miniscutil-0.2.9/miniscutil/lsp/server.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.7/miniscutil/lsp/types.py` & `miniscutil-0.2.9/miniscutil/lsp/types.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from dataclasses import dataclass, field, replace
 from enum import Enum
 from pathlib import Path
 from typing import Any, Generic, Literal, Optional, Union
 from typing import Optional as opt
 import urllib.parse
 from .document import *
+
 try:
     from typing import TypeAlias, TypeVar
 except:
     from typing_extensions import TypeAlias, TypeVar
 T = TypeVar("T")
 
 DocumentUri = str
@@ -23,41 +24,14 @@
 
 https://microsoft.github.io/language-server-protocol/specifications/lsp/3.17/specification
 """
 
 EOL = ["\n", "\r\n", "\r"]
 
 
-def path_of_uri(uri: DocumentUri):
-    x = urllib.parse.urlparse(uri)
-    assert x.netloc == ""
-    assert x.scheme == "file"
-    return Path(x.path)
-
-
-@dataclass
-class TextDocumentIdentifier:
-    """
-    References:
-    - https://microsoft.github.io/language-server-protocol/specifications/lsp/3.17/specification/#textDocumentIdentifier
-
-    """
-
-    uri: str
-    version: Optional[int]
-    """
-    The version number of a document will increase after each change, including undo/redo. The number doesn't need to be consecutive.
-    The server can send `null` to indicate that the version is known and the content on disk is the master (as specified with document content ownership).
-    """
-
-    def __fspath__(self):
-        # https://docs.python.org/3/library/os.html#os.PathLike.__fspath__
-        return str(path_of_uri(self.uri))
-
-
 @dataclass
 class TextDocumentParams:
     textDocument: TextDocumentIdentifier
 
     def __fspath__(self):
         return self.textDocument.__fspath__()
 
@@ -463,17 +437,19 @@
 
 
 @dataclass
 class ApplyWorkspaceEditParams:
     edit: WorkspaceEdit
     label: Optional[str] = field(default=None)
 
+
 @dataclass
 class ApplyWorkspaceEditResponse:
-    applied : bool
+    applied: bool
+
 
 TraceValue: TypeAlias = Literal["off", "messages", "verbose"]
 
 
 @dataclass
 class SetTraceParams:
     value: TraceValue
```

### Comparing `miniscutil-0.2.7/miniscutil/rpc/extrarpc.py` & `miniscutil-0.2.9/miniscutil/rpc/extrarpc.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.7/miniscutil/rpc/io_transport.py` & `miniscutil-0.2.9/miniscutil/rpc/io_transport.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.7/miniscutil/rpc/jsonrpc.py` & `miniscutil-0.2.9/miniscutil/rpc/jsonrpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -409,19 +409,25 @@
                     logger.exception("invalid json")
                     response = Response(
                         error=ResponseError(message=str(e), code=ErrorCode.parse_error)
                     )
                     await self.send(response)
                     continue
                 except ExitNotification as e:
-                    logger.info(f"{self.name} received exit notification, terminating")
+                    logger.info(f"{self.name} received exit notification")
                     return
                 except KeyboardInterrupt as e:
-                    logger.exception(f"recieved kb interrupt, terminating")
+                    logger.info(f"recieved kb interrupt")
                     return
+                except TransportClosedError as e:
+                    logger.error(f"transport closed in error: {e}")
+                    raise e
+                except Exception as e:
+                    logger.exception(f"unhandled exception: {e}")
+                    raise e
         finally:
             logger.info(f"exiting serve_forever loop")
             (_, e, _) = sys.exc_info()  # sys.exception() is 3.11 only
             if e is None:
                 e = ConnectionError(f"{self} shutdown")
             for fut in self.my_requests.values():
                 fut.set_exception(e)
```

### Comparing `miniscutil-0.2.7/miniscutil/rpc/starlette_ws_transport.py` & `miniscutil-0.2.9/miniscutil/rpc/starlette_ws_transport.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.7/miniscutil/rpc/transport.py` & `miniscutil-0.2.9/miniscutil/rpc/transport.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.7/miniscutil/rpc/websocket_transport.py` & `miniscutil-0.2.9/miniscutil/rpc/websocket_transport.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.7/tests/test_classdispatch.py` & `miniscutil-0.2.9/tests/test_classdispatch.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.7/tests/test_config.py` & `miniscutil-0.2.9/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.7/tests/test_current.py` & `miniscutil-0.2.9/tests/test_current.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.7/tests/test_deepeq.py` & `miniscutil-0.2.9/tests/test_deepeq.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.7/tests/test_lsp.py` & `miniscutil-0.2.9/tests/test_lsp.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.7/tests/test_ofdict.py` & `miniscutil-0.2.9/tests/test_ofdict.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.7/tests/test_typing.py` & `miniscutil-0.2.9/tests/test_typing.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.7/.gitignore` & `miniscutil-0.2.9/.gitignore`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.7/LICENSE.txt` & `miniscutil-0.2.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.7/README.md` & `miniscutil-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.7/pyproject.toml` & `miniscutil-0.2.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `miniscutil-0.2.7/PKG-INFO` & `miniscutil-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miniscutil
-Version: 0.2.7
+Version: 0.2.9
 Project-URL: Documentation, https://github.com/EdAyers/sss/miniscutil#readme
 Project-URL: Issues, https://github.com/EdAyers/sss/miniscutil/issues
 Project-URL: Source, https://github.com/EdAyers/sss/miniscutil
 Author-email: "E.W.Ayers" <contact@edayers.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
```

