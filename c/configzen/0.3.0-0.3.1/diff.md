# Comparing `tmp/configzen-0.3.0.tar.gz` & `tmp/configzen-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "configzen-0.3.0.tar", max compression
+gzip compressed data, was "configzen-0.3.1.tar", max compression
```

## Comparing `configzen-0.3.0.tar` & `configzen-0.3.1.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0      765 2023-06-08 07:24:52.012706 configzen-0.3.0/configzen/__init__.py
--rw-r--r--   0        0        0      902 2023-06-08 05:49:03.151216 configzen-0.3.0/configzen/__main__.py
--rw-r--r--   0        0        0    71657 2023-06-08 08:08:27.075017 configzen-0.3.0/configzen/config.py
--rw-r--r--   0        0        0     3495 2023-06-08 07:28:22.234288 configzen-0.3.0/configzen/errors.py
--rw-r--r--   0        0        0    25376 2023-06-08 07:24:53.384157 configzen-0.3.0/configzen/processor.py
--rw-r--r--   0        0        0        0 2023-05-14 03:53:55.304547 configzen-0.3.0/configzen/py.typed
--rw-r--r--   0        0        0     1047 2023-06-05 06:53:17.656362 configzen-0.3.0/configzen/typedefs.py
--rw-r--r--   0        0        0     1083 2023-04-05 18:05:38.524615 configzen-0.3.0/LICENSE
--rw-r--r--   0        0        0     1155 2023-06-08 08:09:32.832701 configzen-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     7155 2023-05-30 19:13:13.036046 configzen-0.3.0/README.md
--rw-r--r--   0        0        0     8127 1970-01-01 00:00:00.000000 configzen-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      919 2023-06-12 23:31:19.528601 configzen-0.3.1/configzen/__init__.py
+-rw-r--r--   0        0        0      935 2023-06-12 23:31:06.893355 configzen-0.3.1/configzen/__main__.py
+-rw-r--r--   0        0        0    71486 2023-06-14 12:12:18.386430 configzen-0.3.1/configzen/config.py
+-rw-r--r--   0        0        0     3226 2023-06-12 23:30:14.533429 configzen-0.3.1/configzen/decorators.py
+-rw-r--r--   0        0        0     3605 2023-06-12 23:30:35.066345 configzen-0.3.1/configzen/errors.py
+-rw-r--r--   0        0        0    26020 2023-06-13 02:08:11.775701 configzen-0.3.1/configzen/processor.py
+-rw-r--r--   0        0        0        0 2023-05-14 03:53:55.304547 configzen-0.3.1/configzen/py.typed
+-rw-r--r--   0        0        0     1080 2023-06-14 12:11:23.623137 configzen-0.3.1/configzen/typedefs.py
+-rw-r--r--   0        0        0     1083 2023-06-12 23:31:22.580649 configzen-0.3.1/LICENSE
+-rw-r--r--   0        0        0     1235 2023-06-15 00:21:30.968194 configzen-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     7371 2023-06-13 02:20:30.758785 configzen-0.3.1/README.md
+-rw-r--r--   0        0        0     8001 1970-01-01 00:00:00.000000 configzen-0.3.1/PKG-INFO
```

### Comparing `configzen-0.3.0/configzen/__main__.py` & `configzen-0.3.1/configzen/__main__.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-import argparse
-
-from configzen import ConfigMeta, ConfigModel
-from configzen.config import get_context
-
-
-class Store(ConfigModel):
-    class Config(ConfigMeta):
-        extra = ConfigMeta.Extra.allow
-
-
-if __name__ == "__main__":
-    p = argparse.ArgumentParser()
-    p.add_argument("--source", help="file to load from")
-    p.add_argument("dest", help="file to save into")
-    p.add_argument("--async", dest="use_async", action="store_true", help="use async")
-
-    opt = p.parse_args()
-
-    if opt.use_async:
-        import asyncio
-
-        store = asyncio.run(Store.load_async(opt.source))
-        print(store)
-        context = get_context(store)
-        context.agent.resource = opt.dest
-        asyncio.run(store.save_async())
-    else:
-        store = Store.load(opt.source)
-        print(store)
-        context = get_context(store)
-        context.agent.resource = opt.dest
-        store.save()
+import argparse
+
+from configzen import ConfigMeta, ConfigModel
+from configzen.config import get_context
+
+
+class Store(ConfigModel):
+    class Config(ConfigMeta):
+        extra = ConfigMeta.Extra.allow
+
+
+if __name__ == "__main__":
+    p = argparse.ArgumentParser()
+    p.add_argument("--source", help="file to load from")
+    p.add_argument("dest", help="file to save into")
+    p.add_argument("--async", dest="use_async", action="store_true", help="use async")
+
+    opt = p.parse_args()
+
+    if opt.use_async:
+        import asyncio
+
+        store = asyncio.run(Store.load_async(opt.source))
+        print(store)
+        context = get_context(store)
+        context.agent.resource = opt.dest
+        asyncio.run(store.save_async())
+    else:
+        store = Store.load(opt.source)
+        print(store)
+        context = get_context(store)
+        context.agent.resource = opt.dest
+        store.save()
```

### Comparing `configzen-0.3.0/configzen/config.py` & `configzen-0.3.1/configzen/config.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,2436 +1,2325 @@
-"""
-The core module of the _configzen_ library.
-
-This module provides an API to manage configuration files and resources
-in a consistent way. It also provides tools to load and save configuration
-files in various formats and within a number of advanced methods.
-
-.. code-block:: python
-
-    from configzen import ConfigModel, ConfigResource, ConfigField, ConfigMeta
-
-    class DatabaseConfig(ConfigModel):
-        host: str
-        port: int
-        user: str
-        password: str = ConfigField(exclude=True)
-
-        class Config(ConfigMeta):
-            resource = "examples/database.json"
-
-    db_config = DatabaseConfig.load()
-    db_config.host = "newhost"
-    db_config.port = 5432
-
-    db_config.save()
-
-    db_config = DatabaseConfig.load()
-    print(db_config.host)
-    print(db_config.port)
-
-    # Output:
-    # newhost
-    # 5432
-
-    db_config.host = "otherhost"
-    db_config.port = 5433
-
-    db_config.at("host").save()
-
-    print(db_config.host)
-    print(db_config.port)
-
-    # Output:
-    # otherhost
-    # 5432  # <- not 5433, because we saved only host
-
-    db_config.host = "anotherhost"
-    db_config.at("port").reload()
-
-    print(db_config.host)
-    print(db_config.port)
-
-    # Output:
-    # otherhost  # <- not anotherhost, because we reloaded only port
-    # 5432
-"""
-
-from __future__ import annotations
-
-import abc
-import asyncio
-import collections.abc
-import contextvars
-import copy
-import dataclasses
-import functools
-import io
-import os
-import pathlib
-import urllib.parse
-import urllib.request
-from typing import (
-    Any,
-    ClassVar,
-    Generic,
-    Literal,
-    Optional,
-    cast,
-    no_type_check,
-    overload,
-)
-
-import anyconfig
-import pydantic
-from anyconfig.utils import filter_options, is_dict_like, is_list_like
-from pydantic.fields import (  # type: ignore[attr-defined]
-    ModelField,
-    make_generic_validator,
-)
-from pydantic.json import ENCODERS_BY_TYPE
-from pydantic.main import BaseModel, ModelMetaclass
-from pydantic.utils import ROOT_KEY
-
-from configzen.errors import (
-    ConfigAccessError,
-    InternalSyntaxError,
-    ResourceLookupError,
-    UnspecifiedParserError,
-    UnavailableParserError,
-    formatted_syntax_error,
-)
-from configzen.processor import EXPORT, DirectiveContext, Processor
-from configzen.typedefs import (
-    AsyncConfigIO,
-    ConfigIO,
-    ConfigModelT,
-    IncludeExcludeT,
-    NormalizedResourceT,
-    RawResourceT,
-    SupportsRoute,
-    T,
-)
-
-try:
-    import aiofiles
-
-    AIOFILES_AVAILABLE = True
-except ImportError:
-    aiofiles = None  # type: ignore[assignment]
-    AIOFILES_AVAILABLE = False
-
-__all__ = (
-    "ConfigAgent",
-    "ConfigModel",
-    "ConfigMeta",
-    "save",
-    "save_async",
-    "reload",
-    "reload_async",
-    "pre_serialize",
-    "with_pre_serialize",
-    "post_deserialize",
-    "with_post_deserialize",
-    "export",
-    "export_async",
-    "with_exporter",
-    "with_async_exporter",
-)
-
-_URL_SCHEMES: set[str] = set(
-    urllib.parse.uses_relative + urllib.parse.uses_netloc + urllib.parse.uses_params
-) - {""}
-CONTEXT: str = "__context__"
-TOKEN: str = "__context_token__"
-LOCAL: str = "__local__"
-
-current_context: contextvars.ContextVar[
-    BaseContext[Any] | None
-] = contextvars.ContextVar("current_context", default=None)
-
-_exporting: contextvars.ContextVar[bool] = contextvars.ContextVar(
-    "_exporting", default=False
-)
-
-
-def _get_defaults_from_model_class(
-    model: type[pydantic.BaseModel],
-) -> dict[str, Any]:
-    defaults = {}
-    for field in model.__fields__.values():
-        default = field.default
-        if not field.field_info.exclude and not field.required:
-            if isinstance(default, pydantic.BaseModel):
-                default = default.dict()
-            defaults[field.alias] = default
-    return defaults
-
-
-def _vars_or_dict(obj: Any) -> dict[str, Any]:
-    obj_dict = obj
-    if not isinstance(obj, dict):
-        obj_dict = obj.__dict__
-    return cast(dict[str, Any], obj_dict)
-
-
-def _is_namedtuple(
-    obj: Any,
-) -> bool:
-    return (
-        isinstance(obj, tuple) and hasattr(obj, "_asdict") and hasattr(obj, "_fields")
-    )
-
-
-@functools.singledispatch
-def pre_serialize(obj: Any) -> Any:
-    """
-    Convert a value to a format that can be safely serialized.
-
-    This function is used to convert values that are not supported by
-    `anyconfig` to a format that can be safely serialized. It is used
-    internally by `ConfigModel` and `AsyncConfigModel` to convert
-    values before saving them to a file.
-
-    Parameters
-    ----------
-    obj
-        The value to convert.
-
-    Returns
-    -------
-    Any
-    """
-    if dataclasses.is_dataclass(obj):
-        return pre_serialize(dataclasses.asdict(obj))
-    if _is_namedtuple(obj):
-        return _ps_namedtuple(obj)
-    return obj
-
-
-for obj_type, obj_encoder in ENCODERS_BY_TYPE.items():
-    pre_serialize.register(obj_type, obj_encoder)
-
-
-def with_pre_serialize(
-    func: collections.abc.Callable[[T], Any], cls: type[T] | None = None
-) -> type[T] | Any:
-    """
-    Register a pre-serialization converter function for a type.
-
-    Parameters
-    ----------
-    func
-        The converter function.
-
-    cls
-        The type to register the converter for.
-        Optional for the decoration syntax.
-
-    Returns
-    -------
-    The conversion result class.
-
-    Usage
-    -----
-    .. code-block:: python
-
-        @with_pre_serialize(converter_func)
-        class MyClass:
-            ...
-
-    """
-    if cls is None:
-        return functools.partial(with_pre_serialize, func)
-
-    pre_serialize.register(cls, func)
-
-    if not hasattr(cls, "__get_validators__"):
-
-        def validator_gen() -> (
-            collections.abc.Iterator[collections.abc.Callable[[Any], Any]]
-        ):
-            yield lambda value: post_deserialize.dispatch(cls)(cls, value)
-
-        cls.__get_validators__ = validator_gen  # type: ignore[attr-defined]
-
-    return cls
-
-
-@functools.singledispatch
-def post_deserialize(cls: Any, value: Any) -> Any:
-    """
-    Load a value into a type after deserialization.
-
-    This function is used to load values that are not supported by
-    `anyconfig` to a format that can be used at runtime. It is used
-    by pydantic while performing validation.
-
-    Parameters
-    ----------
-    cls
-        The type to load the value into.
-
-    value
-        The value to load.
-
-    Returns
-    -------
-    The loaded value.
-    """
-    if isinstance(value, cls):
-        return value
-    return cls(value)
-
-
-def with_post_deserialize(
-    func: collections.abc.Callable[[Any], T], cls: type[T] | None = None
-) -> type[T] | Any:
-    """
-    Register a loader function for a type.
-
-    Parameters
-    ----------
-    func
-        The loader function.
-    cls
-        The type to register the loader for.
-
-    Returns
-    -------
-    The loading result class.
-    """
-
-    if cls is None:
-        return functools.partial(with_post_deserialize, func)
-
-    post_deserialize.register(cls, func)
-    return cls
-
-
-@functools.singledispatch
-def export(obj: Any, **kwargs: Any) -> dict[str, Any]:
-    """
-    Export a ConfigModel to a safely-serializable format.
-    Register a custom exporter for a type using the `with_exporter` decorator,
-    which can help to exclude particular values from the export if needed.
-
-    Parameters
-    ----------
-    obj
-    """
-    if isinstance(obj, ConfigModel) and not _exporting.get():
-        return obj.export(**kwargs)
-    return cast(dict[str, Any], obj.dict(**kwargs))
-
-
-@functools.singledispatch
-async def export_async(obj: Any, **kwargs: Any) -> dict[str, Any]:
-    """
-    Export a ConfigModel to a safely-serializable format.
-    Register a custom exporter for a type using the `with_exporter` decorator,
-    which can help to exclude particular values from the export if needed.
-
-    Parameters
-    ----------
-    obj
-    """
-    if isinstance(obj, ConfigModel) and not _exporting.get():
-        return await obj.export_async(**kwargs)
-    return cast(dict[str, Any], await obj.dict_async(**kwargs))
-
-
-def with_exporter(
-    func: collections.abc.Callable[[ConfigModelT], dict[str, Any]],
-    cls: type[ConfigModelT] | None = None,
-) -> type[ConfigModelT] | Any:
-    """
-    Register a custom exporter for a type.
-
-    Parameters
-    ----------
-    func
-        The exporter function.
-    cls
-        The type to register the exporter for.
-    """
-    if cls is None:
-        return functools.partial(with_exporter, func)
-
-    export.register(cls, func)
-    if export_async.dispatch(cls) is export_async:
-
-        async def default_async_func(obj: Any) -> Any:
-            return func(obj)
-
-        export_async.register(cls, default_async_func)
-    return cls
-
-
-def with_async_exporter(
-    func: collections.abc.Callable[
-        [ConfigModelT], collections.abc.Coroutine[Any, Any, dict[str, Any]]
-    ],
-    cls: type[ConfigModelT] | None = None,
-) -> type[ConfigModelT] | Any:
-    """
-    Register a custom exporter for a type.
-
-    Parameters
-    ----------
-    func
-        The exporter function.
-    cls
-        The type to register the exporter for.
-    """
-    if cls is None:
-        return functools.partial(with_exporter, func)
-
-    export_async.register(cls, func)
-    return cls
-
-
-@pre_serialize.register(list)
-def _ps_list(obj: list[Any]) -> list[Any]:
-    """
-    Convert a list to safely-serializable form.
-
-    Parameters
-    ----------
-    obj
-        The list to convert.
-
-    Returns
-    -------
-    The converted list.
-    """
-    return [pre_serialize(item) for item in obj]
-
-
-@pre_serialize.register(collections.abc.Mapping)
-def _ps_mapping(obj: collections.abc.Mapping[Any, Any]) -> dict[Any, Any]:
-    """
-    Convert a mapping to safely-serializable form.
-
-    Parameters
-    ----------
-    obj
-        The mapping to convert.
-
-    Returns
-    -------
-    The converted mapping.
-    """
-    return {k: pre_serialize(v) for k, v in obj.items()}
-
-
-@functools.singledispatch
-def _ps_namedtuple(obj: tuple[Any, ...]) -> Any:
-    """
-    Convert a namedtuple to safely-serializable form.
-
-    Parameters
-    ----------
-    obj
-        The namedtuple to convert.
-
-    Returns
-    -------
-    The converted namedtuple (likely a list).
-    """
-    # Initially I wanted it to be pre_serialize(obj._asdict()), but
-    # pydantic doesn't seem to be friends with custom NamedTuple-s.
-    return pre_serialize(list(obj))
-
-
-def _delegate_ac_options(
-    load_options: dict[str, Any], dump_options: dict[str, Any], options: dict[str, Any]
-) -> None:
-    for key, value in options.items():
-        if key.startswith("dump_"):
-            actual_key = key.removeprefix("dump_")
-            targets = [dump_options]
-        elif key.startswith("load_"):
-            actual_key = key.removeprefix("load_")
-            targets = [load_options]
-        else:
-            actual_key = key
-            targets = [load_options, dump_options]
-        for target in targets:
-            if actual_key in target:
-                msg = (
-                    f"Option {key}={value!r} overlaps with "
-                    f"defined {actual_key}={target[actual_key]!r}"
-                )
-                raise ValueError(msg)
-            target[actual_key] = value
-
-
-class ConfigAgent(Generic[ConfigModelT]):
-    """
-    Configuration resource agent: loader and saver.
-
-    This class is used to broke between the model and the home resource, which
-    can be a file, a URL, or a file-like object. It is used internally
-    by `ConfigModel` and `AsyncConfigModel` to load and save
-    configuration files.
-
-    Parameters
-    ----------
-    resource
-        The resource to load the configuration from.
-    processor
-        The resource processor to use. If not specified, the processor used will
-        be :class:`DefaultProcessor`.
-    ac_parser
-        The name of the engines to use for loading and saving the
-        configuration. If not specified, the processor will be guessed
-        from the file extension.
-    create_if_missing
-        Whether to create the file if it doesn't exist.
-    use_pydantic_json
-        Whether to use pydantic's JSON serialization for saving the
-        configuration. This is useful for preserving the type of
-        values that are not supported by `anyconfig`.
-    kwargs
-        Additional options to pass to `anyconfig` API functions.
-
-    Attributes
-    ----------
-    create_if_missing
-        Whether to create the file if it doesn't exist.
-    ac_parser
-        The name of the engines to use for loading and saving the
-        configuration. If not specified, the processor will be guessed
-        from the file extension.
-    allowed_url_schemes
-        The URL schemes that are allowed to be used.
-
-    Raises
-    ------
-    ValueError
-    """
-
-    _resource: NormalizedResourceT
-    processor_class: type[Processor[ConfigModelT]]
-    ac_parser: str | None
-    create_if_missing: bool
-    relative: bool = False
-    allowed_url_schemes: set[str]
-    use_pydantic_json: bool = True
-    default_load_options: dict[str, Any] = {}
-    default_dump_options: dict[str, Any] = {
-        # These are usually desirable for configuration files.
-        # If you want to change them, you can do so by monkey-patching
-        # these variables. You can also change `load_options` and
-        # `dump_options` instance attributes to make a local change.
-        "allow_unicode": True,
-        "ensure_ascii": False,
-        "indent": 2,
-    }
-
-    predefined_default_kwargs: ClassVar[dict[str, Any]] = {"encoding": "UTF-8"}
-    default_allowed_url_schemes: ClassVar[set[str]] = {"file", "http", "https"}
-
-    OPEN_KWARGS: ClassVar[set[str]] = {
-        "mode",
-        "buffering",
-        "encoding",
-        "errors",
-        "newline",
-    }
-    URLOPEN_KWARGS: ClassVar[set[str]] = {
-        "data",
-        "timeout",
-        "cafile",
-        "capath",
-        "cadefault",
-        "context",
-    }
-    JSON_KWARGS: ClassVar[set[str]] = {
-        "skipkeys",
-        "ensure_ascii",
-        "check_circular",
-        "allow_nan",
-        "cls",
-        "indent",
-        "separators",
-        "default",
-        "sort_keys",
-    }
-    EXPORT_KWARGS: ClassVar[set[str]] = {
-        "by_alias",
-        "include",
-        "exclude",
-        "exclude_unset",
-        "exclude_defaults",
-        "exclude_none",
-    }
-
-    def __init__(
-        self,
-        resource: RawResourceT,
-        ac_parser: str | None = None,
-        processor_class: type[Processor[ConfigModelT]] | None = None,
-        *,
-        create_if_missing: bool = False,
-        **kwargs: Any,
-    ) -> None:
-        """Parameters
-        ----------
-        resource
-            The URL to the configuration file, or a file-like object.
-        ac_parser
-            The name of the engines to use for loading and saving the configuration.
-            Defaults to 'yaml'.
-        create_if_missing
-            Whether to automatically create missing keys when loading the configuration.
-        default_kwargs
-            Default keyword arguments to pass while opening the resource.
-        use_pydantic_json
-            Whether to use Pydantic's JSON encoder/decoder instead of the default
-            anyconfig one.
-        **kwargs
-            Additional keyword arguments to pass to
-            `anyconfig.loads()` and `anyconfig.dumps()`.
-        """
-        if processor_class is None:
-            processor_class = Processor[ConfigModelT]
-
-        self.processor_class = processor_class
-        self.ac_parser = ac_parser
-
-        if isinstance(resource, (str, os.PathLike)) and not (
-            isinstance(resource, str)
-            and urllib.parse.urlparse(str(resource)).scheme in _URL_SCHEMES
-        ):
-            raw_path = os.fspath(resource)
-            resource = pathlib.Path(raw_path)
-            if raw_path.startswith(".") and len(resource.parts) > 1:
-                self.relative = True
-
-        self.resource = resource
-        self.create_if_missing = create_if_missing
-        self.use_pydantic_json = kwargs.pop("use_pydantic_json", True)
-        self.default_kwargs = kwargs.pop(
-            "default_kwargs", self.predefined_default_kwargs.copy()
-        )
-        self.allowed_url_schemes = kwargs.pop(
-            "allowed_url_schemes", self.default_allowed_url_schemes.copy()
-        )
-
-        self.load_options = self.default_load_options.copy()
-        self.dump_options = self.default_dump_options.copy()
-
-        _delegate_ac_options(self.load_options, self.dump_options, kwargs)
-
-    @property
-    def resource(self) -> NormalizedResourceT:
-        """
-        The resource of the configuration.
-
-        This can be a file path, a URL, or a file-like object.
-
-        Returns
-        -------
-        The resource of the configuration.
-        """
-        return self._resource
-
-    @resource.setter
-    def resource(self, value: NormalizedResourceT) -> None:
-        """
-        The resource of the configuration.
-
-        This can be a file path, a URL, or a file-like object.
-
-        .. note::
-            If the resource is a file path, the processor will be guessed
-            from the file extension.
-
-        Returns
-        -------
-        The resource of the configuration.
-        """
-        self._resource = value
-        if self.ac_parser is None:
-            self.ac_parser = self._guess_ac_parser()
-
-    def _guess_ac_parser(self) -> str | None:
-        ac_parser = None
-        if isinstance(self.resource, pathlib.Path):
-            ac_parser = self.resource.suffix[1:].casefold()
-            if not ac_parser:
-                msg = (
-                    "Could not guess the anyconfig parser to use for "
-                    f"{self.resource!r}.\n"
-                    f"Available parsers: {', '.join(anyconfig.list_types())}"
-                )
-                raise UnspecifiedParserError(msg)
-        return ac_parser
-
-    def load_into(
-        self,
-        config_class: type[ConfigModelT],
-        blob: str,
-        ac_parser: str | None = None,
-        **kwargs: Any,
-    ) -> ConfigModelT:
-        """
-        Load the configuration into a `ConfigModel` subclass.
-
-        Parameters
-        ----------
-        config_class
-            The `ConfigModel` subclass to load the configuration into.
-        blob
-            The configuration to load.
-        ac_parser
-            The name of the engines to use for loading the configuration.
-        **kwargs
-            Additional keyword arguments to pass to `anyconfig.loads()`.
-
-        Returns
-        -------
-        The loaded configuration.
-        """
-        dict_config = self.load_into_dict(blob, ac_parser=ac_parser, **kwargs)
-        if dict_config is None:
-            dict_config = {}
-        return config_class.parse_obj(dict_config)
-
-    async def async_load_into(
-        self,
-        config_class: type[ConfigModelT],
-        blob: str,
-        ac_parser: str | None = None,
-        **kwargs: Any,
-    ) -> ConfigModelT:
-        """
-        Load the configuration into a `ConfigModel` subclass asynchronously.
-
-        Parameters
-        ----------
-        config_class
-            The `ConfigModel` subclass to load the configuration into.
-        blob
-            The configuration to load.
-        ac_parser
-            The name of the engines to use for loading the configuration.
-        **kwargs
-            Additional keyword arguments to pass to `anyconfig.loads()`.
-
-        Returns
-        -------
-        The loaded configuration.
-        """
-        dict_config = await self.load_into_dict_async(
-            blob, ac_parser=ac_parser, **kwargs
-        )
-        if dict_config is None:
-            dict_config = {}
-        return config_class.parse_obj(dict_config)
-
-    def _load_into_dict_impl(
-        self,
-        blob: str,
-        ac_parser: str | None = None,
-        **kwargs: Any,
-    ) -> dict[str, Any]:
-        ac_parser = ac_parser or self.ac_parser or self._guess_ac_parser()
-        if ac_parser is None:
-            msg = "Cannot read configuration because `ac_parser` was not specified"
-            raise UnspecifiedParserError(msg)
-        kwargs = self.load_options | kwargs
-        try:
-            loaded = anyconfig.loads(  # type: ignore[no-untyped-call]
-                blob, ac_parser=ac_parser, **kwargs
-            )
-        except anyconfig.UnknownParserTypeError as exc:
-            raise UnavailableParserError(str(exc).split()[-1], self) from exc
-        if not isinstance(loaded, collections.abc.Mapping):
-            msg = (
-                f"Expected a mapping as a result of loading {self.resource}, "
-                f"got {type(loaded).__name__}."
-            )
-            raise TypeError(msg)
-        return dict(loaded)
-
-    def load_into_dict(
-        self,
-        blob: str,
-        ac_parser: str | None = None,
-        *,
-        preprocess: bool = True,
-        **kwargs: Any,
-    ) -> dict[str, Any]:
-        """
-        Load the configuration into a dictionary. The dictionary is
-        usually used to initialize a `ConfigModel` subclass. If the
-        configuration is empty, None might be returned instead of a dictionary.
-
-        Parameters
-        ----------
-        blob
-            The configuration to load.
-        ac_parser
-            The name of the anyconfig parser to use for loading the configuration.
-        preprocess
-        **kwargs
-            Additional keyword arguments to pass to `anyconfig.loads()`.
-
-        Returns
-        -------
-        The loaded configuration dictionary.
-        """
-        loaded = self._load_into_dict_impl(blob, ac_parser=ac_parser, **kwargs)
-        if preprocess:
-            loaded = self.processor_class(self, loaded).preprocess()
-        return loaded
-
-    async def load_into_dict_async(
-        self,
-        blob: str,
-        ac_parser: str | None = None,
-        *,
-        preprocess: bool = True,
-        **kwargs: Any,
-    ) -> dict[str, Any]:
-        """
-        Load the configuration into a dictionary asynchronously.
-
-        Parameters
-        ----------
-        blob
-            The configuration to load.
-        ac_parser
-            The name of the anyconfig parser to use for loading the configuration.
-        preprocess
-        **kwargs
-            Additional keyword arguments to pass to `anyconfig.loads()`.
-
-        Returns
-        -------
-        The loaded configuration dictionary.
-        """
-        loaded = self._load_into_dict_impl(blob, ac_parser, **kwargs)
-        if preprocess:
-            loaded = await self.processor_class(self, loaded).preprocess_async()
-        return loaded
-
-    def dump_config(
-        self,
-        config: ConfigModelT,
-        ac_parser: str | None = None,
-        **kwargs: Any,
-    ) -> str:
-        """
-        Dump the configuration to a string.
-
-        Parameters
-        ----------
-        config
-            The configuration to dump.
-        ac_parser
-            The name of the anyconfig parser to use for saving the configuration.
-        **kwargs
-            Additional keyword arguments to pass to `anyconfig.dumps()`.
-
-        Returns
-        -------
-        The dumped configuration.
-        """
-        if ac_parser is None:
-            ac_parser = self.ac_parser
-        export_kwargs = filter_options(self.EXPORT_KWARGS, kwargs)
-        if ac_parser == "json" and self.use_pydantic_json:
-            export_kwargs |= filter_options(
-                self.JSON_KWARGS, self.dump_options | kwargs
-            )
-            tok = _exporting.set(True)  # noqa: FBT003
-            ctx = contextvars.copy_context()
-            _exporting.reset(tok)
-            return ctx.run(config.json, **export_kwargs)
-        data = export(config, **export_kwargs)
-        return self.dump_data(data, ac_parser=ac_parser, **kwargs)
-
-    async def dump_config_async(
-        self,
-        config: ConfigModelT,
-        ac_parser: str | None = None,
-        **kwargs: Any,
-    ) -> str:
-        """
-        Dump the configuration to a string.
-
-        Parameters
-        ----------
-        config
-            The configuration to dump.
-        ac_parser
-            The name of the anyconfig parser to use for saving the configuration.
-        **kwargs
-            Additional keyword arguments to pass to `anyconfig.dumps()`.
-
-        Returns
-        -------
-        The dumped configuration.
-        """
-        if ac_parser is None:
-            ac_parser = self.ac_parser
-        export_kwargs = filter_options(self.EXPORT_KWARGS, kwargs)
-        if ac_parser == "json" and self.use_pydantic_json:
-            export_kwargs |= filter_options(
-                self.JSON_KWARGS, self.dump_options | kwargs
-            )
-            tok = _exporting.set(True)  # noqa: FBT003
-            task = asyncio.create_task(config.json_async(**export_kwargs))
-            _exporting.reset(tok)
-            return await task
-        data = await export_async(config, **export_kwargs)
-        return self.dump_data(data, ac_parser=ac_parser, **kwargs)
-
-    def dump_data(
-        self,
-        data: dict[str, Any],
-        ac_parser: str | None = None,
-        **kwargs: Any,
-    ) -> str:
-        """
-        Dump data to a string.
-
-        Parameters
-        ----------
-        data
-            The data to dump.
-        ac_parser
-            The name of the anyconfig parser to use for saving the configuration.
-        kwargs
-            Additional keyword arguments to pass to `anyconfig.dumps()`.
-
-        Returns
-        -------
-        The dumped configuration.
-        """
-        if ac_parser is None:
-            ac_parser = self.ac_parser
-        if ac_parser is None:
-            msg = (
-                "Cannot write configuration because `ac_parser` was not specified"
-                f"for agent {self}"
-            )
-            raise UnspecifiedParserError(msg)
-        kwargs = self.dump_options | kwargs
-        return anyconfig.dumps(
-            pre_serialize(data), ac_parser=ac_parser.casefold(), **kwargs
-        )
-
-    @property
-    def is_url(self) -> bool:
-        """Whether the resource is a URL."""
-        return isinstance(self.resource, str)
-
-    def open_resource(self, **kwds: Any) -> ConfigIO:
-        """
-        Open the configuration file.
-
-        Parameters
-        ----------
-        **kwds
-            Keyword arguments to pass to the opening routine.
-            For URLs, these are passed to ``urllib.request.urllib.request.urlopen()``.
-            For local files, these are passed to ``builtins.open()``.
-
-        Returns
-        -------
-        The opened resource.
-        """
-        if self.resource is None:
-            return io.StringIO()
-        if self.is_url:
-            url = urllib.parse.urlparse(cast(str, self.resource))
-            if url.scheme not in self.allowed_url_schemes:
-                msg = (
-                    f"URL scheme {url.scheme!r} is not allowed, "
-                    f"must be one of {self.allowed_url_schemes!r}"
-                )
-                raise ValueError(msg)
-            kwds = filter_options(self.URLOPEN_KWARGS, kwds)
-            request = urllib.request.Request(url.geturl())
-            return cast(ConfigIO, urllib.request.urlopen(request, **kwds))  # noqa: S310
-        if isinstance(self.resource, (int, pathlib.Path)):
-            kwds = filter_options(self.OPEN_KWARGS, kwds)
-            if isinstance(self.resource, int):
-                return cast(
-                    ConfigIO,
-                    # We intentionally do not use the context manager here
-                    # because we do not want to close the file.
-                    # Moreover, we want to allow the file to be opened
-                    # from a file descriptor, not supported by Path().
-                    open(self.resource, **kwds),  # noqa: PTH123, SIM115
-                )
-            return cast(ConfigIO, pathlib.Path(self.resource).open(**kwds))
-        return cast(ConfigIO, self.resource)
-
-    def open_resource_async(self, **kwds: Any) -> AsyncConfigIO:
-        """
-        Open the configuration file asynchronously.
-
-        Parameters
-        ----------
-        **kwds
-            Keyword arguments to pass to the opening routine.
-
-        Returns
-        -------
-        The opened resource.
-        """
-        if self.is_url:
-            msg = "Asynchronous URL opening is not supported"
-            raise NotImplementedError(msg)
-        if not AIOFILES_AVAILABLE:
-            msg = (
-                "Aiofiles is not available, cannot open file "
-                "asynchronously (install with `pip install aiofiles`)"
-            )
-            raise RuntimeError(msg)
-        if isinstance(self.resource, (int, pathlib.Path)):
-            kwds = filter_options(self.OPEN_KWARGS, kwds)
-            return aiofiles.open(self.resource, **kwds)
-        raise RuntimeError("cannot open resource asynchronously")
-
-    def processor_open_resource(self, **kwargs: Any) -> ConfigIO:
-        """
-        Called by the processor to open a configuration resource
-        with the reading intention.
-
-        Parameters
-        ----------
-        **kwargs
-            Keyword arguments to pass to the opening routine.
-            For URLs, these are passed to ``urllib.request.urlopen()``.
-            For local files, these are passed to ``builtins.open()``.
-
-        Returns
-        -------
-        The opened resource.
-        """
-        kwargs = self._get_default_kwargs("read", kwargs)
-        return self.open_resource(**kwargs)
-
-    def processor_open_resource_async(self, **kwargs: Any) -> AsyncConfigIO:
-        """
-        Called by the processor to open a configuration resource asynchronously
-        with the reading intention.
-
-        Parameters
-        ----------
-        **kwargs
-            Keyword arguments to pass to the opening routine.
-            For URLs, these are passed to ``urllib.request.urlopen()``.
-            For local files, these are passed to ``builtins.open()``.
-
-        Returns
-        -------
-        The opened resource.
-        """
-        kwargs = self._get_default_kwargs("read", kwargs)
-        return self.open_resource_async(**kwargs)
-
-    def _get_default_kwargs(
-        self,
-        method: Literal["read", "write"],
-        kwargs: dict[str, Any] | None = None,
-    ) -> dict[str, Any]:
-        if not kwargs:
-            kwargs = self.default_kwargs
-        new_kwargs = cast(dict[str, Any], kwargs).copy()
-        if not self.is_url:
-            if method == "read":
-                new_kwargs.setdefault("mode", "r")
-            elif method == "write":
-                new_kwargs.setdefault("mode", "w")
-            else:
-                msg = f"Invalid resource access method: {method!r}"
-                raise ValueError(msg)
-        return new_kwargs
-
-    def read(
-        self,
-        *,
-        config_class: type[ConfigModelT],
-        create_kwargs: dict[str, Any] | None = None,
-        **kwargs: Any,
-    ) -> ConfigModelT:
-        """
-        Read the configuration file.
-
-        Parameters
-        ----------
-        config_class
-            The configuration model class to load the configuration into.
-        create_kwargs
-            Keyword arguments to pass to the open method
-            when optionally creating the file.
-        **kwargs
-            Keyword arguments to pass to the open method.
-
-        Returns
-        -------
-        The loaded configuration.
-        """
-        kwargs = self._get_default_kwargs("read", kwargs=kwargs)
-        try:
-            with self.open_resource(**kwargs) as fp:
-                blob = fp.read()
-        except FileNotFoundError:
-            blob = None
-            if self.create_if_missing:
-                defaults = _get_defaults_from_model_class(config_class)
-                blob = self.dump_data(defaults)
-                self.write(blob, **(create_kwargs or {}))
-            else:
-                raise
-        return self.load_into(config_class, cast(str, blob), **self.load_options)
-
-    def write(self, blob: str, **kwargs: Any) -> int:
-        """
-        Write the configuration file.
-
-        Parameters
-        ----------
-        blob
-            The string/bytes to write into the resource.
-        kwargs
-            Keyword arguments to pass to the opening routine.
-
-        Returns
-        -------
-        The number of bytes written.
-        """
-        kwargs = self._get_default_kwargs("write", kwargs=kwargs)
-        with self.open_resource(**kwargs) as fp:
-            return fp.write(blob)
-
-    async def read_async(
-        self,
-        *,
-        config_class: type[ConfigModelT],
-        create_kwargs: dict[str, Any] | None = None,
-        **kwargs: Any,
-    ) -> ConfigModelT:
-        """
-        Read the configuration file asynchronously.
-
-        Parameters
-        ----------
-        config_class
-            The configuration model class to load the configuration into.
-        create_kwargs
-            Keyword arguments to pass to the open method
-            when optionally creating the file.
-        **kwargs
-            Keyword arguments to pass to the open method.
-
-        Returns
-        -------
-        The loaded configuration.
-        """
-        kwargs = self._get_default_kwargs("read", kwargs=kwargs)
-        try:
-            async with self.open_resource_async(**kwargs) as fp:
-                blob = await fp.read()
-        except FileNotFoundError:
-            if self.create_if_missing:
-                defaults = _get_defaults_from_model_class(config_class)
-                blob = self.dump_data(defaults)
-                await self.write_async(blob, **(create_kwargs or {}))
-        return await self.async_load_into(config_class, blob, **self.load_options)
-
-    async def write_async(
-        self,
-        blob: str,
-        **kwargs: Any,
-    ) -> int:
-        """
-        Write the configuration file asynchronously.
-
-        Parameters
-        ----------
-        blob
-            The string/bytes to write into the resource.
-        kwargs
-            Keyword arguments to pass to the opening routine.
-
-        Returns
-        -------
-        The number of bytes written.
-        """
-        kwargs = self._get_default_kwargs("write", kwargs=kwargs)
-        async with self.open_resource_async(**kwargs) as fp:
-            return await fp.write(blob)
-
-    @classmethod
-    def from_directive_context(
-        cls,
-        ctx: DirectiveContext,
-        /,
-        route_separator: str = ":",
-        route_class: type[Route] | None = None,
-    ) -> tuple[ConfigAgent[ConfigModelT], SupportsRoute | None]:
-        """
-        Create a configuration agent from a preprocessor directive context.
-        Return an optional scope that the context points to.
-
-        Parameters
-        ----------
-        route_class
-        route_separator
-        ctx
-
-        Returns
-        -------
-        The configuration agent.
-        """
-        if route_class is None:
-            route_class = Route
-        route: SupportsRoute | None = None
-        args: list[Any] = []
-        kwargs: dict[str, Any] = {}
-        if isinstance(ctx.snippet, str):
-            path, _, route = ctx.snippet.partition(route_separator)
-            route = Route(route.strip().replace(route_separator, route_class.TOK_DOT))
-            args.append(path)
-        elif isinstance(ctx.snippet, int):
-            args.append(ctx.snippet)
-        elif is_dict_like(ctx.snippet):
-            kwargs |= ctx.snippet
-        elif is_list_like(ctx.snippet):
-            args += list(ctx.snippet)
-        else:
-            msg = (
-                f"Invalid snippet for the {ctx.directive!r} directive: {ctx.snippet!r}"
-            )
-            raise ValueError(msg)
-        return cls(*args, **kwargs), str(route)
-
-    def __repr__(self) -> str:
-        resource = self.resource
-        return f"{type(self).__name__}({resource=!r})"
-
-
-class Route:
-    TOK_DOT: ClassVar[str] = "."
-    TOK_ESCAPE: ClassVar[str] = "\\"
-    TOK_DOTLISTESC_ENTER: ClassVar[str] = "["
-    TOK_DOTLISTESC_EXIT: ClassVar[str] = "]"
-
-    def __init__(self, route: SupportsRoute) -> None:
-        self.list_route = self.parse(route)
-
-    @classmethod
-    def parse(cls, route: SupportsRoute) -> list[str]:
-        if isinstance(route, Route):
-            return route.list_route
-        if isinstance(route, list):
-            return route
-        if isinstance(route, str):
-            with formatted_syntax_error(route):
-                return cls._decompose(route)
-        raise TypeError(f"invalid route type {type(route)!r}")
-
-    @classmethod
-    def _decompose(cls, route: str) -> list[str]:  # noqa: C901, PLR0912
-        tok_dot = cls.TOK_DOT
-        tok_escape = cls.TOK_ESCAPE
-        tok_dle_enter = cls.TOK_DOTLISTESC_ENTER
-        tok_dle_exit = cls.TOK_DOTLISTESC_EXIT
-
-        route = route.removesuffix(tok_dot) + tok_dot
-
-        part = ""
-        dle_ctx = None
-        list_route: list[str] = []
-        enter = list_route.append
-        error = functools.partial(InternalSyntaxError, prefix="Route(", suffix=")")
-        escape = False
-
-        for index, char in enumerate(route):
-            if escape:
-                part += char
-                escape = False
-                continue
-            is_last = index == len(route) - 1
-            if char == tok_dot:
-                if dle_ctx is not None:
-                    part += char
-                else:
-                    enter(part)
-                    part = ""
-            elif char == tok_escape:
-                if is_last:
-                    part += char
-                else:
-                    escape = True
-            elif char == tok_dle_enter:
-                if dle_ctx is not None:
-                    # a special character at its place
-                    part += char
-                else:
-                    dle_ctx = index
-            elif char == tok_dle_exit:
-                if is_last or route[index + 1] == tok_dot:
-                    if dle_ctx is None:
-                        msg = (
-                            "Dotlist escape sequence "
-                            f"was not opened with {tok_dle_enter!r}"
-                        )
-                        raise error(msg, index=index)
-                    dle_ctx = None
-                else:
-                    # a special character at its place
-                    part += char
-            else:
-                part += char
-            if is_last and dle_ctx is not None:
-                msg = (
-                    "Unclosed dotlist escape sequence "
-                    f"(expected {tok_dle_exit!r} token)"
-                )
-                raise error(msg, index=dle_ctx)
-        return list_route
-
-    @classmethod
-    def decompose(cls, route: str) -> list[str]:
-        with formatted_syntax_error(route):
-            return cls._decompose(route)
-
-    def compose(self) -> str:
-        escape = (self.TOK_DOTLISTESC_ENTER, self.TOK_DOTLISTESC_EXIT)
-        raw = ("", "")
-        return self.TOK_DOT.join(
-            fragment.join(escape).replace(
-                self.TOK_DOTLISTESC_EXIT + self.TOK_DOT,
-                self.TOK_DOTLISTESC_EXIT + self.TOK_ESCAPE + self.TOK_DOT,
-            )
-            if self.TOK_DOT in fragment
-            else fragment.join(raw)
-            for fragment in self.list_route
-        )
-
-    def enter(self, subroute: SupportsRoute) -> Route:
-        return type(self)(self.list_route + self.parse(subroute))
-
-    def __eq__(self, other: Any) -> bool:
-        if isinstance(other, Route):
-            return self.list_route == other.list_route
-        if isinstance(other, str):
-            return self.list_route == self.decompose(other)
-        if isinstance(other, list):
-            return self.list_route == other
-        return NotImplemented
-
-    def __str__(self) -> str:
-        return self.compose()
-
-    def __iter__(self) -> collections.abc.Iterator[str]:
-        yield from self.list_route
-
-    def __repr__(self) -> str:
-        return f"{type(self).__name__}({self.list_route})"
-
-
-def at(
-    mapping: Any,
-    route: SupportsRoute,
-    converter_func: collections.abc.Callable[[Any], dict[str, Any]] = _vars_or_dict,
-    agent: ConfigAgent[ConfigModelT] | None = None,
-) -> Any:
-    """
-    Get an item at a route.
-
-    Parameters
-    ----------
-    mapping
-        The mapping to use.
-    route
-        The route to the item.
-    converter_func
-    agent
-
-    Returns
-    -------
-    The item at the route.
-    """
-    route = Route(route)
-    route_here = []
-    scope = _vars_or_dict(mapping)
-    try:
-        for part in route:
-            route_here.append(part)
-            scope = converter_func(scope)[part]
-    except KeyError:
-        raise ResourceLookupError(agent, route_here) from None
-    return scope
-
-
-@dataclasses.dataclass(frozen=True)
-class ConfigAt(Generic[ConfigModelT]):
-    """
-    A configuration item at a specific location.
-
-    Attributes
-    ----------
-    owner
-        The configuration model instance.
-    mapping
-        The mapping to use.
-    route
-        The route to the item.
-    """
-
-    owner: ConfigModelT
-    mapping: dict[str, Any] | None
-    route: SupportsRoute
-
-    def get(self) -> Any:
-        """
-        Get the value of the item.
-
-        Returns
-        -------
-        The value of the item.
-        """
-        try:
-            scope = at(self.mapping or self.owner, self.route)
-        except KeyError as err:
-            route_here = err.args[1]
-            raise ConfigAccessError(self.owner, route_here) from None
-        return scope
-
-    def update(self, value: Any) -> Any:
-        """
-        Update the value of the item with regard to this item mapping.
-
-        Parameters
-        ----------
-        value
-            The new value.
-
-        Returns
-        -------
-        The updated mapping.
-        """
-        route = list(Route(self.route))
-        mapping = self.mapping or self.owner
-        key = route.pop()
-        scope = _vars_or_dict(mapping)
-        route_here = []
-        try:
-            for part in route:
-                route_here.append(part)
-                scope = _vars_or_dict(scope[part])
-            scope[key] = value
-        except KeyError:
-            raise ConfigAccessError(self.owner, route_here) from None
-        return mapping
-
-    async def save_async(self, **kwargs: Any) -> int:
-        """
-        Save the configuration asynchronously.
-
-        Parameters
-        ----------
-        **kwargs
-            Keyword arguments to pass to the saving function.
-
-        Returns
-        -------
-        The number of bytes written.
-        """
-        return await save_async(self, **kwargs)
-
-    def save(self, **kwargs: Any) -> int:
-        """
-        Save the configuration.
-
-        Parameters
-        ----------
-        **kwargs
-            Keyword arguments to pass to the saving function.
-
-        Returns
-        -------
-        The number of bytes written.
-        """
-        return save(self, **kwargs)
-
-    async def reload_async(self, **kwargs: Any) -> Any:
-        """
-        Reload the configuration asynchronously.
-
-        Parameters
-        ----------
-        kwargs
-            Keyword arguments to pass to the reloading function.
-
-        Returns
-        -------
-        The reloaded configuration or its belonging item.
-        """
-        return await reload_async(self, **kwargs)
-
-    def reload(self, **kwargs: Any) -> Any:
-        """
-        Reload the configuration.
-
-        Parameters
-        ----------
-        kwargs
-            Keyword arguments to pass to the reloading function.
-
-        Returns
-        -------
-        The reloaded configuration or its belonging item.
-        """
-        return reload(self, **kwargs)
-
-
-def save(
-    section: ConfigModelT | ConfigAt[ConfigModelT],
-    write_kwargs: dict[str, Any] | None = None,
-    **kwargs: Any,
-) -> int:
-    """
-    Save the configuration.
-
-    Parameters
-    ----------
-    section
-        The configuration model instance or the configuration item.
-    write_kwargs
-        Keyword arguments to pass to the writing function.
-    **kwargs
-        Keyword arguments to pass to the dumping function.
-
-    Returns
-    -------
-    The number of bytes written.
-    """
-    if isinstance(section, ConfigModel):
-        config = section
-        return config.save(write_kwargs=write_kwargs, **kwargs)
-
-    if write_kwargs is None:
-        write_kwargs = {}
-
-    config = section.owner
-    data = config.initial_state
-    scope = ConfigAt(config, data, section.route)
-    data = scope.update(section.get())
-    context = get_context(config)
-    blob = context.agent.dump_config(config.copy(update=data), **kwargs)
-    result = config.write(blob, **write_kwargs)
-    context.initial_state = data
-    return result
-
-
-async def save_async(
-    section: ConfigModelT | ConfigAt[ConfigModelT],
-    write_kwargs: dict[str, Any] | None = None,
-    **kwargs: Any,
-) -> int:
-    """
-    Save the configuration asynchronously.
-
-    Parameters
-    ----------
-    section
-        The configuration model instance or the configuration item.
-    write_kwargs
-        Keyword arguments to pass to the writing function.
-    **kwargs
-        Keyword arguments to pass to the dumping function.
-
-    Returns
-    -------
-    The number of bytes written.
-    """
-    if isinstance(section, ConfigModel):
-        config = section
-        return await config.save_async(write_kwargs=write_kwargs, **kwargs)
-
-    if write_kwargs is None:
-        write_kwargs = {}
-
-    config = section.owner
-    data = config.initial_state
-    scope = ConfigAt(config, data, section.route)
-    data = scope.update(section.get())
-    context = get_context(config)
-    blob = context.agent.dump_config(config.copy(update=data), **kwargs)
-    result = await config.write_async(blob, **write_kwargs)
-    context.initial_state = data
-    return result
-
-
-def reload(section: ConfigModelT | ConfigAt[ConfigModelT], **kwargs: Any) -> Any:
-    """
-    Reload the configuration.
-
-    Parameters
-    ----------
-    section
-        The configuration model instance or the configuration item.
-    **kwargs
-        Keyword arguments to pass to the reloading function.
-
-    Returns
-    -------
-    The reloaded configuration or its belonging item.
-    """
-    if isinstance(section, ConfigModel):
-        config = section
-        return config.reload()
-
-    config = section.owner
-    context = get_context(config)
-    state = config.__dict__
-    newest = context.agent.read(config_class=type(config), **kwargs)
-    section_data = ConfigAt(newest, newest.__dict__, section.route).get()
-    ConfigAt(config, state, section.route).update(section_data)
-    return section_data
-
-
-async def reload_async(
-    section: ConfigModelT | ConfigAt[ConfigModelT], **kwargs: Any
-) -> Any:
-    """
-    Reload the configuration asynchronously.
-
-    Parameters
-    ----------
-    section
-        The configuration model instance or the configuration item.
-    kwargs
-        Keyword arguments to pass to the reloading function.
-
-    Returns
-    -------
-    The reloaded configuration or its belonging item.
-    """
-    if isinstance(section, ConfigModel):
-        config = section
-        return await config.reload_async()
-
-    config = section.owner
-    context = get_context(config)
-    state = config.__dict__
-    newest = await context.agent.read_async(config_class=type(config), **kwargs)
-    section_data = ConfigAt(newest, newest.__dict__, section.route).get()
-    ConfigAt(config, state, section.route).update(section_data)
-    return section_data
-
-
-class BaseContext(abc.ABC, Generic[ConfigModelT]):
-    """
-    The base class for configuration context.
-    Contexts are used to
-    - store configuration resource information,
-    - link configuration items to the configuration models they belong to,
-    - keep track of the route leading to particular configuration
-      items that are also ConfigModel subclasses.
-
-    Attributes
-    ----------
-    initial_state
-        The initial configuration state.
-
-    """
-
-    initial_state: dict[str, Any]
-
-    @abc.abstractmethod
-    def trace_route(self) -> collections.abc.Iterator[str]:
-        """Trace the route to where the configuration subcontext points to."""
-
-    @property
-    def route(self) -> Route:
-        """The route to where the configuration subcontext points to."""
-        return Route(list(self.trace_route()))
-
-    @overload
-    def enter(self: BaseContext[ConfigModelT], part: None) -> BaseContext[ConfigModelT]:
-        ...
-
-    @overload
-    def enter(self, part: str) -> Subcontext[ConfigModelT]:
-        ...
-
-    def enter(
-        self, part: str | None
-    ) -> Subcontext[ConfigModelT] | BaseContext[ConfigModelT]:
-        """
-        Enter a subcontext.
-
-        Parameters
-        ----------
-        part
-            The name of the item nested in the item this context points to.
-
-        Returns
-        -------
-        The new subcontext.
-        """
-        if part is None:
-            return self
-        return Subcontext(self, part)
-
-    @property
-    @abc.abstractmethod
-    def agent(self) -> ConfigAgent[ConfigModelT]:
-        """The configuration agent responsible for loading and saving."""
-
-    @property
-    @abc.abstractmethod
-    def owner(self) -> ConfigModelT | None:
-        """
-        The top-level configuration model instance,
-        holding all adjacent contexts.
-        """
-
-    @property
-    @abc.abstractmethod
-    def at(self) -> ConfigModelT | ConfigAt[ConfigModelT] | None:
-        """
-        The configuration model instance or the configuration item
-        this context points to.
-        """
-
-
-class Context(BaseContext[ConfigModelT], Generic[ConfigModelT]):
-    """
-    The context of a configuration model.
-
-    Parameters
-    ----------
-    agent
-        The configuration resource agent.
-    owner
-        The top-level configuration model instance,
-        holding all belonging subcontexts.
-    """
-
-    _initial_state: dict[str, Any]
-
-    def __init__(
-        self,
-        agent: ConfigAgent[ConfigModelT],
-        owner: ConfigModelT | None = None,
-    ) -> None:
-        self._agent = agent
-        self._owner = None
-        self._initial_state = {}
-
-        self.owner = owner
-
-    def trace_route(self) -> collections.abc.Iterator[str]:
-        yield from ()
-
-    @property
-    def agent(self) -> ConfigAgent[ConfigModelT]:
-        return self._agent
-
-    @property
-    def at(self) -> ConfigModelT | None:
-        return self.owner
-
-    @property
-    def owner(self) -> ConfigModelT | None:
-        return self._owner
-
-    @owner.setter
-    def owner(self, config: ConfigModelT | None) -> None:
-        if config is None:
-            return
-        self._owner = config
-
-    @property
-    def initial_state(self) -> dict[str, Any]:
-        return copy.deepcopy(self._initial_state)
-
-    @initial_state.setter
-    def initial_state(self, initial_state: dict[str, Any]) -> None:
-        self._initial_state = copy.deepcopy(initial_state)
-
-    def __repr__(self) -> str:
-        agent = self.agent
-        return (
-            f"<{type(self).__name__} "
-            f"of {type(self.owner).__name__!r} configuration "
-            f"({agent=})>"
-        )
-
-
-class Subcontext(BaseContext[ConfigModelT], Generic[ConfigModelT]):
-    """
-    The subcontext of a configuration model.
-
-    Parameters
-    ----------
-    parent
-        The parent context.
-    part
-        The name of the item nested in the item the parent context points to.
-    """
-
-    def __init__(self, parent: BaseContext[ConfigModelT], part: str) -> None:
-        self._parent = parent
-        self._part = part
-
-    @property
-    def agent(self) -> ConfigAgent[ConfigModelT]:
-        return self._parent.agent
-
-    def trace_route(self) -> collections.abc.Iterator[str]:
-        yield from self._parent.trace_route()
-        yield self._part
-
-    @property
-    def at(self) -> ConfigAt[ConfigModelT]:
-        if self.owner is None:
-            msg = "Cannot get section pointed to by an unbound context"
-            raise ValueError(msg)
-        return ConfigAt(self.owner, None, self.route)
-
-    @property
-    def owner(self) -> ConfigModelT | None:
-        return self._parent.owner
-
-    @property
-    def initial_state(self) -> dict[str, Any]:
-        return self._parent.initial_state
-
-    @initial_state.setter
-    def initial_state(self, value: dict[str, Any]) -> None:
-        data = self._parent.initial_state
-        data[self._part] = copy.deepcopy(value)
-        self._parent.initial_state = data
-
-    def __repr__(self) -> str:
-        agent = self.agent
-        route = self.route
-        return (
-            f"<{type(self).__name__} "
-            f"of {type(self.owner).__name__ + '.' + str(route)!r} configuration "
-            f"({agent=})>"
-        )
-
-
-def get_context(config: ConfigModelT) -> BaseContext[ConfigModelT]:
-    """
-    Get the context of the configuration model.
-
-    Parameters
-    ----------
-    config
-        The configuration model instance.
-
-    Returns
-    -------
-    The context of the configuration model.
-    """
-    context = get_context_or_none(config)
-    if context is None:
-        raise RuntimeError("Cannot get context of unbound configuration model")
-    return context
-
-
-def get_context_or_none(config: ConfigModelT) -> BaseContext[ConfigModelT] | None:
-    """
-    Get the context of the configuration model safely.
-
-    Parameters
-    ----------
-    config
-        The configuration model instance.
-
-    Returns
-    -------
-    The context of the configuration model.
-    """
-    return cast(
-        Optional[BaseContext[ConfigModelT]], getattr(config, LOCAL).get(current_context)
-    )
-
-
-def _json_encoder(
-    model_encoder: collections.abc.Callable[..., Any], value: Any, **kwargs: Any
-) -> Any:
-    initial_state_type = type(value)
-    converted_value = pre_serialize(value)
-    if isinstance(converted_value, initial_state_type):
-        return model_encoder(value, **kwargs)
-    return converted_value
-
-
-class ConfigModelMetaclass(ModelMetaclass):
-    def __new__(
-        cls,
-        name: str,
-        bases: tuple[type, ...],
-        namespace: dict[str, Any],
-        **kwargs: Any,
-    ) -> type:
-        namespace |= dict.fromkeys(
-            (EXPORT, CONTEXT, LOCAL, TOKEN), pydantic.PrivateAttr()
-        )
-
-        if kwargs.pop("root", None):
-            return type.__new__(cls, name, bases, namespace, **kwargs)
-
-        new_class = super().__new__(cls, name, bases, namespace, **kwargs)
-        for field in new_class.__fields__.values():
-            if type(field.outer_type_) is ConfigModelMetaclass:
-                if field.pre_validators is None:
-                    field.pre_validators = []
-                validator = make_generic_validator(
-                    field.outer_type_.__field_setup__  # type: ignore[attr-defined]
-                )
-                field.pre_validators.insert(0, validator)
-        new_class.__json_encoder__ = functools.partial(
-            _json_encoder,
-            new_class.__json_encoder__,
-        )
-        return cast(type, new_class)
-
-
-class ConfigModel(
-    pydantic.BaseSettings,
-    metaclass=ConfigModelMetaclass,
-    root=True,
-):
-    """
-    The base class for configuration models.
-
-    It is not recommended to inherit from this class directly for basic usage.
-    Instead, use either :class:`ConfigModel` or :class:`AsyncConfigModel`.
-    """
-
-    def __init__(self, **kwargs: Any) -> None:
-        # Set private attributes via the constructor
-        # to allow preprocessor-related instances to exist.
-        missing = object()
-        for private_attr in self.__private_attributes__:
-            value = kwargs.pop(private_attr, missing)
-            if value is not missing:
-                setattr(self, private_attr, value)
-                if private_attr == CONTEXT:
-                    current_context.set(value)
-        super().__init__(**kwargs)
-
-    def _init_private_attributes(self) -> None:
-        super()._init_private_attributes()
-        local = contextvars.copy_context()
-        setattr(self, LOCAL, local)
-        tok = getattr(self, TOKEN, None)
-        if tok:
-            current_context.reset(tok)
-
-    def export(self, **kwargs: Any) -> dict[str, Any]:
-        """
-        Export the configuration model.
-
-        Returns
-        -------
-        The exported configuration model.
-        """
-        tok = _exporting.set(True)  # noqa: FBT003
-        ctx = contextvars.copy_context()
-        _exporting.reset(tok)
-        return ctx.run(self.dict, **kwargs)
-
-    async def export_async(self, **kwargs: Any) -> dict[str, Any]:
-        """
-        Export the configuration model.
-
-        Returns
-        -------
-        The exported configuration model.
-        """
-        tok = _exporting.set(True)  # noqa: FBT003
-        task = asyncio.create_task(self.dict_async(**kwargs))
-        _exporting.reset(tok)
-        return await task
-
-    async def dict_async(self, **kwargs: Any) -> dict[str, Any]:
-        """
-        Get the dictionary representation of the configuration model.
-
-        Returns
-        -------
-        The dictionary representation of the configuration model.
-        """
-        return dict(await self._iter_async(to_dict=True, **kwargs))
-
-    async def json_async(  # noqa: PLR0913
-        self,
-        include: IncludeExcludeT = None,
-        exclude: IncludeExcludeT = None,
-        *,
-        by_alias: bool = False,
-        exclude_unset: bool = False,
-        exclude_defaults: bool = False,
-        exclude_none: bool = False,
-        encoder: collections.abc.Callable[[Any], Any] | None = None,
-        models_as_dict: bool = True,
-        **dumps_kwargs: Any,
-    ) -> str:
-        encoder = cast(
-            collections.abc.Callable[[Any], Any], encoder or self.__json_encoder__
-        )
-        data = dict(
-            await self._iter_async(
-                to_dict=models_as_dict,
-                by_alias=by_alias,
-                include=include,
-                exclude=exclude,
-                exclude_unset=exclude_unset,
-                exclude_defaults=exclude_defaults,
-                exclude_none=exclude_none,
-            )
-        )
-        if self.__custom_root_type__:
-            data = data[ROOT_KEY]
-        return self.__config__.json_dumps(data, default=encoder, **dumps_kwargs)
-
-    def _iter(  # type: ignore[override]
-        self, **kwargs: Any
-    ) -> collections.abc.Iterator[tuple[str, Any]]:
-        if kwargs.get("to_dict", False) and _exporting.get():
-            state = {}
-            for key, value in super()._iter(**kwargs):
-                state[key] = value
-            metadata = getattr(self, EXPORT, None)
-            if metadata:
-                context = get_context(self)
-                context.agent.processor_class.export(state, metadata=metadata)
-            yield from state.items()
-        else:
-            yield from super()._iter(**kwargs)
-
-    async def _iter_async(
-        self, **kwargs: Any
-    ) -> collections.abc.Iterator[tuple[str, Any]]:
-        if kwargs.get("to_dict", False) and _exporting.get():
-            state = {}
-            for key, value in super()._iter(**kwargs):
-                state[key] = value
-            metadata = getattr(self, EXPORT, None)
-            if metadata:
-                context = get_context(self)
-                await context.agent.processor_class.export_async(
-                    state, metadata=metadata
-                )
-            return ((key, value) for key, value in state.items())
-        return super()._iter(**kwargs)
-
-    @classmethod
-    @no_type_check
-    def _get_value(cls, value: Any, *, to_dict: bool, **kwds: Any) -> Any:
-        if _exporting.get():
-            exporter = export.dispatch(type(value))
-            if (
-                isinstance(value, BaseModel) or exporter != export.dispatch(object)
-            ) and to_dict:
-                value_dict = export(value, **kwds)
-                if ROOT_KEY in value_dict:
-                    return value_dict[ROOT_KEY]
-                return value_dict
-        return super()._get_value(value, to_dict=to_dict, **kwds)
-
-    @classmethod
-    def _resolve_agent(
-        cls,
-        resource: ConfigAgent[ConfigModelT] | RawResourceT | None = None,
-        *,
-        create_if_missing: bool | None = None,
-        ac_parser: str | None = None,
-    ) -> ConfigAgent[ConfigModelT]:
-        if resource is None:
-            resource = getattr(cls.__config__, "resource", None)
-        if resource is None:
-            raise ValueError("No resource specified")
-        if ac_parser is None:
-            ac_parser = getattr(cls.__config__, "ac_parser", None)
-        agent: ConfigAgent[ConfigModelT]
-        if isinstance(resource, ConfigAgent):
-            agent = resource
-        else:
-            agent = ConfigAgent(
-                resource,
-                ac_parser=ac_parser,
-            )
-        if create_if_missing is not None:
-            agent.create_if_missing = create_if_missing
-        if ac_parser is not None:
-            agent.ac_parser = cast(str, ac_parser)
-        return agent
-
-    @property
-    def initial_state(self) -> dict[str, Any]:
-        """
-        The initial configuration state.
-
-        It is a copy of the configuration state
-        at the last time of loading, reloading or saving.
-        """
-        return get_context(self).initial_state
-
-    def at(
-        self: ConfigModelT,
-        route: SupportsRoute,
-    ) -> ConfigAt[ConfigModelT]:
-        """
-        Lazily point to a specific item in the configuration.
-
-        Parameters
-        ----------
-        route
-            The access route to the item in this configuration.
-
-        Returns
-        -------
-        The configuration accessor.
-        """
-        return ConfigAt(self, None, route)
-
-    def update(self, **kwargs: Any) -> None:
-        """
-        Update the configuration with new values, in-place.
-
-        Parameters
-        ----------
-        kwargs
-            The new values to update the configuration with.
-
-        Returns
-        -------
-        None
-        """
-        # Crucial difference to self.__dict__.update():
-        # self.__dict__.update() would not trigger the validation
-        # of the new values.
-        for key, value in kwargs.items():
-            setattr(self, key, value)
-
-    def rollback(self) -> None:
-        """
-        Rollback the configuration to its initial state.
-
-        Returns
-        -------
-        None
-        """
-        context = get_context(self)
-        self.__dict__.update(context.initial_state)
-
-    def __deepcopy__(
-        self: ConfigModelT, memodict: dict[Any, Any] | None = None
-    ) -> ConfigModelT:
-        state = dict(self._iter(to_dict=False))
-        state.pop(LOCAL, None)
-        state.pop(TOKEN, None)
-        return type(self)(**copy.deepcopy(state))
-
-    @classmethod
-    def load(
-        cls: type[ConfigModelT],
-        resource: ConfigAgent[ConfigModelT] | RawResourceT | None = None,
-        *,
-        create_if_missing: bool | None = None,
-        ac_parser: str | None = None,
-        **kwargs: Any,
-    ) -> ConfigModelT:
-        """
-        Load the configuration file.
-        To reload the configuration, use the `reload()` method.
-
-        Parameters
-        ----------
-        resource
-            The configuration resource to read from/write to.
-        ac_parser
-            The anyconfig parser to use.
-        create_if_missing
-            Whether to create the configuration file if it does not exist.
-        **kwargs
-            Keyword arguments to pass to the read method.
-
-        Returns
-        -------
-        self
-        """
-        agent = cls._resolve_agent(
-            resource,
-            ac_parser=ac_parser,
-            create_if_missing=create_if_missing,
-        )
-        context = Context(agent)  # type: Context[ConfigModelT]
-        current_context.set(context)
-        local = contextvars.copy_context()
-        if getattr(
-            cls.__config__,
-            "autoupdate_forward_refs",
-            ConfigMeta.autoupdate_forward_refs,
-        ):
-            cls.update_forward_refs()
-        config = agent.read(config_class=cls, **kwargs)
-        setattr(config, LOCAL, local)
-        context.owner = config
-        context.initial_state = config.__dict__
-        return config
-
-    def reload(self: ConfigModelT, **kwargs: Any) -> ConfigModelT:
-        """
-        Reload the configuration file.
-
-        Parameters
-        ----------
-        **kwargs
-            Keyword arguments to pass to the read method.
-
-        Returns
-        -------
-        self
-        """
-        context = get_context(self)
-        tok = current_context.set(get_context(context.owner))
-        if context.owner is self:
-            changed = context.agent.read(config_class=type(self), **kwargs)
-        else:
-            changed = reload(cast(ConfigAt[ConfigModelT], context.at), **kwargs)
-        current_context.reset(tok)
-        state = changed.__dict__
-        context.initial_state = state
-        self.update(**state)
-        return self
-
-    def save(
-        self: ConfigModelT, write_kwargs: dict[str, Any] | None = None, **kwargs: Any
-    ) -> int:
-        """
-        Save the configuration to the configuration file.
-
-        Parameters
-        ----------
-        write_kwargs
-            Keyword arguments to pass to the write method.
-        **kwargs
-            Keyword arguments to pass to the dumping method.
-
-        Returns
-        -------
-        The number of bytes written.
-        """
-        context = get_context(self)
-        if context.owner is self:
-            if write_kwargs is None:
-                write_kwargs = {}
-            blob = context.agent.dump_config(self, **kwargs)
-            result = self.write(blob, **write_kwargs)
-            context.initial_state = self.__dict__
-            return result
-        return save(
-            cast(ConfigAt[ConfigModelT], context.at),
-            write_kwargs=write_kwargs,
-            **kwargs,
-        )
-
-    def write(self, blob: str, **kwargs: Any) -> int:
-        """
-        Overwrite the configuration file with the given string or bytes.
-
-        Parameters
-        ----------
-        blob
-            The blob to write to the configuration file.
-        **kwargs
-            Keyword arguments to pass to the open method.
-
-        Returns
-        -------
-        The number of bytes written.
-        """
-        context = get_context(self)
-        if context.agent.is_url:
-            msg = "Writing to URLs is not yet supported"
-            raise NotImplementedError(msg)
-        return context.agent.write(blob, **kwargs)
-
-    @classmethod
-    async def load_async(
-        cls: type[ConfigModelT],
-        resource: ConfigAgent[ConfigModelT] | RawResourceT | None = None,
-        *,
-        ac_parser: str | None = None,
-        create_if_missing: bool | None = None,
-        **kwargs: Any,
-    ) -> ConfigModelT:
-        """
-        Load the configuration file asynchronously.
-        To reload the configuration, use the `reload_async()` method.
-
-        Parameters
-        ----------
-        resource
-            The configuration resource.
-        ac_parser
-            The anyconfig parser to use.
-        create_if_missing
-            Whether to create the configuration file if it does not exist.
-        **kwargs
-            Keyword arguments to pass to the read method.
-
-        Returns
-        -------
-        self
-        """
-        agent = cls._resolve_agent(
-            resource, create_if_missing=create_if_missing, ac_parser=ac_parser
-        )
-        context = Context(agent)  # type: Context[ConfigModelT]
-        current_context.set(context)
-        local = contextvars.copy_context()
-        if getattr(
-            cls.__config__,
-            "autoupdate_forward_refs",
-            ConfigMeta.autoupdate_forward_refs,
-        ):
-            cls.update_forward_refs()
-        config = await agent.read_async(config_class=cls, **kwargs)
-        setattr(config, LOCAL, local)
-        context.owner = config
-        return config
-
-    async def reload_async(self: ConfigModelT, **kwargs: Any) -> ConfigModelT:
-        """
-        Reload the configuration file asynchronously.
-
-        Parameters
-        ----------
-        **kwargs
-            Keyword arguments to pass to the read method.
-
-        Returns
-        -------
-        self
-        """
-        context = get_context(self)
-        tok = current_context.set(get_context(context.owner))
-        if context.owner is self:
-            changed = await context.agent.read_async(config_class=type(self), **kwargs)
-        else:
-            changed = await reload_async(
-                cast(ConfigAt[ConfigModelT], context.at), **kwargs
-            )
-        current_context.reset(tok)
-        state = changed.__dict__
-        context.initial_state = state
-        self.update(**state)
-        return self
-
-    async def save_async(
-        self: ConfigModelT, write_kwargs: dict[str, Any] | None = None, **kwargs: Any
-    ) -> int:
-        """
-        Save the configuration to the configuration file asynchronously.
-
-        Parameters
-        ----------
-        write_kwargs
-            Keyword arguments to pass to the write method.
-        **kwargs
-            Keyword arguments to pass to the dumping method.
-
-        Returns
-        -------
-        The number of bytes written.
-        """
-        context = get_context(self)
-        if context.owner is self:
-            if write_kwargs is None:
-                write_kwargs = {}
-            tok = _exporting.set(True)  # noqa: FBT003
-            task = asyncio.create_task(context.agent.dump_config_async(self, **kwargs))
-            _exporting.reset(tok)
-            blob = await task
-            result = await self.write_async(blob, **write_kwargs)
-            context.initial_state = self.__dict__
-            return result
-        return await save_async(
-            cast(ConfigAt[ConfigModelT], context.at),
-            write_kwargs=write_kwargs,
-            **kwargs,
-        )
-
-    async def write_async(self, blob: str, **kwargs: Any) -> int:
-        """
-        Overwrite the configuration file asynchronously with the given string or bytes.
-
-        Parameters
-        ----------
-        blob
-            The blob to write to the configuration file.
-        **kwargs
-            Keyword arguments to pass to the open method.
-
-        Returns
-        -------
-        The number of bytes written.
-        """
-        context = get_context(self)
-        if context.agent.is_url:
-            msg = "Saving to URLs is not yet supported"
-            raise NotImplementedError(msg)
-        return await context.agent.write_async(blob, **kwargs)
-
-    @classmethod
-    def __field_setup__(cls, value: Any, field: ModelField) -> Any:
-        context = current_context.get()
-        if context is not None:
-            subcontext = context.enter(field.name)
-            tok = current_context.set(subcontext)
-            vs = _vars_or_dict(value)
-            vs[TOKEN] = tok
-            vs[LOCAL] = contextvars.copy_context()
-        return value
-
-
-class ConfigMeta(pydantic.BaseSettings.Config):
-    """
-    Meta-configuration for the `ConfigModel` class.
-
-    Attributes
-    ----------
-    resource
-        The configuration resource to read from/write to.
-
-        If a string, it will be interpreted as a path to a file.
-
-    ac_parser
-        The anyconfig parser to use.
-
-    autoupdate_forward_refs
-        Whether to automatically update forward references
-        when `ConfigModel.load()` or `ConfigModel.load_async()`
-        methods are called. For convenience, defaults to `True`.
-
-    And all other attributes from `pydantic.BaseSettings.Config`.
-    """
-
-    resource: ConfigAgent[ConfigModel] | RawResourceT | None = None
-    ac_parser: str | None = None
-    validate_assignment: bool = True
-    autoupdate_forward_refs: bool = True
-
-    Extra = pydantic.Extra
+"""
+The core module of the _configzen_ library.
+
+This module provides an API to manage configuration files and resources
+in a consistent way. It also provides tools to load and save configuration
+files in various formats and within a number of advanced methods.
+
+.. code-block:: python
+
+    from configzen import ConfigModel, ConfigField, ConfigMeta
+
+    class DatabaseConfig(ConfigModel):
+        host: str
+        port: int
+        user: str
+        password: str = ConfigField(exclude=True)
+
+        class Config(ConfigMeta):
+            resource = "examples/database.json"
+
+    db_config = DatabaseConfig.load()
+    db_config.host = "newhost"
+    db_config.port = 5432
+
+    db_config.save()
+
+    db_config = DatabaseConfig.load()
+    print(db_config.host)
+    print(db_config.port)
+
+    # Output:
+    # newhost
+    # 5432
+
+    db_config.host = "otherhost"
+    db_config.port = 5433
+
+    db_config.at("host").save()
+
+    print(db_config.host)
+    print(db_config.port)
+
+    # Output:
+    # otherhost
+    # 5432  # <- not 5433, because we saved only host
+
+    db_config.host = "anotherhost"
+    db_config.at("port").reload()
+
+    print(db_config.host)
+    print(db_config.port)
+
+    # Output:
+    # otherhost  # <- not anotherhost, because we reloaded only port
+    # 5432
+"""
+
+from __future__ import annotations
+
+import abc
+import asyncio
+import collections.abc
+import contextvars
+import copy
+import dataclasses
+import functools
+import io
+import os
+import pathlib
+import urllib.parse
+import urllib.request
+from typing import (
+    Any,
+    ClassVar,
+    Generic,
+    Literal,
+    Optional,
+    cast,
+    no_type_check,
+    overload,
+)
+
+import anyconfig
+import pydantic
+from anyconfig.utils import filter_options, is_dict_like, is_list_like
+from pydantic.fields import (  # type: ignore[attr-defined]
+    ModelField,
+    make_generic_validator,
+)
+from pydantic.json import ENCODERS_BY_TYPE
+from pydantic.main import BaseModel, ModelMetaclass
+from pydantic.utils import ROOT_KEY
+
+from configzen.errors import (
+    ConfigAccessError,
+    InternalSyntaxError,
+    ResourceLookupError,
+    UnspecifiedParserError,
+    UnavailableParserError,
+    formatted_syntax_error,
+)
+from configzen.processor import EXPORT, DirectiveContext, Processor
+from configzen.typedefs import (
+    AsyncConfigIO,
+    ConfigIO,
+    ConfigModelT,
+    IncludeExcludeT,
+    NormalizedResourceT,
+    RawResourceT,
+    SupportsRoute,
+)
+
+try:
+    import aiofiles
+
+    AIOFILES_AVAILABLE = True
+except ImportError:
+    aiofiles = None  # type: ignore[assignment]
+    AIOFILES_AVAILABLE = False
+
+__all__ = (
+    "ConfigAgent",
+    "ConfigModel",
+    "ConfigMeta",
+    "save",
+    "save_async",
+    "reload",
+    "reload_async",
+    "pre_serialize",
+    "post_deserialize",
+    "export",
+    "export_async",
+)
+
+_URL_SCHEMES: set[str] = set(
+    urllib.parse.uses_relative + urllib.parse.uses_netloc + urllib.parse.uses_params
+) - {""}
+CONTEXT: str = "__context__"
+TOKEN: str = "__context_token__"
+LOCAL: str = "__local__"
+
+current_context: contextvars.ContextVar[
+    BaseContext[Any] | None
+    ] = contextvars.ContextVar("current_context", default=None)
+
+_exporting: contextvars.ContextVar[bool] = contextvars.ContextVar(
+    "_exporting", default=False
+)
+
+
+def _get_defaults_from_model_class(
+    model: type[pydantic.BaseModel],
+) -> dict[str, Any]:
+    defaults = {}
+    for field in model.__fields__.values():
+        default = field.default
+        if not field.field_info.exclude and not field.required:
+            if isinstance(default, pydantic.BaseModel):
+                default = default.dict()
+            defaults[field.alias] = default
+    return defaults
+
+
+def _get_object_dict(obj: Any) -> dict[str, Any]:
+    obj_dict = obj
+    if not isinstance(obj, dict):
+        obj_dict = obj.__dict__
+    return cast(dict[str, Any], obj_dict)
+
+
+def _is_namedtuple(
+    obj: Any,
+) -> bool:
+    return (
+        isinstance(obj, tuple) and hasattr(obj, "_asdict") and hasattr(obj, "_fields")
+    )
+
+
+@functools.singledispatch
+def pre_serialize(obj: Any) -> Any:
+    """
+    Convert a value to a format that can be safely serialized.
+
+    This function is used to convert values that are not supported by
+    `anyconfig` to a format that can be safely serialized. It is used
+    internally by `ConfigModel` and `AsyncConfigModel` to convert
+    values before saving them to a file.
+
+    Parameters
+    ----------
+    obj
+        The value to convert.
+
+    Returns
+    -------
+    Any
+    """
+    if dataclasses.is_dataclass(obj):
+        return pre_serialize(dataclasses.asdict(obj))
+    if _is_namedtuple(obj):
+        return _ps_namedtuple(obj)
+    return obj
+
+
+for obj_type, obj_encoder in ENCODERS_BY_TYPE.items():
+    pre_serialize.register(obj_type, obj_encoder)
+
+
+@functools.singledispatch
+def post_deserialize(cls: Any, value: Any) -> Any:
+    """
+    Load a value into a type after deserialization.
+
+    This function is used to load values that are not supported by
+    `anyconfig` to a format that can be used at runtime. It is used
+    by pydantic while performing validation.
+
+    Parameters
+    ----------
+    cls
+        The type to load the value into.
+
+    value
+        The value to load.
+
+    Returns
+    -------
+    The loaded value.
+    """
+    if isinstance(value, cls):
+        return value
+    return cls(value)
+
+
+@functools.singledispatch
+def export(obj: Any, **kwargs: Any) -> dict[str, Any]:
+    """
+    Export a ConfigModel to a safely-serializable format.
+    Register a custom exporter for a type using the `with_exporter` decorator,
+    which can help to exclude particular values from the export if needed.
+
+    Parameters
+    ----------
+    obj
+    """
+    if isinstance(obj, ConfigModel) and not _exporting.get():
+        return obj.export(**kwargs)
+    return cast(dict[str, Any], obj.dict(**kwargs))
+
+
+@functools.singledispatch
+async def export_async(obj: Any, **kwargs: Any) -> dict[str, Any]:
+    """
+    Export a ConfigModel to a safely-serializable format.
+    Register a custom exporter for a type using the `with_exporter` decorator,
+    which can help to exclude particular values from the export if needed.
+
+    Parameters
+    ----------
+    obj
+    """
+    if isinstance(obj, ConfigModel) and not _exporting.get():
+        return await obj.export_async(**kwargs)
+    return cast(dict[str, Any], await obj.dict_async(**kwargs))
+
+
+@pre_serialize.register(list)
+def _ps_list(obj: list[Any]) -> list[Any]:
+    """
+    Convert a list to safely-serializable form.
+
+    Parameters
+    ----------
+    obj
+        The list to convert.
+
+    Returns
+    -------
+    The converted list.
+    """
+    return [pre_serialize(item) for item in obj]
+
+
+@pre_serialize.register(collections.abc.Mapping)
+def _ps_mapping(obj: collections.abc.Mapping[Any, Any]) -> dict[Any, Any]:
+    """
+    Convert a mapping to safely-serializable form.
+
+    Parameters
+    ----------
+    obj
+        The mapping to convert.
+
+    Returns
+    -------
+    The converted mapping.
+    """
+    return {k: pre_serialize(v) for k, v in obj.items()}
+
+
+@functools.singledispatch
+def _ps_namedtuple(obj: tuple[Any, ...]) -> Any:
+    """
+    Convert a namedtuple to safely-serializable form.
+
+    Parameters
+    ----------
+    obj
+        The namedtuple to convert.
+
+    Returns
+    -------
+    The converted namedtuple (likely a list).
+    """
+    # Initially I wanted it to be pre_serialize(obj._asdict()), but
+    # pydantic doesn't seem to be friends with custom NamedTuple-s.
+    return pre_serialize(list(obj))
+
+
+def _delegate_ac_options(
+    load_options: dict[str, Any], dump_options: dict[str, Any], options: dict[str, Any]
+) -> None:
+    for key, value in options.items():
+        if key.startswith("dump_"):
+            actual_key = key.removeprefix("dump_")
+            targets = [dump_options]
+        elif key.startswith("load_"):
+            actual_key = key.removeprefix("load_")
+            targets = [load_options]
+        else:
+            actual_key = key
+            targets = [load_options, dump_options]
+        for target in targets:
+            if actual_key in target:
+                msg = (
+                    f"Option {key}={value!r} overlaps with "
+                    f"defined {actual_key}={target[actual_key]!r}"
+                )
+                raise ValueError(msg)
+            target[actual_key] = value
+
+
+class ConfigAgent(Generic[ConfigModelT]):
+    """
+    Configuration resource agent: loader and saver.
+
+    This class is used to broke between the model and the home resource, which
+    can be a file, a URL, or a file-like object. It is used internally
+    by `ConfigModel` and `AsyncConfigModel` to load and save
+    configuration files.
+
+    Parameters
+    ----------
+    resource
+        The resource to load the configuration from.
+    processor
+        The resource processor to use. If not specified, the processor used will
+        be :class:`DefaultProcessor`.
+    ac_parser
+        The name of the engines to use for loading and saving the
+        configuration. If not specified, the processor will be guessed
+        from the file extension.
+    create_if_missing
+        Whether to create the file if it doesn't exist.
+    use_pydantic_json
+        Whether to use pydantic's JSON serialization for saving the
+        configuration. This is useful for preserving the type of
+        values that are not supported by `anyconfig`.
+    kwargs
+        Additional options to pass to `anyconfig` API functions.
+
+    Attributes
+    ----------
+    create_if_missing
+        Whether to create the file if it doesn't exist.
+    ac_parser
+        The name of the engines to use for loading and saving the
+        configuration. If not specified, the processor will be guessed
+        from the file extension.
+    allowed_url_schemes
+        The URL schemes that are allowed to be used.
+
+    Raises
+    ------
+    ValueError
+    """
+
+    _resource: NormalizedResourceT
+    processor_class: type[Processor[ConfigModelT]]
+    create_if_missing: bool
+    relative: bool = False
+    allowed_url_schemes: set[str]
+    use_pydantic_json: bool = True
+    default_load_options: dict[str, Any] = {}
+    default_dump_options: dict[str, Any] = {
+        # These are usually desirable for configuration files.
+        # If you want to change them, you can do so by monkey-patching
+        # these variables. You can also change `load_options` and
+        # `dump_options` instance attributes to make a local change.
+        "allow_unicode": True,
+        "ensure_ascii": False,
+        "indent": 2,
+    }
+
+    predefined_default_kwargs: ClassVar[dict[str, Any]] = {"encoding": "UTF-8"}
+    default_allowed_url_schemes: ClassVar[set[str]] = {"file", "http", "https"}
+
+    OPEN_KWARGS: ClassVar[set[str]] = {
+        "mode",
+        "buffering",
+        "encoding",
+        "errors",
+        "newline",
+    }
+    URLOPEN_KWARGS: ClassVar[set[str]] = {
+        "data",
+        "timeout",
+        "cafile",
+        "capath",
+        "cadefault",
+        "context",
+    }
+    JSON_KWARGS: ClassVar[set[str]] = {
+        "skipkeys",
+        "ensure_ascii",
+        "check_circular",
+        "allow_nan",
+        "cls",
+        "indent",
+        "separators",
+        "default",
+        "sort_keys",
+    }
+    EXPORT_KWARGS: ClassVar[set[str]] = {
+        "by_alias",
+        "include",
+        "exclude",
+        "exclude_unset",
+        "exclude_defaults",
+        "exclude_none",
+    }
+
+    def __init__(
+        self,
+        resource: RawResourceT,
+        ac_parser: str | None = None,
+        processor_class: type[Processor[ConfigModelT]] | None = None,
+        *,
+        create_if_missing: bool = False,
+        **kwargs: Any,
+    ) -> None:
+        """Parameters
+        ----------
+        resource
+            The URL to the configuration file, or a file-like object.
+        ac_parser
+            The name of the engines to use for loading and saving the configuration.
+            Defaults to 'yaml'.
+        create_if_missing
+            Whether to automatically create missing keys when loading the configuration.
+        default_kwargs
+            Default keyword arguments to pass while opening the resource.
+        use_pydantic_json
+            Whether to use Pydantic's JSON encoder/decoder instead of the default
+            anyconfig one.
+        **kwargs
+            Additional keyword arguments to pass to
+            `anyconfig.loads()` and `anyconfig.dumps()`.
+        """
+        self._ac_parser = None
+
+        if processor_class is None:
+            processor_class = Processor[ConfigModelT]
+
+        self.processor_class = processor_class
+        self.ac_parser = ac_parser
+
+        if isinstance(resource, (str, os.PathLike)) and not (
+            isinstance(resource, str)
+            and urllib.parse.urlparse(str(resource)).scheme in _URL_SCHEMES
+        ):
+            raw_path = os.fspath(resource)
+            resource = pathlib.Path(raw_path)
+            if raw_path.startswith(".") and len(resource.parts) > 1:
+                self.relative = True
+
+        self.resource = resource
+        self.create_if_missing = create_if_missing
+        self.use_pydantic_json = kwargs.pop("use_pydantic_json", True)
+        self.default_kwargs = kwargs.pop(
+            "default_kwargs", self.predefined_default_kwargs.copy()
+        )
+        self.allowed_url_schemes = kwargs.pop(
+            "allowed_url_schemes", self.default_allowed_url_schemes.copy()
+        )
+
+        self.load_options = self.default_load_options.copy()
+        self.dump_options = self.default_dump_options.copy()
+
+        _delegate_ac_options(self.load_options, self.dump_options, kwargs)
+
+    @property
+    def resource(self) -> NormalizedResourceT:
+        """
+        The resource of the configuration.
+
+        This can be a file path, a URL, or a file-like object.
+
+        Returns
+        -------
+        The resource of the configuration.
+        """
+        return self._resource
+
+    @resource.setter
+    def resource(self, value: NormalizedResourceT) -> None:
+        """
+        The resource of the configuration.
+
+        This can be a file path, a URL, or a file-like object.
+
+        .. note::
+            If the resource is a file path, the processor will be guessed
+            from the file extension.
+
+        Returns
+        -------
+        The resource of the configuration.
+        """
+        self._resource = value
+        if self.ac_parser is None:
+            self.ac_parser = self._guess_ac_parser()
+
+    @property
+    def ac_parser(self) -> str | None:
+        return self._ac_parser
+
+    @ac_parser.setter
+    def ac_parser(self, value: str | None) -> None:
+        if value is not None:
+            value = value.casefold()
+        self._ac_parser = value
+
+    def _guess_ac_parser(self) -> str | None:
+        ac_parser = None
+        if isinstance(self.resource, pathlib.Path):
+            ac_parser = self.resource.suffix[1:]
+            if not ac_parser:
+                msg = (
+                    "Could not guess the anyconfig parser to use for "
+                    f"{self.resource!r}.\n"
+                    f"Available parsers: {', '.join(anyconfig.list_types())}"
+                )
+                raise UnspecifiedParserError(msg)
+        return ac_parser
+
+    def load_into(
+        self,
+        config_class: type[ConfigModelT],
+        blob: str,
+        ac_parser: str | None = None,
+        **kwargs: Any,
+    ) -> ConfigModelT:
+        """
+        Load the configuration into a `ConfigModel` subclass.
+
+        Parameters
+        ----------
+        config_class
+            The `ConfigModel` subclass to load the configuration into.
+        blob
+            The configuration to load.
+        ac_parser
+            The name of the engines to use for loading the configuration.
+        **kwargs
+            Additional keyword arguments to pass to `anyconfig.loads()`.
+
+        Returns
+        -------
+        The loaded configuration.
+        """
+        dict_config = self.load_dict(blob, ac_parser=ac_parser, **kwargs)
+        if dict_config is None:
+            dict_config = {}
+        return config_class.parse_obj(dict_config)
+
+    async def async_load_into(
+        self,
+        config_class: type[ConfigModelT],
+        blob: str,
+        ac_parser: str | None = None,
+        **kwargs: Any,
+    ) -> ConfigModelT:
+        """
+        Load the configuration into a `ConfigModel` subclass asynchronously.
+
+        Parameters
+        ----------
+        config_class
+            The `ConfigModel` subclass to load the configuration into.
+        blob
+            The configuration to load.
+        ac_parser
+            The name of the engines to use for loading the configuration.
+        **kwargs
+            Additional keyword arguments to pass to `anyconfig.loads()`.
+
+        Returns
+        -------
+        The loaded configuration.
+        """
+        dict_config = await self.load_dict_async(
+            blob, ac_parser=ac_parser, **kwargs
+        )
+        if dict_config is None:
+            dict_config = {}
+        return config_class.parse_obj(dict_config)
+
+    def _load_dict_impl(
+        self,
+        blob: str,
+        ac_parser: str | None = None,
+        **kwargs: Any,
+    ) -> dict[str, Any]:
+        ac_parser = ac_parser or self.ac_parser or self._guess_ac_parser()
+        if ac_parser is None:
+            msg = "Cannot read configuration because `ac_parser` was not specified"
+            raise UnspecifiedParserError(msg)
+        kwargs = self.load_options | kwargs
+        try:
+            loaded = anyconfig.loads(  # type: ignore[no-untyped-call]
+                blob, ac_parser=ac_parser, **kwargs
+            )
+        except anyconfig.UnknownParserTypeError as exc:
+            raise UnavailableParserError(str(exc).split()[-1], self) from exc
+        if not isinstance(loaded, collections.abc.Mapping):
+            msg = (
+                f"Expected a mapping as a result of loading {self.resource}, "
+                f"got {type(loaded).__name__}."
+            )
+            raise TypeError(msg)
+        return dict(loaded)
+
+    def load_dict(
+        self,
+        blob: str,
+        ac_parser: str | None = None,
+        *,
+        preprocess: bool = True,
+        **kwargs: Any,
+    ) -> dict[str, Any]:
+        """
+        Load the configuration into a dictionary. The dictionary is
+        usually used to initialize a `ConfigModel` subclass. If the
+        configuration is empty, None might be returned instead of a dictionary.
+
+        Parameters
+        ----------
+        blob
+            The configuration to load.
+        ac_parser
+            The name of the anyconfig parser to use for loading the configuration.
+        preprocess
+        **kwargs
+            Additional keyword arguments to pass to `anyconfig.loads()`.
+
+        Returns
+        -------
+        The loaded configuration dictionary.
+        """
+        loaded = self._load_dict_impl(blob, ac_parser=ac_parser, **kwargs)
+        if preprocess:
+            loaded = self.processor_class(self, loaded).preprocess()
+        return loaded
+
+    async def load_dict_async(
+        self,
+        blob: str,
+        ac_parser: str | None = None,
+        *,
+        preprocess: bool = True,
+        **kwargs: Any,
+    ) -> dict[str, Any]:
+        """
+        Load the configuration into a dictionary asynchronously.
+
+        Parameters
+        ----------
+        blob
+            The configuration to load.
+        ac_parser
+            The name of the anyconfig parser to use for loading the configuration.
+        preprocess
+        **kwargs
+            Additional keyword arguments to pass to `anyconfig.loads()`.
+
+        Returns
+        -------
+        The loaded configuration dictionary.
+        """
+        loaded = self._load_dict_impl(blob, ac_parser, **kwargs)
+        if preprocess:
+            loaded = await self.processor_class(self, loaded).preprocess_async()
+        return loaded
+
+    def dump_config(
+        self,
+        config: ConfigModelT,
+        ac_parser: str | None = None,
+        **kwargs: Any,
+    ) -> str:
+        """
+        Dump the configuration to a string.
+
+        Parameters
+        ----------
+        config
+            The configuration to dump.
+        ac_parser
+            The name of the anyconfig parser to use for saving the configuration.
+        **kwargs
+            Additional keyword arguments to pass to `anyconfig.dumps()`.
+
+        Returns
+        -------
+        The dumped configuration.
+        """
+        if ac_parser is None:
+            ac_parser = self.ac_parser
+        export_kwargs = filter_options(self.EXPORT_KWARGS, kwargs)
+        if ac_parser == "json" and self.use_pydantic_json:
+            export_kwargs |= filter_options(
+                self.JSON_KWARGS, self.dump_options | kwargs
+            )
+            tok = _exporting.set(True)  # noqa: FBT003
+            ctx = contextvars.copy_context()
+            _exporting.reset(tok)
+            return ctx.run(config.json, **export_kwargs)
+        data = export(config, **export_kwargs)
+        return self.dump_data(data, ac_parser=ac_parser, **kwargs)
+
+    async def dump_config_async(
+        self,
+        config: ConfigModelT,
+        ac_parser: str | None = None,
+        **kwargs: Any,
+    ) -> str:
+        """
+        Dump the configuration to a string.
+
+        Parameters
+        ----------
+        config
+            The configuration to dump.
+        ac_parser
+            The name of the anyconfig parser to use for saving the configuration.
+        **kwargs
+            Additional keyword arguments to pass to `anyconfig.dumps()`.
+
+        Returns
+        -------
+        The dumped configuration.
+        """
+        if ac_parser is None:
+            ac_parser = self.ac_parser
+        export_kwargs = filter_options(self.EXPORT_KWARGS, kwargs)
+        if ac_parser == "json" and self.use_pydantic_json:
+            export_kwargs |= filter_options(
+                self.JSON_KWARGS, self.dump_options | kwargs
+            )
+            tok = _exporting.set(True)  # noqa: FBT003
+            task = asyncio.create_task(config.json_async(**export_kwargs))
+            _exporting.reset(tok)
+            return await task
+        data = await export_async(config, **export_kwargs)
+        return self.dump_data(data, ac_parser=ac_parser, **kwargs)
+
+    def dump_data(
+        self,
+        data: dict[str, Any],
+        ac_parser: str | None = None,
+        **kwargs: Any,
+    ) -> str:
+        """
+        Dump data to a string.
+
+        Parameters
+        ----------
+        data
+            The data to dump.
+        ac_parser
+            The name of the anyconfig parser to use for saving the configuration.
+        kwargs
+            Additional keyword arguments to pass to `anyconfig.dumps()`.
+
+        Returns
+        -------
+        The dumped configuration.
+        """
+        if ac_parser is None:
+            ac_parser = self.ac_parser
+        if ac_parser is None:
+            msg = (
+                "Cannot write configuration because `ac_parser` was not specified"
+                f"for agent {self}"
+            )
+            raise UnspecifiedParserError(msg)
+        kwargs = self.dump_options | kwargs
+        return anyconfig.dumps(
+            pre_serialize(data), ac_parser=ac_parser, **kwargs
+        )
+
+    @property
+    def is_url(self) -> bool:
+        """Whether the resource is a URL."""
+        return isinstance(self.resource, str)
+
+    def open_resource(self, **kwds: Any) -> ConfigIO:
+        """
+        Open the configuration file.
+
+        Parameters
+        ----------
+        **kwds
+            Keyword arguments to pass to the opening routine.
+            For URLs, these are passed to ``urllib.request.urllib.request.urlopen()``.
+            For local files, these are passed to ``builtins.open()``.
+
+        Returns
+        -------
+        The opened resource.
+        """
+        if self.resource is None:
+            return io.StringIO()
+        if self.is_url:
+            url = urllib.parse.urlparse(cast(str, self.resource))
+            if url.scheme not in self.allowed_url_schemes:
+                msg = (
+                    f"URL scheme {url.scheme!r} is not allowed, "
+                    f"must be one of {self.allowed_url_schemes!r}"
+                )
+                raise ValueError(msg)
+            kwds = filter_options(self.URLOPEN_KWARGS, kwds)
+            request = urllib.request.Request(url.geturl())
+            return cast(ConfigIO, urllib.request.urlopen(request, **kwds))  # noqa: S310
+        if isinstance(self.resource, (int, pathlib.Path)):
+            kwds = filter_options(self.OPEN_KWARGS, kwds)
+            if isinstance(self.resource, int):
+                return cast(
+                    ConfigIO,
+                    # We intentionally do not use the context manager here
+                    # because we do not want to close the file.
+                    # Moreover, we want to allow the file to be opened
+                    # from a file descriptor, not supported by Path().
+                    open(self.resource, **kwds),  # noqa: PTH123, SIM115
+                )
+            return cast(ConfigIO, pathlib.Path(self.resource).open(**kwds))
+        return cast(ConfigIO, self.resource)
+
+    def open_resource_async(self, **kwds: Any) -> AsyncConfigIO:
+        """
+        Open the configuration file asynchronously.
+
+        Parameters
+        ----------
+        **kwds
+            Keyword arguments to pass to the opening routine.
+
+        Returns
+        -------
+        The opened resource.
+        """
+        if self.is_url:
+            msg = "Asynchronous URL opening is not supported"
+            raise NotImplementedError(msg)
+        if not AIOFILES_AVAILABLE:
+            msg = (
+                "Aiofiles is not available, cannot open file "
+                "asynchronously (install with `pip install aiofiles`)"
+            )
+            raise RuntimeError(msg)
+        if isinstance(self.resource, (int, pathlib.Path)):
+            kwds = filter_options(self.OPEN_KWARGS, kwds)
+            return aiofiles.open(self.resource, **kwds)
+        raise RuntimeError("cannot open resource asynchronously")
+
+    def processor_open_resource(self, **kwargs: Any) -> ConfigIO:
+        """
+        Called by the processor to open a configuration resource
+        with the reading intention.
+
+        Parameters
+        ----------
+        **kwargs
+            Keyword arguments to pass to the opening routine.
+            For URLs, these are passed to ``urllib.request.urlopen()``.
+            For local files, these are passed to ``builtins.open()``.
+
+        Returns
+        -------
+        The opened resource.
+        """
+        kwargs = self._get_default_kwargs("read", kwargs)
+        return self.open_resource(**kwargs)
+
+    def processor_open_resource_async(self, **kwargs: Any) -> AsyncConfigIO:
+        """
+        Called by the processor to open a configuration resource asynchronously
+        with the reading intention.
+
+        Parameters
+        ----------
+        **kwargs
+            Keyword arguments to pass to the opening routine.
+            For URLs, these are passed to ``urllib.request.urlopen()``.
+            For local files, these are passed to ``builtins.open()``.
+
+        Returns
+        -------
+        The opened resource.
+        """
+        kwargs = self._get_default_kwargs("read", kwargs)
+        return self.open_resource_async(**kwargs)
+
+    def _get_default_kwargs(
+        self,
+        method: Literal["read", "write"],
+        kwargs: dict[str, Any] | None = None,
+    ) -> dict[str, Any]:
+        if not kwargs:
+            kwargs = self.default_kwargs
+        new_kwargs = cast(dict[str, Any], kwargs).copy()
+        if not self.is_url:
+            if method == "read":
+                new_kwargs.setdefault("mode", "r")
+            elif method == "write":
+                new_kwargs.setdefault("mode", "w")
+            else:
+                msg = f"Invalid resource access method: {method!r}"
+                raise ValueError(msg)
+        return new_kwargs
+
+    def read(
+        self,
+        *,
+        config_class: type[ConfigModelT],
+        create_kwargs: dict[str, Any] | None = None,
+        **kwargs: Any,
+    ) -> ConfigModelT:
+        """
+        Read the configuration file.
+
+        Parameters
+        ----------
+        config_class
+            The configuration model class to load the configuration into.
+        create_kwargs
+            Keyword arguments to pass to the open method
+            when optionally creating the file.
+        **kwargs
+            Keyword arguments to pass to the open method.
+
+        Returns
+        -------
+        The loaded configuration.
+        """
+        kwargs = self._get_default_kwargs("read", kwargs=kwargs)
+        try:
+            with self.open_resource(**kwargs) as fp:
+                blob = fp.read()
+        except FileNotFoundError:
+            if self.create_if_missing:
+                defaults = _get_defaults_from_model_class(config_class)
+                blob = self.dump_data(defaults)
+                self.write(blob, **(create_kwargs or {}))
+            else:
+                raise
+        return self.load_into(config_class, blob, **self.load_options)
+
+    def write(self, blob: str, **kwargs: Any) -> int:
+        """
+        Write the configuration file.
+
+        Parameters
+        ----------
+        blob
+            The string/bytes to write into the resource.
+        kwargs
+            Keyword arguments to pass to the opening routine.
+
+        Returns
+        -------
+        The number of bytes written.
+        """
+        kwargs = self._get_default_kwargs("write", kwargs=kwargs)
+        with self.open_resource(**kwargs) as fp:
+            return fp.write(blob)
+
+    async def read_async(
+        self,
+        *,
+        config_class: type[ConfigModelT],
+        create_kwargs: dict[str, Any] | None = None,
+        **kwargs: Any,
+    ) -> ConfigModelT:
+        """
+        Read the configuration file asynchronously.
+
+        Parameters
+        ----------
+        config_class
+            The configuration model class to load the configuration into.
+        create_kwargs
+            Keyword arguments to pass to the open method
+            when optionally creating the file.
+        **kwargs
+            Keyword arguments to pass to the open method.
+
+        Returns
+        -------
+        The loaded configuration.
+        """
+        kwargs = self._get_default_kwargs("read", kwargs=kwargs)
+        try:
+            async with self.open_resource_async(**kwargs) as fp:
+                blob = await fp.read()
+        except FileNotFoundError:
+            if self.create_if_missing:
+                defaults = _get_defaults_from_model_class(config_class)
+                blob = self.dump_data(defaults)
+                await self.write_async(blob, **(create_kwargs or {}))
+        return await self.async_load_into(config_class, blob, **self.load_options)
+
+    async def write_async(
+        self,
+        blob: str,
+        **kwargs: Any,
+    ) -> int:
+        """
+        Write the configuration file asynchronously.
+
+        Parameters
+        ----------
+        blob
+            The string/bytes to write into the resource.
+        kwargs
+            Keyword arguments to pass to the opening routine.
+
+        Returns
+        -------
+        The number of bytes written.
+        """
+        kwargs = self._get_default_kwargs("write", kwargs=kwargs)
+        async with self.open_resource_async(**kwargs) as fp:
+            return await fp.write(blob)
+
+    @classmethod
+    def from_directive_context(
+        cls,
+        ctx: DirectiveContext,
+        /,
+        route_separator: str = ":",
+        route_class: type[Route] | None = None,
+    ) -> tuple[ConfigAgent[ConfigModelT], SupportsRoute | None]:
+        """
+        Create a configuration agent from a preprocessor directive context.
+        Return an optional scope that the context points to.
+
+        Parameters
+        ----------
+        route_class
+        route_separator
+        ctx
+
+        Returns
+        -------
+        The configuration agent.
+        """
+        if route_class is None:
+            route_class = Route
+        route: SupportsRoute | None = None
+        args: list[Any] = []
+        kwargs: dict[str, Any] = {}
+        if isinstance(ctx.snippet, str):
+            path, _, route = ctx.snippet.partition(route_separator)
+            route = Route(route.strip().replace(route_separator, route_class.TOK_DOT))
+            args.append(path)
+        elif isinstance(ctx.snippet, int):
+            args.append(ctx.snippet)
+        elif is_dict_like(ctx.snippet):
+            kwargs |= ctx.snippet
+        elif is_list_like(ctx.snippet):
+            args += list(ctx.snippet)
+        else:
+            msg = (
+                f"Invalid snippet for the {ctx.directive!r} directive: {ctx.snippet!r}"
+            )
+            raise ValueError(msg)
+        return cls(*args, **kwargs), str(route)
+
+    def __repr__(self) -> str:
+        resource = self.resource
+        return f"{type(self).__name__}({resource=!r})"
+
+
+class Route:
+    TOK_DOT: ClassVar[str] = "."
+    TOK_ESCAPE: ClassVar[str] = "\\"
+    TOK_DOTLISTESC_ENTER: ClassVar[str] = "["
+    TOK_DOTLISTESC_EXIT: ClassVar[str] = "]"
+
+    def __init__(self, route: SupportsRoute) -> None:
+        self.list_route = self.parse(route)
+
+    @classmethod
+    def parse(cls, route: SupportsRoute) -> list[str]:
+        if isinstance(route, Route):
+            return route.list_route
+        if isinstance(route, list):
+            return route
+        if isinstance(route, str):
+            with formatted_syntax_error(route):
+                return cls._decompose(route)
+        raise TypeError(f"invalid route type {type(route)!r}")
+
+    @classmethod
+    def _decompose(cls, route: str) -> list[str]:  # noqa: C901, PLR0912
+        tok_dot = cls.TOK_DOT
+        tok_escape = cls.TOK_ESCAPE
+        tok_dle_enter = cls.TOK_DOTLISTESC_ENTER
+        tok_dle_exit = cls.TOK_DOTLISTESC_EXIT
+
+        route = route.removesuffix(tok_dot) + tok_dot
+
+        part = ""
+        dle_ctx = None
+        list_route: list[str] = []
+        enter = list_route.append
+        error = functools.partial(InternalSyntaxError, prefix="Route(", suffix=")")
+        escape = False
+
+        for index, char in enumerate(route):
+            if escape:
+                part += char
+                escape = False
+                continue
+            is_last = index == len(route) - 1
+            if char == tok_dot:
+                if dle_ctx is not None:
+                    part += char
+                else:
+                    enter(part)
+                    part = ""
+            elif char == tok_escape:
+                if is_last:
+                    part += char
+                else:
+                    escape = True
+            elif char == tok_dle_enter:
+                if dle_ctx is not None:
+                    # a special character at its place
+                    part += char
+                else:
+                    dle_ctx = index
+            elif char == tok_dle_exit:
+                if is_last or route[index + 1] == tok_dot:
+                    if dle_ctx is None:
+                        msg = (
+                            "Dotlist escape sequence "
+                            f"was not opened with {tok_dle_enter!r}"
+                        )
+                        raise error(msg, index=index)
+                    dle_ctx = None
+                else:
+                    # a special character at its place
+                    part += char
+            else:
+                part += char
+            if is_last and dle_ctx is not None:
+                msg = (
+                    "Unclosed dotlist escape sequence "
+                    f"(expected {tok_dle_exit!r} token)"
+                )
+                raise error(msg, index=dle_ctx)
+        return list_route
+
+    @classmethod
+    def decompose(cls, route: str) -> list[str]:
+        with formatted_syntax_error(route):
+            return cls._decompose(route)
+
+    def compose(self) -> str:
+        escape = (self.TOK_DOTLISTESC_ENTER, self.TOK_DOTLISTESC_EXIT)
+        raw = ("", "")
+        return self.TOK_DOT.join(
+            fragment.join(escape).replace(
+                self.TOK_DOTLISTESC_EXIT + self.TOK_DOT,
+                self.TOK_DOTLISTESC_EXIT + self.TOK_ESCAPE + self.TOK_DOT,
+            )
+            if self.TOK_DOT in fragment
+            else fragment.join(raw)
+            for fragment in self.list_route
+        )
+
+    def enter(self, subroute: SupportsRoute) -> Route:
+        return type(self)(self.list_route + self.parse(subroute))
+
+    def __eq__(self, other: Any) -> bool:
+        if isinstance(other, Route):
+            return self.list_route == other.list_route
+        if isinstance(other, str):
+            return self.list_route == self.decompose(other)
+        if isinstance(other, list):
+            return self.list_route == other
+        return NotImplemented
+
+    def __str__(self) -> str:
+        return self.compose()
+
+    def __iter__(self) -> collections.abc.Iterator[str]:
+        yield from self.list_route
+
+    def __repr__(self) -> str:
+        return f"{type(self).__name__}({self.list_route})"
+
+
+def at(
+    mapping: Any,
+    route: SupportsRoute,
+    converter_func: collections.abc.Callable[[Any], dict[str, Any]] = _get_object_dict,
+    agent: ConfigAgent[ConfigModelT] | None = None,
+) -> Any:
+    """
+    Get an item at a route.
+
+    Parameters
+    ----------
+    mapping
+        The mapping to use.
+    route
+        The route to the item.
+    converter_func
+    agent
+
+    Returns
+    -------
+    The item at the route.
+    """
+    route = Route(route)
+    route_here = []
+    scope = _get_object_dict(mapping)
+    try:
+        for part in route:
+            route_here.append(part)
+            scope = converter_func(scope)[part]
+    except KeyError:
+        raise ResourceLookupError(agent, route_here) from None
+    return scope
+
+
+@dataclasses.dataclass(frozen=True)
+class ConfigAt(Generic[ConfigModelT]):
+    """
+    A configuration item at a specific location.
+
+    Attributes
+    ----------
+    owner
+        The configuration model instance.
+    mapping
+        The mapping to use.
+    route
+        The route to the item.
+    """
+
+    owner: ConfigModelT
+    mapping: dict[str, Any] | None
+    route: SupportsRoute
+
+    def get(self) -> Any:
+        """
+        Get the value of the item.
+
+        Returns
+        -------
+        The value of the item.
+        """
+        try:
+            scope = at(self.mapping or self.owner, self.route)
+        except KeyError as err:
+            route_here = err.args[1]
+            raise ConfigAccessError(self.owner, route_here) from None
+        return scope
+
+    def update(self, value: Any) -> Any:
+        """
+        Update the value of the item with regard to this item mapping.
+
+        Parameters
+        ----------
+        value
+            The new value.
+
+        Returns
+        -------
+        The updated mapping.
+        """
+        route = list(Route(self.route))
+        mapping = self.mapping or self.owner
+        key = route.pop()
+        scope = _get_object_dict(mapping)
+        route_here = []
+        try:
+            for part in route:
+                route_here.append(part)
+                scope = _get_object_dict(scope[part])
+            scope[key] = value
+        except KeyError:
+            raise ConfigAccessError(self.owner, route_here) from None
+        return mapping
+
+    async def save_async(self, **kwargs: Any) -> int:
+        """
+        Save the configuration asynchronously.
+
+        Parameters
+        ----------
+        **kwargs
+            Keyword arguments to pass to the saving function.
+
+        Returns
+        -------
+        The number of bytes written.
+        """
+        return await save_async(self, **kwargs)
+
+    def save(self, **kwargs: Any) -> int:
+        """
+        Save the configuration.
+
+        Parameters
+        ----------
+        **kwargs
+            Keyword arguments to pass to the saving function.
+
+        Returns
+        -------
+        The number of bytes written.
+        """
+        return save(self, **kwargs)
+
+    async def reload_async(self, **kwargs: Any) -> Any:
+        """
+        Reload the configuration asynchronously.
+
+        Parameters
+        ----------
+        kwargs
+            Keyword arguments to pass to the reloading function.
+
+        Returns
+        -------
+        The reloaded configuration or its belonging item.
+        """
+        return await reload_async(self, **kwargs)
+
+    def reload(self, **kwargs: Any) -> Any:
+        """
+        Reload the configuration.
+
+        Parameters
+        ----------
+        kwargs
+            Keyword arguments to pass to the reloading function.
+
+        Returns
+        -------
+        The reloaded configuration or its belonging item.
+        """
+        return reload(self, **kwargs)
+
+
+def save(
+    section: ConfigModelT | ConfigAt[ConfigModelT],
+    write_kwargs: dict[str, Any] | None = None,
+    **kwargs: Any,
+) -> int:
+    """
+    Save the configuration.
+
+    Parameters
+    ----------
+    section
+        The configuration model instance or the configuration item.
+    write_kwargs
+        Keyword arguments to pass to the writing function.
+    **kwargs
+        Keyword arguments to pass to the dumping function.
+
+    Returns
+    -------
+    The number of bytes written.
+    """
+    if isinstance(section, ConfigModel):
+        config = section
+        return config.save(write_kwargs=write_kwargs, **kwargs)
+
+    if write_kwargs is None:
+        write_kwargs = {}
+
+    config = section.owner
+    data = config.initial_state
+    scope = ConfigAt(config, data, section.route)
+    data = scope.update(section.get())
+    context = get_context(config)
+    blob = context.agent.dump_config(config.copy(update=data), **kwargs)
+    result = config.write(blob, **write_kwargs)
+    context.initial_state = data
+    return result
+
+
+async def save_async(
+    section: ConfigModelT | ConfigAt[ConfigModelT],
+    write_kwargs: dict[str, Any] | None = None,
+    **kwargs: Any,
+) -> int:
+    """
+    Save the configuration asynchronously.
+
+    Parameters
+    ----------
+    section
+        The configuration model instance or the configuration item.
+    write_kwargs
+        Keyword arguments to pass to the writing function.
+    **kwargs
+        Keyword arguments to pass to the dumping function.
+
+    Returns
+    -------
+    The number of bytes written.
+    """
+    if isinstance(section, ConfigModel):
+        config = section
+        return await config.save_async(write_kwargs=write_kwargs, **kwargs)
+
+    if write_kwargs is None:
+        write_kwargs = {}
+
+    config = section.owner
+    data = config.initial_state
+    scope = ConfigAt(config, data, section.route)
+    data = scope.update(section.get())
+    context = get_context(config)
+    blob = context.agent.dump_config(config.copy(update=data), **kwargs)
+    result = await config.write_async(blob, **write_kwargs)
+    context.initial_state = data
+    return result
+
+
+def reload(section: ConfigModelT | ConfigAt[ConfigModelT], **kwargs: Any) -> Any:
+    """
+    Reload the configuration.
+
+    Parameters
+    ----------
+    section
+        The configuration model instance or the configuration item.
+    **kwargs
+        Keyword arguments to pass to the reloading function.
+
+    Returns
+    -------
+    The reloaded configuration or its belonging item.
+    """
+    if isinstance(section, ConfigModel):
+        config = section
+        return config.reload()
+
+    config = section.owner
+    context = get_context(config)
+    state = config.__dict__
+    newest = context.agent.read(config_class=type(config), **kwargs)
+    section_data = ConfigAt(newest, newest.__dict__, section.route).get()
+    ConfigAt(config, state, section.route).update(section_data)
+    return section_data
+
+
+async def reload_async(
+    section: ConfigModelT | ConfigAt[ConfigModelT], **kwargs: Any
+) -> Any:
+    """
+    Reload the configuration asynchronously.
+
+    Parameters
+    ----------
+    section
+        The configuration model instance or the configuration item.
+    kwargs
+        Keyword arguments to pass to the reloading function.
+
+    Returns
+    -------
+    The reloaded configuration or its belonging item.
+    """
+    if isinstance(section, ConfigModel):
+        config = section
+        return await config.reload_async()
+
+    config = section.owner
+    context = get_context(config)
+    state = config.__dict__
+    newest = await context.agent.read_async(config_class=type(config), **kwargs)
+    section_data = ConfigAt(newest, newest.__dict__, section.route).get()
+    ConfigAt(config, state, section.route).update(section_data)
+    return section_data
+
+
+class BaseContext(abc.ABC, Generic[ConfigModelT]):
+    """
+    The base class for configuration context.
+    Contexts are used to
+    - store configuration resource information,
+    - link configuration items to the configuration models they belong to,
+    - keep track of the route leading to particular configuration
+      items that are also ConfigModel subclasses.
+
+    Attributes
+    ----------
+    initial_state
+        The initial configuration state.
+
+    """
+
+    initial_state: dict[str, Any]
+
+    @abc.abstractmethod
+    def trace_route(self) -> collections.abc.Iterator[str]:
+        """Trace the route to where the configuration subcontext points to."""
+
+    @property
+    def route(self) -> Route:
+        """The route to where the configuration subcontext points to."""
+        return Route(list(self.trace_route()))
+
+    @overload
+    def enter(self: BaseContext[ConfigModelT], part: None) -> BaseContext[ConfigModelT]:
+        ...
+
+    @overload
+    def enter(self, part: str) -> Subcontext[ConfigModelT]:
+        ...
+
+    def enter(
+        self, part: str | None
+    ) -> Subcontext[ConfigModelT] | BaseContext[ConfigModelT]:
+        """
+        Enter a subcontext.
+
+        Parameters
+        ----------
+        part
+            The name of the item nested in the item this context points to.
+
+        Returns
+        -------
+        The new subcontext.
+        """
+        if part is None:
+            return self
+        return Subcontext(self, part)
+
+    @property
+    @abc.abstractmethod
+    def agent(self) -> ConfigAgent[ConfigModelT]:
+        """The configuration agent responsible for loading and saving."""
+
+    @property
+    @abc.abstractmethod
+    def owner(self) -> ConfigModelT | None:
+        """
+        The top-level configuration model instance,
+        holding all adjacent contexts.
+        """
+
+    @property
+    @abc.abstractmethod
+    def at(self) -> ConfigModelT | ConfigAt[ConfigModelT] | None:
+        """
+        The configuration model instance or the configuration item
+        this context points to.
+        """
+
+
+class Context(BaseContext[ConfigModelT], Generic[ConfigModelT]):
+    """
+    The context of a configuration model.
+
+    Parameters
+    ----------
+    agent
+        The configuration resource agent.
+    owner
+        The top-level configuration model instance,
+        holding all belonging subcontexts.
+    """
+
+    _initial_state: dict[str, Any]
+
+    def __init__(
+        self,
+        agent: ConfigAgent[ConfigModelT],
+        owner: ConfigModelT | None = None,
+    ) -> None:
+        self._agent = agent
+        self._owner = None
+        self._initial_state = {}
+
+        self.owner = owner
+
+    def trace_route(self) -> collections.abc.Iterator[str]:
+        yield from ()
+
+    @property
+    def agent(self) -> ConfigAgent[ConfigModelT]:
+        return self._agent
+
+    @property
+    def at(self) -> ConfigModelT | None:
+        return self.owner
+
+    @property
+    def owner(self) -> ConfigModelT | None:
+        return self._owner
+
+    @owner.setter
+    def owner(self, config: ConfigModelT | None) -> None:
+        if config is None:
+            return
+        self._owner = config
+
+    @property
+    def initial_state(self) -> dict[str, Any]:
+        return copy.deepcopy(self._initial_state)
+
+    @initial_state.setter
+    def initial_state(self, initial_state: dict[str, Any]) -> None:
+        self._initial_state = copy.deepcopy(initial_state)
+
+    def __repr__(self) -> str:
+        agent = self.agent
+        return (
+            f"<{type(self).__name__} "
+            f"of {type(self.owner).__name__!r} configuration "
+            f"({agent=})>"
+        )
+
+
+class Subcontext(BaseContext[ConfigModelT], Generic[ConfigModelT]):
+    """
+    The subcontext of a configuration model.
+
+    Parameters
+    ----------
+    parent
+        The parent context.
+    part
+        The name of the item nested in the item the parent context points to.
+    """
+
+    def __init__(self, parent: BaseContext[ConfigModelT], part: str) -> None:
+        self._parent = parent
+        self._part = part
+
+    @property
+    def agent(self) -> ConfigAgent[ConfigModelT]:
+        return self._parent.agent
+
+    def trace_route(self) -> collections.abc.Iterator[str]:
+        yield from self._parent.trace_route()
+        yield self._part
+
+    @property
+    def at(self) -> ConfigAt[ConfigModelT]:
+        if self.owner is None:
+            msg = "Cannot get section pointed to by an unbound context"
+            raise ValueError(msg)
+        return ConfigAt(self.owner, None, self.route)
+
+    @property
+    def owner(self) -> ConfigModelT | None:
+        return self._parent.owner
+
+    @property
+    def initial_state(self) -> dict[str, Any]:
+        return self._parent.initial_state
+
+    @initial_state.setter
+    def initial_state(self, value: dict[str, Any]) -> None:
+        data = self._parent.initial_state
+        data[self._part] = copy.deepcopy(value)
+        self._parent.initial_state = data
+
+    def __repr__(self) -> str:
+        agent = self.agent
+        route = self.route
+        return (
+            f"<{type(self).__name__} "
+            f"of {type(self.owner).__name__ + '.' + str(route)!r} configuration "
+            f"({agent=})>"
+        )
+
+
+def get_context(config: ConfigModelT) -> BaseContext[ConfigModelT]:
+    """
+    Get the context of the configuration model.
+
+    Parameters
+    ----------
+    config
+        The configuration model instance.
+
+    Returns
+    -------
+    The context of the configuration model.
+    """
+    context = get_context_or_none(config)
+    if context is None:
+        raise RuntimeError("Cannot get context of unbound configuration model")
+    return context
+
+
+def get_context_or_none(config: ConfigModelT) -> BaseContext[ConfigModelT] | None:
+    """
+    Get the context of the configuration model safely.
+
+    Parameters
+    ----------
+    config
+        The configuration model instance.
+
+    Returns
+    -------
+    The context of the configuration model.
+    """
+    return cast(
+        Optional[BaseContext[ConfigModelT]], getattr(config, LOCAL).get(current_context)
+    )
+
+
+def _json_encoder(
+    model_encoder: collections.abc.Callable[..., Any], value: Any, **kwargs: Any
+) -> Any:
+    initial_state_type = type(value)
+    converted_value = pre_serialize(value)
+    if isinstance(converted_value, initial_state_type):
+        return model_encoder(value, **kwargs)
+    return converted_value
+
+
+class ConfigModelMetaclass(ModelMetaclass):
+    def __new__(
+        cls,
+        name: str,
+        bases: tuple[type, ...],
+        namespace: dict[str, Any],
+        **kwargs: Any,
+    ) -> type:
+        namespace |= dict.fromkeys(
+            (EXPORT, CONTEXT, LOCAL, TOKEN), pydantic.PrivateAttr()
+        )
+
+        if kwargs.pop("root", None):
+            return type.__new__(cls, name, bases, namespace, **kwargs)
+
+        new_class = super().__new__(cls, name, bases, namespace, **kwargs)
+        for field in new_class.__fields__.values():
+            if type(field.outer_type_) is ConfigModelMetaclass:
+                if field.pre_validators is None:
+                    field.pre_validators = []
+                validator = make_generic_validator(
+                    field.outer_type_.__field_setup__  # type: ignore[attr-defined]
+                )
+                field.pre_validators.insert(0, validator)
+        new_class.__json_encoder__ = functools.partial(
+            _json_encoder,
+            new_class.__json_encoder__,
+        )
+        return cast(type, new_class)
+
+
+class ConfigModel(
+    pydantic.BaseSettings,
+    metaclass=ConfigModelMetaclass,
+    root=True,
+):
+    """
+    The base class for configuration models.
+
+    It is not recommended to inherit from this class directly for basic usage.
+    Instead, use either :class:`ConfigModel` or :class:`AsyncConfigModel`.
+    """
+
+    def __init__(self, **kwargs: Any) -> None:
+        # Set private attributes via the constructor
+        # to allow preprocessor-related instances to exist.
+        missing = object()
+        for private_attr in self.__private_attributes__:
+            value = kwargs.pop(private_attr, missing)
+            if value is not missing:
+                setattr(self, private_attr, value)
+                if private_attr == CONTEXT:
+                    current_context.set(value)
+        super().__init__(**kwargs)
+
+    def _init_private_attributes(self) -> None:
+        super()._init_private_attributes()
+        local = contextvars.copy_context()
+        setattr(self, LOCAL, local)
+        tok = getattr(self, TOKEN, None)
+        if tok:
+            current_context.reset(tok)
+
+    def export(self, **kwargs: Any) -> dict[str, Any]:
+        """
+        Export the configuration model.
+
+        Returns
+        -------
+        The exported configuration model.
+        """
+        tok = _exporting.set(True)  # noqa: FBT003
+        ctx = contextvars.copy_context()
+        _exporting.reset(tok)
+        return ctx.run(self.dict, **kwargs)
+
+    async def export_async(self, **kwargs: Any) -> dict[str, Any]:
+        """
+        Export the configuration model.
+
+        Returns
+        -------
+        The exported configuration model.
+        """
+        tok = _exporting.set(True)  # noqa: FBT003
+        task = asyncio.create_task(self.dict_async(**kwargs))
+        _exporting.reset(tok)
+        return await task
+
+    async def dict_async(self, **kwargs: Any) -> dict[str, Any]:
+        """
+        Get the dictionary representation of the configuration model.
+
+        Returns
+        -------
+        The dictionary representation of the configuration model.
+        """
+        return dict(await self._iter_async(to_dict=True, **kwargs))
+
+    async def json_async(  # noqa: PLR0913
+        self,
+        include: IncludeExcludeT = None,
+        exclude: IncludeExcludeT = None,
+        *,
+        by_alias: bool = False,
+        exclude_unset: bool = False,
+        exclude_defaults: bool = False,
+        exclude_none: bool = False,
+        encoder: collections.abc.Callable[[Any], Any] | None = None,
+        models_as_dict: bool = True,
+        **dumps_kwargs: Any,
+    ) -> str:
+        encoder = cast(
+            collections.abc.Callable[[Any], Any], encoder or self.__json_encoder__
+        )
+        data = dict(
+            await self._iter_async(
+                to_dict=models_as_dict,
+                by_alias=by_alias,
+                include=include,
+                exclude=exclude,
+                exclude_unset=exclude_unset,
+                exclude_defaults=exclude_defaults,
+                exclude_none=exclude_none,
+            )
+        )
+        if self.__custom_root_type__:
+            data = data[ROOT_KEY]
+        return self.__config__.json_dumps(data, default=encoder, **dumps_kwargs)
+
+    def _iter(  # type: ignore[override]
+        self, **kwargs: Any
+    ) -> collections.abc.Iterator[tuple[str, Any]]:
+        if kwargs.get("to_dict", False) and _exporting.get():
+            state = {}
+            for key, value in super()._iter(**kwargs):
+                state[key] = value
+            metadata = getattr(self, EXPORT, None)
+            if metadata:
+                context = get_context(self)
+                context.agent.processor_class.export(state, metadata=metadata)
+            yield from state.items()
+        else:
+            yield from super()._iter(**kwargs)
+
+    async def _iter_async(
+        self, **kwargs: Any
+    ) -> collections.abc.Iterator[tuple[str, Any]]:
+        if kwargs.get("to_dict", False) and _exporting.get():
+            state = {}
+            for key, value in super()._iter(**kwargs):
+                state[key] = value
+            metadata = getattr(self, EXPORT, None)
+            if metadata:
+                context = get_context(self)
+                await context.agent.processor_class.export_async(
+                    state, metadata=metadata
+                )
+            return ((key, value) for key, value in state.items())
+        return super()._iter(**kwargs)
+
+    @classmethod
+    @no_type_check
+    def _get_value(cls, value: Any, *, to_dict: bool, **kwds: Any) -> Any:
+        if _exporting.get():
+            exporter = export.dispatch(type(value))
+            if (
+                isinstance(value, BaseModel) or exporter != export.dispatch(object)
+            ) and to_dict:
+                value_dict = export(value, **kwds)
+                if ROOT_KEY in value_dict:
+                    return value_dict[ROOT_KEY]
+                return value_dict
+        return super()._get_value(value, to_dict=to_dict, **kwds)
+
+    @classmethod
+    def _resolve_agent(
+        cls,
+        resource: ConfigAgent[ConfigModelT] | RawResourceT | None = None,
+        *,
+        create_if_missing: bool | None = None,
+        ac_parser: str | None = None,
+    ) -> ConfigAgent[ConfigModelT]:
+        if resource is None:
+            resource = getattr(cls.__config__, "resource", None)
+        if resource is None:
+            raise ValueError("No resource specified")
+        if ac_parser is None:
+            ac_parser = getattr(cls.__config__, "ac_parser", None)
+        agent: ConfigAgent[ConfigModelT]
+        if isinstance(resource, ConfigAgent):
+            agent = resource
+        else:
+            agent = ConfigAgent(
+                resource,
+                ac_parser=ac_parser,
+            )
+        if create_if_missing is not None:
+            agent.create_if_missing = create_if_missing
+        if ac_parser is not None:
+            agent.ac_parser = cast(str, ac_parser)
+        return agent
+
+    @property
+    def initial_state(self) -> dict[str, Any]:
+        """
+        The initial configuration state.
+
+        It is a copy of the configuration state
+        at the last time of loading, reloading or saving.
+        """
+        return get_context(self).initial_state
+
+    def at(
+        self: ConfigModelT,
+        route: SupportsRoute,
+    ) -> ConfigAt[ConfigModelT]:
+        """
+        Lazily point to a specific item in the configuration.
+
+        Parameters
+        ----------
+        route
+            The access route to the item in this configuration.
+
+        Returns
+        -------
+        The configuration accessor.
+        """
+        return ConfigAt(self, None, route)
+
+    def update(self, **kwargs: Any) -> None:
+        """
+        Update the configuration with new values, in-place.
+
+        Parameters
+        ----------
+        kwargs
+            The new values to update the configuration with.
+
+        Returns
+        -------
+        None
+        """
+        # Crucial difference to self.__dict__.update():
+        # self.__dict__.update() would not trigger the validation
+        # of the new values.
+        for key, value in kwargs.items():
+            setattr(self, key, value)
+
+    def rollback(self) -> None:
+        """
+        Rollback the configuration to its initial state.
+
+        Returns
+        -------
+        None
+        """
+        context = get_context(self)
+        self.__dict__.update(context.initial_state)
+
+    def __deepcopy__(
+        self: ConfigModelT, memodict: dict[Any, Any] | None = None
+    ) -> ConfigModelT:
+        state = dict(self._iter(to_dict=False))
+        state.pop(LOCAL, None)
+        state.pop(TOKEN, None)
+        return type(self)(**copy.deepcopy(state))
+
+    @classmethod
+    def load(
+        cls: type[ConfigModelT],
+        resource: ConfigAgent[ConfigModelT] | RawResourceT | None = None,
+        *,
+        create_if_missing: bool | None = None,
+        ac_parser: str | None = None,
+        **kwargs: Any,
+    ) -> ConfigModelT:
+        """
+        Load the configuration file.
+        To reload the configuration, use the `reload()` method.
+
+        Parameters
+        ----------
+        resource
+            The configuration resource to read from/write to.
+        ac_parser
+            The anyconfig parser to use.
+        create_if_missing
+            Whether to create the configuration file if it does not exist.
+        **kwargs
+            Keyword arguments to pass to the read method.
+
+        Returns
+        -------
+        self
+        """
+        agent = cls._resolve_agent(
+            resource,
+            ac_parser=ac_parser,
+            create_if_missing=create_if_missing,
+        )
+        context = Context(agent)  # type: Context[ConfigModelT]
+        current_context.set(context)
+        local = contextvars.copy_context()
+        if getattr(
+            cls.__config__,
+            "autoupdate_forward_refs",
+            ConfigMeta.autoupdate_forward_refs,
+        ):
+            cls.update_forward_refs()
+        config = agent.read(config_class=cls, **kwargs)
+        setattr(config, LOCAL, local)
+        context.owner = config
+        context.initial_state = config.__dict__
+        return config
+
+    def reload(self: ConfigModelT, **kwargs: Any) -> ConfigModelT:
+        """
+        Reload the configuration file.
+
+        Parameters
+        ----------
+        **kwargs
+            Keyword arguments to pass to the read method.
+
+        Returns
+        -------
+        self
+        """
+        context = get_context(self)
+        tok = current_context.set(get_context(context.owner))
+        if context.owner is self:
+            changed = context.agent.read(config_class=type(self), **kwargs)
+        else:
+            changed = reload(cast(ConfigAt[ConfigModelT], context.at), **kwargs)
+        current_context.reset(tok)
+        state = changed.__dict__
+        context.initial_state = state
+        self.update(**state)
+        return self
+
+    def save(
+        self: ConfigModelT, write_kwargs: dict[str, Any] | None = None, **kwargs: Any
+    ) -> int:
+        """
+        Save the configuration to the configuration file.
+
+        Parameters
+        ----------
+        write_kwargs
+            Keyword arguments to pass to the write method.
+        **kwargs
+            Keyword arguments to pass to the dumping method.
+
+        Returns
+        -------
+        The number of bytes written.
+        """
+        context = get_context(self)
+        if context.owner is self:
+            if write_kwargs is None:
+                write_kwargs = {}
+            blob = context.agent.dump_config(self, **kwargs)
+            result = self.write(blob, **write_kwargs)
+            context.initial_state = self.__dict__
+            return result
+        return save(
+            cast(ConfigAt[ConfigModelT], context.at),
+            write_kwargs=write_kwargs,
+            **kwargs,
+        )
+
+    def write(self, blob: str, **kwargs: Any) -> int:
+        """
+        Overwrite the configuration file with the given string or bytes.
+
+        Parameters
+        ----------
+        blob
+            The blob to write to the configuration file.
+        **kwargs
+            Keyword arguments to pass to the open method.
+
+        Returns
+        -------
+        The number of bytes written.
+        """
+        context = get_context(self)
+        if context.agent.is_url:
+            msg = "Writing to URLs is not yet supported"
+            raise NotImplementedError(msg)
+        return context.agent.write(blob, **kwargs)
+
+    @classmethod
+    async def load_async(
+        cls: type[ConfigModelT],
+        resource: ConfigAgent[ConfigModelT] | RawResourceT | None = None,
+        *,
+        ac_parser: str | None = None,
+        create_if_missing: bool | None = None,
+        **kwargs: Any,
+    ) -> ConfigModelT:
+        """
+        Load the configuration file asynchronously.
+        To reload the configuration, use the `reload_async()` method.
+
+        Parameters
+        ----------
+        resource
+            The configuration resource.
+        ac_parser
+            The anyconfig parser to use.
+        create_if_missing
+            Whether to create the configuration file if it does not exist.
+        **kwargs
+            Keyword arguments to pass to the read method.
+
+        Returns
+        -------
+        self
+        """
+        agent = cls._resolve_agent(
+            resource, create_if_missing=create_if_missing, ac_parser=ac_parser
+        )
+        context = Context(agent)  # type: Context[ConfigModelT]
+        current_context.set(context)
+        local = contextvars.copy_context()
+        if getattr(
+            cls.__config__,
+            "autoupdate_forward_refs",
+            ConfigMeta.autoupdate_forward_refs,
+        ):
+            cls.update_forward_refs()
+        config = await agent.read_async(config_class=cls, **kwargs)
+        setattr(config, LOCAL, local)
+        context.owner = config
+        return config
+
+    async def reload_async(self: ConfigModelT, **kwargs: Any) -> ConfigModelT:
+        """
+        Reload the configuration file asynchronously.
+
+        Parameters
+        ----------
+        **kwargs
+            Keyword arguments to pass to the read method.
+
+        Returns
+        -------
+        self
+        """
+        context = get_context(self)
+        tok = current_context.set(get_context(context.owner))
+        if context.owner is self:
+            changed = await context.agent.read_async(config_class=type(self), **kwargs)
+        else:
+            changed = await reload_async(
+                cast(ConfigAt[ConfigModelT], context.at), **kwargs
+            )
+        current_context.reset(tok)
+        state = changed.__dict__
+        context.initial_state = state
+        self.update(**state)
+        return self
+
+    async def save_async(
+        self: ConfigModelT, write_kwargs: dict[str, Any] | None = None, **kwargs: Any
+    ) -> int:
+        """
+        Save the configuration to the configuration file asynchronously.
+
+        Parameters
+        ----------
+        write_kwargs
+            Keyword arguments to pass to the write method.
+        **kwargs
+            Keyword arguments to pass to the dumping method.
+
+        Returns
+        -------
+        The number of bytes written.
+        """
+        context = get_context(self)
+        if context.owner is self:
+            if write_kwargs is None:
+                write_kwargs = {}
+            tok = _exporting.set(True)  # noqa: FBT003
+            task = asyncio.create_task(context.agent.dump_config_async(self, **kwargs))
+            _exporting.reset(tok)
+            blob = await task
+            result = await self.write_async(blob, **write_kwargs)
+            context.initial_state = self.__dict__
+            return result
+        return await save_async(
+            cast(ConfigAt[ConfigModelT], context.at),
+            write_kwargs=write_kwargs,
+            **kwargs,
+        )
+
+    async def write_async(self, blob: str, **kwargs: Any) -> int:
+        """
+        Overwrite the configuration file asynchronously with the given string or bytes.
+
+        Parameters
+        ----------
+        blob
+            The blob to write to the configuration file.
+        **kwargs
+            Keyword arguments to pass to the open method.
+
+        Returns
+        -------
+        The number of bytes written.
+        """
+        context = get_context(self)
+        if context.agent.is_url:
+            msg = "Saving to URLs is not yet supported"
+            raise NotImplementedError(msg)
+        return await context.agent.write_async(blob, **kwargs)
+
+    @classmethod
+    def __field_setup__(cls, value: Any, field: ModelField) -> Any:
+        """
+        Called when this configuration model is being initialized as a field
+        of some other configuration model.
+        """
+        context = current_context.get()
+        if context is not None:
+            subcontext = context.enter(field.name)
+            tok = current_context.set(subcontext)
+            vs = _get_object_dict(value)
+            vs[TOKEN] = tok
+            vs[LOCAL] = contextvars.copy_context()
+        return value
+
+
+class ConfigMeta(pydantic.BaseSettings.Config):
+    """
+    Meta-configuration for the `ConfigModel` class.
+
+    Attributes
+    ----------
+    resource
+        The configuration resource to read from/write to.
+
+        If a string, it will be interpreted as a path to a file.
+
+    ac_parser
+        The anyconfig parser to use.
+
+    autoupdate_forward_refs
+        Whether to automatically update forward references
+        when `ConfigModel.load()` or `ConfigModel.load_async()`
+        methods are called. For convenience, defaults to `True`.
+
+    And all other attributes from `pydantic.BaseSettings.Config`.
+    """
+
+    resource: ConfigAgent[ConfigModel] | RawResourceT | None = None
+    ac_parser: str | None = None
+    validate_assignment: bool = True
+    autoupdate_forward_refs: bool = True
+
+    Extra = pydantic.Extra
```

### Comparing `configzen-0.3.0/configzen/errors.py` & `configzen-0.3.1/configzen/errors.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,112 +1,111 @@
-"""This module contains all the custom errors raised by _configzen_."""
-
-from __future__ import annotations
-
-import collections.abc
-import contextlib
-from typing import TYPE_CHECKING, Any
-
-
-if TYPE_CHECKING:
-    from configzen.config import ConfigAgent
-    from configzen.typedefs import ConfigModelT
-
-
-class ConfigError(Exception):
-    """An error occurred while loading a configuration."""
-
-
-class IncorrectConfigError(ConfigError):
-    """An error occurred while loading a configuration."""
-
-
-class InternalSyntaxError(ConfigError):
-    """Error in route syntax."""
-
-    def __init__(
-        self,
-        msg: str,
-        index: Any = None,
-        prefix: str = "",
-        suffix: str = "",
-    ) -> None:
-        super().__init__(msg)
-        self.index = index
-        self.prefix = prefix
-        self.suffix = suffix
-
-
-class ConfigSyntaxError(ConfigError):
-    """An error occurred while parsing arguments."""
-
-
-@contextlib.contextmanager
-def formatted_syntax_error(source: str) -> collections.abc.Iterator[None]:
-    """Raise a SyntaxError with a message and a source."""
-    try:
-        yield
-    except InternalSyntaxError as exc:
-        idx = len(exc.prefix) + exc.index + 1
-        charlist = [" "] * len(exc.prefix + repr(source) + exc.suffix)
-        charlist[idx] = "^"
-        indicator = "".join(charlist)
-        msg = "\n".join(
-            map(str, (exc, exc.prefix + repr(source) + exc.suffix, indicator))
-        )
-        raise ConfigSyntaxError(msg) from None
-
-
-class UnspecifiedParserError(ConfigError):
-    """Could not determine the parser to use."""
-
-
-class UnavailableParserError(ConfigError):
-    MISSING_DEPENDENCIES: dict[str, str] = {
-        "yaml": "pyyaml (or ruamel.yaml)",
-        "toml": "toml",
-        "ion": "anyconfig-ion-backend",
-        "bson": "anyconfig-bson-backend",
-        "msgpack": "anyconfig-msgpack-backend",
-        "cbor": "anyconfig-cbor-backend (or anyconfig-cbor2-backend)",
-        "configobj": "anyconfig-configobj-backend",
-    }
-
-    def __init__(self, parser_name: str, agent: ConfigAgent[ConfigModelT]) -> None:
-        missing_dependency: str = self.MISSING_DEPENDENCIES.get(
-            parser_name, f"the proper anyconfig backend for {parser_name} files"
-        )
-        super().__init__(
-            f"The {parser_name!r} parser required to load configuration "
-            f"for agent {agent} is not available.\n"
-            f"Install it with `pip install {missing_dependency}`."
-        )
-
-
-class ConfigAccessError(ConfigError, LookupError):
-    """An error occurred while accessing configuration part."""
-
-    def __init__(self, config: ConfigModelT, route: str | list[str]) -> None:
-        if not isinstance(route, str):
-            route = ".".join(route)
-        self.route = route
-        super().__init__(
-            f"could not get {type(config).__name__}.{route}",
-        )
-
-
-class ConfigProcessorError(ConfigError):
-    """An error occurred while preprocessing/exporting a configuration."""
-
-
-class ResourceLookupError(ConfigError, LookupError):
-    """An error occurred while looking up a resource."""
-
-    def __init__(
-        self, resource: ConfigAgent[ConfigModelT] | None, route: list[str]
-    ) -> None:
-        resource_name = resource.resource if resource else "the provided resource"
-        super().__init__(f"{route} not found in {resource_name}")
-
-
-class ConfigPreprocessingError(ConfigProcessorError, ValueError):
-    """An error occurred while preprocessing a configuration value."""
+"""This module contains all the custom errors raised by _configzen_."""
+
+from __future__ import annotations
+
+import collections.abc
+import contextlib
+from typing import TYPE_CHECKING, Any
+
+if TYPE_CHECKING:
+    from configzen.config import ConfigAgent
+    from configzen.typedefs import ConfigModelT
+
+
+class ConfigError(Exception):
+    """An error occurred while loading a configuration."""
+
+
+class IncorrectConfigError(ConfigError):
+    """An error occurred while loading a configuration."""
+
+
+class InternalSyntaxError(ConfigError):
+    """Error in route syntax."""
+
+    def __init__(
+        self,
+        msg: str,
+        index: Any = None,
+        prefix: str = "",
+        suffix: str = "",
+    ) -> None:
+        super().__init__(msg)
+        self.index = index
+        self.prefix = prefix
+        self.suffix = suffix
+
+
+class ConfigSyntaxError(ConfigError):
+    """An error occurred while parsing arguments."""
+
+
+@contextlib.contextmanager
+def formatted_syntax_error(source: str) -> collections.abc.Iterator[None]:
+    """Raise a SyntaxError with a message and a source."""
+    try:
+        yield
+    except InternalSyntaxError as exc:
+        idx = len(exc.prefix) + exc.index + 1
+        charlist = [" "] * len(exc.prefix + repr(source) + exc.suffix)
+        charlist[idx] = "^"
+        indicator = "".join(charlist)
+        msg = "\n".join(
+            map(str, (exc, exc.prefix + repr(source) + exc.suffix, indicator))
+        )
+        raise ConfigSyntaxError(msg) from None
+
+
+class UnspecifiedParserError(ConfigError):
+    """Could not determine the parser to use."""
+
+
+class UnavailableParserError(ConfigError):
+    MISSING_DEPENDENCIES: dict[str, str] = {
+        "yaml": "pyyaml (or ruamel.yaml)",
+        "toml": "toml",
+        "ion": "anyconfig-ion-backend",
+        "bson": "anyconfig-bson-backend",
+        "msgpack": "anyconfig-msgpack-backend",
+        "cbor": "anyconfig-cbor-backend (or anyconfig-cbor2-backend)",
+        "configobj": "anyconfig-configobj-backend",
+    }
+
+    def __init__(self, parser_name: str, agent: ConfigAgent[ConfigModelT]) -> None:
+        missing_dependency: str = self.MISSING_DEPENDENCIES.get(
+            parser_name, f"the proper anyconfig backend for {parser_name} files"
+        )
+        super().__init__(
+            f"The {parser_name!r} parser required to load configuration "
+            f"for agent {agent} is not available.\n"
+            f"Install it with `pip install {missing_dependency}`."
+        )
+
+
+class ConfigAccessError(ConfigError, LookupError):
+    """An error occurred while accessing configuration part."""
+
+    def __init__(self, config: ConfigModelT, route: str | list[str]) -> None:
+        if not isinstance(route, str):
+            route = ".".join(route)
+        self.route = route
+        super().__init__(
+            f"could not get {type(config).__name__}.{route}",
+        )
+
+
+class ConfigProcessorError(ConfigError):
+    """An error occurred while preprocessing/exporting a configuration."""
+
+
+class ResourceLookupError(ConfigError, LookupError):
+    """An error occurred while looking up a resource."""
+
+    def __init__(
+        self, resource: ConfigAgent[ConfigModelT] | None, route: list[str]
+    ) -> None:
+        resource_name = resource.resource if resource else "the provided resource"
+        super().__init__(f"{route} not found in {resource_name}")
+
+
+class ConfigPreprocessingError(ConfigProcessorError, ValueError):
+    """An error occurred while preprocessing a configuration value."""
```

### Comparing `configzen-0.3.0/configzen/processor.py` & `configzen-0.3.1/configzen/processor.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,842 +1,839 @@
-from __future__ import annotations
-
-import asyncio
-import copy
-import dataclasses
-import enum
-import pathlib
-from collections.abc import Callable
-from typing import TYPE_CHECKING, Any, ClassVar, Generic, TypedDict, TypeVar, cast
-
-from anyconfig.utils import is_dict_like, is_list_like
-
-from configzen.errors import (
-    ConfigPreprocessingError,
-)
-from configzen.typedefs import ConfigModelT, SupportsRoute
-
-if TYPE_CHECKING:
-    from configzen.config import BaseContext, ConfigAgent
-
-__all__ = (
-    "DirectiveContext",
-    "directive",
-    "Processor",
-)
-
-
-DirectiveT = TypeVar("DirectiveT")
-
-EXPORT: str = "__configzen_export__"
-EXECUTES_DIRECTIVES: str = "__configzen_executes_directives__"
-EXECUTES_DIRECTIVES_ASYNC: str = "__configzen_executes_directives_async__"
-
-
-def directive(
-    name: str | enum.Enum,
-    *,
-    asynchronous: bool | None = None,
-) -> Callable[..., Any]:
-    """
-    Decorator for creating processor directives.
-
-    Parameters
-    ----------
-    name
-        The name of the directive.
-    asynchronous
-        Whether the decorated directive function is asynchronous.
-
-    Returns
-    -------
-    The decorated function.
-    """
-    if isinstance(name, enum.Enum):
-        name = name.value.casefold()
-
-    def decorator(func: Any) -> Any:
-        nonlocal asynchronous
-        if asynchronous is None:
-            asynchronous = asyncio.iscoroutinefunction(func)
-        attr = EXECUTES_DIRECTIVES_ASYNC if asynchronous else EXECUTES_DIRECTIVES
-        if not hasattr(func, attr):
-            setattr(func, attr, set())
-        getattr(func, attr).add(name)
-        return func
-
-    return decorator
-
-
-@dataclasses.dataclass
-class DirectiveContext:
-    """
-    Context for processor directives.
-
-    Attributes
-    ----------
-    directive
-        The directive.
-    key
-        The key of the directive.
-    prefix
-        The prefix of the directive.
-    arguments
-        The arguments of the directive.
-    snippet
-        The config snippet where this directive was invoked.
-    container
-        The dictionary that contains the :attr:`dict`.
-
-    """
-
-    directive: str
-    key: str
-    prefix: str
-    snippet: dict[str, Any]
-    container: dict[str, Any]
-
-
-def parse_directive_call(
-    prefix: str,
-    directive_name: str,
-) -> str:
-    if directive_name.startswith(prefix):
-        directive_name = directive_name[len(prefix) :].casefold()
-
-        if not directive_name.isidentifier():
-            msg = f"Invalid directive name: {directive_name}"
-            raise ConfigPreprocessingError(msg)
-
-    return directive_name
-
-
-if TYPE_CHECKING:
-
-    class ExportMetadata(TypedDict, Generic[ConfigModelT]):
-        route: str | None
-        context: BaseContext[ConfigModelT]
-        key_order: list[str]
-        preprocess: bool
-
-else:
-
-    class ExportMetadata(TypedDict):
-        """
-        Metadata for exporting.
-
-        Attributes
-        ----------
-        route
-            The route to import from.
-        context
-            The context attached to the import.
-        """
-
-        route: str | None
-        context: BaseContext[ConfigModelT]
-        key_order: list[str]
-        preprocess: bool
-
-
-class BaseProcessor(Generic[ConfigModelT]):
-    """
-    Processor that executes directives.
-
-    Attributes
-    ----------
-    dict_config
-        The dictionary config to parse and update.
-    directive_prefix
-        The prefix for directives.
-    """
-
-    _directive_handlers: dict[str, Any] = None  # type: ignore[assignment]
-    _async_directive_handlers: dict[str, Any] = None  # type: ignore[assignment]
-    directive_prefix: ClassVar[str]
-    extension_prefix: ClassVar[str]
-
-    def __init__(
-        self,
-        agent: ConfigAgent[ConfigModelT],
-        dict_config: dict[str, Any],
-    ) -> None:
-        self.agent = agent
-        self.dict_config = dict_config
-
-    @classmethod
-    def export(
-        cls,
-        state: Any,
-        *,
-        metadata: ExportMetadata[ConfigModelT] | None = None,
-    ) -> None:
-        """
-        Export the state.
-
-        Parameters
-        ----------
-        state
-            The state to export.
-        metadata
-            The metadata of the substitution.
-        """
-        if is_dict_like(state):
-            if metadata is None:
-                from configzen.config import CONTEXT
-
-                state.pop(CONTEXT, None)
-                metadata = state.pop(EXPORT, None)
-            if metadata:
-                cls._export(state, metadata)
-            else:
-                cls.export(list(state.values()), metadata=None)
-        elif is_list_like(state):
-            for item in state:
-                cls.export(item, metadata=None)
-
-    @classmethod
-    async def export_async(
-        cls,
-        state: Any,
-        *,
-        metadata: ExportMetadata[ConfigModelT] | None = None,
-    ) -> None:
-        """
-        Export the state asynchronously.
-
-        Parameters
-        ----------
-        state
-            The state to export.
-        metadata
-            The metadata of the substitution.
-        """
-        if is_dict_like(state):
-            if metadata is None:
-                from configzen.config import CONTEXT
-
-                state.pop(CONTEXT, None)
-                metadata = state.pop(EXPORT, None)
-            if metadata:
-                await cls._export_async(state, metadata)
-            else:
-                await cls.export_async(list(state.values()), metadata=None)
-        elif is_list_like(state):
-            for item in state:
-                await cls.export_async(item, metadata=None)
-
-    @classmethod
-    def _export(
-        cls,
-        state: Any,
-        metadata: ExportMetadata[ConfigModelT],
-    ) -> None:
-        raise NotImplementedError
-
-    @classmethod
-    async def _export_async(
-        cls,
-        state: Any,
-        metadata: ExportMetadata[ConfigModelT],
-    ) -> None:
-        raise NotImplementedError
-
-    async def preprocess_async(self) -> dict[str, Any]:
-        """
-        Parse the dictionary config and return the parsed config,
-        ready for instantiating the model.
-
-        Returns
-        -------
-        The parsed config.
-        """
-        return cast(dict[str, Any], await self._preprocess_async(self.dict_config))
-
-    def preprocess(self) -> dict[str, Any]:
-        """
-        Parse the dictionary config and return the parsed config,
-        ready for instantiating the model.
-
-        Returns
-        -------
-        The parsed config.
-        """
-        return cast(dict[str, Any], self._preprocess(self.dict_config))
-
-    def _preprocess(self, container: Any) -> Any:
-        if not is_dict_like(container):
-            if is_list_like(container):
-                return [self._preprocess(v) for v in container]
-            return container
-
-        result: dict[str, Any] = {}
-
-        for key, value in sorted(
-            cast(dict[str, Any], container).items(),
-            key=lambda item: item[0] == self.directive_prefix,
-        ):
-            if key.startswith(self.extension_prefix):
-                actual_key = key.lstrip(self.extension_prefix)
-                overridden = result.get(actual_key, {})
-                if not is_dict_like(overridden):
-                    raise ConfigPreprocessingError(
-                        f"{self.extension_prefix} can be used only for overriding "
-                        f"dictionary sections but item at {actual_key!r} "
-                        f"is not a dictionary"
-                    )
-                replacement = overridden | value
-                result[actual_key] = self._preprocess(replacement)
-            elif key.startswith(self.directive_prefix):
-                directive_name = parse_directive_call(self.directive_prefix, key)
-                context_container = container.copy()
-                del context_container[key]
-                context = DirectiveContext(
-                    directive=directive_name,
-                    key=key,
-                    prefix=self.directive_prefix,
-                    snippet=value,
-                    container=context_container,
-                )
-                self._call_directive(context)
-                new_container = self._preprocess(context.container)
-                result |= new_container
-            else:
-                result[key] = self._preprocess(value)
-        return result
-
-    async def _preprocess_async(self, container: Any) -> Any:
-        if not is_dict_like(container):
-            if is_list_like(container):
-                return [await self._preprocess_async(v) for v in container]
-            return container
-
-        result: dict[str, Any] = {}
-
-        for key, value in sorted(
-            cast(dict[str, Any], container).items(),
-            key=lambda item: item[0] == self.directive_prefix,
-        ):
-            if key.startswith(self.extension_prefix):
-                actual_key = key.lstrip(self.extension_prefix)
-                overridden = result.get(actual_key, {})
-                if not is_dict_like(overridden):
-                    raise ConfigPreprocessingError(
-                        f"{self.extension_prefix} can be used only for overriding "
-                        f"dictionary sections but item at {actual_key!r} "
-                        f"is not a dictionary"
-                    )
-                replacement = overridden | value
-                result[actual_key] = await self._preprocess_async(replacement)
-            elif key.startswith(self.directive_prefix):
-                directive_name = parse_directive_call(self.directive_prefix, key)
-                context_container = container.copy()
-                del context_container[key]
-                context = DirectiveContext(
-                    directive=directive_name,
-                    key=key,
-                    prefix=self.directive_prefix,
-                    snippet=value,
-                    container=context_container,
-                )
-                await self._call_directive_async(context)
-                new_container = await self._preprocess_async(context.container)
-                result |= new_container
-            else:
-                result[key] = await self._preprocess_async(value)
-        return result
-
-    def _call_directive(self, context: DirectiveContext) -> None:
-        handler = self._directive_handlers.get(context.directive)
-        if handler is None:
-            raise ConfigPreprocessingError(
-                f"unknown preprocessing directive: {context.directive!r}"
-            )
-        handler(self, context)
-
-    async def _call_directive_async(self, context: DirectiveContext) -> None:
-        handler = self._async_directive_handlers.get(context.directive)
-        if handler is None:
-            raise ConfigPreprocessingError(
-                f"unknown preprocessing directive: {context.directive!r}"
-            )
-        await handler(self, context)
-
-    def __init_subclass__(cls, **kwargs: Any) -> None:
-        super().__init_subclass__(**kwargs)
-        if cls._directive_handlers is None:
-            cls._directive_handlers = {}
-        else:
-            cls._directive_handlers = cls._directive_handlers.copy()
-        if cls._async_directive_handlers is None:
-            cls._async_directive_handlers = {}
-        else:
-            cls._async_directive_handlers = cls._async_directive_handlers.copy()
-        for _name, func in cls.__dict__.items():
-            if hasattr(func, EXECUTES_DIRECTIVES):
-                for directive_name in getattr(func, EXECUTES_DIRECTIVES):
-                    cls._directive_handlers[directive_name] = func
-            elif hasattr(func, EXECUTES_DIRECTIVES_ASYNC):
-                for directive_name in getattr(func, EXECUTES_DIRECTIVES_ASYNC):
-                    cls._async_directive_handlers[directive_name] = func
-
-    @classmethod
-    def register_directive(cls, name: str, func: Any) -> None:
-        if cls._directive_handlers is None:
-            cls._directive_handlers = {}
-        cls._directive_handlers[name] = func
-
-    @classmethod
-    def directive(cls, directive_name: str) -> str:
-        """
-        Create a directive call.
-
-        Parameters
-        ----------
-        directive_name
-            The name of the directive.
-
-        Returns
-        -------
-        The directive call.
-        """
-        if isinstance(directive_name, enum.Enum):
-            directive_name = directive_name.value
-
-        return cls.directive_prefix + directive_name
-
-
-class Directives(str, enum.Enum):
-    EXTEND = "extend"
-    INCLUDE = "include"
-    COPY = "copy"
-
-
-class Processor(BaseProcessor[ConfigModelT]):
-    directive_prefix = "^"
-    extension_prefix = "+"
-    route_separator: ClassVar[str] = ":"
-
-    @directive(Directives.EXTEND)
-    def extend(self, ctx: DirectiveContext) -> None:
-        """
-        Extend a configuration with another configuration.
-        Recursively preprocess the referenced configuration.
-        Preserve information about the referenced configuration.
-
-        Visual example
-        --------------
-
-        With `base.yaml` containing:
-        ```yaml
-        section:
-          foo: 1
-          bar: 2
-        ```
-
-        and `config.yaml` containing:
-
-        ```yaml
-        ^extend: base.yaml
-        +section:
-          foo: 3
-        ```
-
-        -> `load()` -> `save()` ->
-
-        ```yaml
-        ^extend: base.yaml
-        +section:
-          foo: 3
-        ```
-        """
-        self._substitute(ctx, preprocess=True, preserve=True)
-
-    @directive(Directives.INCLUDE)
-    def include(self, ctx: DirectiveContext) -> None:
-        """
-        Include a configuration in another configuration.
-        Recursively preprocess the referenced configuration.
-        Do not preserve information about the referenced configuration.
-
-        Visual example
-        --------------
-        With `biz.yaml` containing:
-
-        ```yaml
-        section:
-          biz: 3
-        ```
-
-        and `base.yaml` containing:
-
-        ```yaml
-        ^extend: biz.yaml
-        +section:
-          foo: 1
-          bar: 2
-        ```
-
-        and `config.yaml` containing:
-
-        ```yaml
-        ^include: base.yaml
-        +section:
-          foo: 3
-        ```
-
-        -> `load()` -> `save()` ->
-
-        ```yaml
-        ^extend: biz.yaml
-        +section:
-          bar: 2
-          foo: 3
-        ```
-        """
-        self._substitute(ctx, preprocess=True, preserve=False)
-
-    @directive(Directives.COPY)
-    def copy(self, ctx: DirectiveContext) -> None:
-        """
-        Copy a configuration and paste into another configuration.
-        This is just a literal copy-paste.
-        Do not preprocess the referenced configuration.
-        Do not preserve information about the referenced configuration.
-
-        Visual example
-        --------------
-        With `base.yaml` containing:
-
-        ```yaml
-        section:
-          foo: 1
-          bar: 2
-        ```
-
-        and `config.yaml` containing:
-
-        ```yaml
-        ^copy: base.yaml
-        +section:
-          foo: 3
-        ```
-
-        -> `load()` -> `save()` ->
-
-        ```yaml
-        section:
-          foo: 3
-          bar: 2
-        ```
-        """
-        self._substitute(ctx, preprocess=False, preserve=False)
-
-    @directive(Directives.EXTEND)
-    async def extend_async(self, ctx: DirectiveContext) -> None:
-        """
-        Extend a configuration with another configuration asynchronously.
-        For more information see `extend`.
-        """
-        await self._substitute_async(ctx, preprocess=True, preserve=True)
-
-    @directive(Directives.INCLUDE)
-    async def include_async(self, ctx: DirectiveContext) -> None:
-        """
-        Include a configuration in another configuration asynchronously.
-        For more information see `include`.
-        """
-        await self._substitute_async(ctx, preprocess=True, preserve=False)
-
-    @directive(Directives.COPY)
-    async def copy_async(self, ctx: DirectiveContext) -> None:
-        """
-        Copy a configuration and paste into another configuration asynchronously.
-        For more information see `copy`.
-        """
-        await self._substitute_async(ctx, preprocess=False, preserve=False)
-
-    def _get_substitution_means(
-        self, ctx: DirectiveContext  # , *, preserve: bool
-    ) -> tuple[
-        ConfigAgent[ConfigModelT], ConfigAgent[ConfigModelT], SupportsRoute | None
-    ]:
-        agent_class = type(self.agent)
-
-        # todo(bswck): raise on include and extend combined
-        # if preserve and ???:
-        #     msg = (
-        #         "Using more than one ??? directive "
-        #         "in the same scope is not allowed"
-        #     )
-        #     raise ConfigPreprocessingError(msg)
-
-        agent, route = agent_class.from_directive_context(
-            ctx, route_separator=self.route_separator
-        )
-
-        if agent.resource == self.agent.resource:
-            raise ConfigPreprocessingError(
-                f"{agent.resource} tried to {ctx.directive!r} on itself"
-            )
-
-        actual_agent = agent
-        if agent.relative:
-            parent = cast(pathlib.Path, self.agent.resource).parent
-            child = cast(pathlib.Path, agent.resource)
-
-            actual_agent = copy.copy(agent)
-            actual_agent.resource = parent / child
-
-        return actual_agent, agent, route
-
-    def _substitute(
-        self, ctx: DirectiveContext, *, preprocess: bool, preserve: bool
-    ) -> None:
-        agent, orig_agent, route = self._get_substitution_means(ctx)
-
-        with agent.processor_open_resource() as reader:
-            source = orig_agent.load_into_dict(reader.read(), preprocess=preprocess)
-
-        self._substitute_impl(
-            ctx,
-            route,
-            source=source,
-            agent=orig_agent,
-            preprocess=preprocess,
-            preserve=preserve,
-        )
-
-    async def _substitute_async(
-        self, ctx: DirectiveContext, *, preprocess: bool, preserve: bool
-    ) -> None:
-        agent, orig_agent, route = self._get_substitution_means(ctx)
-
-        async with agent.processor_open_resource_async() as reader:
-            source = orig_agent.load_into_dict(
-                await reader.read(), preprocess=preprocess
-            )
-
-        self._substitute_impl(
-            ctx,
-            route,
-            source=source,
-            agent=orig_agent,
-            preprocess=preprocess,
-            preserve=preserve,
-        )
-
-    @staticmethod
-    def _substitute_impl(  # noqa: PLR0913
-        ctx: DirectiveContext,
-        route: SupportsRoute | None,
-        *,
-        source: dict[str, Any],
-        agent: ConfigAgent[ConfigModelT],
-        preprocess: bool,
-        preserve: bool,
-    ) -> None:
-        from configzen.config import CONTEXT, Context, at
-
-        if route:
-            source = at(source, route, agent=agent)
-            if not is_dict_like(source):
-                raise ConfigPreprocessingError(
-                    f"imported item {route!r} "
-                    f"from {agent.resource} is not a dictionary"
-                )
-
-        context: Context[ConfigModelT] = Context(agent)
-        ctx.container = source | ctx.container
-
-        if preserve:
-            ctx.container |= {
-                CONTEXT: context,
-                EXPORT: ExportMetadata(
-                    route=str(route),
-                    context=context,
-                    preprocess=preprocess,
-                    key_order=list(ctx.container),
-                ),
-            }
-
-    @classmethod
-    def _export(
-        cls,
-        state: dict[str, Any],
-        metadata: ExportMetadata[ConfigModelT],
-    ) -> None:
-        """
-        Exports model state preserving substition directive calls in the model state.
-
-        Parameters
-        ----------
-        metadata
-        state
-        """
-        from configzen.config import CONTEXT, at, pre_serialize
-
-        overrides = {}
-
-        route = metadata["route"]
-        context = metadata["context"]
-        key_order = metadata["key_order"]
-        agent = context.agent
-
-        with agent.processor_open_resource() as reader:
-            # Here we intentionally always preprocess the loaded configuration.
-            loaded = agent.load_into_dict(reader.read())
-
-            if route:
-                loaded = at(loaded, route, agent=agent)
-
-        substituted_values = loaded.copy()
-
-        missing = object()
-
-        for key, value in loaded.items():
-            counterpart_value = state.pop(key, missing)
-            if counterpart_value is missing:
-                continue
-            counterpart_value = pre_serialize(counterpart_value)
-
-            if is_dict_like(value):
-                if EXPORT in value:
-                    value.pop(CONTEXT, None)
-                    cls.export(value, metadata=value.pop(EXPORT))
-                overrides_for_key = {
-                    sub_key: comp
-                    for sub_key, comp in counterpart_value.items()
-                    if (
-                        (orig := value.get(sub_key, missing)) is missing or orig != comp
-                    )
-                }
-                if overrides_for_key:
-                    export_key = agent.processor_class.extension_prefix + key
-                    overrides[export_key] = overrides_for_key
-
-            elif is_list_like(value):
-                cls.export(value, metadata=None)
-
-            elif counterpart_value != value:
-                overrides[key] = counterpart_value
-                del substituted_values[key]
-
-        for value in state.values():
-            cls.export(value, metadata=None)
-
-        cls._export_finalize(
-            context=context,
-            state=state,
-            overrides=overrides,
-            values=substituted_values,
-            route=route,
-            key_order=key_order,
-        )
-
-    @classmethod
-    async def _export_async(
-        cls,
-        state: dict[str, Any],
-        metadata: ExportMetadata[ConfigModelT],
-    ) -> None:
-        """
-        Exports model state preserving substition directive calls in the model state.
-
-        Parameters
-        ----------
-        metadata
-        state
-        """
-        from configzen.config import CONTEXT, at, pre_serialize
-
-        overrides = {}
-
-        route = metadata["route"]
-        context = metadata["context"]
-        key_order = metadata["key_order"]
-        agent = context.agent
-
-        async with agent.processor_open_resource_async() as reader:
-            # Here we intentionally always preprocess the loaded configuration.
-            loaded = await agent.load_into_dict_async(await reader.read())
-
-            if route:
-                loaded = at(loaded, route, agent=agent)
-
-        substituted_values = loaded.copy()
-
-        missing = object()
-
-        for key, value in loaded.items():
-            counterpart_value = state.pop(key, missing)
-            if counterpart_value is missing:
-                continue
-            counterpart_value = pre_serialize(counterpart_value)
-
-            if is_dict_like(value):
-                if EXPORT in value:
-                    value.pop(CONTEXT, None)
-                    await cls.export_async(value, metadata=value.pop(EXPORT))
-                overrides_for_key = {
-                    sub_key: comp
-                    for sub_key, comp in counterpart_value.items()
-                    if (
-                        (orig := value.get(sub_key, missing)) is missing or orig != comp
-                    )
-                }
-                if overrides_for_key:
-                    export_key = agent.processor_class.extension_prefix + key
-                    overrides[export_key] = overrides_for_key
-
-            elif is_list_like(value):
-                await cls.export_async(value, metadata=None)
-
-            elif counterpart_value != value:
-                overrides[key] = counterpart_value
-                del substituted_values[key]
-
-        for value in state.values():
-            await cls.export_async(value, metadata=None)
-
-        cls._export_finalize(
-            context=context,
-            state=state,
-            overrides=overrides,
-            values=substituted_values,
-            route=route,
-            key_order=key_order,
-        )
-
-    @classmethod
-    def _export_finalize(  # noqa: PLR0913
-        cls,
-        context: BaseContext[ConfigModelT],
-        *,
-        state: dict[str, Any],
-        overrides: dict[str, Any],
-        values: dict[str, Any],
-        route: str | None,
-        key_order: list[str],
-    ) -> None:
-        # TODO: Optimize. We iterate over the same way too many times.
-
-        state |= overrides
-        extras: dict[str, Any] = {
-            key: state.pop(key) for key in set(state) if key not in key_order
-        }
-
-        if values:
-            substitution_directive = cls.directive(Directives.EXTEND)
-            resource = str(context.agent.resource)
-            if route:
-                resource = cls.route_separator.join((resource, route))
-            # Put the substitution directive at the beginning of the state in-place.
-            state |= {substitution_directive: resource} | {
-                key: state.pop(key) for key in set(state)
-            }
-
-        # Preserve the order of keys in the original configuration.
-        for key in filter(state.__contains__, key_order):
-            state[key] = state.pop(key)
-
-        state |= extras
+from __future__ import annotations
+
+import asyncio
+import copy
+import dataclasses
+import enum
+import pathlib
+from collections.abc import Callable
+from typing import TYPE_CHECKING, Any, ClassVar, Generic, TypedDict, TypeVar, cast
+
+from anyconfig.utils import is_dict_like, is_list_like
+
+from configzen.errors import (
+    ConfigPreprocessingError,
+)
+from configzen.typedefs import ConfigModelT, SupportsRoute
+
+if TYPE_CHECKING:
+    from configzen.config import BaseContext, ConfigAgent
+
+__all__ = (
+    "DirectiveContext",
+    "directive",
+    "Processor",
+)
+
+DirectiveT = TypeVar("DirectiveT")
+
+EXPORT: str = "__configzen_export__"
+EXECUTES_DIRECTIVES: str = "__configzen_executes_directives__"
+EXECUTES_DIRECTIVES_ASYNC: str = "__configzen_executes_directives_async__"
+
+
+def directive(
+    name: str | enum.Enum,
+    *,
+    asynchronous: bool | None = None,
+) -> Callable[..., Any]:
+    """
+    Decorator for creating processor directives.
+
+    Parameters
+    ----------
+    name
+        The name of the directive.
+    asynchronous
+        Whether the decorated directive function is asynchronous.
+
+    Returns
+    -------
+    The decorated function.
+    """
+    if isinstance(name, enum.Enum):
+        name = name.value.casefold()
+
+    def decorator(func: Any) -> Any:
+        nonlocal asynchronous
+        if asynchronous is None:
+            asynchronous = asyncio.iscoroutinefunction(func)
+        attr = EXECUTES_DIRECTIVES_ASYNC if asynchronous else EXECUTES_DIRECTIVES
+        if not hasattr(func, attr):
+            setattr(func, attr, set())
+        getattr(func, attr).add(name)
+        return func
+
+    return decorator
+
+
+@dataclasses.dataclass
+class DirectiveContext:
+    """
+    Context for processor directives.
+
+    Attributes
+    ----------
+    directive
+        The directive.
+    key
+        The key of the directive.
+    prefix
+        The prefix of the directive.
+    snippet
+        The config snippet where this directive was invoked.
+    container
+        The dictionary that contains the :attr:`dict`.
+
+    """
+
+    directive: str
+    key: str
+    prefix: str
+    snippet: dict[str, Any]
+    container: dict[str, Any]
+
+
+def parse_directive_call(
+    prefix: str,
+    directive_name: str,
+) -> str:
+    if directive_name.startswith(prefix):
+        directive_name = directive_name[len(prefix) :].casefold()
+
+        if not directive_name.isidentifier():
+            msg = f"Invalid directive name: {directive_name}"
+            raise ConfigPreprocessingError(msg)
+
+    return directive_name
+
+
+if TYPE_CHECKING:
+
+    class ExportMetadata(TypedDict, Generic[ConfigModelT]):
+        route: str | None
+        context: BaseContext[ConfigModelT]
+        key_order: list[str]
+        preprocess: bool
+
+else:
+
+    class ExportMetadata(TypedDict):
+        """
+        Metadata for exporting.
+
+        Attributes
+        ----------
+        route
+            The route to import from.
+        context
+            The context attached to the import.
+        """
+
+        route: str | None
+        context: BaseContext[ConfigModelT]
+        key_order: list[str]
+        preprocess: bool
+
+
+class BaseProcessor(Generic[ConfigModelT]):
+    """
+    Processor that executes directives.
+
+    Attributes
+    ----------
+    dict_config
+        The dictionary config to parse and update.
+    directive_prefix
+        The prefix for directives.
+    """
+
+    _directive_handlers: dict[str, Any] = None  # type: ignore[assignment]
+    _async_directive_handlers: dict[str, Any] = None  # type: ignore[assignment]
+    directive_prefix: ClassVar[str]
+    extension_prefix: ClassVar[str]
+
+    def __init__(
+        self,
+        agent: ConfigAgent[ConfigModelT],
+        dict_config: dict[str, Any],
+    ) -> None:
+        self.agent = agent
+        self.dict_config = dict_config
+
+    @classmethod
+    def export(
+        cls,
+        state: Any,
+        *,
+        metadata: ExportMetadata[ConfigModelT] | None = None,
+    ) -> None:
+        """
+        Export the state.
+
+        Parameters
+        ----------
+        state
+            The state to export.
+        metadata
+            The metadata of the substitution.
+        """
+        if is_dict_like(state):
+            if metadata is None:
+                from configzen.config import CONTEXT
+
+                state.pop(CONTEXT, None)
+                metadata = state.pop(EXPORT, None)
+            if metadata:
+                cls._export(state, metadata)
+            else:
+                cls.export(list(state.values()))
+        elif is_list_like(state):
+            for item in state:
+                cls.export(item)
+
+    @classmethod
+    async def export_async(
+        cls,
+        state: Any,
+        *,
+        metadata: ExportMetadata[ConfigModelT] | None = None,
+    ) -> None:
+        """
+        Export the state asynchronously.
+
+        Parameters
+        ----------
+        state
+            The state to export.
+        metadata
+            The metadata of the substitution.
+        """
+        if is_dict_like(state):
+            if metadata is None:
+                from configzen.config import CONTEXT
+
+                state.pop(CONTEXT, None)
+                metadata = state.pop(EXPORT, None)
+            if metadata:
+                await cls._export_async(state, metadata)
+            else:
+                await cls.export_async(list(state.values()))
+        elif is_list_like(state):
+            for item in state:
+                await cls.export_async(item)
+
+    @classmethod
+    def _export(
+        cls,
+        state: Any,
+        metadata: ExportMetadata[ConfigModelT],
+    ) -> None:
+        raise NotImplementedError
+
+    @classmethod
+    async def _export_async(
+        cls,
+        state: Any,
+        metadata: ExportMetadata[ConfigModelT],
+    ) -> None:
+        raise NotImplementedError
+
+    async def preprocess_async(self) -> dict[str, Any]:
+        """
+        Parse the dictionary config and return the parsed config,
+        ready for instantiating the model.
+
+        Returns
+        -------
+        The parsed config.
+        """
+        return cast(dict[str, Any], await self._preprocess_async(self.dict_config))
+
+    def preprocess(self) -> dict[str, Any]:
+        """
+        Parse the dictionary config and return the parsed config,
+        ready for instantiating the model.
+
+        Returns
+        -------
+        The parsed config.
+        """
+        return cast(dict[str, Any], self._preprocess(self.dict_config))
+
+    def _preprocess(self, container: Any) -> Any:
+        if not is_dict_like(container):
+            if is_list_like(container):
+                return [self._preprocess(v) for v in container]
+            return container
+
+        result: dict[str, Any] = {}
+
+        for key, value in sorted(
+            cast(dict[str, Any], container).items(),
+            key=lambda item: item[0] == self.directive_prefix,
+        ):
+            if key.startswith(self.extension_prefix):
+                actual_key = key.lstrip(self.extension_prefix)
+                overridden = result.get(actual_key, {})
+                if not is_dict_like(overridden):
+                    raise ConfigPreprocessingError(
+                        f"{self.extension_prefix} can be used only for overriding "
+                        f"dictionary sections but item at {actual_key!r} "
+                        f"is not a dictionary"
+                    )
+                replacement = overridden | value
+                result[actual_key] = self._preprocess(replacement)
+            elif key.startswith(self.directive_prefix):
+                directive_name = parse_directive_call(self.directive_prefix, key)
+                context_container = container.copy()
+                del context_container[key]
+                context = DirectiveContext(
+                    directive=directive_name,
+                    key=key,
+                    prefix=self.directive_prefix,
+                    snippet=value,
+                    container=context_container,
+                )
+                self._call_directive(context)
+                new_container = self._preprocess(context.container)
+                result |= new_container
+            else:
+                result[key] = self._preprocess(value)
+        return result
+
+    async def _preprocess_async(self, container: Any) -> Any:
+        if not is_dict_like(container):
+            if is_list_like(container):
+                return [await self._preprocess_async(v) for v in container]
+            return container
+
+        result: dict[str, Any] = {}
+
+        for key, value in sorted(
+            cast(dict[str, Any], container).items(),
+            key=lambda item: item[0] == self.directive_prefix,
+        ):
+            if key.startswith(self.extension_prefix):
+                actual_key = key.lstrip(self.extension_prefix)
+                overridden = result.get(actual_key, {})
+                if not is_dict_like(overridden):
+                    raise ConfigPreprocessingError(
+                        f"{self.extension_prefix} can be used only for overriding "
+                        f"dictionary sections but item at {actual_key!r} "
+                        f"is not a dictionary"
+                    )
+                replacement = overridden | value
+                result[actual_key] = await self._preprocess_async(replacement)
+            elif key.startswith(self.directive_prefix):
+                directive_name = parse_directive_call(self.directive_prefix, key)
+                context_container = container.copy()
+                del context_container[key]
+                context = DirectiveContext(
+                    directive=directive_name,
+                    key=key,
+                    prefix=self.directive_prefix,
+                    snippet=value,
+                    container=context_container,
+                )
+                await self._call_directive_async(context)
+                new_container = await self._preprocess_async(context.container)
+                result |= new_container
+            else:
+                result[key] = await self._preprocess_async(value)
+        return result
+
+    def _call_directive(self, context: DirectiveContext) -> None:
+        handler = self._directive_handlers.get(context.directive)
+        if handler is None:
+            raise ConfigPreprocessingError(
+                f"unknown preprocessing directive: {context.directive!r}"
+            )
+        handler(self, context)
+
+    async def _call_directive_async(self, context: DirectiveContext) -> None:
+        handler = self._async_directive_handlers.get(context.directive)
+        if handler is None:
+            raise ConfigPreprocessingError(
+                f"unknown preprocessing directive: {context.directive!r}"
+            )
+        await handler(self, context)
+
+    def __init_subclass__(cls, **kwargs: Any) -> None:
+        super().__init_subclass__(**kwargs)
+        if cls._directive_handlers is None:
+            cls._directive_handlers = {}
+        else:
+            cls._directive_handlers = cls._directive_handlers.copy()
+        if cls._async_directive_handlers is None:
+            cls._async_directive_handlers = {}
+        else:
+            cls._async_directive_handlers = cls._async_directive_handlers.copy()
+        for _name, func in cls.__dict__.items():
+            if hasattr(func, EXECUTES_DIRECTIVES):
+                for directive_name in getattr(func, EXECUTES_DIRECTIVES):
+                    cls._directive_handlers[directive_name] = func
+            elif hasattr(func, EXECUTES_DIRECTIVES_ASYNC):
+                for directive_name in getattr(func, EXECUTES_DIRECTIVES_ASYNC):
+                    cls._async_directive_handlers[directive_name] = func
+
+    @classmethod
+    def register_directive(cls, name: str, func: Any) -> None:
+        if cls._directive_handlers is None:
+            cls._directive_handlers = {}
+        cls._directive_handlers[name] = func
+
+    @classmethod
+    def directive(cls, directive_name: str) -> str:
+        """
+        Create a directive call.
+
+        Parameters
+        ----------
+        directive_name
+            The name of the directive.
+
+        Returns
+        -------
+        The directive call.
+        """
+        if isinstance(directive_name, enum.Enum):
+            directive_name = directive_name.value
+
+        return cls.directive_prefix + directive_name
+
+
+class Directives(str, enum.Enum):
+    EXTEND = "extend"
+    INCLUDE = "include"
+    COPY = "copy"
+
+
+class Processor(BaseProcessor[ConfigModelT]):
+    directive_prefix = "^"
+    extension_prefix = "+"
+    route_separator: ClassVar[str] = ":"
+
+    @directive(Directives.EXTEND)
+    def extend(self, ctx: DirectiveContext) -> None:
+        """
+        Extend a configuration with another configuration.
+        Recursively preprocess the referenced configuration.
+        Preserve information about the referenced configuration.
+
+        Visual example
+        --------------
+
+        With `base.yaml` containing:
+        ```yaml
+        section:
+          foo: 1
+          bar: 2
+        ```
+
+        and `config.yaml` containing:
+
+        ```yaml
+        ^extend: base.yaml
+        +section:
+          foo: 3
+        ```
+
+        -> `load()` -> `save()` ->
+
+        ```yaml
+        ^extend: base.yaml
+        +section:
+          foo: 3
+        ```
+        """
+        self._substitute(ctx, preprocess=True, preserve=True)
+
+    @directive(Directives.INCLUDE)
+    def include(self, ctx: DirectiveContext) -> None:
+        """
+        Include a configuration in another configuration.
+        Recursively preprocess the referenced configuration.
+        Do not preserve information about the referenced configuration.
+
+        Visual example
+        --------------
+        With `biz.yaml` containing:
+
+        ```yaml
+        section:
+          biz: 3
+        ```
+
+        and `base.yaml` containing:
+
+        ```yaml
+        ^extend: biz.yaml
+        +section:
+          foo: 1
+          bar: 2
+        ```
+
+        and `config.yaml` containing:
+
+        ```yaml
+        ^include: base.yaml
+        +section:
+          foo: 3
+        ```
+
+        -> `load()` -> `save()` ->
+
+        ```yaml
+        ^extend: biz.yaml
+        +section:
+          bar: 2
+          foo: 3
+        ```
+        """
+        self._substitute(ctx, preprocess=True, preserve=False)
+
+    @directive(Directives.COPY)
+    def copy(self, ctx: DirectiveContext) -> None:
+        """
+        Copy a configuration and paste into another configuration.
+        This is just a literal copy-paste.
+        Do not preprocess the referenced configuration.
+        Do not preserve information about the referenced configuration.
+
+        Visual example
+        --------------
+        With `base.yaml` containing:
+
+        ```yaml
+        section:
+          foo: 1
+          bar: 2
+        ```
+
+        and `config.yaml` containing:
+
+        ```yaml
+        ^copy: base.yaml
+        +section:
+          foo: 3
+        ```
+
+        -> `load()` -> `save()` ->
+
+        ```yaml
+        section:
+          foo: 3
+          bar: 2
+        ```
+        """
+        self._substitute(ctx, preprocess=False, preserve=False)
+
+    @directive(Directives.EXTEND)
+    async def extend_async(self, ctx: DirectiveContext) -> None:
+        """
+        Extend a configuration with another configuration asynchronously.
+        For more information see `extend`.
+        """
+        await self._substitute_async(ctx, preprocess=True, preserve=True)
+
+    @directive(Directives.INCLUDE)
+    async def include_async(self, ctx: DirectiveContext) -> None:
+        """
+        Include a configuration in another configuration asynchronously.
+        For more information see `include`.
+        """
+        await self._substitute_async(ctx, preprocess=True, preserve=False)
+
+    @directive(Directives.COPY)
+    async def copy_async(self, ctx: DirectiveContext) -> None:
+        """
+        Copy a configuration and paste into another configuration asynchronously.
+        For more information see `copy`.
+        """
+        await self._substitute_async(ctx, preprocess=False, preserve=False)
+
+    def _get_substitution_means(
+        self, ctx: DirectiveContext  # , *, preserve: bool
+    ) -> tuple[
+        ConfigAgent[ConfigModelT], ConfigAgent[ConfigModelT], SupportsRoute | None
+    ]:
+        agent_class = type(self.agent)
+
+        # todo(bswck): raise on include and extend combined
+        # if preserve and ???:
+        #     msg = (
+        #         "Using more than one ??? directive "
+        #         "in the same scope is not allowed"
+        #     )
+        #     raise ConfigPreprocessingError(msg)
+
+        agent, route = agent_class.from_directive_context(
+            ctx, route_separator=self.route_separator
+        )
+
+        if agent.resource == self.agent.resource:
+            raise ConfigPreprocessingError(
+                f"{agent.resource} tried to {ctx.directive!r} on itself"
+            )
+
+        actual_agent = agent
+        if agent.relative:
+            parent = cast(pathlib.Path, self.agent.resource).parent
+            child = cast(pathlib.Path, agent.resource)
+
+            actual_agent = copy.copy(agent)
+            actual_agent.resource = parent / child
+
+        return actual_agent, agent, route
+
+    def _substitute(
+        self, ctx: DirectiveContext, *, preprocess: bool, preserve: bool
+    ) -> None:
+        agent, orig_agent, route = self._get_substitution_means(ctx)
+
+        with agent.processor_open_resource() as reader:
+            source = orig_agent.load_dict(reader.read(), preprocess=preprocess)
+
+        self._substitute_impl(
+            ctx,
+            route,
+            source=source,
+            agent=orig_agent,
+            preprocess=preprocess,
+            preserve=preserve,
+        )
+
+    async def _substitute_async(
+        self, ctx: DirectiveContext, *, preprocess: bool, preserve: bool
+    ) -> None:
+        agent, orig_agent, route = self._get_substitution_means(ctx)
+
+        async with agent.processor_open_resource_async() as reader:
+            source = orig_agent.load_dict(
+                await reader.read(), preprocess=preprocess
+            )
+
+        self._substitute_impl(
+            ctx,
+            route,
+            source=source,
+            agent=orig_agent,
+            preprocess=preprocess,
+            preserve=preserve,
+        )
+
+    @staticmethod
+    def _substitute_impl(  # noqa: PLR0913
+        ctx: DirectiveContext,
+        route: SupportsRoute | None,
+        *,
+        source: dict[str, Any],
+        agent: ConfigAgent[ConfigModelT],
+        preprocess: bool,
+        preserve: bool,
+    ) -> None:
+        from configzen.config import CONTEXT, Context, at
+
+        if route:
+            source = at(source, route, agent=agent)
+            if not is_dict_like(source):
+                raise ConfigPreprocessingError(
+                    f"imported item {route!r} "
+                    f"from {agent.resource} is not a dictionary"
+                )
+
+        context: Context[ConfigModelT] = Context(agent)
+        ctx.container = source | ctx.container
+
+        if preserve:
+            ctx.container |= {
+                CONTEXT: context,
+                EXPORT: ExportMetadata(
+                    route=str(route),
+                    context=context,
+                    preprocess=preprocess,
+                    key_order=list(ctx.container),
+                ),
+            }
+
+    @classmethod
+    def _export(
+        cls,
+        state: dict[str, Any],
+        metadata: ExportMetadata[ConfigModelT],
+    ) -> None:
+        """
+        Exports model state preserving substition directive calls in the model state.
+
+        Parameters
+        ----------
+        metadata
+        state
+        """
+        from configzen.config import CONTEXT, at, pre_serialize
+
+        overrides = {}
+
+        route = metadata["route"]
+        context = metadata["context"]
+        key_order = metadata["key_order"]
+        agent = context.agent
+
+        with agent.processor_open_resource() as reader:
+            # Here we intentionally always preprocess the loaded configuration.
+            loaded = agent.load_dict(reader.read())
+
+            if route:
+                loaded = at(loaded, route, agent=agent)
+
+        substituted_values = loaded.copy()
+
+        missing = object()
+
+        for key, value in loaded.items():
+            counterpart_value = state.pop(key, missing)
+            if counterpart_value is missing:
+                continue
+            counterpart_value = pre_serialize(counterpart_value)
+
+            if is_dict_like(value):
+                if EXPORT in value:
+                    value.pop(CONTEXT, None)
+                    cls.export(value, metadata=value.pop(EXPORT))
+                overrides_for_key = {
+                    sub_key: comp
+                    for sub_key, comp in counterpart_value.items()
+                    if (
+                        (orig := value.get(sub_key, missing)) is missing or orig != comp
+                    )
+                }
+                if overrides_for_key:
+                    export_key = agent.processor_class.extension_prefix + key
+                    overrides[export_key] = overrides_for_key
+
+            elif is_list_like(value):
+                cls.export(value)
+
+            elif counterpart_value != value:
+                overrides[key] = counterpart_value
+                del substituted_values[key]
+
+        for value in state.values():
+            cls.export(value)
+
+        cls._export_finalize(
+            context=context,
+            state=state,
+            overrides=overrides,
+            values=substituted_values,
+            route=route,
+            key_order=key_order,
+        )
+
+    @classmethod
+    async def _export_async(
+        cls,
+        state: dict[str, Any],
+        metadata: ExportMetadata[ConfigModelT],
+    ) -> None:
+        """
+        Exports model state preserving substition directive calls in the model state.
+
+        Parameters
+        ----------
+        metadata
+        state
+        """
+        from configzen.config import CONTEXT, at, pre_serialize
+
+        overrides = {}
+
+        route = metadata["route"]
+        context = metadata["context"]
+        key_order = metadata["key_order"]
+        agent = context.agent
+
+        async with agent.processor_open_resource_async() as reader:
+            # Here we intentionally always preprocess the loaded configuration.
+            loaded = await agent.load_dict_async(await reader.read())
+
+            if route:
+                loaded = at(loaded, route, agent=agent)
+
+        substituted_values = loaded.copy()
+
+        missing = object()
+
+        for key, value in loaded.items():
+            counterpart_value = state.pop(key, missing)
+            if counterpart_value is missing:
+                continue
+            counterpart_value = pre_serialize(counterpart_value)
+
+            if is_dict_like(value):
+                if EXPORT in value:
+                    value.pop(CONTEXT, None)
+                    await cls.export_async(value, metadata=value.pop(EXPORT))
+                overrides_for_key = {
+                    sub_key: comp
+                    for sub_key, comp in counterpart_value.items()
+                    if (
+                        (orig := value.get(sub_key, missing)) is missing or orig != comp
+                    )
+                }
+                if overrides_for_key:
+                    export_key = agent.processor_class.extension_prefix + key
+                    overrides[export_key] = overrides_for_key
+
+            elif is_list_like(value):
+                await cls.export_async(value)
+
+            elif counterpart_value != value:
+                overrides[key] = counterpart_value
+                del substituted_values[key]
+
+        for value in state.values():
+            await cls.export_async(value)
+
+        cls._export_finalize(
+            context=context,
+            state=state,
+            overrides=overrides,
+            values=substituted_values,
+            route=route,
+            key_order=key_order,
+        )
+
+    @classmethod
+    def _export_finalize(  # noqa: PLR0913
+        cls,
+        context: BaseContext[ConfigModelT],
+        *,
+        state: dict[str, Any],
+        overrides: dict[str, Any],
+        values: dict[str, Any],
+        route: str | None,
+        key_order: list[str],
+    ) -> None:
+        # TODO: Optimize. We iterate over the same way too many times.
+
+        state |= overrides
+        extras: dict[str, Any] = {
+            key: state.pop(key) for key in set(state) if key not in key_order
+        }
+
+        if values:
+            substitution_directive = cls.directive(Directives.EXTEND)
+            resource = str(context.agent.resource)
+            if route:
+                resource = cls.route_separator.join((resource, route))
+            # Put the substitution directive at the beginning of the state in-place.
+            state |= {substitution_directive: resource} | {
+                key: state.pop(key) for key in set(state)
+            }
+
+        # Preserve the order of keys in the original configuration.
+        for key in filter(state.__contains__, key_order):
+            state[key] = state.pop(key)
+
+        state |= extras
```

### Comparing `configzen-0.3.0/configzen/typedefs.py` & `configzen-0.3.1/configzen/typedefs.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-import collections.abc
-import contextlib
-import os
-import pathlib
-import sys
-from typing import TYPE_CHECKING, Any, Optional, TextIO, TypeVar, Union
-
-if sys.version_info >= (3, 10):
-    from typing import TypeAlias
-else:
-    from typing_extensions import TypeAlias
-
-if TYPE_CHECKING:
-    from aiofiles.base import AiofilesContextManager
-    from aiofiles.threadpool.text import AsyncTextIOWrapper
-
-    from configzen.config import ConfigModel, Route
-
-T = TypeVar("T")
-
-ConfigModelT = TypeVar("ConfigModelT", bound="ConfigModel")
-SupportsRoute: TypeAlias = Union[str, list[str], "Route"]
-
-ConfigIO: TypeAlias = contextlib.AbstractContextManager[TextIO]
-AsyncConfigIO: TypeAlias = "AiofilesContextManager[None, None, AsyncTextIOWrapper]"
-RawResourceT: TypeAlias = Union[ConfigIO, str, int, os.PathLike, pathlib.Path]
-NormalizedResourceT: TypeAlias = Union[ConfigIO, str, int, pathlib.Path]
-IncludeExcludeT: TypeAlias = Optional[
-    Union[
-        collections.abc.Set[Union[int, str]],
-        collections.abc.Mapping[Union[int, str], Any],
-    ]
-]
+import collections.abc
+import contextlib
+import os
+import pathlib
+import sys
+from typing import TYPE_CHECKING, Any, Optional, TextIO, TypeVar, Union
+
+if sys.version_info >= (3, 10):
+    from typing import TypeAlias
+else:
+    from typing_extensions import TypeAlias
+
+if TYPE_CHECKING:
+    from aiofiles.base import AiofilesContextManager
+    from aiofiles.threadpool.text import AsyncTextIOWrapper
+
+    from configzen.config import ConfigModel, Route
+
+T = TypeVar("T")
+
+ConfigModelT = TypeVar("ConfigModelT", bound="ConfigModel")
+SupportsRoute: TypeAlias = Union[str, list[str], "Route"]
+
+ConfigIO: TypeAlias = contextlib.AbstractContextManager[TextIO]
+AsyncConfigIO: TypeAlias = "AiofilesContextManager[None, None, AsyncTextIOWrapper]"
+RawResourceT: TypeAlias = Union[ConfigIO, str, int, os.PathLike, pathlib.Path]
+NormalizedResourceT: TypeAlias = Union[ConfigIO, str, int, pathlib.Path]
+IncludeExcludeT: TypeAlias = Optional[
+    Union[
+        collections.abc.Set[Union[int, str]],
+        collections.abc.Mapping[Union[int, str], Any],
+    ]
+]
```

### Comparing `configzen-0.3.0/LICENSE` & `configzen-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `configzen-0.3.0/README.md` & `configzen-0.3.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,69 +1,96 @@
+Metadata-Version: 2.1
+Name: configzen
+Version: 0.3.1
+Summary: The easiest way to manage configuration files in Python
+Home-page: https://github.com/bswck/configzen
+License: MIT
+Author: bswck
+Author-email: bswck.dev@gmail.com
+Requires-Python: >=3.9,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: aiofiles (>=23.1.0,<24.0.0)
+Requires-Dist: anyconfig (>=0.13.0,<0.14.0)
+Requires-Dist: pydantic (>=1.10.7,<2.0.0)
+Requires-Dist: pyyaml (>=6.0,<7.0)
+Requires-Dist: toml (>=0.10.2,<0.11.0)
+Requires-Dist: typing-extensions (>=4.5.0,<5.0.0) ; python_version >= "3.9" and python_version < "3.11"
+Description-Content-Type: text/markdown
+
 # configzen
+
 _configzen_ – managing configuration files easily.
 Currently under development, not ready for production use.
 
 ⭐ Contributions welcome! ⭐
 
 ## What is this?
-For a more precise and also philosophic explanation, see the wiki article [configzen – explanation without code](https://github.com/bswck/configzen/wiki/configzen-%E2%80%93-explanation-without-code).
 
-_configzen_ combines the power of [pydantic](https://pydantic-docs.helpmanual.io/) 
+For a more precise and also philosophic explanation, see the wiki
+article [configzen – explanation without code](https://github.com/bswck/configzen/wiki/configzen-%E2%80%93-explanation-without-code).
+
+_configzen_ combines the power of [pydantic](https://pydantic-docs.helpmanual.io/)
 and [anyconfig](https://github.com/ssato/python-anyconfig) to provide the most simplistic
 way on Earth of managing configuration files in your Python projects.
 
-Thanks to this, instead of manually using 
-`pyyaml` for YAML configuration files, `configparser` for INI files, `json` for JSON files, etc. 
-you can create a data model of your configuration and let _configzen_ do the rest and provide you 
-with some extra features on top of that, such as both synchronous and asynchronous, 
+Thanks to this, instead of manually using
+`pyyaml` for YAML configuration files, `configparser` for INI files, `json` for JSON files, etc.
+you can create a data model of your configuration and let _configzen_ do the rest and provide you
+with some extra features on top of that, such as both synchronous and asynchronous,
 preferably full or partial reloading and saving of your structured configuration.
 
-_configzen_ will help you to organize your configuration files and make them easy to use 
-and maintain. One of the core features of _configzen_ is that it allows you to import 
+_configzen_ will help you to organize your configuration files and make them easy to use
+and maintain. One of the core features of _configzen_ is that it allows you to import
 configuration files inside other configuration files, which is especially useful when you
 have a lot of configuration files, and you want to avoid repeating yourself.
 
-
 ## Features
 
 ### Managing content
+
 Let's see how it looks like in practice. Let's say you have a YAML configuration file like this:
+
 ```yaml
 # database.yaml
 host: 127.0.0.1
 port: 5432
 user: postgres
 ```
+
 You can create a data model for it like this:
 
 ```python
 # config.py
 from ipaddress import IPv4Address, IPv6Address
 from configzen import ConfigModel, ConfigMeta, ConfigField
 
 
 class DatabaseConfig(ConfigModel):
     host: IPv4Address | IPv6Address
     port: int
     user: str
     password: str = ConfigField(exclude=True)
