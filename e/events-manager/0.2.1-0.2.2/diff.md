# Comparing `tmp/events-manager-0.2.1.tar.gz` & `tmp/events-manager-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "events-manager-0.2.1.tar", last modified: Tue May 10 03:31:28 2022, max compression
+gzip compressed data, was "events-manager-0.2.2.tar", last modified: Thu Jun 15 09:22:08 2023, max compression
```

## Comparing `events-manager-0.2.1.tar` & `events-manager-0.2.2.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-10 03:31:28.383337 events-manager-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1068 2022-05-10 03:31:14.000000 events-manager-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-05-10 03:31:14.000000 events-manager-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     5109 2022-05-10 03:31:28.383337 events-manager-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4331 2022-05-10 03:31:14.000000 events-manager-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-10 03:31:28.383337 events-manager-0.2.1/events_manager/
--rw-r--r--   0 runner    (1001) docker     (121)     2800 2022-05-10 03:31:14.000000 events-manager-0.2.1/events_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-05-10 03:31:14.000000 events-manager-0.2.1/events_manager/event.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-10 03:31:28.383337 events-manager-0.2.1/events_manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5109 2022-05-10 03:31:27.000000 events-manager-0.2.1/events_manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      258 2022-05-10 03:31:28.000000 events-manager-0.2.1/events_manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-10 03:31:27.000000 events-manager-0.2.1/events_manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-05-10 03:31:28.000000 events-manager-0.2.1/events_manager.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-10 03:31:14.000000 events-manager-0.2.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-05-10 03:31:28.383337 events-manager-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1558 2022-05-10 03:31:14.000000 events-manager-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:22:08.951452 events-manager-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-15 09:21:57.000000 events-manager-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-15 09:21:57.000000 events-manager-0.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5190 2023-06-15 09:22:08.951452 events-manager-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4449 2023-06-15 09:21:57.000000 events-manager-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:22:08.947452 events-manager-0.2.2/events_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-06-15 09:21:57.000000 events-manager-0.2.2/events_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-15 09:21:57.000000 events-manager-0.2.2/events_manager/event.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:22:08.947452 events-manager-0.2.2/events_manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5190 2023-06-15 09:22:08.000000 events-manager-0.2.2/events_manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-15 09:22:08.000000 events-manager-0.2.2/events_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 09:22:08.000000 events-manager-0.2.2/events_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-15 09:22:08.000000 events-manager-0.2.2/events_manager.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:21:57.000000 events-manager-0.2.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 09:22:08.951452 events-manager-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-06-15 09:21:57.000000 events-manager-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:22:08.947452 events-manager-0.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4985 2023-06-15 09:21:57.000000 events-manager-0.2.2/tests/test_events_manager.py
```

### Comparing `events-manager-0.2.1/LICENSE` & `events-manager-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `events-manager-0.2.1/PKG-INFO` & `events-manager-0.2.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,35 +1,33 @@
 Metadata-Version: 2.1
 Name: events-manager
-Version: 0.2.1
+Version: 0.2.2
 Summary: Python implementation for the Events Management system (aka Observer pattern)
 Home-page: https://github.com/webfucktory/python-events-manager
 Author: webfucktory
 Author-email: root@webfucktory.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-[![Lint & Test](https://github.com/webfucktory/python-events-manager/actions/workflows/lint-test.yml/badge.svg)](https://github.com/webfucktory/python-events-manager/actions/workflows/lint-test.yml)
+[![Lint & Test](https://github.com/webfucktory/python-events-manager/actions/workflows/lint-and-test.yml/badge.svg)](https://github.com/webfucktory/python-events-manager/actions/workflows/lint-and-test.yml)
 [![PyPI version](https://badge.fury.io/py/events-manager.svg)](https://pypi.org/project/events-manager)
 [![Downloads count](https://img.shields.io/pypi/dm/events-manager)](https://pypistats.org/packages/events-manager)
 
 # Events Manager
 
-Python implementation for the **Events Management** system (aka [Observer pattern](https://en.wikipedia.org/wiki/Observer_pattern)).
+Python implementation of the **Events Management** system (aka [Observer pattern](https://en.wikipedia.org/wiki/Observer_pattern)).
 
 ## Getting started
 
 ### Requirements
 
 - Python >= 3.8
 
@@ -136,15 +134,15 @@
 
 
 async def foo_listener(event: FooEvent, bar, baz):
     print(f"'foo_listener' invoked with {event}, {bar} and {baz}")
 
 
 async def main():
-    listen(FooEvent, foo_listener, 'bar', baz='baz')
+    listen(FooEvent, foo_listener, False, 'bar', baz='baz')
 
     print("Emitting event...")
     emit(FooEvent())
 
     # do the other stuff...
     await sleep(1)
 
@@ -251,12 +249,24 @@
 Emitting first event...
 'foo_listener' invoked with <__main__.FooEvent object at 0x7f92c79b9070>
 Emitting second event...
 
 Process finished with exit code 0
 ```
 