-    
+
     class Config(ConfigMeta):
         resource = "database.yaml"
         env_prefix = "DB_"
 
 
 db_config = DatabaseConfig.load()
 ```
 
 As simple as that!
 This way, you can load your configuration from a file as well as from the environment variables
-`DB_HOST`, `DB_PORT`, `DB_USER` and `DB_PASSWORD`. Since `password` is a field created with 
+`DB_HOST`, `DB_PORT`, `DB_USER` and `DB_PASSWORD`. Since `password` is a field created with
 the option `exclude=True`, it will not be included in the configuration's exported data: that
-guarantees that your password won't leak into `database.yaml` on save – but you may still pass it 
+guarantees that your password won't leak into `database.yaml` on save – but you may still pass it
 through an environment variable (here – the mentioned `DB_PASSWORD`). Secret files are also supported though.
 
 [pydantic](https://docs.pydantic.dev/latest/) will take care of parsing and validating the loaded data.
 
 You can now use the `db_config` object to access the configuration values:
 
 ```python
@@ -117,18 +144,20 @@
 
 ```python
 >>> db_config.save()
 39
 ```
 
 ### Preprocessing directives
+
 _configzen_ allows you to use built-in preprocessing directives in your configuration files,
-offering features such as importing other configuration files in order to extend 
+offering features such as importing other configuration files in order to extend
 your base configuration without writing any code. You might think of it as something
-that is analogous to [Azure DevOps YAML templates](https://docs.microsoft.com/en-us/azure/devops/pipelines/process/templates?view=azure-devops),
+that is analogous
+to [Azure DevOps YAML templates](https://docs.microsoft.com/en-us/azure/devops/pipelines/process/templates?view=azure-devops),
 but for configuration files, broadened to any configuration file format and with some extra features planned.
 
 Thanks to this, you can write your configuration in a modular way, and avoid repeating yourself.
 
 Let's say you have a base configuration file like this (`base.json`):
 
 ```json
@@ -153,15 +182,15 @@
 +app:
   debug: false
 ```
 
 Using `+` in front of a key will update the section already defined at that key,
 instead of replacing it.
 
-Notice how configuration file formats don't matter in _configzen_: you can 
+Notice how configuration file formats don't matter in _configzen_: you can
 extend JSON configurations in YAML, but that might be as well any other format
 among [JSON](https://en.wikipedia.org/wiki/JSON), [INI](https://en.wikipedia.org/wiki/INI_file),
 [XML](https://en.wikipedia.org/wiki/XML), [.properties](https://en.wikipedia.org/wiki/.properties),
 shellvars (
 see [Augeas docs on shellvars](https://augeas.net/docs/references/1.4.0/lenses/files/shellvars-aug.html)),
 [YAML](https://yaml.org), [TOML](https://en.wikipedia.org/wiki/TOML),
 [Amazon Ion](https://en.wikipedia.org/wiki/Ion_(serialization_format)),
@@ -180,32 +209,38 @@
   debug: false
 ```
 
 With the difference that the primary example, while saving the configuration,
 will preserve the relation to the base configuration file, so that you can reload
 the configuration, and it will be updated with the changes made in the base configuration file.
 
-
 ## Setup
+
 For using _configzen_ in your project, you need to install it first:
 
 ```bash
 pip install configzen
 ```
 
 For development, you can clone the repository and install its dependencies with [poetry](https://python-poetry.org/):
+
 ```bash
 poetry install --with dev
 ```
 
 ## License
+
 [MIT License](https://choosealicense.com/licenses/mit/)
 
 ## Contributing
-Contributions are welcome! Feel free to [open an issue](https://github.com/bswck/configzen/issues/new/choose) 
+
+Contributions are welcome! Feel free to [open an issue](https://github.com/bswck/configzen/issues/new/choose)
 or [submit a pull request](https://github.com/bswck/configzen/compare).
 
 ## Credits
+
 * [@Lunarmagpie](https://github.com/Lunarmagpie) for _crucial_ design tips and ideas.
- 
+
 ## Author
+
 * [bswck](https://github.com/bswck) (contact: bswck.dev@gmail.com or via [Discord](https://discord.com/) `bswck#8238`)
+
```

### Comparing `configzen-0.3.0/PKG-INFO` & `configzen-0.3.1/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,237 +1,223 @@
-Metadata-Version: 2.1
-Name: configzen
-Version: 0.3.0
-Summary: The easiest way to manage configuration files in Python
-Home-page: https://github.com/bswck/configzen
-License: MIT
-Author: bswck
-Author-email: bswck.dev@gmail.com
-Requires-Python: >=3.9,<4.0
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Provides-Extra: async
-Provides-Extra: toml
-Provides-Extra: yaml
-Requires-Dist: aiofiles (>=23.1.0,<24.0.0) ; extra == "async"
-Requires-Dist: anyconfig (>=0.13.0,<0.14.0)
-Requires-Dist: pydantic (>=1.10.7,<2.0.0)
-Requires-Dist: pyyaml (>=6.0,<7.0) ; extra == "yaml"
-Requires-Dist: toml (>=0.10.2,<0.11.0) ; extra == "toml"
-Requires-Dist: typing-extensions (>=4.5.0,<5.0.0) ; python_version >= "3.9" and python_version < "3.11"
-Description-Content-Type: text/markdown
-
-# configzen
-_configzen_ – managing configuration files easily.
-Currently under development, not ready for production use.
-
-⭐ Contributions welcome! ⭐
-
-## What is this?
-For a more precise and also philosophic explanation, see the wiki article [configzen – explanation without code](https://github.com/bswck/configzen/wiki/configzen-%E2%80%93-explanation-without-code).
-
-_configzen_ combines the power of [pydantic](https://pydantic-docs.helpmanual.io/) 
-and [anyconfig](https://github.com/ssato/python-anyconfig) to provide the most simplistic
-way on Earth of managing configuration files in your Python projects.
-
-Thanks to this, instead of manually using 
-`pyyaml` for YAML configuration files, `configparser` for INI files, `json` for JSON files, etc. 
-you can create a data model of your configuration and let _configzen_ do the rest and provide you 
-with some extra features on top of that, such as both synchronous and asynchronous, 
-preferably full or partial reloading and saving of your structured configuration.
-
-_configzen_ will help you to organize your configuration files and make them easy to use 
-and maintain. One of the core features of _configzen_ is that it allows you to import 
-configuration files inside other configuration files, which is especially useful when you
-have a lot of configuration files, and you want to avoid repeating yourself.
-
-
-## Features
-
-### Managing content
-Let's see how it looks like in practice. Let's say you have a YAML configuration file like this:
-```yaml
-# database.yaml
-host: 127.0.0.1
-port: 5432
-user: postgres
-```
-You can create a data model for it like this:
-
-```python
-# config.py
-from ipaddress import IPv4Address, IPv6Address
-from configzen import ConfigModel, ConfigMeta, ConfigField
-
-
-class DatabaseConfig(ConfigModel):
-    host: IPv4Address | IPv6Address
-    port: int
-    user: str
-    password: str = ConfigField(exclude=True)
-    
-    class Config(ConfigMeta):
-        resource = "database.yaml"
-        env_prefix = "DB_"
-
-
-db_config = DatabaseConfig.load()
-```
-
-As simple as that!
-This way, you can load your configuration from a file as well as from the environment variables
-`DB_HOST`, `DB_PORT`, `DB_USER` and `DB_PASSWORD`. Since `password` is a field created with 
-the option `exclude=True`, it will not be included in the configuration's exported data: that
-guarantees that your password won't leak into `database.yaml` on save – but you may still pass it 
-through an environment variable (here – the mentioned `DB_PASSWORD`). Secret files are also supported though.
-
-[pydantic](https://docs.pydantic.dev/latest/) will take care of parsing and validating the loaded data.
-
-You can now use the `db_config` object to access the configuration values:
-
-```python
->>> db_config.host
-IPv4Address('127.0.0.1')
-```
-
-modify them, if the pydantic model allows it:
-
-```python
->>> db_config.host = "0.0.0.0"
->>> db_config.host
-IPv4Address('0.0.0.0')
-```
-
-as well as reload particular values, without touching the rest of the configuration:
-
-```python
->>> db_config.at("port").reload()
-5432
->>> db_config
-DatabaseConfig(host=IPv4Address('0.0.0.0'), port=5432, user='postgres', password='password')
->>> db_config.at("host").reload()
-IPv4Address('127.0.0.1')
->>> db_config
-DatabaseConfig(host=IPv4Address('127.0.0.1'), port=5432, user='postgres', password='password')
-```
-
-or reload the whole configuration:
-
-```python
->>> db_config.port = 1234
->>> db_config.reload()
-DatabaseConfig(host=IPv4Address('127.0.0.1'), port=5432, user='postgres', password='password')
-```
-
-or save a particular value, without touching the rest of the configuration:
-
-```python
->>> db_config.host = "0.0.0.0"
->>> db_config.port = 443
->>> db_config
-DatabaseConfig(host=IPv4Address('0.0.0.0'), port=443, user='postgres', password='password')
->>> db_config.at("host").save()
-40
->>> db_config.reload()
-DatabaseConfig(host=IPv4Address('0.0.0.0'), port=5432, user='postgres', password='password')
-```
-
-or save the whole configuration:
-
-```python
->>> db_config.save()
-39
-```
-
-### Preprocessing directives
-_configzen_ allows you to use built-in preprocessing directives in your configuration files,
-offering features such as importing other configuration files in order to extend 
-your base configuration without writing any code. You might think of it as something
-that is analogous to [Azure DevOps YAML templates](https://docs.microsoft.com/en-us/azure/devops/pipelines/process/templates?view=azure-devops),
-but for configuration files, broadened to any configuration file format and with some extra features planned.
-
-Thanks to this, you can write your configuration in a modular way, and avoid repeating yourself.
-
-Let's say you have a base configuration file like this (`base.json`):
-
-```json
-{
-  "i18n": {
-    "language": "en",
-    "timezone": "UTC"
-  },
-  "app": {
-    "debug": true
-  }
-}
-```
-
-To extend this configuration, you can create another configuration file like this,
-overriding desired sections as needed:
-
-```yaml
-# production.yaml
-^extend: base.json
-
-+app:
-  debug: false
-```
-
-Using `+` in front of a key will update the section already defined at that key,
-instead of replacing it.
-
-Notice how configuration file formats don't matter in _configzen_: you can 
-extend JSON configurations in YAML, but that might be as well any other format
-among [JSON](https://en.wikipedia.org/wiki/JSON), [INI](https://en.wikipedia.org/wiki/INI_file),
-[XML](https://en.wikipedia.org/wiki/XML), [.properties](https://en.wikipedia.org/wiki/.properties),
-shellvars (
-see [Augeas docs on shellvars](https://augeas.net/docs/references/1.4.0/lenses/files/shellvars-aug.html)),
-[YAML](https://yaml.org), [TOML](https://en.wikipedia.org/wiki/TOML),
-[Amazon Ion](https://en.wikipedia.org/wiki/Ion_(serialization_format)),
-[BSON](https://en.wikipedia.org/wiki/BSON), [CBOR](https://en.wikipedia.org/wiki/CBOR),
-[ConfigObj](https://configobj.readthedocs.io/en/latest/configobj.html#introduction) or
-[MessagePack](https://en.wikipedia.org/wiki/MessagePack).
-
-The above example is equivalent to as if you used:
-
-```yaml
-# production.yaml
-i18n:
-  language: en
-  timezone: UTC
-app:
-  debug: false
-```
-
-With the difference that the primary example, while saving the configuration,
-will preserve the relation to the base configuration file, so that you can reload
-the configuration, and it will be updated with the changes made in the base configuration file.
-
-
-## Setup
-For using _configzen_ in your project, you need to install it first:
-
-```bash
-pip install configzen
-```
-
-For development, you can clone the repository and install its dependencies with [poetry](https://python-poetry.org/):
-```bash
-poetry install --with dev
-```
-
-## License
-[MIT License](https://choosealicense.com/licenses/mit/)
-
-## Contributing
-Contributions are welcome! Feel free to [open an issue](https://github.com/bswck/configzen/issues/new/choose) 
-or [submit a pull request](https://github.com/bswck/configzen/compare).
-
-## Credits
-* [@Lunarmagpie](https://github.com/Lunarmagpie) for _crucial_ design tips and ideas.
- 
-## Author
-* [bswck](https://github.com/bswck) (contact: bswck.dev@gmail.com or via [Discord](https://discord.com/) `bswck#8238`)
-
+# configzen
+
+_configzen_ – managing configuration files easily.
+Currently under development, not ready for production use.
+
+⭐ Contributions welcome! ⭐
+
+## What is this?
+
+For a more precise and also philosophic explanation, see the wiki
+article [configzen – explanation without code](https://github.com/bswck/configzen/wiki/configzen-%E2%80%93-explanation-without-code).
+
+_configzen_ combines the power of [pydantic](https://pydantic-docs.helpmanual.io/)
+and [anyconfig](https://github.com/ssato/python-anyconfig) to provide the most simplistic
+way on Earth of managing configuration files in your Python projects.
+
+Thanks to this, instead of manually using
+`pyyaml` for YAML configuration files, `configparser` for INI files, `json` for JSON files, etc.
+you can create a data model of your configuration and let _configzen_ do the rest and provide you
+with some extra features on top of that, such as both synchronous and asynchronous,
+preferably full or partial reloading and saving of your structured configuration.
+
+_configzen_ will help you to organize your configuration files and make them easy to use
+and maintain. One of the core features of _configzen_ is that it allows you to import
+configuration files inside other configuration files, which is especially useful when you
+have a lot of configuration files, and you want to avoid repeating yourself.
+
+## Features
+
+### Managing content
+
+Let's see how it looks like in practice. Let's say you have a YAML configuration file like this:
+
+```yaml
+# database.yaml
+host: 127.0.0.1
+port: 5432
+user: postgres
+```
+
+You can create a data model for it like this:
+
+```python
+# config.py
+from ipaddress import IPv4Address, IPv6Address
+from configzen import ConfigModel, ConfigMeta, ConfigField
+
+
+class DatabaseConfig(ConfigModel):
+    host: IPv4Address | IPv6Address
+    port: int
+    user: str
+    password: str = ConfigField(exclude=True)
+
+    class Config(ConfigMeta):
+        resource = "database.yaml"
+        env_prefix = "DB_"
+
+
+db_config = DatabaseConfig.load()
+```
+
+As simple as that!
+This way, you can load your configuration from a file as well as from the environment variables
+`DB_HOST`, `DB_PORT`, `DB_USER` and `DB_PASSWORD`. Since `password` is a field created with
+the option `exclude=True`, it will not be included in the configuration's exported data: that
+guarantees that your password won't leak into `database.yaml` on save – but you may still pass it
+through an environment variable (here – the mentioned `DB_PASSWORD`). Secret files are also supported though.
+
+[pydantic](https://docs.pydantic.dev/latest/) will take care of parsing and validating the loaded data.
+
+You can now use the `db_config` object to access the configuration values:
+
+```python
+>>> db_config.host
+IPv4Address('127.0.0.1')
+```
+
+modify them, if the pydantic model allows it:
+
+```python
+>>> db_config.host = "0.0.0.0"
+>>> db_config.host
+IPv4Address('0.0.0.0')
+```
+
+as well as reload particular values, without touching the rest of the configuration:
+
+```python
+>>> db_config.at("port").reload()
+5432
+>>> db_config
+DatabaseConfig(host=IPv4Address('0.0.0.0'), port=5432, user='postgres', password='password')
+>>> db_config.at("host").reload()
+IPv4Address('127.0.0.1')
+>>> db_config
+DatabaseConfig(host=IPv4Address('127.0.0.1'), port=5432, user='postgres', password='password')
+```
+
+or reload the whole configuration:
+
+```python
+>>> db_config.port = 1234
+>>> db_config.reload()
+DatabaseConfig(host=IPv4Address('127.0.0.1'), port=5432, user='postgres', password='password')
+```
+
+or save a particular value, without touching the rest of the configuration:
+
+```python
+>>> db_config.host = "0.0.0.0"
+>>> db_config.port = 443
+>>> db_config
+DatabaseConfig(host=IPv4Address('0.0.0.0'), port=443, user='postgres', password='password')
+>>> db_config.at("host").save()
+40
+>>> db_config.reload()
+DatabaseConfig(host=IPv4Address('0.0.0.0'), port=5432, user='postgres', password='password')
+```
+
+or save the whole configuration:
+
+```python
+>>> db_config.save()
+39
+```
+
+### Preprocessing directives
+
+_configzen_ allows you to use built-in preprocessing directives in your configuration files,
+offering features such as importing other configuration files in order to extend
+your base configuration without writing any code. You might think of it as something
+that is analogous
+to [Azure DevOps YAML templates](https://docs.microsoft.com/en-us/azure/devops/pipelines/process/templates?view=azure-devops),
+but for configuration files, broadened to any configuration file format and with some extra features planned.
+
+Thanks to this, you can write your configuration in a modular way, and avoid repeating yourself.
+
+Let's say you have a base configuration file like this (`base.json`):
+
+```json
+{
+  "i18n": {
+    "language": "en",
+    "timezone": "UTC"
+  },
+  "app": {
+    "debug": true
+  }
+}
+```
+
+To extend this configuration, you can create another configuration file like this,
+overriding desired sections as needed:
+
+```yaml
+# production.yaml
+^extend: base.json
+
++app:
+  debug: false
+```
+
+Using `+` in front of a key will update the section already defined at that key,
+instead of replacing it.
+
+Notice how configuration file formats don't matter in _configzen_: you can
+extend JSON configurations in YAML, but that might be as well any other format
+among [JSON](https://en.wikipedia.org/wiki/JSON), [INI](https://en.wikipedia.org/wiki/INI_file),
+[XML](https://en.wikipedia.org/wiki/XML), [.properties](https://en.wikipedia.org/wiki/.properties),
+shellvars (
+see [Augeas docs on shellvars](https://augeas.net/docs/references/1.4.0/lenses/files/shellvars-aug.html)),
+[YAML](https://yaml.org), [TOML](https://en.wikipedia.org/wiki/TOML),
+[Amazon Ion](https://en.wikipedia.org/wiki/Ion_(serialization_format)),
+[BSON](https://en.wikipedia.org/wiki/BSON), [CBOR](https://en.wikipedia.org/wiki/CBOR),
+[ConfigObj](https://configobj.readthedocs.io/en/latest/configobj.html#introduction) or
+[MessagePack](https://en.wikipedia.org/wiki/MessagePack).
+
+The above example is equivalent to as if you used:
+
+```yaml
+# production.yaml
+i18n:
+  language: en
+  timezone: UTC
+app:
+  debug: false
+```
+
+With the difference that the primary example, while saving the configuration,
+will preserve the relation to the base configuration file, so that you can reload
+the configuration, and it will be updated with the changes made in the base configuration file.
+
+## Setup
+
+For using _configzen_ in your project, you need to install it first:
+
+```bash
+pip install configzen
+```
+
+For development, you can clone the repository and install its dependencies with [poetry](https://python-poetry.org/):
+
+```bash
+poetry install --with dev
+```
+
+## License
+
+[MIT License](https://choosealicense.com/licenses/mit/)
+
+## Contributing
+
+Contributions are welcome! Feel free to [open an issue](https://github.com/bswck/configzen/issues/new/choose)
+or [submit a pull request](https://github.com/bswck/configzen/compare).
+
+## Credits
+
+* [@Lunarmagpie](https://github.com/Lunarmagpie) for _crucial_ design tips and ideas.
+
+## Author
+
+* [bswck](https://github.com/bswck) (contact: bswck.dev@gmail.com or via [Discord](https://discord.com/) `bswck#8238`)
```