-## License
+## Development
 
-Distributed under the MIT License. See `LICENSE` file for more information.
+### Run Tests
 
+```shell script
+./test
+```
 
+### Style Check
+
+```shell script
+./lint
+```
+
+## License
+
+Distributed under the MIT License. See `LICENSE` file for more information.
```

### Comparing `events-manager-0.2.1/README.md` & `events-manager-0.2.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-[![Lint & Test](https://github.com/webfucktory/python-events-manager/actions/workflows/lint-test.yml/badge.svg)](https://github.com/webfucktory/python-events-manager/actions/workflows/lint-test.yml)
+[![Lint & Test](https://github.com/webfucktory/python-events-manager/actions/workflows/lint-and-test.yml/badge.svg)](https://github.com/webfucktory/python-events-manager/actions/workflows/lint-and-test.yml)
 [![PyPI version](https://badge.fury.io/py/events-manager.svg)](https://pypi.org/project/events-manager)
 [![Downloads count](https://img.shields.io/pypi/dm/events-manager)](https://pypistats.org/packages/events-manager)
 
 # Events Manager
 
-Python implementation for the **Events Management** system (aka [Observer pattern](https://en.wikipedia.org/wiki/Observer_pattern)).
+Python implementation of the **Events Management** system (aka [Observer pattern](https://en.wikipedia.org/wiki/Observer_pattern)).
 
 ## Getting started
 
 ### Requirements
 
 - Python >= 3.8
 
@@ -115,15 +115,15 @@
 
 
 async def foo_listener(event: FooEvent, bar, baz):
     print(f"'foo_listener' invoked with {event}, {bar} and {baz}")
 
 
 async def main():
-    listen(FooEvent, foo_listener, 'bar', baz='baz')
+    listen(FooEvent, foo_listener, False, 'bar', baz='baz')
 
     print("Emitting event...")
     emit(FooEvent())
 
     # do the other stuff...
     await sleep(1)
 
@@ -230,10 +230,24 @@
 Emitting first event...
 'foo_listener' invoked with <__main__.FooEvent object at 0x7f92c79b9070>
 Emitting second event...
 
 Process finished with exit code 0
 ```
 
+## Development
+
+### Run Tests
+
+```shell script
+./test
+```
+
+### Style Check
+
+```shell script
+./lint
+```
+
 ## License
 
 Distributed under the MIT License. See `LICENSE` file for more information.
```

### Comparing `events-manager-0.2.1/events_manager/__init__.py` & `events-manager-0.2.2/events_manager/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # PEP0440 compatible formatted version, see:
 # https://www.python.org/dev/peps/pep-0440/
 #
 # Generic release markers:
 #   X.Y.0   # For first release after an increment in Y
 #   X.Y.Z   # For bugfix releases
-__version__ = '0.2.1'
+__version__ = '0.2.2'
 
 import logging
 from asyncio import CancelledError, create_task, iscoroutinefunction
 from typing import Any, Awaitable, Callable, Dict, List, Tuple, Type, TypeVar, Union
 
 from .event import Event
 
@@ -23,14 +23,15 @@
             Union[CallableType, AsyncCallableType],
             Tuple[Tuple[Any, ...], Dict[str, Any]],
         ]
     ]
 ]
 
 _listeners: ListenersType = {}
+_background_tasks = set()
 
 
 class ListenerAlreadyExistsError(ValueError):
     pass
 
 
 def listen(event_type: Type[Event], listener: ListenerType, check_if_exists: bool = False, *args, **kwargs) -> None:
@@ -67,31 +68,37 @@
 
         return listener
 
     return register
 
 
 def emit(e: Event) -> None:
-    create_task(__run_listeners(e))
+    logging.debug(f'emitting {e.__class__}: {e}')
+
+    task = create_task(_run_listeners(e))
+    _background_tasks.add(task)
+    task.add_done_callback(_background_tasks.discard)
 
 
 def get_listeners(
         event_type: Type[Event]
 ) -> List[Tuple[Union[CallableType, AsyncCallableType], Tuple[Tuple[Any, ...], Dict[str, Any]]]]:
     return _listeners.get(event_type, [])
 
 
-async def __run_listeners(e: Event) -> None:
+async def _run_listeners(e: Event) -> None:
     listeners = _listeners.get(e.__class__) or []
 
     for (listener, (args, kwargs)) in listeners:
-        create_task(__run_listener(e, listener, *args, **kwargs))
+        task = create_task(_run_listener(e, listener, *args, **kwargs))
+        _background_tasks.add(task)
+        task.add_done_callback(_background_tasks.discard)
 
 
-async def __run_listener(e: Event, listener: ListenerType, *args, **kwargs) -> None:
+async def _run_listener(e: Event, listener: ListenerType, *args, **kwargs) -> None:
     # noinspection PyBroadException
     try:
         if iscoroutinefunction(listener):
             await listener(e, *args, **kwargs)
 
         else:
             listener(e, *args, **kwargs)
```

### Comparing `events-manager-0.2.1/events_manager.egg-info/PKG-INFO` & `events-manager-0.2.2/events_manager.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,35 +1,33 @@
 Metadata-Version: 2.1
 Name: events-manager
-Version: 0.2.1
+Version: 0.2.2
 Summary: Python implementation for the Events Management system (aka Observer pattern)
 Home-page: https://github.com/webfucktory/python-events-manager
 Author: webfucktory
 Author-email: root@webfucktory.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-[![Lint & Test](https://github.com/webfucktory/python-events-manager/actions/workflows/lint-test.yml/badge.svg)](https://github.com/webfucktory/python-events-manager/actions/workflows/lint-test.yml)
+[![Lint & Test](https://github.com/webfucktory/python-events-manager/actions/workflows/lint-and-test.yml/badge.svg)](https://github.com/webfucktory/python-events-manager/actions/workflows/lint-and-test.yml)
 [![PyPI version](https://badge.fury.io/py/events-manager.svg)](https://pypi.org/project/events-manager)
 [![Downloads count](https://img.shields.io/pypi/dm/events-manager)](https://pypistats.org/packages/events-manager)
 
 # Events Manager
 
-Python implementation for the **Events Management** system (aka [Observer pattern](https://en.wikipedia.org/wiki/Observer_pattern)).
+Python implementation of the **Events Management** system (aka [Observer pattern](https://en.wikipedia.org/wiki/Observer_pattern)).
 
 ## Getting started
 
 ### Requirements
 
 - Python >= 3.8
 
@@ -136,15 +134,15 @@
 
 
 async def foo_listener(event: FooEvent, bar, baz):
     print(f"'foo_listener' invoked with {event}, {bar} and {baz}")
 
 
 async def main():
-    listen(FooEvent, foo_listener, 'bar', baz='baz')
+    listen(FooEvent, foo_listener, False, 'bar', baz='baz')
 
     print("Emitting event...")
     emit(FooEvent())
 
     # do the other stuff...
     await sleep(1)
 
@@ -251,12 +249,24 @@
 Emitting first event...
 'foo_listener' invoked with <__main__.FooEvent object at 0x7f92c79b9070>
 Emitting second event...
 
 Process finished with exit code 0
 ```
 
-## License
+## Development
 
-Distributed under the MIT License. See `LICENSE` file for more information.
+### Run Tests
 
+```shell script
+./test
+```
 
+### Style Check
+
+```shell script
+./lint
+```
+
+## License
+
+Distributed under the MIT License. See `LICENSE` file for more information.
```

### Comparing `events-manager-0.2.1/setup.py` & `events-manager-0.2.2/setup.py`

 * *Files identical despite different names*

