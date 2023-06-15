# Comparing `tmp/HABApp-1.0.8.tar.gz` & `tmp/HABApp-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HABApp-1.0.8.tar", last modified: Thu Feb  9 13:00:28 2023, max compression
+gzip compressed data, was "HABApp-1.1.0.tar", last modified: Thu Jun 15 10:24:28 2023, max compression
```

## Comparing `HABApp-1.0.8.tar` & `HABApp-1.1.0.tar`

### file list

```diff
@@ -1,301 +1,305 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 13:00:28.462700 HABApp-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-02-09 13:00:19.000000 HABApp-1.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-02-09 13:00:19.000000 HABApp-1.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    12371 2023-02-09 13:00:28.462700 HABApp-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-02-09 13:00:19.000000 HABApp-1.0.8/requirements_setup.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-09 13:00:28.462700 HABApp-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-02-09 13:00:19.000000 HABApp-1.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 13:00:28.430700 HABApp-1.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 13:00:28.434700 HABApp-1.0.8/src/HABApp/
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/__check_dependency_packages__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/__cmd_args__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/__debug_info__.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/__setup_packages__.py
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/__splash_screen__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 13:00:28.438700 HABApp-1.0.8/src/HABApp/config/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/config/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/config/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/config/loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 13:00:28.438700 HABApp-1.0.8/src/HABApp/config/logging/
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/config/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/config/logging/buffered_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     5855 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/config/logging/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/config/logging/default_logfile.py
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/config/logging/handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/config/logging/queue_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 13:00:28.438700 HABApp-1.0.8/src/HABApp/config/models/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/config/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/config/models/application.py
--rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/config/models/directories.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/config/models/habapp.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/config/models/location.py
--rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/config/models/mqtt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/config/models/openhab.py
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/config/platform_defaults.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 13:00:28.438700 HABApp-1.0.8/src/HABApp/core/
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/core/asyncio.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 13:00:28.438700 HABApp-1.0.8/src/HABApp/core/const/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/core/const/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/core/const/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/core/const/hints.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/core/const/json.py
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/core/const/loop.py
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/core/const/topics.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/core/const/yml.py
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/core/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 13:00:28.438700 HABApp-1.0.8/src/HABApp/core/events/
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/core/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/core/events/events.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 13:00:28.442700 HABApp-1.0.8/src/HABApp/core/events/filter/
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/core/events/filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/core/events/filter/event.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/core/events/filter/groups.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/core/events/filter/habapp_events.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/core/events/filter/no_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/core/events/habapp_events.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 13:00:28.442700 HABApp-1.0.8/src/HABApp/core/files/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/core/files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/core/files/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 13:00:28.442700 HABApp-1.0.8/src/HABApp/core/files/file/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/core/files/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4746 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/core/files/file/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/core/files/file/file_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/core/files/file/file_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/core/files/file/properties.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 13:00:28.442700 HABApp-1.0.8/src/HABApp/core/files/folders/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/core/files/folders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/core/files/folders/folders.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 13:00:28.442700 HABApp-1.0.8/src/HABApp/core/files/manager/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/core/files/manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/core/files/manager/files.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/core/files/manager/listen_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/core/files/manager/worker.py
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/core/files/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 13:00:28.442700 HABApp-1.0.8/src/HABApp/core/files/watcher/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/core/files/watcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/core/files/watcher/base_watcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/core/files/watcher/file_watcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/core/files/watcher/folder_watcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 13:00:28.442700 HABApp-1.0.8/src/HABApp/core/internals/
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/core/internals/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 13:00:28.442700 HABApp-1.0.8/src/HABApp/core/internals/context/
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/core/internals/context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/core/internals/context/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/core/internals/context/get_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 13:00:28.442700 HABApp-1.0.8/src/HABApp/core/internals/event_bus/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/core/internals/event_bus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/core/internals/event_bus/base_listener.py
--rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/core/internals/event_bus/event_bus.py
--rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/core/internals/event_bus_listener.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/core/internals/event_filter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 13:00:28.446700 HABApp-1.0.8/src/HABApp/core/internals/item_registry/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/core/internals/item_registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/core/internals/item_registry/item_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/core/internals/item_registry/item_registry_item.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 13:00:28.446700 HABApp-1.0.8/src/HABApp/core/internals/proxy/
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/core/internals/proxy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/core/internals/proxy/proxies.py
--rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/core/internals/proxy/proxy_obj.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 13:00:28.446700 HABApp-1.0.8/src/HABApp/core/internals/wrapped_function/
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/core/internals/wrapped_function/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/core/internals/wrapped_function/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/core/internals/wrapped_function/wrapped_async.py
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/core/internals/wrapped_function/wrapped_sync.py
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/core/internals/wrapped_function/wrapped_thread.py
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/core/internals/wrapped_function/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 13:00:28.446700 HABApp-1.0.8/src/HABApp/core/items/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/core/items/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4756 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/core/items/base_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/core/items/base_item_times.py
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/core/items/base_item_watch.py
--rw-r--r--   0 runner    (1001) docker     (123)    10421 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/core/items/base_valueitem.py
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/core/items/item.py
--rw-r--r--   0 runner    (1001) docker     (123)     5317 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/core/items/item_aggregation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4763 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/core/items/item_color.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/core/items/tmp_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 13:00:28.446700 HABApp-1.0.8/src/HABApp/core/lib/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/core/lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 13:00:28.446700 HABApp-1.0.8/src/HABApp/core/lib/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/core/lib/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/core/lib/exceptions/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/core/lib/exceptions/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/core/lib/exceptions/format_frame.py
--rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/core/lib/exceptions/format_frame_vars.py
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/core/lib/funcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 13:00:28.450700 HABApp-1.0.8/src/HABApp/core/lib/parameters/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/core/lib/parameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/core/lib/parameters/positive_time_diff.py
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/core/lib/pending_future.py
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/core/lib/rgb_hsv.py
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/core/lib/single_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/core/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 13:00:28.450700 HABApp-1.0.8/src/HABApp/core/types/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/core/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7658 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/core/types/color.py
--rw-r--r--   0 runner    (1001) docker     (123)     4179 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/core/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 13:00:28.450700 HABApp-1.0.8/src/HABApp/mqtt/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/mqtt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 13:00:28.450700 HABApp-1.0.8/src/HABApp/mqtt/events/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/mqtt/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/mqtt/events/mqtt_events.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/mqtt/events/mqtt_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/mqtt/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 13:00:28.450700 HABApp-1.0.8/src/HABApp/mqtt/items/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/mqtt/items/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/mqtt/items/mqtt_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/mqtt/items/mqtt_pair_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     5863 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/mqtt/mqtt_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/mqtt/mqtt_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/mqtt/mqtt_payload.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 13:00:28.450700 HABApp-1.0.8/src/HABApp/openhab/
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/openhab/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 13:00:28.450700 HABApp-1.0.8/src/HABApp/openhab/connection_handler/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/openhab/connection_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11159 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/openhab/connection_handler/func_async.py
--rw-r--r--   0 runner    (1001) docker     (123)    12592 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/openhab/connection_handler/func_sync.py
--rw-r--r--   0 runner    (1001) docker     (123)    13433 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/openhab/connection_handler/http_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/openhab/connection_handler/http_connection_waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4328 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/openhab/connection_handler/sse_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 13:00:28.450700 HABApp-1.0.8/src/HABApp/openhab/connection_logic/
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/openhab/connection_logic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/openhab/connection_logic/_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/openhab/connection_logic/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/openhab/connection_logic/plugin_load_items.py
--rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/openhab/connection_logic/plugin_ping.py
--rw-r--r--   0 runner    (1001) docker     (123)     3470 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/openhab/connection_logic/plugin_thing_overview.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 13:00:28.454700 HABApp-1.0.8/src/HABApp/openhab/connection_logic/plugin_things/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/openhab/connection_logic/plugin_things/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/openhab/connection_logic/plugin_things/_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     5259 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/openhab/connection_logic/plugin_things/cfg_validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 13:00:28.454700 HABApp-1.0.8/src/HABApp/openhab/connection_logic/plugin_things/file_writer/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/openhab/connection_logic/plugin_things/file_writer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/openhab/connection_logic/plugin_things/file_writer/formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/openhab/connection_logic/plugin_things/file_writer/formatter_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/openhab/connection_logic/plugin_things/file_writer/writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/openhab/connection_logic/plugin_things/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     5453 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/openhab/connection_logic/plugin_things/item_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     7675 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/openhab/connection_logic/plugin_things/plugin_things.py
--rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/openhab/connection_logic/plugin_things/str_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4684 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/openhab/connection_logic/plugin_things/thing_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/openhab/connection_logic/plugin_things/thing_worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 13:00:28.454700 HABApp-1.0.8/src/HABApp/openhab/definitions/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/openhab/definitions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/openhab/definitions/definitions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 13:00:28.454700 HABApp-1.0.8/src/HABApp/openhab/definitions/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/openhab/definitions/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4204 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/openhab/definitions/helpers/log_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/openhab/definitions/helpers/persistence_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 13:00:28.454700 HABApp-1.0.8/src/HABApp/openhab/definitions/rest/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/openhab/definitions/rest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/openhab/definitions/rest/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/openhab/definitions/rest/habapp_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/openhab/definitions/rest/items.py
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/openhab/definitions/rest/links.py
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/openhab/definitions/rest/things.py
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/openhab/definitions/topics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/openhab/definitions/values.py
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/openhab/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 13:00:28.454700 HABApp-1.0.8/src/HABApp/openhab/events/
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/openhab/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/openhab/events/base_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/openhab/events/channel_events.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/openhab/events/event_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7172 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/openhab/events/item_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     5725 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/openhab/events/thing_events.py
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/openhab/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/openhab/interface_async.py
--rw-r--r--   0 runner    (1001) docker     (123)     3929 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/openhab/item_to_reg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 13:00:28.458700 HABApp-1.0.8/src/HABApp/openhab/items/
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/openhab/items/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4935 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/openhab/items/base_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/openhab/items/call_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     5501 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/openhab/items/color_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/openhab/items/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/openhab/items/contact_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/openhab/items/datetime_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/openhab/items/dimmer_item.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/openhab/items/group_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/openhab/items/image_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/openhab/items/number_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/openhab/items/rollershutter_item.py
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/openhab/items/string_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/openhab/items/switch_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/openhab/items/thing_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/openhab/map_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/openhab/map_items.py
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/openhab/map_values.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 13:00:28.458700 HABApp-1.0.8/src/HABApp/parameters/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/parameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6730 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/parameters/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/parameters/parameter_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/parameters/parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 13:00:28.458700 HABApp-1.0.8/src/HABApp/rule/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/rule/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 13:00:28.458700 HABApp-1.0.8/src/HABApp/rule/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/rule/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/rule/interfaces/_http.py
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/rule/interfaces/http_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/rule/interfaces/rule_subprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)    13868 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/rule/rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/rule/rule_hook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 13:00:28.458700 HABApp-1.0.8/src/HABApp/rule/scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/rule/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/rule/scheduler/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5486 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/rule/scheduler/habappschedulerview.py
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/rule/scheduler/scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 13:00:28.458700 HABApp-1.0.8/src/HABApp/rule_ctx/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/rule_ctx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/rule_ctx/rule_ctx.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 13:00:28.458700 HABApp-1.0.8/src/HABApp/rule_manager/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/rule_manager/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 13:00:28.462700 HABApp-1.0.8/src/HABApp/rule_manager/benchmark/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/rule_manager/benchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/rule_manager/benchmark/bench_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/rule_manager/benchmark/bench_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/rule_manager/benchmark/bench_habapp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/rule_manager/benchmark/bench_mqtt.py
--rw-r--r--   0 runner    (1001) docker     (123)     5473 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/rule_manager/benchmark/bench_oh.py
--rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/rule_manager/benchmark/bench_times.py
--rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/rule_manager/rule_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     5557 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/rule_manager/rule_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 13:00:28.462700 HABApp-1.0.8/src/HABApp/runtime/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/runtime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/runtime/runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/runtime/shutdown.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 13:00:28.462700 HABApp-1.0.8/src/HABApp/util/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/util/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 13:00:28.462700 HABApp-1.0.8/src/HABApp/util/fade/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/util/fade/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/util/fade/fade.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 13:00:28.462700 HABApp-1.0.8/src/HABApp/util/functions/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/util/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/util/functions/min_max.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 13:00:28.462700 HABApp-1.0.8/src/HABApp/util/listener_groups/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/util/listener_groups/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/util/listener_groups/listener_creator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5874 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/util/listener_groups/listener_groups.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 13:00:28.462700 HABApp-1.0.8/src/HABApp/util/multimode/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/util/multimode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4878 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/util/multimode/item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/util/multimode/mode_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/util/multimode/mode_switch.py
--rw-r--r--   0 runner    (1001) docker     (123)     7400 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/util/multimode/mode_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/util/statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-02-09 13:00:19.000000 HABApp-1.0.8/src/HABApp/util/threshold.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 13:00:28.434700 HABApp-1.0.8/src/HABApp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12371 2023-02-09 13:00:28.000000 HABApp-1.0.8/src/HABApp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9922 2023-02-09 13:00:28.000000 HABApp-1.0.8/src/HABApp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-09 13:00:28.000000 HABApp-1.0.8/src/HABApp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-02-09 13:00:28.000000 HABApp-1.0.8/src/HABApp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-02-09 13:00:28.000000 HABApp-1.0.8/src/HABApp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-02-09 13:00:28.000000 HABApp-1.0.8/src/HABApp.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 13:00:28.462700 HABApp-1.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-02-09 13:00:19.000000 HABApp-1.0.8/tests/test_cmd_args.py
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-02-09 13:00:19.000000 HABApp-1.0.8/tests/test_debug_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-02-09 13:00:19.000000 HABApp-1.0.8/tests/test_docs.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-02-09 13:00:19.000000 HABApp-1.0.8/tests/test_packages.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:24:28.662346 HABApp-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-15 10:24:10.000000 HABApp-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-15 10:24:10.000000 HABApp-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    13801 2023-06-15 10:24:28.662346 HABApp-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-15 10:24:10.000000 HABApp-1.1.0/requirements_setup.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 10:24:28.662346 HABApp-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-06-15 10:24:10.000000 HABApp-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:24:28.618345 HABApp-1.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:24:28.626345 HABApp-1.1.0/src/HABApp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/__check_dependency_packages__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/__cmd_args__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/__debug_info__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/__setup_packages__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/__splash_screen__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:24:28.626345 HABApp-1.1.0/src/HABApp/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/config/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/config/loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:24:28.626345 HABApp-1.1.0/src/HABApp/config/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/config/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/config/logging/buffered_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5852 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/config/logging/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/config/logging/default_logfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/config/logging/handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/config/logging/queue_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:24:28.626345 HABApp-1.1.0/src/HABApp/config/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/config/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/config/models/application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/config/models/directories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/config/models/habapp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/config/models/location.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/config/models/mqtt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/config/models/openhab.py
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/config/platform_defaults.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:24:28.630345 HABApp-1.1.0/src/HABApp/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/core/asyncio.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:24:28.630345 HABApp-1.1.0/src/HABApp/core/const/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/core/const/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/core/const/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/core/const/hints.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/core/const/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/core/const/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/core/const/loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/core/const/topics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/core/const/yml.py
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/core/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:24:28.630345 HABApp-1.1.0/src/HABApp/core/events/
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/core/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/core/events/events.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:24:28.630345 HABApp-1.1.0/src/HABApp/core/events/filter/
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/core/events/filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/core/events/filter/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/core/events/filter/groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/core/events/filter/habapp_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/core/events/filter/no_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/core/events/habapp_events.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:24:28.630345 HABApp-1.1.0/src/HABApp/core/files/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/core/files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/core/files/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:24:28.634345 HABApp-1.1.0/src/HABApp/core/files/file/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/core/files/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4746 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/core/files/file/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/core/files/file/file_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/core/files/file/file_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/core/files/file/properties.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:24:28.634345 HABApp-1.1.0/src/HABApp/core/files/folders/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/core/files/folders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/core/files/folders/folders.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:24:28.634345 HABApp-1.1.0/src/HABApp/core/files/manager/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/core/files/manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/core/files/manager/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/core/files/manager/listen_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/core/files/manager/worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/core/files/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:24:28.634345 HABApp-1.1.0/src/HABApp/core/files/watcher/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/core/files/watcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/core/files/watcher/base_watcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/core/files/watcher/file_watcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/core/files/watcher/folder_watcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:24:28.634345 HABApp-1.1.0/src/HABApp/core/internals/
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/core/internals/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:24:28.634345 HABApp-1.1.0/src/HABApp/core/internals/context/
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/core/internals/context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/core/internals/context/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/core/internals/context/get_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:24:28.634345 HABApp-1.1.0/src/HABApp/core/internals/event_bus/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/core/internals/event_bus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/core/internals/event_bus/base_listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/core/internals/event_bus/event_bus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/core/internals/event_bus_listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/core/internals/event_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:24:28.634345 HABApp-1.1.0/src/HABApp/core/internals/item_registry/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/core/internals/item_registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/core/internals/item_registry/item_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/core/internals/item_registry/item_registry_item.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:24:28.638345 HABApp-1.1.0/src/HABApp/core/internals/proxy/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/core/internals/proxy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/core/internals/proxy/proxies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/core/internals/proxy/proxy_obj.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:24:28.638345 HABApp-1.1.0/src/HABApp/core/internals/wrapped_function/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/core/internals/wrapped_function/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/core/internals/wrapped_function/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/core/internals/wrapped_function/wrapped_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/core/internals/wrapped_function/wrapped_sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/core/internals/wrapped_function/wrapped_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/core/internals/wrapped_function/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:24:28.638345 HABApp-1.1.0/src/HABApp/core/items/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/core/items/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4756 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/core/items/base_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/core/items/base_item_times.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/core/items/base_item_watch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10485 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/core/items/base_valueitem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/core/items/item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5317 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/core/items/item_aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4763 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/core/items/item_color.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/core/items/tmp_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:24:28.638345 HABApp-1.1.0/src/HABApp/core/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/core/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:24:28.638345 HABApp-1.1.0/src/HABApp/core/lib/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/core/lib/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/core/lib/exceptions/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/core/lib/exceptions/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/core/lib/exceptions/format_frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/core/lib/exceptions/format_frame_vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/core/lib/funcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:24:28.642346 HABApp-1.1.0/src/HABApp/core/lib/parameters/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/core/lib/parameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/core/lib/parameters/positive_time_diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/core/lib/pending_future.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/core/lib/rgb_hsv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/core/lib/single_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/core/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:24:28.642346 HABApp-1.1.0/src/HABApp/core/types/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/core/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7658 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/core/types/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/core/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:24:28.642346 HABApp-1.1.0/src/HABApp/mqtt/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/mqtt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:24:28.642346 HABApp-1.1.0/src/HABApp/mqtt/events/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/mqtt/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/mqtt/events/mqtt_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/mqtt/events/mqtt_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/mqtt/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:24:28.642346 HABApp-1.1.0/src/HABApp/mqtt/items/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/mqtt/items/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/mqtt/items/mqtt_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/mqtt/items/mqtt_pair_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5860 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/mqtt/mqtt_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/mqtt/mqtt_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/mqtt/mqtt_payload.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:24:28.642346 HABApp-1.1.0/src/HABApp/openhab/
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/openhab/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:24:28.646345 HABApp-1.1.0/src/HABApp/openhab/connection_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/openhab/connection_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11403 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/openhab/connection_handler/func_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12673 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/openhab/connection_handler/func_sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15028 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/openhab/connection_handler/http_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/openhab/connection_handler/http_connection_waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4526 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/openhab/connection_handler/sse_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:24:28.646345 HABApp-1.1.0/src/HABApp/openhab/connection_logic/
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/openhab/connection_logic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/openhab/connection_logic/_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/openhab/connection_logic/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5916 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/openhab/connection_logic/plugin_load_items.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/openhab/connection_logic/plugin_ping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3470 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/openhab/connection_logic/plugin_thing_overview.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:24:28.646345 HABApp-1.1.0/src/HABApp/openhab/connection_logic/plugin_things/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/openhab/connection_logic/plugin_things/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/openhab/connection_logic/plugin_things/_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5247 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/openhab/connection_logic/plugin_things/cfg_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:24:28.646345 HABApp-1.1.0/src/HABApp/openhab/connection_logic/plugin_things/file_writer/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/openhab/connection_logic/plugin_things/file_writer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/openhab/connection_logic/plugin_things/file_writer/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/openhab/connection_logic/plugin_things/file_writer/formatter_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/openhab/connection_logic/plugin_things/file_writer/writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/openhab/connection_logic/plugin_things/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5459 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/openhab/connection_logic/plugin_things/item_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7675 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/openhab/connection_logic/plugin_things/plugin_things.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/openhab/connection_logic/plugin_things/str_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4684 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/openhab/connection_logic/plugin_things/thing_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/openhab/connection_logic/plugin_things/thing_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/openhab/connection_logic/wait_startup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:24:28.650346 HABApp-1.1.0/src/HABApp/openhab/definitions/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/openhab/definitions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:24:28.650346 HABApp-1.1.0/src/HABApp/openhab/definitions/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/openhab/definitions/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4204 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/openhab/definitions/helpers/log_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/openhab/definitions/helpers/persistence_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/openhab/definitions/items.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:24:28.650346 HABApp-1.1.0/src/HABApp/openhab/definitions/rest/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/openhab/definitions/rest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/openhab/definitions/rest/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/openhab/definitions/rest/habapp_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/openhab/definitions/rest/items.py
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/openhab/definitions/rest/links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/openhab/definitions/rest/things.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/openhab/definitions/things.py
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/openhab/definitions/topics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3493 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/openhab/definitions/values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/openhab/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:24:28.650346 HABApp-1.1.0/src/HABApp/openhab/events/
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/openhab/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/openhab/events/base_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/openhab/events/channel_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/openhab/events/event_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7572 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/openhab/events/item_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7665 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/openhab/events/thing_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/openhab/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/openhab/interface_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4336 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/openhab/item_to_reg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:24:28.654346 HABApp-1.1.0/src/HABApp/openhab/items/
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/openhab/items/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5118 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/openhab/items/base_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5689 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/openhab/items/color_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/openhab/items/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/openhab/items/contact_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/openhab/items/datetime_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/openhab/items/dimmer_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/openhab/items/group_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/openhab/items/image_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/openhab/items/number_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/openhab/items/rollershutter_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/openhab/items/string_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/openhab/items/switch_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/openhab/items/thing_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/openhab/items/tuple_items.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/openhab/map_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/openhab/map_items.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/openhab/map_values.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:24:28.654346 HABApp-1.1.0/src/HABApp/parameters/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/parameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6730 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/parameters/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/parameters/parameter_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/parameters/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:24:28.654346 HABApp-1.1.0/src/HABApp/rule/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/rule/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:24:28.654346 HABApp-1.1.0/src/HABApp/rule/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/rule/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/rule/interfaces/_http.py
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/rule/interfaces/http_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/rule/interfaces/rule_subprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14066 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/rule/rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/rule/rule_hook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:24:28.654346 HABApp-1.1.0/src/HABApp/rule/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/rule/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/rule/scheduler/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5486 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/rule/scheduler/habappschedulerview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/rule/scheduler/scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:24:28.654346 HABApp-1.1.0/src/HABApp/rule_ctx/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/rule_ctx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/rule_ctx/rule_ctx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:24:28.654346 HABApp-1.1.0/src/HABApp/rule_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/rule_manager/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:24:28.658346 HABApp-1.1.0/src/HABApp/rule_manager/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/rule_manager/benchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/rule_manager/benchmark/bench_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/rule_manager/benchmark/bench_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/rule_manager/benchmark/bench_habapp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/rule_manager/benchmark/bench_mqtt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5473 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/rule_manager/benchmark/bench_oh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/rule_manager/benchmark/bench_times.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/rule_manager/rule_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5318 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/rule_manager/rule_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:24:28.658346 HABApp-1.1.0/src/HABApp/runtime/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/runtime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/runtime/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/runtime/shutdown.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:24:28.658346 HABApp-1.1.0/src/HABApp/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/util/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:24:28.658346 HABApp-1.1.0/src/HABApp/util/fade/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/util/fade/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/util/fade/fade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:24:28.658346 HABApp-1.1.0/src/HABApp/util/functions/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/util/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/util/functions/min_max.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:24:28.658346 HABApp-1.1.0/src/HABApp/util/listener_groups/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/util/listener_groups/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/util/listener_groups/listener_creator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5874 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/util/listener_groups/listener_groups.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:24:28.658346 HABApp-1.1.0/src/HABApp/util/multimode/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/util/multimode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4878 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/util/multimode/item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/util/multimode/mode_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/util/multimode/mode_switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7400 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/util/multimode/mode_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/util/statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-06-15 10:24:10.000000 HABApp-1.1.0/src/HABApp/util/threshold.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:24:28.626345 HABApp-1.1.0/src/HABApp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13801 2023-06-15 10:24:28.000000 HABApp-1.1.0/src/HABApp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10060 2023-06-15 10:24:28.000000 HABApp-1.1.0/src/HABApp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 10:24:28.000000 HABApp-1.1.0/src/HABApp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-15 10:24:28.000000 HABApp-1.1.0/src/HABApp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-15 10:24:28.000000 HABApp-1.1.0/src/HABApp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-15 10:24:28.000000 HABApp-1.1.0/src/HABApp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:24:28.662346 HABApp-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-06-15 10:24:10.000000 HABApp-1.1.0/tests/test_cmd_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-15 10:24:10.000000 HABApp-1.1.0/tests/test_debug_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-06-15 10:24:10.000000 HABApp-1.1.0/tests/test_docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-06-15 10:24:10.000000 HABApp-1.1.0/tests/test_packages.py
```

### Comparing `HABApp-1.0.8/LICENSE` & `HABApp-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `HABApp-1.0.8/PKG-INFO` & `HABApp-1.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HABApp
-Version: 1.0.8
+Version: 1.1.0
 Summary: Easy automation with MQTT and/or openHAB. Create home automation rules in python.
 Home-page: https://github.com/spacemanspiff2007/HABApp
 Author: spaceman_spiff
 Project-URL: Documentation, https://habapp.readthedocs.io/
 Project-URL: GitHub, https://github.com/spacemanspiff2007/HABApp
 Keywords: mqtt,openhab,habapp,home automation
 Classifier: Development Status :: 4 - Beta
@@ -42,14 +42,25 @@
 ## Goals
 The goal of this application is to provide a simple way to create home automation rules in python.
 With full syntax highlighting and descriptive names it should almost never be required to look something up in the documentation
 
 ## Documentation
 [The documentation can be found at here](https://habapp.readthedocs.io)
 
+## Help out
+HABApp was created for my own use, but I wanted others to profit from it, too.
+Creating, maintaining and developing it takes a lot of time.
+If you think this is a great tool and want to support it you can donate,
+so I can buy some more coffee to keep development going. :wink:
+
+[![Donate with PayPal](https://img.shields.io/badge/Donate-PayPal-informational?logo=paypal)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=YU5U9YQN56JVA)
+
+All donations are greatly appreciated!
+
+
 ## Examples
 
 ### MQTT Rule example
 ```python
 import datetime
 import random
 
@@ -93,25 +104,25 @@
 ```
 
 ### openHAB rule example
 
 ```python
 import HABApp
 from HABApp.core.events import ValueUpdateEvent, ValueChangeEvent, ValueChangeEventFilter, ValueUpdateEventFilter
-from HABApp.openhab.events import ItemCommandEvent, ItemStateEventFilter, ItemCommandEventFilter, \
+from HABApp.openhab.events import ItemCommandEvent, ItemStateUpdatedEventFilter, ItemCommandEventFilter, \
   ItemStateChangedEventFilter
 
 
 class MyOpenhabRule(HABApp.Rule):
 
   def __init__(self):
     super().__init__()
 
     # Trigger on item updates
-    self.listen_event('TestContact', self.item_state_update, ItemStateEventFilter())
+    self.listen_event('TestContact', self.item_state_update, ItemStateUpdatedEventFilter())
     self.listen_event('TestDateTime', self.item_state_update, ValueUpdateEventFilter())
 
     # Trigger on item changes
     self.listen_event('TestDateTime', self.item_state_change, ItemStateChangedEventFilter())
     self.listen_event('TestSwitch', self.item_state_change, ValueChangeEventFilter())
 
     # Trigger on item commands
@@ -136,14 +147,31 @@
     self.oh.post_update('TestItemUpdate', 123)
 
 
 MyOpenhabRule()
 ```
 
 # Changelog
+#### 1.1.0 (2023-06-15)
+- This is a breaking change!
+- Renamed `GroupItemStateChangedEvent` to `GroupStateChangedEvent`
+- Groups issue a `GroupStateUpdateEvent` when the state updates on OH3 (consistent with OH4 behavior)
+- Groups work now with `ValueUpdateEvent` and `ValueChangedEvent` as expected
+- Renamed `ItemStateEvent` to `ItemStateUpdatedEvent`
+- Ignored ItemStateEvent on OH4
+- Fewer warnings for long-running functions (execution of <FUNC_NAME> took too long)
+- `Thing` status and status_detail are now an Enum
+- Added `status_detail` to `Thing`
+- `LocationItem` now provides the location as a tuple
+- Added support for `Point` events
+- Improved item sync from openHAB (no more false item state `None` after startup)
+- Improved startup behavior when openHAB and HABApp get started together (e.g. after reboot)
+- Fixed an issue with short tracebacks for HABApp internal files
+- Doc improvements
+
 #### 1.0.8 (2023-02-09)
 - Fixed an issue when using token based authentication with openHAB
 - Fixed an issue with the asyncio event loop under Python < 3.10
 
 #### 1.0.7 (2023-02-09)
 - ``ContactItem`` has ``open()``/``closed()`` methods
 - Setting persistence values now works for some persistence services
```

### Comparing `HABApp-1.0.8/setup.py` & `HABApp-1.1.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,14 +47,15 @@
     url="https://github.com/spacemanspiff2007/HABApp",
     project_urls={
         'Documentation': 'https://habapp.readthedocs.io/',
         'GitHub': 'https://github.com/spacemanspiff2007/HABApp',
     },
     package_dir={'': 'src'},
     packages=find_packages('src', exclude=['tests*']),
+    package_data={'HABApp': ['py.typed']},
     install_requires=load_req(),
     python_requires='>=3.8',
     classifiers=[
         "Development Status :: 4 - Beta",
         "Framework :: AsyncIO",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
```

### Comparing `HABApp-1.0.8/src/HABApp/__check_dependency_packages__.py` & `HABApp-1.1.0/src/HABApp/__check_dependency_packages__.py`

 * *Files identical despite different names*

### Comparing `HABApp-1.0.8/src/HABApp/__cmd_args__.py` & `HABApp-1.1.0/src/HABApp/__cmd_args__.py`

 * *Files identical despite different names*

### Comparing `HABApp-1.0.8/src/HABApp/__debug_info__.py` & `HABApp-1.1.0/src/HABApp/__debug_info__.py`

 * *Files identical despite different names*

### Comparing `HABApp-1.0.8/src/HABApp/__init__.py` & `HABApp-1.1.0/src/HABApp/__init__.py`

 * *Files identical despite different names*

### Comparing `HABApp-1.0.8/src/HABApp/__main__.py` & `HABApp-1.1.0/src/HABApp/__main__.py`

 * *Files identical despite different names*

### Comparing `HABApp-1.0.8/src/HABApp/__setup_packages__.py` & `HABApp-1.1.0/src/HABApp/__setup_packages__.py`

 * *Files identical despite different names*

### Comparing `HABApp-1.0.8/src/HABApp/__splash_screen__.py` & `HABApp-1.1.0/src/HABApp/__splash_screen__.py`

 * *Files identical despite different names*

### Comparing `HABApp-1.0.8/src/HABApp/config/loader.py` & `HABApp-1.1.0/src/HABApp/config/loader.py`

 * *Files identical despite different names*

### Comparing `HABApp-1.0.8/src/HABApp/config/logging/buffered_logger.py` & `HABApp-1.1.0/src/HABApp/config/logging/buffered_logger.py`

 * *Files identical despite different names*

### Comparing `HABApp-1.0.8/src/HABApp/config/logging/config.py` & `HABApp-1.1.0/src/HABApp/config/logging/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,15 +112,15 @@
         except Exception as e:
             HABApp.core.wrapper.process_exception(rotate_files, e)
         finally:
             handler.release()
 
 
 def inject_log_buffer(cfg: dict, log: BufferedLogger):
-    from HABApp.core.const.topics import TOPIC_EVENTS
+    from HABApp.core.const.log import TOPIC_EVENTS
 
     handler_cfg = cfg.setdefault('handlers', {})
 
     prefix = 'HABAppQueue_'
 
     # Check that the prefix is unique
     for handler_name in handler_cfg:
```

### Comparing `HABApp-1.0.8/src/HABApp/config/logging/default_logfile.py` & `HABApp-1.1.0/src/HABApp/config/logging/default_logfile.py`

 * *Files identical despite different names*

### Comparing `HABApp-1.0.8/src/HABApp/config/logging/queue_handler.py` & `HABApp-1.1.0/src/HABApp/config/logging/queue_handler.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,70 +1,80 @@
 import logging
 from queue import SimpleQueue, Empty
-from threading import Thread
+from threading import Thread, Lock
 from time import sleep
 from typing import Optional, Final
 
 import HABApp
 from .config import CONFIG
 
 log = logging.getLogger('HABApp.logging')
 
 
+LOCK = Lock()
+
+
 class HABAppQueueHandler:
     FLUSH_DELAY: float = CONFIG.habapp.logging.flush_every
 
     def __init__(self, queue: SimpleQueue, handler_name: str, thread_name: str):
         self._handler: Optional[logging.Handler] = None
         self._handler_name: Final = handler_name
         self._queue: Final = queue
         self._name: Final = thread_name
         self._thread: Optional[Thread] = None
 
     def start(self) -> None:
-        if self._thread is not None:
-            raise RuntimeError('Thread can only be started once!')
+        with LOCK:
+            if self._thread is not None:
+                raise RuntimeError('Thread can only be started once!')
 
-        # resolve handler
-        self._handler = logging._handlers[self._handler_name]
+            # resolve handler
+            self._handler = logging._handlers[self._handler_name]
 
-        self._thread = Thread(target=self._worker, name=f'HABApp_{self._name}')
-        self._thread.start()
+            self._thread = thread = Thread(target=self._worker, name=f'HABApp_{self._name}')
+
+        thread.start()
 
     def signal_stop(self):
         self._queue.put_nowait(None)
 
     def stop(self) -> None:
-        if self._thread is None:
-            return None
-        thread = self._thread
+        with LOCK:
+            if (thread := self._thread) is None:
+                return None
 
         self.signal_stop()
         thread.join()
 
     def _worker(self):
         try:
-            assert self._handler is not None
-            while True:
-                sleep(self.FLUSH_DELAY)
-                if self.process_queue():
-                    break
+            log.debug(f'{self._name} thread running')
 
-            log.debug(f'{self._name} thread stopped')
-        except Exception as e:
-            HABApp.core.wrapper.process_exception(self._worker, e)
+            try:
+                assert self._handler is not None
+                while True:
+                    sleep(self.FLUSH_DELAY)
+                    if self.process_queue():
+                        break
+
+            except Exception as e:
+                HABApp.core.wrapper.process_exception(self._worker, e)
+
+            # clean up queue
+            try:
+                while True:
+                    self._queue.get_nowait()
+            except Empty:
+                pass
 
-        # clean up queue
-        try:
-            while True:
-                self._queue.get_nowait()
-        except Empty:
-            pass
-
-        self._thread = None
+            log.debug(f'{self._name} thread stopped')
+        finally:
+            with LOCK:
+                self._thread = None
 
     def process_queue(self) -> bool:
         q = self._queue
         handler = self._handler
 
         first_rec = True
```

### Comparing `HABApp-1.0.8/src/HABApp/config/models/application.py` & `HABApp-1.1.0/src/HABApp/config/models/application.py`

 * *Files identical despite different names*

### Comparing `HABApp-1.0.8/src/HABApp/config/models/directories.py` & `HABApp-1.1.0/src/HABApp/config/models/directories.py`

 * *Files identical despite different names*

### Comparing `HABApp-1.0.8/src/HABApp/config/models/habapp.py` & `HABApp-1.1.0/src/HABApp/config/models/habapp.py`

 * *Files identical despite different names*

### Comparing `HABApp-1.0.8/src/HABApp/config/models/mqtt.py` & `HABApp-1.1.0/src/HABApp/config/models/mqtt.py`

 * *Files identical despite different names*

### Comparing `HABApp-1.0.8/src/HABApp/config/models/openhab.py` & `HABApp-1.1.0/src/HABApp/config/models/openhab.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     topic_filter: str = Field(
         'openhab/items/*,'      # Item updates
         'openhab/channels/*,'   # Channel update
         # Thing events - don't listen to updated events
         # todo: check if this might be a good filter: 'openhab/things/*',
         'openhab/things/*',
         alias='topic filter', in_file=False,
-        description='Topic filter for subscribing to openHAB. This filter is processed by openHAB and only events'
+        description='Topic filter for subscribing to openHAB. This filter is processed by openHAB and only events '
                     'matching this filter will be sent to HABApp.'
     )
 
     @validator('buffer')
     def validate_see_buffer(cls, value: ByteSize):
         valid_values = (
             '64kib', '128kib', '256kib', '512kib',
```

### Comparing `HABApp-1.0.8/src/HABApp/core/__init__.py` & `HABApp-1.1.0/src/HABApp/core/__init__.py`

 * *Files identical despite different names*

### Comparing `HABApp-1.0.8/src/HABApp/core/errors.py` & `HABApp-1.1.0/src/HABApp/core/errors.py`

 * *Files identical despite different names*

### Comparing `HABApp-1.0.8/src/HABApp/core/events/events.py` & `HABApp-1.1.0/src/HABApp/core/events/events.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,76 +1,76 @@
-from typing import Any, Union
+from typing import Any, Union, Final
 
 
 class ComplexEventValue:
     def __init__(self, value):
         self.value: Any = value
 
 
 class ValueUpdateEvent:
     """
     :ivar str name:
-    :ivar     value:
+    :ivar Any value:
     """
 
     name: str
     value: Any
 
-    def __init__(self, name: str = None, value=None):
-        self.name: str = name
-        self.value = value
+    def __init__(self, name: str, value: Any):
+        self.name: Final = name
+        self.value: Final = value
 
     def __repr__(self):
         return f'<{self.__class__.__name__} name: {self.name}, value: {self.value}>'
 
 
 class ValueChangeEvent:
     """
     :ivar str name:
-    :ivar     value:
-    :ivar     old_value:
+    :ivar Any value:
+    :ivar Any old_value:
     """
 
     name: str
     value: Any
     old_value: Any
 
-    def __init__(self, name: str = None, value=None, old_value=None):
-        self.name: str = name
-        self.value = value
-        self.old_value = old_value
+    def __init__(self, name: str, value: Any, old_value: Any):
+        self.name: Final = name
+        self.value: Final = value
+        self.old_value: Final = old_value
 
     def __repr__(self):
         return f'<{self.__class__.__name__} name: {self.name}, value: {self.value}, old_value: {self.old_value}>'
 
 
 class ItemNoChangeEvent:
     """
     :ivar str               name:
     :ivar Union[int, float] seconds:
     """
 
     name: str
     seconds: Union[int, float]
 
-    def __init__(self, name=None, seconds=None):
-        self.name: str = name
-        self.seconds: int = seconds
+    def __init__(self, name: str, seconds: Union[int, float]):
+        self.name: Final = name
+        self.seconds: Final = seconds
 
     def __repr__(self):
         return f'<{self.__class__.__name__} name: {self.name}, seconds: {self.seconds}>'
 
 
 class ItemNoUpdateEvent:
     """
     :ivar str               name:
     :ivar Union[int, float] seconds:
     """
     name: str
     seconds: Union[int, float]
 
-    def __init__(self, name=None, seconds=None):
-        self.name: str = name
-        self.seconds: int = seconds
+    def __init__(self, name: str, seconds: Union[int, float]):
+        self.name: Final = name
+        self.seconds: Final = seconds
 
     def __repr__(self):
         return f'<{self.__class__.__name__} name: {self.name}, seconds: {self.seconds}>'
```

### Comparing `HABApp-1.0.8/src/HABApp/core/events/filter/event.py` & `HABApp-1.1.0/src/HABApp/core/events/filter/event.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,36 @@
+from typing import Optional
+from typing import get_type_hints as _get_type_hints
+
 from HABApp.core.const import MISSING
 from HABApp.core.const.hints import HINT_ANY_CLASS
 from HABApp.core.internals import EventFilterBase
 
 
 class EventFilter(EventFilterBase):
     """Triggers on event types and optionally on their values, too"""
 
     def __init__(self, event_class: HINT_ANY_CLASS, **kwargs):
         assert len(kwargs) < 3, 'EventFilter only allows up to two args that will be used to filter'
 
         self.event_class = event_class
 
         # Property filters
-        self.attr_name1 = None
+        self.attr_name1: Optional[str] = None
         self.attr_value1 = None
-        self.attr_name2 = None
+        self.attr_name2: Optional[str] = None
         self.attr_value2 = None
 
+        type_hints = _get_type_hints(event_class)
+
         for arg, value in kwargs.items():
             if value is MISSING:
                 continue
 
-            if arg not in event_class.__annotations__:
+            if arg not in type_hints:
                 raise AttributeError(f'Filter attribute "{arg}" does not exist for "{event_class.__name__}"')
 
             if self.attr_name1 is None:
                 self.attr_name1 = arg
                 self.attr_value1 = value
             elif self.attr_name2 is None:
                 self.attr_name2 = arg
```

### Comparing `HABApp-1.0.8/src/HABApp/core/events/filter/groups.py` & `HABApp-1.1.0/src/HABApp/core/events/filter/groups.py`

 * *Files identical despite different names*

### Comparing `HABApp-1.0.8/src/HABApp/core/events/filter/habapp_events.py` & `HABApp-1.1.0/src/HABApp/core/events/filter/habapp_events.py`

 * *Files identical despite different names*

### Comparing `HABApp-1.0.8/src/HABApp/core/events/habapp_events.py` & `HABApp-1.1.0/src/HABApp/core/events/habapp_events.py`

 * *Files identical despite different names*

### Comparing `HABApp-1.0.8/src/HABApp/core/files/file/file.py` & `HABApp-1.1.0/src/HABApp/core/files/file/file.py`

 * *Files identical despite different names*

### Comparing `HABApp-1.0.8/src/HABApp/core/files/file/file_types.py` & `HABApp-1.1.0/src/HABApp/core/files/file/file_types.py`

 * *Files identical despite different names*

### Comparing `HABApp-1.0.8/src/HABApp/core/files/file/properties.py` & `HABApp-1.1.0/src/HABApp/core/files/file/properties.py`

 * *Files identical despite different names*

### Comparing `HABApp-1.0.8/src/HABApp/core/files/folders/folders.py` & `HABApp-1.1.0/src/HABApp/core/files/folders/folders.py`

 * *Files identical despite different names*

### Comparing `HABApp-1.0.8/src/HABApp/core/files/manager/listen_events.py` & `HABApp-1.1.0/src/HABApp/core/files/manager/listen_events.py`

 * *Files identical despite different names*

### Comparing `HABApp-1.0.8/src/HABApp/core/files/manager/worker.py` & `HABApp-1.1.0/src/HABApp/core/files/manager/worker.py`

 * *Files identical despite different names*

### Comparing `HABApp-1.0.8/src/HABApp/core/files/watcher/base_watcher.py` & `HABApp-1.1.0/src/HABApp/core/files/watcher/base_watcher.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 import logging
 from pathlib import Path
 
 from watchdog.events import FileSystemEvent
+from watchdog.events import EVENT_TYPE_CLOSED as WD_EVENT_TYPE_CLOSED
+from watchdog.events import EVENT_TYPE_OPENED as WD_EVENT_TYPE_OPENED
+
 
 log = logging.getLogger('HABApp.file.events')
 log.setLevel(logging.INFO)
 
 
 class EventFilterBase:
     def notify(self, path: str) -> bool:
@@ -30,19 +33,23 @@
 
         self.folder: Path = folder
         self.watch_subfolders: bool = watch_subfolders
 
         self.filter: EventFilterBase = filter
 
     def dispatch(self, event: FileSystemEvent):
+        log.debug(event)
+
         # we don't process directory events
         if event.is_directory:
             return None
 
-        log.debug(event)
+        # we don't process open and close events
+        if (e_type := event.event_type) == WD_EVENT_TYPE_OPENED or e_type == WD_EVENT_TYPE_CLOSED:
+            return None
 
         src = event.src_path
         if self.filter.notify(src):
             self.file_changed(src)
 
         # moved events have a dst, so we process it, too
         if hasattr(event, 'dest_path'):
```

### Comparing `HABApp-1.0.8/src/HABApp/core/files/watcher/file_watcher.py` & `HABApp-1.1.0/src/HABApp/core/files/watcher/file_watcher.py`

 * *Files identical despite different names*

### Comparing `HABApp-1.0.8/src/HABApp/core/files/watcher/folder_watcher.py` & `HABApp-1.1.0/src/HABApp/core/files/watcher/folder_watcher.py`

 * *Files identical despite different names*

### Comparing `HABApp-1.0.8/src/HABApp/core/internals/__init__.py` & `HABApp-1.1.0/src/HABApp/core/internals/__init__.py`

 * *Files identical despite different names*

### Comparing `HABApp-1.0.8/src/HABApp/core/internals/context/context.py` & `HABApp-1.1.0/src/HABApp/core/internals/context/context.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 
     def remove_obj(self, obj: HINT_CONTEXT_BOUND_OBJ):
         assert isinstance(obj, ContextBoundObj)
         self.objs.remove(obj)
 
     def link(self, obj: HINT_CONTEXT_BOUND_OBJ) -> HINT_CONTEXT_BOUND_OBJ:
         assert isinstance(obj, ContextBoundObj)
+        # noinspection PyProtectedMember
         obj._ctx_link(self)
         return obj
 
     def get_callback_name(self, callback: Callable) -> Optional[str]:
         raise NotImplementedError()
```

### Comparing `HABApp-1.0.8/src/HABApp/core/internals/context/get_context.py` & `HABApp-1.1.0/src/HABApp/core/internals/context/get_context.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,39 +1,38 @@
-import sys
+# noinspection PyProtectedMember
+from sys import _getframe as sys_get_frame
 from types import FrameType
 from typing import Optional, Union, TYPE_CHECKING
 
 from HABApp.core.errors import ContextNotSetError, ContextNotFoundError
 from HABApp.core.internals.context import ContextProvidingObj, ContextBoundObj, HINT_CONTEXT_OBJ
 
 if TYPE_CHECKING:
     import HABApp
 
 
-# todo: use inspect.currentframe
+# noinspection PyProtectedMember
 def get_current_context(obj: Optional[ContextProvidingObj] = None) -> 'HABApp.rule_ctx.HABAppRuleContext':
     if obj is not None:
         return obj._habapp_ctx
 
-    depth = 0
-    while True:
-        depth += 1
-        try:
-            frm: FrameType = sys._getframe(depth)
-        except ValueError:
-            raise ContextNotFoundError() from None
-
-        ctx_obj: Union[None, object, ContextProvidingObj] = frm.f_locals.get('self', None)
-        if ctx_obj is None or not isinstance(ctx_obj, ContextProvidingObj):
-            continue
-
-        ctx = ctx_obj._habapp_ctx
-        if ctx is None:
-            raise ContextNotSetError()
-        return ctx
+    frame: Optional[FrameType] = sys_get_frame(1)
+
+    while frame is not None:
+
+        ctx_obj: Union[None, object, ContextProvidingObj] = frame.f_locals.get('self')
+        if ctx_obj is not None and isinstance(ctx_obj, ContextProvidingObj):
+            ctx = ctx_obj._habapp_ctx
+            if ctx is None:
+                raise ContextNotSetError()
+            return ctx
+
+        frame = frame.f_back
+
+    raise ContextNotFoundError()
 
 
 class AutoContextBoundObj(ContextBoundObj):
     def __init__(self, parent_ctx: Optional['HINT_CONTEXT_OBJ'] = None, **kwargs):
         if parent_ctx is None:
             parent_ctx = get_current_context()
         super().__init__(parent_ctx=parent_ctx, **kwargs)
```

### Comparing `HABApp-1.0.8/src/HABApp/core/internals/event_bus/event_bus.py` & `HABApp-1.1.0/src/HABApp/core/internals/event_bus/event_bus.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 import threading
 from typing import Any, TypeVar
 from typing import Dict, List
 
 from HABApp.core.events import ComplexEventValue, ValueChangeEvent
 from .base_listener import EventBusBaseListener
-from HABApp.core.const.topics import TOPIC_EVENTS
+from HABApp.core.const.log import TOPIC_EVENTS
 
 event_log = logging.getLogger(TOPIC_EVENTS)
 habapp_log = logging.getLogger('HABApp')
 
 _TYPE_LISTENER = TypeVar('_TYPE_LISTENER', bound=EventBusBaseListener)
```

### Comparing `HABApp-1.0.8/src/HABApp/core/internals/event_bus_listener.py` & `HABApp-1.1.0/src/HABApp/core/internals/event_bus_listener.py`

 * *Files identical despite different names*

### Comparing `HABApp-1.0.8/src/HABApp/core/internals/item_registry/item_registry.py` & `HABApp-1.1.0/src/HABApp/core/internals/item_registry/item_registry.py`

 * *Files identical despite different names*

### Comparing `HABApp-1.0.8/src/HABApp/core/internals/item_registry/item_registry_item.py` & `HABApp-1.1.0/src/HABApp/core/internals/item_registry/item_registry_item.py`

 * *Files identical despite different names*

### Comparing `HABApp-1.0.8/src/HABApp/core/internals/proxy/proxies.py` & `HABApp-1.1.0/src/HABApp/core/internals/proxy/proxies.py`

 * *Files identical despite different names*

### Comparing `HABApp-1.0.8/src/HABApp/core/internals/proxy/proxy_obj.py` & `HABApp-1.1.0/src/HABApp/core/internals/proxy/proxy_obj.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-import sys
+# noinspection PyProtectedMember
+from sys import _getframe as sys_get_frame
 from typing import Dict, List, Optional, Final, Callable
 
 from HABApp.core.errors import ProxyObjHasNotBeenReplacedError
 
 PROXIES: List['StartUpProxyObj'] = []
 
 
@@ -13,15 +14,15 @@
 
     def __getattr__(self, item):
         raise ProxyObjHasNotBeenReplacedError(self)
 
     def __call__(self, *args, **kwargs):
         raise ProxyObjHasNotBeenReplacedError(self)
 
-    def __str__(self):
+    def __repr__(self):
         return f'<{self.__class__.__name__} {self.to_replace_name}>'
 
 
 class ConstProxyObj(ProxyObjBase):
     def __init__(self, name: str):
         self.name: Final = name
 
@@ -56,15 +57,15 @@
             raise ValueError(f'"{self.to_replace_name}" should be replaced but was not found in {file}!')
 
         self.globals = None
         self.to_replace = None
 
 
 def create_proxy(to_replace: Callable) -> StartUpProxyObj:
-    frm = sys._getframe(2)
+    frm = sys_get_frame(2)
     return StartUpProxyObj(to_replace, frm.f_globals)
 
 
 class RestoreableObj:
     def __init__(self, key: str, globals: dict, proxy: 'StartUpProxyObj'):
         self.key = key
         self.globals = globals
```

### Comparing `HABApp-1.0.8/src/HABApp/core/internals/wrapped_function/base.py` & `HABApp-1.1.0/src/HABApp/core/internals/wrapped_function/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,16 +40,16 @@
         lines = format_exception(e)
 
         # Log Exception
         self.log.error(f'Error in {self.name}: {e}')
         for line in lines:
             self.log.error(line)
 
-        # Create HABApp event, but only if we are not currently processing an exception while processing an error.
-        # Otherwise we might create an endless loop!
+        # Create an HABApp event, but only if we are not currently processing an exception while processing an error.
+        # Otherwise, we might create an endless loop!
         if not args or not isinstance(args[0], HABAppException):
             event_bus.post_event(
                 TOPIC_ERRORS, HABAppException(func_name=self.name, exception=e, traceback='\n'.join(lines))
             )
 
 
 TYPE_WRAPPED_FUNC_OBJ = TypeVar('TYPE_WRAPPED_FUNC_OBJ', bound=WrappedFunctionBase)
```

### Comparing `HABApp-1.0.8/src/HABApp/core/internals/wrapped_function/wrapped_async.py` & `HABApp-1.1.0/src/HABApp/core/internals/wrapped_function/wrapped_async.py`

 * *Files identical despite different names*

### Comparing `HABApp-1.0.8/src/HABApp/core/internals/wrapped_function/wrapped_sync.py` & `HABApp-1.1.0/src/HABApp/core/internals/wrapped_function/wrapped_sync.py`

 * *Files identical despite different names*

### Comparing `HABApp-1.0.8/src/HABApp/core/internals/wrapped_function/wrapper.py` & `HABApp-1.1.0/src/HABApp/core/internals/wrapped_function/wrapper.py`

 * *Files identical despite different names*

### Comparing `HABApp-1.0.8/src/HABApp/core/items/base_item.py` & `HABApp-1.1.0/src/HABApp/core/items/base_item.py`

 * *Files identical despite different names*

### Comparing `HABApp-1.0.8/src/HABApp/core/items/base_item_times.py` & `HABApp-1.1.0/src/HABApp/core/items/base_item_times.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import logging
 from typing import Generic, TypeVar, List, Union, Type
 
 from pendulum import DateTime
 
-from HABApp.core.asyncio import create_task
-from HABApp.core.wrapper import log_exception
+from HABApp.core.asyncio import run_func_from_async
 from .base_item_watch import BaseWatch, ItemNoChangeWatch, ItemNoUpdateWatch
 
 log = logging.getLogger('HABApp')
 
 WATCH_OBJ = TypeVar("WATCH_OBJ", bound=BaseWatch)
 
 
@@ -22,31 +21,30 @@
 
     def set(self, dt: DateTime, events=True):
         self.dt = dt
         if not self.tasks:
             return
 
         if events:
-            create_task(self.schedule_events())
+            run_func_from_async(self.__async_schedule_events)
         return None
 
     def add_watch(self, secs: Union[int, float]) -> WATCH_OBJ:
         # don't add the watch two times
         for t in self.tasks:
             if not t.fut.is_canceled and t.fut.secs == secs:
                 log.warning(f'Watcher {self.WATCH.__name__} ({t.fut.secs}s) for {self.name} has already been created')
                 return t
 
         w = self.WATCH(self.name, secs)
         self.tasks.append(w)
         log.debug(f'Added {self.WATCH.__name__} ({w.fut.secs}s) for {self.name}')
         return w
 
-    @log_exception
-    async def schedule_events(self):
+    def __async_schedule_events(self):
         canceled = []
         for t in self.tasks:
             if t.fut.is_canceled:
                 canceled.append(t)
             else:
                 t.fut.reset()
```

### Comparing `HABApp-1.0.8/src/HABApp/core/items/base_item_watch.py` & `HABApp-1.1.0/src/HABApp/core/items/base_item_watch.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
 import typing
 
 import HABApp
-from HABApp.core.asyncio import create_task
+from HABApp.core.asyncio import run_func_from_async
 from HABApp.core.events import ItemNoChangeEvent, ItemNoUpdateEvent, EventFilter
 from HABApp.core.lib import PendingFuture
 from HABApp.core.const.hints import HINT_EVENT_CALLBACK
 from HABApp.core.internals import uses_post_event, get_current_context, AutoContextBoundObj, wrap_func
 from HABApp.core.internals import ContextBoundEventBusListener
 
 log = logging.getLogger('HABApp')
@@ -21,22 +21,22 @@
         super().__init__()
         self.fut = PendingFuture(self._post_event, secs)
         self.name: str = name
 
     async def _post_event(self):
         post_event(self.name, self.EVENT(self.name, self.fut.secs))
 
-    async def __cancel_watch(self):
+    def __cancel_watch(self):
         self.fut.cancel()
         log.debug(f'Canceled {self.__class__.__name__} ({self.fut.secs}s) for {self.name}')
 
     def cancel(self):
         """Cancel the item watch"""
         self._ctx_unlink()
-        create_task(self.__cancel_watch())
+        run_func_from_async(self.__cancel_watch)
 
     def listen_event(self, callback: HINT_EVENT_CALLBACK) -> 'HABApp.core.base.HINT_EVENT_BUS_LISTENER':
         """Listen to (only) the event that is emitted by this watcher"""
         context = get_current_context()
         return context.add_event_listener(
             ContextBoundEventBusListener(
                 self.name,
```

### Comparing `HABApp-1.0.8/src/HABApp/core/items/base_valueitem.py` & `HABApp-1.1.0/src/HABApp/core/items/base_valueitem.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,37 @@
 import logging
 import typing
+from datetime import datetime
 from math import ceil, floor
 
 from pendulum import UTC
 from pendulum import now as pd_now
 
+from HABApp.core.const import MISSING
 from HABApp.core.events import ValueChangeEvent, ValueUpdateEvent
 from HABApp.core.internals import uses_post_event
 from HABApp.core.items.base_item import BaseItem
-from HABApp.core.const import MISSING
 from HABApp.core.lib.funcs import compare as _compare
 
+if typing.TYPE_CHECKING:
+    datetime = datetime
+
+
 log = logging.getLogger('HABApp')
 
 post_event = uses_post_event()
 
 
 class BaseValueItem(BaseItem):
     """Simple item
 
     :ivar str name: Name of the item (read only)
     :ivar value: Value of the item, can be anything (read only)
-    :ivar datetime.datetime last_change: Timestamp of the last time when the item has changed the value (read only)
-    :ivar datetime.datetime last_update: Timestamp of the last time when the item has updated the value (read only)
+    :ivar datetime last_change: Timestamp of the last time when the item has changed the value (read only)
+    :ivar datetime last_update: Timestamp of the last time when the item has updated the value (read only)
     """
 
     def __init__(self, name: str, initial_value=None):
         super().__init__(name)
 
         self.value: typing.Any = initial_value
 
@@ -80,15 +85,15 @@
         :param lower_than: item state has to be lower than the passed value
         :param lt: item state has to be lower than the passed value
         :param lower_equal: item state has to be lower equal the passed value
         :param le: item state has to be lower equal the passed value
         :param greater_than: item state has to be greater than the passed value
         :param gt: item state has to be greater than the passed value
         :param greater_equal: item state has to be greater equal the passed value
-        :param ge: tem state has to be greater equal the passed value
+        :param ge: item state has to be greater equal the passed value
         :param is_: item state has to be the same object as the passt value (e.g. None)
         :param is_not: item state has to be not the same object as the passt value (e.g. None)
 
         :return: `True` if the new value was posted else `False`
         """
 
         if _compare(self.value, equal=equal, eq=eq, not_equal=not_equal, ne=ne,
```

### Comparing `HABApp-1.0.8/src/HABApp/core/items/item.py` & `HABApp-1.1.0/src/HABApp/core/items/item.py`

 * *Files identical despite different names*

### Comparing `HABApp-1.0.8/src/HABApp/core/items/item_aggregation.py` & `HABApp-1.1.0/src/HABApp/core/items/item_aggregation.py`

 * *Files identical despite different names*

### Comparing `HABApp-1.0.8/src/HABApp/core/items/item_color.py` & `HABApp-1.1.0/src/HABApp/core/items/item_color.py`

 * *Files identical despite different names*

### Comparing `HABApp-1.0.8/src/HABApp/core/items/tmp_data.py` & `HABApp-1.1.0/src/HABApp/core/items/tmp_data.py`

 * *Files identical despite different names*

### Comparing `HABApp-1.0.8/src/HABApp/core/lib/exceptions/format.py` & `HABApp-1.1.0/src/HABApp/core/lib/exceptions/format.py`

 * *Files identical despite different names*

### Comparing `HABApp-1.0.8/src/HABApp/core/lib/exceptions/format_frame.py` & `HABApp-1.1.0/src/HABApp/core/lib/exceptions/format_frame.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,36 +26,38 @@
     # Libraries of base installation
     re.compile(r'[/\\](?:python\d\.\d+|python\d{2,3})[/\\](?:lib[/\\]|site-packages[/\\]|\w+\.py.*$)', re.IGNORECASE),
     # Libraries in venv
     re.compile(r'[/\\]lib[/\\]site-packages[/\\]', re.IGNORECASE),
 )
 
 
-def is_habapp_file(name: str) -> bool:
+def is_suppressed_habapp_file(name: str) -> bool:
     for r in SUPPRESSED_HABAPP_PATHS:
         if r.search(name):
             return True
     return False
 
 
 def is_lib_file(name: str) -> bool:
     for r in SUPPRESSED_PATHS:
         if r.search(name):
+            if '/HABApp/' in name or '\\HABApp\\' in name:
+                continue
             return True
     return False
 
 
 def format_frame_info(tb: List[str], frame_info: FrameInfo, is_last=False) -> bool:
     filename = frame_info.filename
 
     # always skip system and python libraries
     if is_lib_file(filename):
         return False
 
-    if not is_last and is_habapp_file(filename):
+    if not is_last and is_suppressed_habapp_file(filename):
         return False
 
     # calc max line nr for indentation
     max_line = frame_info.lineno + frame_info.options.after
     # it's possible that his list is empty (e.g. if we execode in sphinx-exec-code)
     if frame_info.lines:
         max_line = frame_info.lines[-1].lineno
```

### Comparing `HABApp-1.0.8/src/HABApp/core/lib/exceptions/format_frame_vars.py` & `HABApp-1.1.0/src/HABApp/core/lib/exceptions/format_frame_vars.py`

 * *Files identical despite different names*

### Comparing `HABApp-1.0.8/src/HABApp/core/lib/funcs.py` & `HABApp-1.1.0/src/HABApp/core/lib/funcs.py`

 * *Files identical despite different names*

### Comparing `HABApp-1.0.8/src/HABApp/core/lib/parameters/positive_time_diff.py` & `HABApp-1.1.0/src/HABApp/core/lib/parameters/positive_time_diff.py`

 * *Files identical despite different names*

### Comparing `HABApp-1.0.8/src/HABApp/core/lib/pending_future.py` & `HABApp-1.1.0/src/HABApp/core/lib/pending_future.py`

 * *Files identical despite different names*

### Comparing `HABApp-1.0.8/src/HABApp/core/lib/rgb_hsv.py` & `HABApp-1.1.0/src/HABApp/core/lib/rgb_hsv.py`

 * *Files identical despite different names*

### Comparing `HABApp-1.0.8/src/HABApp/core/lib/single_task.py` & `HABApp-1.1.0/src/HABApp/core/lib/single_task.py`

 * *Files identical despite different names*

### Comparing `HABApp-1.0.8/src/HABApp/core/logger.py` & `HABApp-1.1.0/src/HABApp/core/logger.py`

 * *Files identical despite different names*

### Comparing `HABApp-1.0.8/src/HABApp/core/types/color.py` & `HABApp-1.1.0/src/HABApp/core/types/color.py`

 * *Files identical despite different names*

### Comparing `HABApp-1.0.8/src/HABApp/core/wrapper.py` & `HABApp-1.1.0/src/HABApp/core/wrapper.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import asyncio
 import functools
 import logging
-import sys
 import typing
 from logging import Logger
+# noinspection PyProtectedMember
+from sys import _getframe as sys_get_frame
 
 from HABApp.core.const.topics import TOPIC_ERRORS as TOPIC_ERRORS
 from HABApp.core.const.topics import TOPIC_WARNINGS as TOPIC_WARNINGS
 from HABApp.core.events.habapp_events import HABAppException
 from HABApp.core.internals import uses_post_event
 from HABApp.core.lib import format_exception
 
@@ -109,15 +110,15 @@
 
         # possibility to reprocess tb
         if self.proc_tb is not None:
             tb = self.proc_tb(tb)
 
         # try to get the parent function name
         try:
-            f_name = sys._getframe().f_back.f_code.co_name
+            f_name = sys_get_frame().f_back.f_code.co_name
         except Exception:
             f_name = 'Exception while getting the function name!'
 
         # log error
         if self.log is not None:
             self.log.log(self.log_level, f'Error "{exc_val}" in {f_name}:')
             for line in tb:
```

### Comparing `HABApp-1.0.8/src/HABApp/mqtt/events/mqtt_filters.py` & `HABApp-1.1.0/src/HABApp/mqtt/events/mqtt_filters.py`

 * *Files identical despite different names*

### Comparing `HABApp-1.0.8/src/HABApp/mqtt/items/mqtt_item.py` & `HABApp-1.1.0/src/HABApp/mqtt/items/mqtt_item.py`

 * *Files identical despite different names*

### Comparing `HABApp-1.0.8/src/HABApp/mqtt/items/mqtt_pair_item.py` & `HABApp-1.1.0/src/HABApp/mqtt/items/mqtt_pair_item.py`

 * *Files identical despite different names*

### Comparing `HABApp-1.0.8/src/HABApp/mqtt/mqtt_connection.py` & `HABApp-1.1.0/src/HABApp/mqtt/mqtt_connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import logging
 import typing
 
 import paho.mqtt.client as mqtt
 
 import HABApp
 from HABApp.core.asyncio import async_context
-from HABApp.core.const.topics import TOPIC_EVENTS
+from HABApp.core.const.log import TOPIC_EVENTS
 from HABApp.core.errors import ItemNotFoundException
 from HABApp.core.internals import uses_post_event, uses_get_item, uses_item_registry
 from HABApp.core.wrapper import log_exception
 from HABApp.mqtt.events import MqttValueChangeEvent, MqttValueUpdateEvent
 from HABApp.mqtt.mqtt_payload import get_msg_payload
 from HABApp.runtime import shutdown
```

### Comparing `HABApp-1.0.8/src/HABApp/mqtt/mqtt_interface.py` & `HABApp-1.1.0/src/HABApp/mqtt/mqtt_interface.py`

 * *Files identical despite different names*

### Comparing `HABApp-1.0.8/src/HABApp/mqtt/mqtt_payload.py` & `HABApp-1.1.0/src/HABApp/mqtt/mqtt_payload.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 from typing import Tuple, Any, Optional
 
 from paho.mqtt.client import MQTTMessage
 
 from HABApp.core.const.json import load_json
-from HABApp.core.const.topics import TOPIC_EVENTS
+from HABApp.core.const.log import TOPIC_EVENTS
 from HABApp.core.wrapper import process_exception
 
 log = logging.getLogger(f'{TOPIC_EVENTS}.mqtt')
 
 
 def get_msg_payload(msg: MQTTMessage) -> Tuple[Optional[str], Any]:
     try:
```

### Comparing `HABApp-1.0.8/src/HABApp/openhab/connection_handler/func_async.py` & `HABApp-1.1.0/src/HABApp/openhab/connection_handler/func_async.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,16 +21,16 @@
     async_get_root = async_get_root
     async_get_uuid = async_get_uuid
     async_send_command = async_send_command
     async_post_update = async_post_update
 
 
 def convert_to_oh_type(_in: Any) -> str:
-    if isinstance(_in, BaseValueItem):
-        raise ValueError()
+    if isinstance(_in, (str, int, float, bool)):
+        return str(_in)
 
     if isinstance(_in, datetime.datetime):
         # Add timezone (if not yet defined) to string, then remote anything below ms.
         # 2018-11-19T09:47:38.284000+0100 -> 2018-11-19T09:47:38.284+0100
         out = _in.astimezone(None).strftime('%Y-%m-%dT%H:%M:%S.%f%z')
         return out
 
@@ -42,34 +42,43 @@
 
     if isinstance(_in, RGB):
         _in = _in.to_hsb()
 
     if isinstance(_in, HSB):
         return f'{_in._hue:.2f},{_in._saturation:.2f},{_in._brightness:.2f}'
 
+    if isinstance(_in, BaseValueItem):
+        raise ValueError()
+
     return str(_in)
 
 
 async def async_item_exists(item) -> bool:
     ret = await get(f'/rest/items/{item:s}', log_404=False)
     return ret.status == 200
 
 
 async def async_get_items(include_habapp_meta=False, metadata: Optional[str] = None,
-                          all_metadata=False) -> Optional[List[Dict[str, Any]]]:
+                          all_metadata=False,
+                          only_item_state=False) -> Optional[List[Dict[str, Any]]]:
     params = None
     if include_habapp_meta:
         params = {'metadata': 'HABApp'}
     if metadata is not None:
         if params is not None:
             raise ValueError('Use include_habapp_meta or metadata')
         params = {'metadata': metadata}
     if all_metadata:
         params = {'metadata': '.+'}
 
+    if only_item_state:
+        if params is None:
+            params = {}
+        params['fields'] = 'name,state,type'
+
     resp = await get('/rest/items', params=params)
     return await resp.json(loads=load_json, encoding='utf-8')
 
 
 async def async_get_item(item: str, metadata: Optional[str] = None, all_metadata=False) -> dict:
     params = None if metadata is None else {'metadata': metadata}
     if all_metadata:
```

### Comparing `HABApp-1.0.8/src/HABApp/openhab/connection_handler/func_sync.py` & `HABApp-1.1.0/src/HABApp/openhab/connection_handler/func_sync.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import datetime
 from typing import Any, Optional, List, Dict
 
 import HABApp
 import HABApp.core
 import HABApp.openhab.events
-from HABApp.core.asyncio import run_coro_from_thread, create_task
+from HABApp.core.asyncio import run_coro_from_thread, run_func_from_async
 from HABApp.core.items import BaseValueItem
 from HABApp.openhab.definitions.rest import OpenhabItemDefinition, OpenhabThingDefinition, ItemChannelLinkDefinition
 from .func_async import async_post_update, async_send_command, async_create_item, async_get_item, \
     async_get_thing, async_set_thing_enabled, \
     async_set_metadata, async_remove_metadata, async_get_channel_link, async_create_channel_link, \
     async_remove_channel_link, async_channel_link_exists, \
     async_remove_item, async_item_exists, async_get_persistence_data, async_set_persistence_data
@@ -24,30 +24,30 @@
     :param state: new item state
     """
     assert isinstance(item_name, (str, BaseValueItem)), type(item_name)
 
     if isinstance(item_name, BaseValueItem):
         item_name = item_name.name
 
-    create_task(async_post_update(item_name, state))
+    run_func_from_async(async_post_update, item_name, state)
 
 
 def send_command(item_name: str, command):
     """
     Send the specified command to the item
 
     :param item_name: item name or item
     :param command: command
     """
     assert isinstance(item_name, (str, BaseValueItem)), type(item_name)
 
     if isinstance(item_name, BaseValueItem):
         item_name = item_name.name
 
-    create_task(async_send_command(item_name, command))
+    run_func_from_async(async_send_command, item_name, command)
 
 
 def create_item(item_type: str, name: str, label="", category="",
                 tags: List[str] = [], groups: List[str] = [],
                 group_type: str = '', group_function: str = '', group_function_params: List[str] = []):
     """Creates a new item in the openHAB item registry or updates an existing one
 
@@ -157,17 +157,17 @@
 
 
 def set_metadata(item_name: str, namespace: str, value: str, config: dict):
     """
     Add/set metadata to an item
 
     :param item_name: name of the item or item
-    :param namespace: namespace
+    :param namespace: namespace, e.g. ``stateDescription``
     :param value: value
-    :param config: configuration
+    :param config: configuration e.g. ``{"options": "A,B,C"}``
     :return: True if metadata was successfully created/updated
     """
     if isinstance(item_name, BaseValueItem):
         item_name = item_name.name
     assert isinstance(item_name, str), type(item_name)
     assert isinstance(namespace, str), type(namespace)
     assert isinstance(value, str), type(value)
```

### Comparing `HABApp-1.0.8/src/HABApp/openhab/connection_handler/http_connection.py` & `HABApp-1.1.0/src/HABApp/openhab/connection_handler/http_connection.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 import asyncio
 import logging
 import traceback
-import typing
 from asyncio import Queue, sleep, QueueEmpty
-from typing import Any, Optional, Final
+from time import monotonic
+from typing import Any, Optional, Final, Tuple, Callable, Union
 
 import aiohttp
+from aiohttp import ContentTypeError
 from aiohttp.client import ClientResponse, _RequestContextManager
 from aiohttp.hdrs import METH_GET, METH_POST, METH_PUT, METH_DELETE
 from aiohttp_sse_client import client as sse_client
 
 import HABApp
 import HABApp.core
 import HABApp.openhab.events
 from HABApp.core.asyncio import async_context
 from HABApp.core.const.json import dump_json, load_json
 from HABApp.core.logger import log_info, log_warning
 from HABApp.core.wrapper import process_exception, ignore_exception
 from HABApp.openhab.errors import OpenhabDisconnectedError, ExpectedSuccessFromOpenhab
 from .http_connection_waiter import WaitBetweenConnects
-from ...core.const.topics import TOPIC_EVENTS
+from ...core.const.log import TOPIC_EVENTS
 from ...core.lib import SingleTask
 
 log = logging.getLogger('HABApp.openhab.connection')
 log_events = logging.getLogger(f'{TOPIC_EVENTS}.openhab')
 
 
 IS_ONLINE: bool = False
@@ -33,16 +34,19 @@
 # HTTP options
 HTTP_ALLOW_REDIRECTS: bool = True
 HTTP_VERIFY_SSL: Optional[bool] = None
 HTTP_SESSION: aiohttp.ClientSession = None
 
 CONNECT_WAIT: WaitBetweenConnects = WaitBetweenConnects()
 
-ON_CONNECTED: typing.Callable = None
-ON_DISCONNECTED: typing.Callable = None
+ON_CONNECTED: Callable = None
+ON_DISCONNECTED: Callable = None
+
+
+OH_3: bool = False
 
 
 async def get(url: str, log_404=True, **kwargs: Any) -> ClientResponse:
 
     mgr = _RequestContextManager(
         HTTP_SESSION._request(METH_GET, url, allow_redirects=HTTP_ALLOW_REDIRECTS, ssl=HTTP_VERIFY_SSL, **kwargs)
     )
@@ -226,14 +230,15 @@
 
     async_context.set('SSE')
 
     try:
         # cache so we don't have to look up every event
         _load_json = load_json
         _see_handler = on_sse_event
+        oh3 = OH_3
 
         async with sse_client.EventSource(url=f'/rest/events?topics={HABApp.CONFIG.openhab.connection.topic_filter}',
                                           session=HTTP_SESSION, ssl=HTTP_VERIFY_SSL) as event_source:
             async for event in event_source:
 
                 e_str = event.data
 
@@ -241,23 +246,28 @@
                     e_json = _load_json(e_str)
                 except (ValueError, TypeError):
                     log_events.warning(f'Invalid json: {e_str}')
                     continue
 
                 # Alive event from openhab to detect dropped connections
                 # -> Can be ignored on the HABApp side
-                if e_json.get('type') == 'ALIVE':
+                e_type = e_json.get('type')
+                if e_type == 'ALIVE':
                     continue
 
                 # Log raw sse event
                 if log_events.isEnabledFor(logging.DEBUG):
                     log_events._log(logging.DEBUG, e_str, [])
 
+                # With OH4 we have the ItemStateUpdatedEvent, so we can ignore the ItemStateEvent
+                if not oh3 and e_type == 'ItemStateEvent':
+                    continue
+
                 # process
-                _see_handler(e_json)
+                _see_handler(e_json, oh3)
     except Exception as e:
         disconnect = is_disconnect_exception(e)
         lvl = logging.WARNING if disconnect else logging.ERROR
         log.log(lvl, f'SSE request Error: {e}')
         for line in traceback.format_exc().splitlines():
             log.log(lvl, line)
 
@@ -317,85 +327,120 @@
             if lower <= last_info_at:
                 lower = -1
                 log_info(log, 'queue OK')
             else:
                 log_info(log, f'{size} messages in queue')
 
 
-async def async_post_update(item, state: Any):
+def async_post_update(item, state: Any):
     QUEUE.put_nowait((item, state, False))
 
 
-async def async_send_command(item, state: Any):
+def async_send_command(item, state: Any):
     QUEUE.put_nowait((item, state, True))
 
 
 async def async_get_uuid() -> str:
     resp = await get('/rest/uuid', log_404=False)
     return await resp.text(encoding='utf-8')
 
 
-async def async_get_root() -> dict:
+async def async_get_root() -> Optional[dict]:
     resp = await get('/rest/', log_404=False)
     if resp.status == 404:
-        return {}
-    return await resp.json(loads=load_json, encoding='utf-8')
+        return None
+
+    try:
+        return await resp.json(loads=load_json, encoding='utf-8')
+    except ContentTypeError:
+        # during start up openHAB sends an empty response with a wrong
+        # content type which causes the above error
+        return None
 
 
 async def async_get_system_info() -> dict:
     resp = await get('/rest/systeminfo', log_404=False)
     if resp.status == 404:
         return {}
     return await resp.json(loads=load_json, encoding='utf-8')
 
 
-async def async_get_start_level(default_level: int = -10) -> int:
+async def _start_level_reached() -> Tuple[bool, Union[None, int]]:
+    start_level_min = HABApp.CONFIG.openhab.general.min_start_level
+
     system_info = await async_get_system_info()
-    return system_info.get('systemInfo', {}).get('startLevel', default_level)
+    start_level_is = system_info.get('systemInfo', {}).get('startLevel')    # type: Optional[int]
+
+    if start_level_is is None:
+        return False, None
+
+    return start_level_is >= start_level_min, start_level_is
+
+
+WAITED_FOR_OPENHAB: bool = False
 
 
 async def wait_for_min_start_level():
+    global WAITED_FOR_OPENHAB
 
-    waited_for_oh = False
-    last_level = -100
+    level_reached, level = await _start_level_reached()
+    if level_reached:
+        return None
 
-    while True:
-        start_level_is = await async_get_start_level()
-        start_level_min = HABApp.CONFIG.openhab.general.min_start_level
-        if start_level_is >= start_level_min:
-            break
+    WAITED_FOR_OPENHAB = True
+    log.info('Waiting for openHAB startup to be complete')
 
-        # show msg only once
-        if not waited_for_oh:
-            log.info('Waiting for openHAB startup to be complete')
+    last_level: int = -100
 
-        # show start level change
-        if last_level != start_level_is:
-            log.debug(f'Startlevel: {start_level_is}')
-        last_level = start_level_is
+    timeout_duration = 10 * 60
+    timeout_start_at_level = 70
+    timeout_timestamp = 0
 
-        # wait for openhab
-        waited_for_oh = True
+    while not level_reached:
         await asyncio.sleep(1)
 
-    # Startup complete
-    if waited_for_oh:
-        log.info('openHAB startup complete')
+        level_reached, level = await _start_level_reached()
+
+        # show start level change
+        if last_level != level:
+            if level is None:
+                log.debug('Start level: not received!')
+                level = -10
+            else:
+                log.debug(f'Start level: {level}')
+
+            # Wait but start eventually because sometimes we have a thing that prevents the start level from advancing
+            # This is a safety net, so we properly start e.g. after a power outage
+            # When starting manually one should fix the blocking thing
+            if level >= timeout_start_at_level:
+                timeout_timestamp = monotonic()
+                log.debug('Starting start level timeout')
+
+        # timeout is running
+        if timeout_timestamp and monotonic() - timeout_timestamp > timeout_duration:
+            log.warning(f'Starting even though openHAB is not ready yet (start level: {level})')
+            break
+
+        # update last level!
+        last_level = level
+
+    log.info('openHAB startup complete')
 
 
 async def try_connect():
-    global IS_ONLINE
+    global IS_ONLINE, OH_3
 
     while True:
         try:
             # sleep before reconnect
             await CONNECT_WAIT.wait()
 
             log.debug('Trying to connect to OpenHAB ...')
-            root = await async_get_root()
+            if (root := await async_get_root()) is None:
+                root = {}
 
             # It's possible that we get status 4XX during startup and then the response is empty
             runtime_info = root.get('runtimeInfo')
             if not runtime_info:
                 log.info('... offline!')
                 continue
 
@@ -404,14 +449,17 @@
 
             # todo: remove this 2023
             # Show warning (convenience)
             vers = tuple(map(int, runtime_info["version"].split('.')[:2]))
             if vers < (3, 3):
                 log.warning('HABApp requires at least openHAB version 3.3!')
 
+            if vers < (4, 0):
+                OH_3 = True
+
             # wait for openhab startup to be complete
             await wait_for_min_start_level()
             break
         except Exception as e:
             if isinstance(e, (OpenhabDisconnectedError, ExpectedSuccessFromOpenhab)):
                 log.info('... offline!')
             else:
```

### Comparing `HABApp-1.0.8/src/HABApp/openhab/connection_handler/http_connection_waiter.py` & `HABApp-1.1.0/src/HABApp/openhab/connection_handler/http_connection_waiter.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 class WaitBetweenConnects:
     def __init__(self):
         self.last_try: float = 0
         self.wait_time = 0
 
     async def wait(self):
 
-        # wenn wir lang connected sind oder beim ersten mal versuchen wir den reconnect gleich
+        # wenn wir lang connected sind oder beim ersten Mal versuchen wir den reconnect gleich
         if time.time() - self.last_try > MAX_WAIT:
             wait = 0
         else:
             wait = self.wait_time
             wait = wait * 2 if wait <= 16 else wait + 8
             wait = max(wait, 1)
             wait = min(wait, MAX_WAIT)
```

### Comparing `HABApp-1.0.8/src/HABApp/openhab/connection_handler/sse_handler.py` & `HABApp-1.1.0/src/HABApp/openhab/connection_handler/sse_handler.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,59 +6,60 @@
 import HABApp.openhab.events
 from HABApp.core.errors import ItemNotFoundException
 from HABApp.core.events import ValueUpdateEvent, ValueChangeEvent
 from HABApp.core.internals import uses_post_event, uses_get_item
 from HABApp.core.logger import log_warning
 from HABApp.core.wrapper import process_exception
 from HABApp.openhab.connection_handler import http_connection
-from HABApp.openhab.events import GroupItemStateChangedEvent, ItemAddedEvent, ItemRemovedEvent, ItemUpdatedEvent, \
+from HABApp.openhab.definitions.topics import TOPIC_THINGS, TOPIC_ITEMS
+from HABApp.openhab.events import GroupStateChangedEvent, GroupStateUpdatedEvent, \
+    ItemAddedEvent, ItemRemovedEvent, ItemUpdatedEvent, \
     ThingStatusInfoEvent, ThingAddedEvent, ThingRemovedEvent, ThingUpdatedEvent, ThingConfigStatusInfoEvent
 from HABApp.openhab.item_to_reg import add_to_registry, remove_from_registry, remove_thing_from_registry, \
     add_thing_to_registry
 from HABApp.openhab.map_events import get_event
 from HABApp.openhab.map_items import map_item
-from HABApp.openhab.definitions.topics import TOPIC_THINGS, TOPIC_ITEMS
 
 log = http_connection.log
 
 
 post_event = uses_post_event()
 get_item = uses_get_item()
 
 
-def on_sse_event(event_dict: dict):
+def on_sse_event(event_dict: dict, oh_3: bool):
     try:
         # Lookup corresponding OpenHAB event
         event = get_event(event_dict)
 
         # Update item in registry BEFORE posting to the event bus
         # so the items have the correct state when we process the event in a rule
         try:
             if isinstance(event, ValueUpdateEvent):
                 __item = get_item(event.name)  # type: HABApp.core.items.base_valueitem.BaseValueItem
                 __item.set_value(event.value)
                 post_event(event.name, event)
                 return None
 
             if isinstance(event, ValueChangeEvent):
+                # Workaround because there is no GroupItemStateEvent in OH3
+                if oh_3 and isinstance(event, GroupStateChangedEvent):
+                    __item = get_item(event.name)  # type: HABApp.openhab.items.GroupItem
+                    __item.set_value(event.value)
+                    # Manually issue an GroupStateUpdatedEvent so we are consistent with OH4 behavior
+                    post_event(event.name, GroupStateUpdatedEvent(event.name, event.item, event.value))
                 post_event(event.name, event)
                 return None
 
             if isinstance(event, (ThingStatusInfoEvent, ThingUpdatedEvent, ThingConfigStatusInfoEvent)):
                 __thing = get_item(event.name)   # type: HABApp.openhab.items.Thing
                 __thing.process_event(event)
                 post_event(event.name, event)
                 return None
 
-            # Workaround because there is no GroupItemStateEvent
-            if isinstance(event, GroupItemStateChangedEvent):
-                __item = get_item(event.name)  # type: HABApp.openhab.items.GroupItem
-                __item.set_value(event.value)
-                post_event(event.name, event)
-                return None
         except ItemNotFoundException:
             log_warning(log, f'Received {event.__class__.__name__} for {event.name} but item does not exist!')
 
             # Post the event anyway
             post_event(event.name, event)
             return None
```

### Comparing `HABApp-1.0.8/src/HABApp/openhab/connection_logic/_plugin.py` & `HABApp-1.1.0/src/HABApp/openhab/connection_logic/_plugin.py`

 * *Files 10% similar despite different names*

```diff
@@ -34,19 +34,23 @@
         self.fut: Optional[asyncio.Future] = None
 
     def setup(self):
         pass
 
     def on_connect(self):
         self.fut = asyncio.create_task(self.on_connect_function())
+        self.fut.add_done_callback(self._connect_function_complete)
+
+    def _connect_function_complete(self, fut: asyncio.Future):
+        if self.fut is fut:
+            self.fut = None
 
     def on_disconnect(self):
-        if self.fut is not None:
+        if self.fut is not None and not self.fut.done():
             self.fut.cancel()
-            self.fut = None
 
     async def on_connect_function(self):
         raise NotImplementedError()
 
 
 PLUGINS: List[PluginBase] = []
```

### Comparing `HABApp-1.0.8/src/HABApp/openhab/connection_logic/connection.py` & `HABApp-1.1.0/src/HABApp/openhab/connection_logic/connection.py`

 * *Files identical despite different names*

### Comparing `HABApp-1.0.8/src/HABApp/openhab/connection_logic/plugin_ping.py` & `HABApp-1.1.0/src/HABApp/openhab/connection_logic/plugin_ping.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 
         if not HABApp.config.CONFIG.openhab.ping.enabled:
             return None
 
         self.listener = HABApp.core.internals.EventBusListener(
             HABApp.config.CONFIG.openhab.ping.item,
             HABApp.core.internals.wrap_func(self.ping_received),
-            HABApp.core.events.EventFilter(HABApp.openhab.events.ItemStateEvent)
+            HABApp.core.events.EventFilter(HABApp.openhab.events.ItemStateUpdatedEvent)
         )
         EVENT_BUS.add_listener(self.listener)
 
         self.on_connect()
 
     async def ping_received(self, event: HABApp.openhab.events.ItemStateEvent):
         value = event.value
@@ -98,15 +98,15 @@
             while True:
 
                 self.ping_value = self.ping_new
                 self.ping_new = None
                 self.ping_sent = time.time()
 
                 if send_ping:
-                    await HABApp.openhab.interface_async.async_post_update(
+                    HABApp.openhab.interface_async.async_post_update(
                         item_name,
                         f'{self.ping_value:.1f}' if self.ping_value is not None else None
                     )
                 else:
                     send_ping = ITEM_REGISTRY.item_exists(item_name)
 
                 await asyncio.sleep(HABApp.config.CONFIG.openhab.ping.interval)
```

### Comparing `HABApp-1.0.8/src/HABApp/openhab/connection_logic/plugin_thing_overview.py` & `HABApp-1.1.0/src/HABApp/openhab/connection_logic/plugin_thing_overview.py`

 * *Files identical despite different names*

### Comparing `HABApp-1.0.8/src/HABApp/openhab/connection_logic/plugin_things/cfg_validator.py` & `HABApp-1.1.0/src/HABApp/openhab/connection_logic/plugin_things/cfg_validator.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from typing import Iterator, Optional, Union
 
 from pydantic import BaseModel, Field, ValidationError, parse_obj_as, validator
 
 from HABApp.core.logger import HABAppError
 from HABApp.openhab.connection_logic.plugin_things.filters import ChannelFilter, ThingFilter
 from HABApp.openhab.connection_logic.plugin_things.str_builder import StrBuilder
-from HABApp.openhab.definitions.definitions import ITEM_TYPES
+from HABApp.openhab.definitions import ITEM_TYPES
 from ._log import log
 
 RE_VALID_NAME = re.compile(r'\w+')
 
 
 @dataclass
 class UserItem:
```

### Comparing `HABApp-1.0.8/src/HABApp/openhab/connection_logic/plugin_things/file_writer/formatter.py` & `HABApp-1.1.0/src/HABApp/openhab/connection_logic/plugin_things/file_writer/formatter.py`

 * *Files identical despite different names*

### Comparing `HABApp-1.0.8/src/HABApp/openhab/connection_logic/plugin_things/file_writer/formatter_builder.py` & `HABApp-1.1.0/src/HABApp/openhab/connection_logic/plugin_things/file_writer/formatter_builder.py`

 * *Files identical despite different names*

### Comparing `HABApp-1.0.8/src/HABApp/openhab/connection_logic/plugin_things/file_writer/writer.py` & `HABApp-1.1.0/src/HABApp/openhab/connection_logic/plugin_things/file_writer/writer.py`

 * *Files identical despite different names*

### Comparing `HABApp-1.0.8/src/HABApp/openhab/connection_logic/plugin_things/filters.py` & `HABApp-1.1.0/src/HABApp/openhab/connection_logic/plugin_things/filters.py`

 * *Files identical despite different names*

### Comparing `HABApp-1.0.8/src/HABApp/openhab/connection_logic/plugin_things/item_worker.py` & `HABApp-1.1.0/src/HABApp/openhab/connection_logic/plugin_things/item_worker.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     async_remove_item, async_create_channel_link, async_get_items, \
     async_remove_channel_link, async_remove_metadata, async_set_metadata, async_get_item_with_habapp_meta
 from HABApp.openhab.definitions.rest.habapp_data import HABAppThingPluginData, load_habapp_meta
 from ._log import log_item as log
 from .cfg_validator import UserItem
 
 
-def _filter_items(i):
+def _filter_items(i: dict):
     if not i.get('editable', False):
         return False
 
     if 'HABApp' not in i.setdefault('metadata', {}):
         return False
 
     load_habapp_meta(i)
```

### Comparing `HABApp-1.0.8/src/HABApp/openhab/connection_logic/plugin_things/plugin_things.py` & `HABApp-1.1.0/src/HABApp/openhab/connection_logic/plugin_things/plugin_things.py`

 * *Files identical despite different names*

### Comparing `HABApp-1.0.8/src/HABApp/openhab/connection_logic/plugin_things/str_builder.py` & `HABApp-1.1.0/src/HABApp/openhab/connection_logic/plugin_things/str_builder.py`

 * *Files identical despite different names*

### Comparing `HABApp-1.0.8/src/HABApp/openhab/connection_logic/plugin_things/thing_config.py` & `HABApp-1.1.0/src/HABApp/openhab/connection_logic/plugin_things/thing_config.py`

 * *Files identical despite different names*

### Comparing `HABApp-1.0.8/src/HABApp/openhab/connection_logic/plugin_things/thing_worker.py` & `HABApp-1.1.0/src/HABApp/openhab/connection_logic/plugin_things/thing_worker.py`

 * *Files identical despite different names*

### Comparing `HABApp-1.0.8/src/HABApp/openhab/definitions/definitions.py` & `HABApp-1.1.0/src/HABApp/openhab/definitions/items.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,18 @@
-from enum import Enum as _Enum
 import typing
+from enum import Enum as _Enum
+
+from HABApp.core.const.const import StrEnum
 
 
 def _get_str_enum_values(obj: typing.Type[_Enum]) -> typing.Set[str]:
     return {_member.value for _member in obj}
 
 
-class ItemType(str, _Enum):
+class ItemType(StrEnum):
     STRING = 'String'
     NUMBER = 'Number'
     SWITCH = 'Switch'
     CONTACT = 'Contact'
     DIMMER = 'Dimmer'
     ROLLERSHUTTER = 'Rollershutter'
     COLOR = 'Color'
@@ -21,15 +23,15 @@
     IMAGE = 'Image'
     CALL = 'Call'
 
 
 ITEM_TYPES: typing.Final = _get_str_enum_values(ItemType)
 
 
-class ItemDimensions(str, _Enum):
+class ItemDimensions(StrEnum):
     ACCELERATION = 'Acceleration'
     ANGLE = 'Angle'
     AREAL_DENSITY = 'ArealDensity'
     CATALYTIC_ACTIVITY = 'CatalyticActivity'
     DATA_AMOUNT = 'DataAmount'
     DATA_TRANSFER_RATE = 'DataTransferRate'
     DENSITY = 'Density'
@@ -65,15 +67,15 @@
     VOLUME = 'Volume'
     VOLUMETRIC_FLOW_RATE = 'VolumetricFlowRate'
 
 
 ITEM_DIMENSIONS: typing.Final = _get_str_enum_values(ItemDimensions)
 
 
-class GroupItemFunctions(str, _Enum):
+class GroupItemFunctions(StrEnum):
     AND = 'AND'
     AVG = 'AVG'
     MAX = 'MAX'
     MIN = 'MIN'
     NAND = 'NAND'
     NOR = 'NOR'
     OR = 'OR'
```

### Comparing `HABApp-1.0.8/src/HABApp/openhab/definitions/helpers/log_table.py` & `HABApp-1.1.0/src/HABApp/openhab/definitions/helpers/log_table.py`

 * *Files identical despite different names*

### Comparing `HABApp-1.0.8/src/HABApp/openhab/definitions/helpers/persistence_data.py` & `HABApp-1.1.0/src/HABApp/openhab/definitions/helpers/persistence_data.py`

 * *Files identical despite different names*

### Comparing `HABApp-1.0.8/src/HABApp/openhab/definitions/rest/habapp_data.py` & `HABApp-1.1.0/src/HABApp/openhab/definitions/rest/habapp_data.py`

 * *Files identical despite different names*

### Comparing `HABApp-1.0.8/src/HABApp/openhab/definitions/rest/items.py` & `HABApp-1.1.0/src/HABApp/openhab/definitions/rest/items.py`

 * *Files identical despite different names*

### Comparing `HABApp-1.0.8/src/HABApp/openhab/definitions/rest/things.py` & `HABApp-1.1.0/src/HABApp/openhab/definitions/rest/things.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from typing import Any, Dict, Optional, Tuple
 
-from pydantic import BaseModel, Field, validator
+from pydantic import BaseModel, Field
+
+from HABApp.openhab.definitions import ThingStatusEnum, ThingStatusDetailEnum
 
 
 class OpenhabThingChannelDefinition(BaseModel):
     uid: str
     id: str
     channel_type: str = Field(..., alias='channelTypeUID')
     kind: str
@@ -17,22 +19,18 @@
     default_tags: Tuple[str, ...] = Field(default_factory=tuple, alias='defaultTags')
 
     properties: Dict[str, Any] = Field(default_factory=dict)
     configuration: Dict[str, Any] = Field(default_factory=dict)
 
 
 class OpenhabThingStatus(BaseModel):
-    status: str
-    detail: str = Field(..., alias='statusDetail')
+    status: ThingStatusEnum
+    detail: ThingStatusDetailEnum = Field(..., alias='statusDetail')
     description: Optional[str] = None
 
-    @validator('detail')
-    def _parse_detail(cls, v):
-        return '' if v == 'NONE' else v
-
 
 class OpenhabThingDefinition(BaseModel):
     # These are mandatory fields
     editable: bool
     status: OpenhabThingStatus = Field(..., alias='statusInfo')
     thing_type: str = Field(..., alias='thingTypeUID')
     uid: str = Field(..., alias='UID')
```

### Comparing `HABApp-1.0.8/src/HABApp/openhab/definitions/values.py` & `HABApp-1.1.0/src/HABApp/openhab/definitions/values.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-import base64
-import typing
+from base64 import b64decode
+from typing import Tuple, Union
 
 from HABApp.core.events import ComplexEventValue
 
 
 class OnOffValue(ComplexEventValue):
     ON = 'ON'
     OFF = 'OFF'
@@ -57,38 +57,60 @@
     def __init__(self, value: str):
         super().__init__(tuple(float(k) for k in value.split(',')))
 
     def __str__(self):
         return f'{self.value[0]}°,{self.value[1]}%,{self.value[2]}%'
 
 
+class PointValue(ComplexEventValue):
+    def __init__(self, value: str):
+        ret = []
+        for k in value.split(','):
+            if k is None:
+                ret.append(k)
+            else:
+                ret.append(float(k))
+        super().__init__(tuple(ret))
+
+    def __str__(self):
+        if len(self.value) == 2:
+            return f'{self.value[0]},{self.value[1]},'
+        else:
+            return f'{self.value[0]},{self.value[1]},{self.value[2]}'
+
+
 class QuantityValue(ComplexEventValue):
 
     @staticmethod
-    def split_unit(value: str) -> typing.Tuple[str, str]:
+    def split_unit(value: str) -> Tuple[str, str]:
         p = value.rfind(' ')
         # dimensionless has no unit
         if p < 0:
             return value, ''
         val = value[0:p]
         unit = value[p + 1:]
         return val, unit
 
     def __init__(self, value: str):
         value, unit = QuantityValue.split_unit(value)
         try:
-            val: typing.Union[int, float] = int(value)
+            val: Union[int, float] = int(value)
         except ValueError:
             val = float(value)
         super().__init__(val)
         self.unit = unit
 
     def __str__(self):
         return f'{self.value} {self.unit}'
 
+    def __eq__(self, other):
+        if not isinstance(other, QuantityValue):
+            return NotImplemented
+        return self.value == other.value and self.unit == other.unit
+
 
 class RawValue(ComplexEventValue):
     def __init__(self, value: str):
         # The data is in this format
         # data:image/png;base64,iVBORw0KGgo....
 
         # extract the contents from "data:"
@@ -97,11 +119,11 @@
 
         # this is our encoded payload
         sep_enc = value.find(',', sep_type)
         encoding = value[sep_type + 1: sep_enc]
         assert encoding == 'base64', f'"{encoding}"'
 
         # set the bytes as value
-        super().__init__(base64.b64decode(value[sep_enc + 1:]))
+        super().__init__(b64decode(value[sep_enc + 1:]))
 
     def __str__(self):
         return f'{self.type}'
```

### Comparing `HABApp-1.0.8/src/HABApp/openhab/errors.py` & `HABApp-1.1.0/src/HABApp/openhab/errors.py`

 * *Files identical despite different names*

### Comparing `HABApp-1.0.8/src/HABApp/openhab/events/__init__.py` & `HABApp-1.1.0/src/HABApp/openhab/events/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 from .base_event import OpenhabEvent
-from .item_events import ItemStateEvent, ItemStateChangedEvent, ItemCommandEvent, ItemAddedEvent,\
-    ItemUpdatedEvent, ItemRemovedEvent, ItemStatePredictedEvent, GroupItemStateChangedEvent
+from .item_events import ItemStateEvent, ItemStateUpdatedEvent, ItemStateChangedEvent, ItemCommandEvent, ItemAddedEvent,\
+    ItemUpdatedEvent, ItemRemovedEvent, ItemStatePredictedEvent, GroupStateUpdatedEvent, GroupStateChangedEvent
 from .channel_events import ChannelTriggeredEvent, ChannelDescriptionChangedEvent
 from .thing_events import ThingStatusInfoChangedEvent, ThingStatusInfoEvent, \
     ThingFirmwareStatusInfoEvent, ThingAddedEvent, ThingRemovedEvent, ThingUpdatedEvent, ThingConfigStatusInfoEvent
-from .event_filters import ItemStateEventFilter, ItemStateChangedEventFilter, ItemCommandEventFilter
+from .event_filters import ItemStateUpdatedEventFilter, ItemStateChangedEventFilter, ItemCommandEventFilter
```

### Comparing `HABApp-1.0.8/src/HABApp/openhab/events/channel_events.py` & `HABApp-1.1.0/src/HABApp/openhab/events/channel_events.py`

 * *Files identical despite different names*

### Comparing `HABApp-1.0.8/src/HABApp/openhab/events/event_filters.py` & `HABApp-1.1.0/src/HABApp/openhab/events/event_filters.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from typing import Any
 
 from HABApp.core.const import MISSING
 from HABApp.core.events.filter.event import TypeBoundEventFilter
-from . import ItemStateChangedEvent, ItemStateEvent, ItemCommandEvent
+from . import ItemStateChangedEvent, ItemStateUpdatedEvent, ItemCommandEvent
 
 
-class ItemStateEventFilter(TypeBoundEventFilter):
+class ItemStateUpdatedEventFilter(TypeBoundEventFilter):
     def __init__(self, value: Any = MISSING):
-        super().__init__(ItemStateEvent, value=value)
+        super().__init__(ItemStateUpdatedEvent, value=value)
 
 
 class ItemStateChangedEventFilter(TypeBoundEventFilter):
     def __init__(self, value: Any = MISSING, old_value: Any = MISSING):
         super().__init__(ItemStateChangedEvent, value=value, old_value=old_value)
```

### Comparing `HABApp-1.0.8/src/HABApp/openhab/events/item_events.py` & `HABApp-1.1.0/src/HABApp/openhab/events/item_events.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,77 +1,60 @@
-from typing import Any, FrozenSet, Optional
+from typing import Any, FrozenSet, Optional, Final
 
 import HABApp.core
 from .base_event import OpenhabEvent
 from ..map_values import map_openhab_values
 
 
 class ItemStateEvent(OpenhabEvent, HABApp.core.events.ValueUpdateEvent):
-    """
-    :ivar str name:
-    :ivar value:
-    """
-    name: str
-    value: Any
-
-    def __init__(self, name: str = '', value: Any = None):
-        super().__init__()
-
-        # smarthome/items/NAME/state
-        self.name: str = name
-        self.value: Any = value
 
     @classmethod
     def from_dict(cls, topic: str, payload: dict):
-        # smarthome/items/NAME/state
+        # openhab/items/NAME/state
         return cls(topic[14:-6], map_openhab_values(payload['type'], payload['value']))
 
     def __repr__(self):
         return f'<{self.__class__.__name__} name: {self.name}, value: {self.value}>'
 
 
-class ItemStateChangedEvent(OpenhabEvent, HABApp.core.events.ValueChangeEvent):
-    """
-    :ivar str name:
-    :ivar value:
-    :ivar old_value:
-    """
-    name: str
-    value: Any
-    old_value: Any
+class ItemStateUpdatedEvent(OpenhabEvent, HABApp.core.events.ValueUpdateEvent):
 
-    def __init__(self, name: str = '', value: Any = None, old_value: Any = None):
-        super().__init__()
+    @classmethod
+    def from_dict(cls, topic: str, payload: dict):
+        # openhab/items/NAME/stateupdated
+        return cls(topic[14:-13], map_openhab_values(payload['type'], payload['value']))
 
-        self.name: str = name
-        self.value: Any = value
-        self.old_value: Any = old_value
+    def __repr__(self):
+        return f'<{self.__class__.__name__} name: {self.name}, value: {self.value}>'
+
+
+class ItemStateChangedEvent(OpenhabEvent, HABApp.core.events.ValueChangeEvent):
 
     @classmethod
     def from_dict(cls, topic: str, payload: dict):
-        # smarthome/items/Ping/statechanged
+        # openhab/items/Ping/statechanged
         return cls(
             topic[14:-13],
             map_openhab_values(payload['type'], payload['value']),
             map_openhab_values(payload['oldType'], payload['oldValue'])
         )
 
     def __repr__(self):
         return f'<{self.__class__.__name__} name: {self.name}, value: {self.value}, old_value: {self.old_value}>'
 
 
 class ItemCommandEvent(OpenhabEvent):
     """
     :ivar str name:
-    :ivar value:
+    :ivar Any value:
     """
     name: str
     value: Any
 
-    def __init__(self, name: str = '', value: Any = None):
+    def __init__(self, name: str, value: Any):
         super().__init__()
 
         self.name: str = name
         self.value: Any = value
 
     @classmethod
     def from_dict(cls, topic: str, payload: dict):
@@ -83,36 +66,36 @@
 
 
 class ItemAddedEvent(OpenhabEvent):
     """
     :ivar str name:
     :ivar str type:
     :ivar Optional[str] label:
-    :ivar Tuple[str,...] tags:
-    :ivar Tuple[str,...] group_names:
+    :ivar FrozenSet[str] tags:
+    :ivar FrozenSet[str] groups:
     """
     name: str
     type: str
     label: Optional[str]
     tags: FrozenSet[str]
     groups: FrozenSet[str]
 
-    def __init__(self, name: str = '', type: str = '', label: Optional[str] = None,
-                 tags: FrozenSet[str] = frozenset(), group_names: FrozenSet[str] = frozenset()):
+    def __init__(self, name: str, type: str, label: Optional[str],
+                 tags: FrozenSet[str], group_names: FrozenSet[str]):
         super().__init__()
 
         self.name: str = name
         self.type: str = type
         self.label: Optional[str] = label
         self.tags: FrozenSet[str] = tags
         self.groups: FrozenSet[str] = group_names
 
     @classmethod
     def from_dict(cls, topic: str, payload: dict):
-        # {'topic': 'smarthome/items/NAME/added'
+        # {'topic': 'openhab/items/NAME/added'
         # 'payload': '{"type":"Contact","name":"Test","tags":[],"groupNames":[]}'
         # 'type': 'ItemAddedEvent'}
         return cls(
             payload['name'], payload['type'], label=payload.get('label'),
             tags=frozenset(payload['tags']), group_names=frozenset(payload['groupNames'])
         )
 
@@ -122,36 +105,37 @@
         return f'<{self.__class__.__name__} name: {self.name}, type: {self.type}, tags:{tags}, groups:{grps}>'
 
 
 class ItemUpdatedEvent(OpenhabEvent):
     """
     :ivar str name:
     :ivar str type:
-    :ivar Tuple[str,...] tags:
-    :ivar Tuple[str,...] group_names:
+    :ivar Optional[str] label:
+    :ivar FrozenSet[str] tags:
+    :ivar FrozenSet[str] groups:
     """
     name: str
     type: str
     label: Optional[str]
     tags: FrozenSet[str]
     groups: FrozenSet[str]
 
-    def __init__(self, name: str = '', type: str = '', label: Optional[str] = None,
-                 tags: FrozenSet[str] = frozenset(), group_names: FrozenSet[str] = frozenset()):
+    def __init__(self, name: str, type: str, label: Optional[str],
+                 tags: FrozenSet[str], group_names: FrozenSet[str]):
         super().__init__()
 
         self.name: str = name
         self.type: str = type
         self.label: Optional[str] = label
         self.tags: FrozenSet[str] = tags
         self.groups: FrozenSet[str] = group_names
 
     @classmethod
     def from_dict(cls, topic: str, payload: dict):
-        # smarthome/items/NAME/updated
+        # openhab/items/NAME/updated
         # 'payload': '[{"type":"Switch","name":"Test","tags":[],"groupNames":[]},
         #              {"type":"Contact","name":"Test","tags":[],"groupNames":[]}]',
         # 'type': 'ItemUpdatedEvent'
         new = payload[0]
         return cls(
             topic[14:-8], new['type'], label=new.get('label'),
             tags=frozenset(new['tags']), group_names=frozenset(new['groupNames'])
@@ -165,79 +149,96 @@
 
 class ItemRemovedEvent(OpenhabEvent):
     """
     :ivar str name:
     """
     name: str
 
-    def __init__(self, name: str = ''):
+    def __init__(self, name: str):
         super().__init__()
-
         self.name = name
 
     @classmethod
     def from_dict(cls, topic: str, payload: dict):
         # smarthome/items/Test/removed
         return cls(topic[14:-8])
 
     def __repr__(self):
         return f'<{self.__class__.__name__} name: {self.name}>'
 
 
 class ItemStatePredictedEvent(OpenhabEvent):
     """
     :ivar str name:
-    :ivar value:
+    :ivar Any value:
     """
     name: str
     value: Any
 
-    def __init__(self, name: str = '', value: Any = None):
+    def __init__(self, name: str, value: Any):
         super().__init__()
-
-        # smarthome/items/NAME/state
-        self.name: str = name
-        self.value: Any = value
+        self.name: Final = name
+        self.value: Final = value
 
     @classmethod
     def from_dict(cls, topic: str, payload: dict):
-        # 'smarthome/items/NAME/statepredicted'
+        # 'openhab/items/NAME/statepredicted'
         return cls(topic[14:-15], map_openhab_values(payload['predictedType'], payload['predictedValue']))
 
     def __repr__(self):
         return f'<{self.__class__.__name__} name: {self.name}, value: {self.value}>'
 
 
-class GroupItemStateChangedEvent(OpenhabEvent):
+class GroupStateUpdatedEvent(OpenhabEvent, HABApp.core.events.ValueUpdateEvent):
+    """
+    :ivar str name: Group name
+    :ivar str item: Group item that caused the update
+    :ivar Any value:
+    """
+    name: str
+    item: str
+    value: Any
+
+    def __init__(self, name: str, item: str, value: Any):
+        super().__init__(name, value)
+        self.item: Final = item
+
+    @classmethod
+    def from_dict(cls, topic: str, payload: dict):
+        # openhab/items/GroupItem/ItemThatChanged/stateupdated
+        parts = topic.split('/')
+        return cls(parts[2], parts[3], map_openhab_values(payload['type'], payload['value']))
+
+    def __repr__(self):
+        return f'<{self.__class__.__name__} name: {self.name}, item: {self.item}, value: {self.value}>'
+
+
+class GroupStateChangedEvent(OpenhabEvent, HABApp.core.events.ValueChangeEvent):
     """
     :ivar str name:
     :ivar str item:
-    :ivar value:
-    :ivar old_value:
+    :ivar Any value:
+    :ivar Any old_value:
     """
     name: str
     item: str
     value: Any
     old_value: Any
 
-    def __init__(self, name: str = '', item: str = '', value: Any = None, old_value: Any = None):
-        super().__init__()
-
-        self.name: str = name
-        self.item: str = item
-
-        self.value: Any = value
-        self.old_value: Any = old_value
+    def __init__(self, name: str, item: str, value: Any, old_value: Any):
+        super().__init__(name, value, old_value)
+        self.item: Final = item
 
     @classmethod
     def from_dict(cls, topic: str, payload: dict):
-        # 'smarthome/items/TestGroupAVG/TestNumber1/statechanged'
+        # 'openhab/items/TestGroupAVG/TestNumber1/statechanged'
         parts = topic.split('/')
 
         return cls(
             parts[2], parts[3],
             map_openhab_values(payload['type'], payload['value']),
             map_openhab_values(payload['oldType'], payload['oldValue'])
         )
 
     def __repr__(self):
-        return f'<{self.__class__.__name__} name: {self.name}, value: {self.value}, old_value: {self.old_value}>'
+        return f'<{self.__class__.__name__} name: {self.name}, item: {self.item}, ' \
+               f'value: {self.value}, old_value: {self.old_value}>'
```

### Comparing `HABApp-1.0.8/src/HABApp/openhab/item_to_reg.py` & `HABApp-1.1.0/src/HABApp/openhab/item_to_reg.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 
 from immutables import Map
 
 import HABApp
 
 from HABApp.core.internals import uses_item_registry
 from HABApp.core.logger import log_warning
+from HABApp.openhab.definitions.things import THING_STATUS_DEFAULT, THING_STATUS_DETAIL_DEFAULT, ThingStatusEnum, \
+    ThingStatusDetailEnum
 
 if TYPE_CHECKING:
     import HABApp.openhab.definitions.rest
 
 log = logging.getLogger('HABApp.openhab.items')
 
 Items = uses_item_registry()
@@ -82,20 +84,22 @@
 # Thing handling
 # ----------------------------------------------------------------------------------------------------------------------
 def add_thing_to_registry(data: Union['HABApp.openhab.definitions.rest.OpenhabThingDefinition',
                                       'HABApp.openhab.events.thing_events.ThingAddedEvent']):
 
     if isinstance(data, HABApp.openhab.events.thing_events.ThingAddedEvent):
         name = data.name
-        status: str = 'UNINITIALIZED'
-        status_detail: str = 'NONE'
+        status: ThingStatusEnum = THING_STATUS_DEFAULT
+        status_detail: ThingStatusDetailEnum = THING_STATUS_DETAIL_DEFAULT
+        status_description: str = ''
     elif isinstance(data, HABApp.openhab.definitions.rest.OpenhabThingDefinition):
         name = data.uid
         status = data.status.status
         status_detail = data.status.detail
+        status_description = data.status.description if data.status.description else ''
     else:
         raise ValueError()
 
     if Items.item_exists(name):
         existing = Items.get_item(name)
         if isinstance(existing, HABApp.openhab.items.Thing):
             new_thing = existing
@@ -105,18 +109,19 @@
             log_warning(log, f'Item type changed from {existing.__class__} to {new_thing.__class__}')
             Items.pop_item(name)
     else:
         new_thing = HABApp.openhab.items.Thing(name=name)
 
     new_thing.status = status
     new_thing.status_detail = status_detail
+    new_thing.status_description = status_description
     new_thing.label = data.label
+    new_thing.location = data.location
     new_thing.configuration = Map(data.configuration)
     new_thing.properties = Map(data.properties)
-    Items.add_item(new_thing)
-    return None
+    return Items.add_item(new_thing)
 
 
 def remove_thing_from_registry(name: str):
     if not Items.item_exists(name):
         return None
     return Items.pop_item(name)
```

### Comparing `HABApp-1.0.8/src/HABApp/openhab/items/base_item.py` & `HABApp-1.1.0/src/HABApp/openhab/items/base_item.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,29 +22,35 @@
 
     :ivar Optional[str] label:
     :ivar FrozenSet[str] tags:
     :ivar FrozenSet[str] groups:
     :ivar Mapping[str, MetaData] metadata:
     """
 
-    def __init__(self, name: str, initial_value=None,
+    def __init__(self, name: str, initial_value: Any = None,
                  label: Optional[str] = None, tags: FrozenSet[str] = frozenset(), groups: FrozenSet[str] = frozenset(),
                  metadata: Mapping[str, MetaData] = Map()):
         super().__init__(name, initial_value)
         self.label: Optional[str] = label
         self.tags: FrozenSet[str] = tags
         self.groups: FrozenSet[str] = groups
         self.metadata: Mapping[str, MetaData] = metadata
 
     @classmethod
     def from_oh(cls, name: str, value=None,
                 label: Optional[str] = None, tags: FrozenSet[str] = frozenset(), groups: FrozenSet[str] = frozenset(),
                 metadata: Mapping[str, MetaData] = Map()):
+        if value is not None:
+            value = cls._state_from_oh_str(value)
         return cls(name, value, label=label, tags=tags, groups=groups, metadata=metadata)
 
+    @staticmethod
+    def _state_from_oh_str(state: str):
+        raise NotImplementedError()
+
     def oh_send_command(self, value: Any = MISSING):
         """Send a command to the openHAB item
 
         :param value: (optional) value to be sent. If not specified the current item value will be used.
         """
         send_command(self.name, self.value if value is MISSING else value)
 
@@ -71,15 +77,15 @@
         :param lower_than: item state has to be lower than the passed value
         :param lt: item state has to be lower than the passed value
         :param lower_equal: item state has to be lower equal the passed value
         :param le: item state has to be lower equal the passed value
         :param greater_than: item state has to be greater than the passed value
         :param gt: item state has to be greater than the passed value
         :param greater_equal: item state has to be greater equal the passed value
-        :param ge: tem state has to be greater equal the passed value
+        :param ge: item state has to be greater equal the passed value
         :param is_: item state has to be the same object as the passt value (e.g. None)
         :param is_not: item state has to be not the same object as the passt value (e.g. None)
 
         :return: `True` if the new value was posted else `False`
         """
 
         if _compare(self.value, equal=equal, eq=eq, not_equal=not_equal, ne=ne,
```

### Comparing `HABApp-1.0.8/src/HABApp/openhab/items/call_item.py` & `HABApp-1.1.0/src/HABApp/openhab/items/datetime_item.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,32 @@
-from typing import FrozenSet, Mapping, Optional
-
-from immutables import Map
+from datetime import datetime
+from typing import TYPE_CHECKING, Optional, FrozenSet, Mapping
 
 from HABApp.openhab.items.base_item import OpenhabItem, MetaData
 
+if TYPE_CHECKING:
+    Optional = Optional
+    FrozenSet = FrozenSet
+    Mapping = Mapping
+    MetaData = MetaData
+
 
-class CallItem(OpenhabItem):
-    """CallItem which accepts and converts the data types from OpenHAB
+class DatetimeItem(OpenhabItem):
+    """DateTimeItem which accepts and converts the data types from OpenHAB
 
     :ivar str name:
-    :ivar Tuple[str, ...] value:
+    :ivar datetime value:
 
     :ivar Optional[str] label:
     :ivar FrozenSet[str] tags:
     :ivar FrozenSet[str] groups:
     :ivar Mapping[str, MetaData] metadata:
     """
 
-    @classmethod
-    def from_oh(cls, name: str, value=None, label: Optional[str] = None, tags: FrozenSet[str] = frozenset(),
-                groups: FrozenSet[str] = frozenset(), metadata: Mapping[str, MetaData] = Map()):
-        if value is not None:
-            value = tuple(value.split(','))
-        return cls(name, value, label=label, tags=tags, groups=groups, metadata=metadata)
-
-    def set_value(self, new_value) -> bool:
-        if isinstance(new_value, str):
-            new_value = tuple(new_value.split(','))
-        return super().set_value(new_value)
+    @staticmethod
+    def _state_from_oh_str(state: str):
+        dt = datetime.strptime(state, '%Y-%m-%dT%H:%M:%S.%f%z')
+        # all datetime objs from openHAB have a timezone set so we can't easily compare them
+        # --> TypeError: can't compare offset-naive and offset-aware datetime
+        dt = dt.astimezone(tz=None)  # Changes datetime object so it uses system timezone
+        value = dt.replace(tzinfo=None)  # Removes timezone awareness
+        return value
```

### Comparing `HABApp-1.0.8/src/HABApp/openhab/items/color_item.py` & `HABApp-1.1.0/src/HABApp/openhab/items/color_item.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,30 +22,35 @@
 
     :ivar Optional[str] label:
     :ivar FrozenSet[str] tags:
     :ivar FrozenSet[str] groups:
     :ivar Mapping[str, MetaData] metadata:
     """
 
-    def __init__(self, name: str, h=0.0, s=0.0, b=0.0,
+    def __init__(self, name: str, h: float = 0.0, s: float = 0.0, b: float = 0.0,
                  label: Optional[str] = None, tags: FrozenSet[str] = frozenset(), groups: FrozenSet[str] = frozenset(),
                  metadata: Mapping[str, MetaData] = Map()):
         super().__init__(name=name, initial_value=(h, s, b), label=label, tags=tags, groups=groups, metadata=metadata)
 
         self.hue: float = min(max(0.0, h), HUE_FACTOR)
         self.saturation: float = min(max(0.0, s), PERCENT_FACTOR)
         self.brightness: float = min(max(0.0, b), PERCENT_FACTOR)
 
+    @staticmethod
+    def _state_from_oh_str(state: str) -> Tuple[float, float, float]:
+        h, s, b = state.split(',')
+        return float(h), float(s), float(b)
+
     @classmethod
     def from_oh(cls, name: str, value=None, label: Optional[str] = None, tags: FrozenSet[str] = frozenset(),
                 groups: FrozenSet[str] = frozenset(), metadata: Mapping[str, MetaData] = Map()):
         if value is None:
             return cls(name, label=label, tags=tags, groups=groups, metadata=metadata)
         return cls(
-            name, *[float(k) for k in value.split(',')], label=label, tags=tags, groups=groups, metadata=metadata)
+            name, *cls._state_from_oh_str(value), label=label, tags=tags, groups=groups, metadata=metadata)
 
     def set_value(self, hue=0.0, saturation=0.0, brightness=0.0):
         """Set the color value
 
         :param hue: hue (in °)
         :param saturation: saturation (in %)
         :param brightness: brightness (in %)
```

### Comparing `HABApp-1.0.8/src/HABApp/openhab/items/commands.py` & `HABApp-1.1.0/src/HABApp/openhab/items/commands.py`

 * *Files identical despite different names*

### Comparing `HABApp-1.0.8/src/HABApp/openhab/items/contact_item.py` & `HABApp-1.1.0/src/HABApp/openhab/items/contact_item.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,21 @@
-from typing import Any
+from typing import Any, TYPE_CHECKING, Optional, FrozenSet, Mapping
 
-from HABApp.openhab.items.base_item import OpenhabItem
+from HABApp.openhab.items.base_item import OpenhabItem, MetaData
 from ..definitions import OpenClosedValue
 from ...core.const import MISSING
 from ..errors import SendCommandNotSupported
 from HABApp.openhab.interface import post_update
 
+if TYPE_CHECKING:
+    Optional = Optional
+    FrozenSet = FrozenSet
+    Mapping = Mapping
+    MetaData = MetaData
+
 
 OPEN = OpenClosedValue.OPEN
 CLOSED = OpenClosedValue.CLOSED
 
 
 class ContactItem(OpenhabItem):
     """ContactItem
@@ -19,14 +25,20 @@
 
     :ivar Optional[str] label:
     :ivar FrozenSet[str] tags:
     :ivar FrozenSet[str] groups:
     :ivar Mapping[str, MetaData] metadata:
     """
 
+    @staticmethod
+    def _state_from_oh_str(state: str):
+        if state != OPEN and state != CLOSED:
+            raise ValueError(f'Invalid value for ContactItem: {state}')
+        return state
+
     def set_value(self, new_value) -> bool:
 
         if isinstance(new_value, OpenClosedValue):
             new_value = new_value.value
 
         if new_value is not None and new_value != OPEN and new_value != CLOSED:
             raise ValueError(f'Invalid value for ContactItem: {new_value}')
```

### Comparing `HABApp-1.0.8/src/HABApp/openhab/items/datetime_item.py` & `HABApp-1.1.0/src/HABApp/openhab/items/number_item.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,30 +1,44 @@
-from datetime import datetime
-from typing import Optional, FrozenSet, Mapping
-
-from immutables import Map
+from typing import Optional, FrozenSet, Mapping, Union, TYPE_CHECKING
 
 from HABApp.openhab.items.base_item import OpenhabItem, MetaData
+from ..definitions import QuantityValue
+
+if TYPE_CHECKING:
+    Union = Union
+    MetaData = MetaData
+    FrozenSet = FrozenSet
+    Mapping = Mapping
 
 
-class DatetimeItem(OpenhabItem):
-    """DateTimeItem which accepts and converts the data types from OpenHAB
+class NumberItem(OpenhabItem):
+    """NumberItem which accepts and converts the data types from OpenHAB
 
     :ivar str name:
-    :ivar datetime value:
+    :ivar Union[int, float] value:
 
     :ivar Optional[str] label:
     :ivar FrozenSet[str] tags:
     :ivar FrozenSet[str] groups:
     :ivar Mapping[str, MetaData] metadata:
     """
 
-    @classmethod
-    def from_oh(cls, name: str, value=None, label: Optional[str] = None, tags: FrozenSet[str] = frozenset(),
-                groups: FrozenSet[str] = frozenset(), metadata: Mapping[str, MetaData] = Map()):
-        if value is not None:
-            dt = datetime.strptime(value, '%Y-%m-%dT%H:%M:%S.%f%z')
-            # all datetime objs from openHAB have a timezone set so we can't easily compare them
-            # --> TypeError: can't compare offset-naive and offset-aware datetime
-            dt = dt.astimezone(tz=None)   # Changes datetime object so it uses system timezone
-            value = dt.replace(tzinfo=None)  # Removes timezone awareness
-        return cls(name, value, label=label, tags=tags, groups=groups, metadata=metadata)
+    @property
+    def unit(self) -> Optional[str]:
+        """Return the item unit if it is a "Unit of Measurement" item else None"""
+        if (unit := self.metadata.get('unit')) is None:
+            return None
+        return unit.value
+
+    @staticmethod
+    def _state_from_oh_str(state: str):
+        try:
+            return int(state)
+        except ValueError:
+            return float(state)
+
+    def set_value(self, new_value) -> bool:
+
+        if isinstance(new_value, QuantityValue):
+            return super().set_value(new_value.value)
+
+        return super().set_value(new_value)
```

### Comparing `HABApp-1.0.8/src/HABApp/openhab/items/dimmer_item.py` & `HABApp-1.1.0/src/HABApp/openhab/items/dimmer_item.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,39 @@
-from typing import Optional, FrozenSet, Mapping
-
-from immutables import Map
+from typing import Union, TYPE_CHECKING, Optional, FrozenSet, Mapping
 
 from HABApp.openhab.items.base_item import OpenhabItem, MetaData
 from HABApp.openhab.items.commands import OnOffCommand, PercentCommand
 from ..definitions import OnOffValue, PercentValue
 
+if TYPE_CHECKING:
+    Union = Union
+    Optional = Optional
+    FrozenSet = FrozenSet
+    Mapping = Mapping
+    MetaData = MetaData
+
 
 class DimmerItem(OpenhabItem, OnOffCommand, PercentCommand):
     """DimmerItem which accepts and converts the data types from OpenHAB
 
     :ivar str name:
     :ivar Union[int, float] value:
 
     :ivar Optional[str] label:
     :ivar FrozenSet[str] tags:
     :ivar FrozenSet[str] groups:
     :ivar Mapping[str, MetaData] metadata:
     """
 
-    @classmethod
-    def from_oh(cls, name: str, value=None, label: Optional[str] = None, tags: FrozenSet[str] = frozenset(),
-                groups: FrozenSet[str] = frozenset(), metadata: Mapping[str, MetaData] = Map()):
-        if value is not None:
-            value = float(value)
-        return cls(name, value, label=label, tags=tags, groups=groups, metadata=metadata)
+    @staticmethod
+    def _state_from_oh_str(state: str):
+        try:
+            return int(state)
+        except ValueError:
+            return float(state)
 
     def set_value(self, new_value) -> bool:
 
         if isinstance(new_value, OnOffValue):
             new_value = 100 if new_value.on else 0
         elif isinstance(new_value, PercentValue):
             new_value = new_value.value
```

### Comparing `HABApp-1.0.8/src/HABApp/openhab/items/image_item.py` & `HABApp-1.1.0/src/HABApp/openhab/items/image_item.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,21 @@
 from base64 import b64encode
-from typing import FrozenSet, Mapping, Optional
+from typing import Any, TYPE_CHECKING, Optional, FrozenSet, Mapping
 
 from immutables import Map
 
 from HABApp.openhab.items.base_item import OpenhabItem, MetaData
 from ..definitions import RawValue
 
+if TYPE_CHECKING:
+    Optional = Optional
+    FrozenSet = FrozenSet
+    Mapping = Mapping
+    MetaData = MetaData
+
 
 def _convert_bytes(data: bytes, img_type: Optional[str]) -> str:
     assert isinstance(data, bytes), type(data)
 
     # try to automatically found out what kind of file we have
     if img_type is None:
         if data.startswith(b'\xFF\xD8\xFF'):
@@ -30,22 +36,26 @@
 
     :ivar Optional[str] label:
     :ivar FrozenSet[str] tags:
     :ivar FrozenSet[str] groups:
     :ivar Mapping[str, MetaData] metadata:
     """
 
-    def __init__(self, name: str, initial_value=None,
-                 label: Optional[str] = None, tags: FrozenSet[str] = frozenset(), groups: FrozenSet[str] = frozenset(),
+    def __init__(self, name: str, initial_value: Any = None, label: Optional[str] = None,
+                 tags: FrozenSet[str] = frozenset(), groups: FrozenSet[str] = frozenset(),
                  metadata: Mapping[str, MetaData] = Map()):
         super().__init__(name, initial_value, label, tags, groups, metadata)
 
         # this item is unique because we also save the image type and thus have two states
         self.image_type: Optional[str] = None
 
+    @staticmethod
+    def _state_from_oh_str(state: str):
+        return RawValue(state).value
+
     @classmethod
     def from_oh(cls, name: str, value=None, label: Optional[str] = None, tags: FrozenSet[str] = frozenset(),
                 groups: FrozenSet[str] = frozenset(), metadata: Mapping[str, MetaData] = Map()):
 
         c = cls(name, value, label=label, tags=tags, groups=groups, metadata=metadata)
         if value is not None:
             c.set_value(RawValue(value))
```

### Comparing `HABApp-1.0.8/src/HABApp/openhab/items/number_item.py` & `HABApp-1.1.0/src/HABApp/openhab/items/rollershutter_item.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,39 +1,51 @@
-from typing import Optional, FrozenSet, Mapping
-
-from immutables import Map
+from typing import TYPE_CHECKING, Optional, FrozenSet, Mapping, Union
 
 from HABApp.openhab.items.base_item import OpenhabItem, MetaData
-from ..definitions import QuantityValue
+from HABApp.openhab.items.commands import UpDownCommand, PercentCommand
+from ..definitions import UpDownValue, PercentValue
+
+if TYPE_CHECKING:
+    Union = Union
+    Optional = Optional
+    FrozenSet = FrozenSet
+    Mapping = Mapping
+    MetaData = MetaData
 
 
-class NumberItem(OpenhabItem):
-    """NumberItem which accepts and converts the data types from OpenHAB
+class RollershutterItem(OpenhabItem, UpDownCommand, PercentCommand):
+    """RollershutterItem which accepts and converts the data types from OpenHAB
 
     :ivar str name:
     :ivar Union[int, float] value:
 
     :ivar Optional[str] label:
     :ivar FrozenSet[str] tags:
     :ivar FrozenSet[str] groups:
     :ivar Mapping[str, MetaData] metadata:
     """
 
-
-    @classmethod
-    def from_oh(cls, name: str, value=None, label: Optional[str] = None, tags: FrozenSet[str] = frozenset(),
-                groups: FrozenSet[str] = frozenset(), metadata: Mapping[str, MetaData] = Map()):
-        if value is None:
-            return cls(name, value, label=label, tags=tags, groups=groups, metadata=metadata)
-
+    @staticmethod
+    def _state_from_oh_str(state: str):
         try:
-            value = int(value)
+            return int(state)
         except ValueError:
-            value = float(value)
-        return cls(name, value, label, tags, groups, metadata)
+            return float(state)
 
     def set_value(self, new_value) -> bool:
 
-        if isinstance(new_value, QuantityValue):
-            return super().set_value(new_value.value)
+        if isinstance(new_value, UpDownValue):
+            new_value = 0 if new_value.up else 100
+        elif isinstance(new_value, PercentValue):
+            new_value = new_value.value
 
+        assert isinstance(new_value, (int, float)) or new_value is None, new_value
         return super().set_value(new_value)
+
+    def is_up(self) -> bool:
+        return self.value <= 0
+
+    def is_down(self) -> bool:
+        return self.value >= 100
+
+    def __str__(self):
+        return self.value
```

### Comparing `HABApp-1.0.8/src/HABApp/openhab/items/rollershutter_item.py` & `HABApp-1.1.0/src/HABApp/openhab/items/tuple_items.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,45 +1,74 @@
-from typing import Optional, FrozenSet, Mapping
-
-from immutables import Map
+from typing import FrozenSet, Mapping, Optional, Tuple, TYPE_CHECKING
 
+from HABApp.openhab.definitions.values import PointValue
 from HABApp.openhab.items.base_item import OpenhabItem, MetaData
-from HABApp.openhab.items.commands import UpDownCommand, PercentCommand
-from ..definitions import UpDownValue, PercentValue
+
+if TYPE_CHECKING:
+    Tuple = Tuple
+    Optional = Optional
+    FrozenSet = FrozenSet
+    Mapping = Mapping
+    MetaData = MetaData
 
 
-class RollershutterItem(OpenhabItem, UpDownCommand, PercentCommand):
-    """RollershutterItem which accepts and converts the data types from OpenHAB
+class CallItem(OpenhabItem):
+    """CallItem which accepts and converts the data types from OpenHAB
 
     :ivar str name:
-    :ivar Union[int, float] value:
+    :ivar Tuple[str, ...] value:
 
     :ivar Optional[str] label:
     :ivar FrozenSet[str] tags:
     :ivar FrozenSet[str] groups:
     :ivar Mapping[str, MetaData] metadata:
     """
 
-    def __init__(self, name: str, initial_value=None, label: Optional[str] = None, tags: FrozenSet[str] = frozenset(),
-                 groups: FrozenSet[str] = frozenset(), metadata: Mapping[str, MetaData] = Map()):
-        if initial_value is not None:
-            initial_value = float(initial_value)
-        super().__init__(name, initial_value, label, tags, groups, metadata)
+    @staticmethod
+    def _state_from_oh_str(state: str):
+        return tuple(state.split(','))
 
     def set_value(self, new_value) -> bool:
+        if isinstance(new_value, str):
+            return super().set_value(tuple(new_value.split(',')))
+
+        if isinstance(new_value, tuple):
+            return super().set_value(new_value)
+
+        assert new_value is None
+        return super().set_value(tuple())
 
-        if isinstance(new_value, UpDownValue):
-            new_value = 0 if new_value.up else 100
-        elif isinstance(new_value, PercentValue):
-            new_value = new_value.value
-
-        assert isinstance(new_value, (int, float)) or new_value is None, new_value
-        return super().set_value(new_value)
 
-    def is_up(self) -> bool:
-        return self.value <= 0
+class LocationItem(OpenhabItem):
+    """LocationItem which accepts and converts the data types from OpenHAB
+
+    :ivar str name:
+    :ivar Optional[Tuple[float, float, Optional[float]]] value:
+
+    :ivar Optional[str] label:
+    :ivar FrozenSet[str] tags:
+    :ivar FrozenSet[str] groups:
+    :ivar Mapping[str, MetaData] metadata:
+    """
+
+    @staticmethod
+    def _state_from_oh_str(state: str):
+        value = tuple(state.split(','))
+        assert 2 <= len(value) <= 3
+        return value
+
+    def set_value(self, new_value) -> bool:
+        if isinstance(new_value, PointValue):
+            return super().set_value(new_value.value)
 
-    def is_down(self) -> bool:
-        return self.value >= 100
+        if new_value is None:
+            return super().set_value(new_value)
 
-    def __str__(self):
-        return self.value
+        if isinstance(new_value, tuple):
+            assert 2 <= len(new_value) <= 3
+            return super().set_value(new_value)
+
+        parts = new_value.split(',')    # type: list[Optional[str]]
+        if len(parts) == 2:
+            parts.append(None)
+        assert len(parts) == 3
+        return super().set_value(tuple(parts))
```

### Comparing `HABApp-1.0.8/src/HABApp/openhab/map_events.py` & `HABApp-1.1.0/src/HABApp/openhab/map_events.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,47 +1,46 @@
 from typing import Dict, Type
 from HABApp.core.const.json import load_json
 
 from .events import OpenhabEvent, \
-    ItemStateEvent, ItemStateChangedEvent, ItemCommandEvent, ItemAddedEvent, \
-    ItemUpdatedEvent, ItemRemovedEvent, ItemStatePredictedEvent, GroupItemStateChangedEvent, \
+    ItemStateEvent, ItemStateUpdatedEvent, ItemStateChangedEvent, ItemCommandEvent, ItemAddedEvent, \
+    ItemUpdatedEvent, ItemRemovedEvent, ItemStatePredictedEvent, \
+    GroupStateUpdatedEvent, GroupStateChangedEvent, \
     ChannelTriggeredEvent, ChannelDescriptionChangedEvent, \
     ThingAddedEvent, ThingRemovedEvent, ThingUpdatedEvent, \
     ThingStatusInfoChangedEvent, ThingStatusInfoEvent, ThingFirmwareStatusInfoEvent, \
     ThingConfigStatusInfoEvent
 
 
 EVENT_LIST = [
     # item events
-    ItemStateEvent, ItemStateChangedEvent, ItemCommandEvent, ItemAddedEvent,
-    ItemUpdatedEvent, ItemRemovedEvent, ItemStatePredictedEvent, GroupItemStateChangedEvent,
+    ItemStateEvent, ItemStateUpdatedEvent, ItemStateChangedEvent, ItemCommandEvent, ItemAddedEvent,
+    ItemUpdatedEvent, ItemRemovedEvent, ItemStatePredictedEvent,
+
+    GroupStateUpdatedEvent, GroupStateChangedEvent,
 
     # channel events
     ChannelTriggeredEvent, ChannelDescriptionChangedEvent,
 
     # thing events
     ThingAddedEvent, ThingRemovedEvent, ThingUpdatedEvent,
     ThingStatusInfoEvent, ThingStatusInfoChangedEvent,
     ThingFirmwareStatusInfoEvent,
     ThingConfigStatusInfoEvent,
 ]
 
 _events: Dict[str, Type[OpenhabEvent]] = {k.__name__: k for k in EVENT_LIST}
+_events['GroupItemStateChangedEvent'] = GroupStateChangedEvent       # Naming from openHAB is inconsistent here
 _events['FirmwareStatusInfoEvent'] = ThingFirmwareStatusInfoEvent    # Naming from openHAB is inconsistent here
 _events['ConfigStatusInfoEvent'] = ThingConfigStatusInfoEvent        # Naming from openHAB is inconsistent here
 
 
 def get_event(_in_dict: dict) -> OpenhabEvent:
     event_type: str = _in_dict['type']
     topic: str = _in_dict['topic']
-
-    # Workaround for None values in the payload str
-    p_str: str = _in_dict['payload']
-    if '"NONE"' in p_str:
-        p_str = p_str.replace('"NONE"', 'null')
-    payload = load_json(p_str)
+    payload: dict = load_json(_in_dict['payload'])
 
     # Find event from implemented events
     try:
         return _events[event_type].from_dict(topic, payload)
     except KeyError:
         raise ValueError(f'Unknown Event: {event_type:s} for {_in_dict}')
```

### Comparing `HABApp-1.0.8/src/HABApp/openhab/map_items.py` & `HABApp-1.1.0/src/HABApp/openhab/map_items.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from HABApp.core.wrapper import process_exception
 from HABApp.openhab.definitions.values import QuantityValue
 from HABApp.openhab.items import ColorItem, ContactItem, DatetimeItem, DimmerItem, GroupItem, ImageItem, LocationItem, \
     NumberItem, PlayerItem, RollershutterItem, StringItem, SwitchItem, CallItem
 from HABApp.openhab.items.base_item import HINT_TYPE_OPENHAB_ITEM
 from HABApp.openhab.items.base_item import MetaData
 
-log = logging.getLogger('HABApp.openhab')
+log = logging.getLogger('HABApp.openhab.items')
 
 
 _items: Dict[str, HINT_TYPE_OPENHAB_ITEM] = {
     'String': StringItem,
     'Number': NumberItem,
     'Switch': SwitchItem,
     'Contact': ContactItem,
@@ -35,31 +35,33 @@
              label: Optional[str], tags: FrozenSet[str],
              groups: FrozenSet[str], metadata: Optional[Dict[str, Dict[str, Any]]]) -> \
         Optional['HABApp.openhab.items.OpenhabItem']:
     try:
         assert isinstance(type, str)
         assert value is None or isinstance(value, str)
 
-        if value == 'NULL' or value == 'UNDEF':
-            value = None
-
         # map Metadata
         if metadata is not None:
             meta = Map({k: MetaData(v['value'], Map(v.get('config', {}))) for k, v in metadata.items()})
         else:
             meta = Map()
 
         # Quantity types are like this: Number:Temperature and have a unit set: "12.3 °C".
         # We have to remove the dimension from the type and remove the unit from the value
         if ':' in type:
             type, dimension = type.split(':')
             # if the item is not initialized its None and has no dimension
             if value is not None:
                 value, _ = QuantityValue.split_unit(value)
 
+            # Show warning
+            # https://github.com/spacemanspiff2007/HABApp/issues/383
+            if 'unit' not in meta:
+                log.warning(f'Item {name:s} is a UoM item but "unit" is not found in item metadata')
+
         cls = _items.get(type)
         if cls is not None:
             return cls.from_oh(name, value, label=label, tags=tags, groups=groups, metadata=meta)
 
         raise ValueError(f'Unknown openHAB type: {type} for {name}')
 
     except Exception as e:
```

### Comparing `HABApp-1.0.8/src/HABApp/openhab/map_values.py` & `HABApp-1.1.0/src/HABApp/openhab/map_values.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import datetime
 
 from HABApp.openhab.definitions import HSBValue, OnOffValue, OpenClosedValue, PercentValue, QuantityValue, RawValue, \
     UpDownValue
+from HABApp.openhab.definitions.values import PointValue
 
 
 def map_openhab_values(openhab_type: str, openhab_value: str):
     # because we preprocess the string value can be None.
     # Either remove the preprocessing or remove this here
     if openhab_value is None:
         return None
@@ -21,14 +22,17 @@
 
     if openhab_type == "Decimal":
         try:
             return int(openhab_value)
         except ValueError:
             return float(openhab_value)
 
+    if openhab_type == "String":
+        return openhab_value
+
     if openhab_type == "DateTime":
         dt = datetime.datetime.strptime(openhab_value, '%Y-%m-%dT%H:%M:%S.%f%z')
         # all datetimes from openHAB have a timezone set, so we can't easily compare them
         # --> TypeError: can't compare offset-naive and offset-aware datetimes
         dt = dt.astimezone(tz=None)   # Changes datetime object so it uses system timezone
         dt = dt.replace(tzinfo=None)  # Removes timezone awareness
         return dt
@@ -50,8 +54,11 @@
 
     if openhab_type == 'Quantity':
         return QuantityValue(openhab_value)
 
     if openhab_type == 'Raw':
         return RawValue(openhab_value)
 
+    if openhab_type == 'Point':
+        return PointValue(openhab_value)
+
     return openhab_value
```

### Comparing `HABApp-1.0.8/src/HABApp/parameters/parameter.py` & `HABApp-1.1.0/src/HABApp/parameters/parameter.py`

 * *Files identical despite different names*

### Comparing `HABApp-1.0.8/src/HABApp/parameters/parameter_files.py` & `HABApp-1.1.0/src/HABApp/parameters/parameter_files.py`

 * *Files identical despite different names*

### Comparing `HABApp-1.0.8/src/HABApp/parameters/parameters.py` & `HABApp-1.1.0/src/HABApp/parameters/parameters.py`

 * *Files identical despite different names*

### Comparing `HABApp-1.0.8/src/HABApp/rule/interfaces/_http.py` & `HABApp-1.1.0/src/HABApp/rule/interfaces/_http.py`

 * *Files identical despite different names*

### Comparing `HABApp-1.0.8/src/HABApp/rule/interfaces/rule_subprocess.py` & `HABApp-1.1.0/src/HABApp/rule/interfaces/rule_subprocess.py`

 * *Files identical despite different names*

### Comparing `HABApp-1.0.8/src/HABApp/rule/rule.py` & `HABApp-1.1.0/src/HABApp/rule/rule.py`

 * *Files 5% similar despite different names*

```diff
@@ -153,14 +153,15 @@
                          In case of failure (return code != 0) a log entry and an error event will be created.
                          This is the default and should be fine for almost all use cases.
 
                          ``True``: The callback will always be called with an
                          instance of :class:`~HABApp.rule.FinishedProcessInfo`.
         :param capture_output: Capture program output, set to ``False`` to only capture the return code
         :param additional_python_path: additional folders which will be added to the env variable ``PYTHONPATH``
+        :param kwargs: Additional kwargs that will be passed to ``asyncio.create_subprocess_exec``
         :return:
         """
 
         cb = wrap_func(callback, context=self._habapp_ctx)
 
         call_args, call_kwargs = build_exec_params(
             program, *args, _capture_output=capture_output, _additional_python_path=additional_python_path, **kwargs
@@ -197,14 +198,15 @@
                          In case of failure (return code != 0) a log entry and an error event will be created.
                          This is the default and should be fine for almost all use cases.
 
                          ``True``: The callback will always be called with an
                          instance of :class:`~HABApp.rule.FinishedProcessInfo`.
         :param capture_output: Capture program output, set to ``False`` to only capture the return code
         :param additional_python_path: additional folders which will be added to the env variable ``PYTHONPATH``
+        :param kwargs: Additional kwargs that will be passed to ``asyncio.create_subprocess_exec``
         :return:
         """
 
         new_args = list(args)
 
         p = Path(module_or_package)
         if p.suffix.lower() == '.py':
```

### Comparing `HABApp-1.0.8/src/HABApp/rule/scheduler/habappschedulerview.py` & `HABApp-1.1.0/src/HABApp/rule/scheduler/habappschedulerview.py`

 * *Files identical despite different names*

### Comparing `HABApp-1.0.8/src/HABApp/rule/scheduler/scheduler.py` & `HABApp-1.1.0/src/HABApp/rule/scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `HABApp-1.0.8/src/HABApp/rule_ctx/rule_ctx.py` & `HABApp-1.1.0/src/HABApp/rule_ctx/rule_ctx.py`

 * *Files identical despite different names*

### Comparing `HABApp-1.0.8/src/HABApp/rule_manager/benchmark/bench_base.py` & `HABApp-1.1.0/src/HABApp/rule_manager/benchmark/bench_base.py`

 * *Files identical despite different names*

### Comparing `HABApp-1.0.8/src/HABApp/rule_manager/benchmark/bench_file.py` & `HABApp-1.1.0/src/HABApp/rule_manager/benchmark/bench_file.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 
 
 class BenchFile(RuleFile):
     def __init__(self, rule_manager):
         super().__init__(rule_manager, 'BenchmarkFile', path=Path('BenchmarkFile'))
 
     def create_rules(self, created_rules: list):
-        HABAppRuleHook.in_dict(globals(), created_rules.append, self.suggest_rule_name, self.rule_manager.runtime, self)
+        hook = HABAppRuleHook(created_rules.append, self.suggest_rule_name, self.rule_manager.runtime, self)
+        hook.in_dict(globals())
 
         rule_ha = rule = HABAppBenchRule()
         if HABApp.CONFIG.mqtt.connection.host:
             rule = rule.link_rule(MqttBenchRule())
         if HABApp.CONFIG.openhab.connection.url:
             rule = rule.link_rule(OpenhabBenchRule())
```

### Comparing `HABApp-1.0.8/src/HABApp/rule_manager/benchmark/bench_habapp.py` & `HABApp-1.1.0/src/HABApp/rule_manager/benchmark/bench_habapp.py`

 * *Files identical despite different names*

### Comparing `HABApp-1.0.8/src/HABApp/rule_manager/benchmark/bench_mqtt.py` & `HABApp-1.1.0/src/HABApp/rule_manager/benchmark/bench_mqtt.py`

 * *Files identical despite different names*

### Comparing `HABApp-1.0.8/src/HABApp/rule_manager/benchmark/bench_oh.py` & `HABApp-1.1.0/src/HABApp/rule_manager/benchmark/bench_oh.py`

 * *Files identical despite different names*

### Comparing `HABApp-1.0.8/src/HABApp/rule_manager/benchmark/bench_times.py` & `HABApp-1.1.0/src/HABApp/rule_manager/benchmark/bench_times.py`

 * *Files identical despite different names*

### Comparing `HABApp-1.0.8/src/HABApp/rule_manager/rule_file.py` & `HABApp-1.1.0/src/HABApp/rule_manager/rule_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,20 +55,21 @@
         return None
 
     def __process_tc(self, tb: list):
         tb.insert(0, f"Could not load {self.path}!")
         return [line.replace('<module>', self.path.name) for line in tb]
 
     def create_rules(self, created_rules: list):
-        init_globals = HABAppRuleHook.in_dict(
-            {}, created_rules.append, self.suggest_rule_name, self.rule_manager.runtime, self)
+
+        rule_hook = HABAppRuleHook(created_rules.append, self.suggest_rule_name, self.rule_manager.runtime, self)
 
         # It seems like python 3.8 doesn't allow path like objects any more:
         # https://github.com/spacemanspiff2007/HABApp/issues/111
-        runpy.run_path(str(self.path), run_name=str(self.path), init_globals=init_globals)
+        with rule_hook:
+            runpy.run_path(str(self.path), run_name=str(self.path), init_globals=rule_hook.in_dict())
 
     def load(self) -> bool:
 
         created_rules: typing.List[HABApp.rule.Rule] = []
 
         ign = HABApp.core.wrapper.ExceptionToHABApp(logger=log)
         ign.proc_tb = self.__process_tc
```

### Comparing `HABApp-1.0.8/src/HABApp/rule_manager/rule_manager.py` & `HABApp-1.1.0/src/HABApp/rule_manager/rule_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from HABApp.core.files.watcher import AggregatingAsyncEventHandler
 from HABApp.core.logger import log_warning
 from HABApp.core.wrapper import log_exception
 from HABApp.runtime import shutdown
 from .rule_file import RuleFile
 from ..core.internals import uses_item_registry
 from HABApp.core.internals.wrapped_function import run_function
+from ..openhab.connection_logic.wait_startup import wait_for_openhab
 
 log = logging.getLogger('HABApp.Rules')
 
 item_registry = uses_item_registry()
 
 
 class RuleManager:
@@ -67,28 +68,21 @@
 
         # Initial loading of rules
         HABApp.core.internals.wrap_func(self.load_rules_on_startup, logger=log).run()
 
     async def load_rules_on_startup(self):
 
         if HABApp.CONFIG.openhab.connection.url and HABApp.CONFIG.openhab.general.wait_for_openhab:
-            items_found = False
-            while not items_found:
-                await sleep(3)
-                for item in item_registry.get_items():
-                    if isinstance(item, HABApp.openhab.items.OpenhabItem):
-                        items_found = True
-                        break
-
-                # stop waiting if we want to shut down
-                if HABApp.runtime.shutdown.requested:
-                    return None
-            await sleep(2.2)
+            await wait_for_openhab()
         else:
-            await sleep(5.2)
+            await sleep(1)
+
+        # if we want to shut down we don't load the rules
+        if HABApp.runtime.shutdown.requested:
+            return None
 
         # trigger event for every file
         await self.watcher.trigger_all()
         return None
 
     @log_exception
     def get_rule(self, rule_name):
```

### Comparing `HABApp-1.0.8/src/HABApp/runtime/runtime.py` & `HABApp-1.1.0/src/HABApp/runtime/runtime.py`

 * *Files identical despite different names*

### Comparing `HABApp-1.0.8/src/HABApp/runtime/shutdown.py` & `HABApp-1.1.0/src/HABApp/runtime/shutdown.py`

 * *Files identical despite different names*

### Comparing `HABApp-1.0.8/src/HABApp/util/fade/fade.py` & `HABApp-1.1.0/src/HABApp/util/fade/fade.py`

 * *Files identical despite different names*

### Comparing `HABApp-1.0.8/src/HABApp/util/functions/min_max.py` & `HABApp-1.1.0/src/HABApp/util/functions/min_max.py`

 * *Files identical despite different names*

### Comparing `HABApp-1.0.8/src/HABApp/util/listener_groups/listener_creator.py` & `HABApp-1.1.0/src/HABApp/util/listener_groups/listener_creator.py`

 * *Files identical despite different names*

### Comparing `HABApp-1.0.8/src/HABApp/util/listener_groups/listener_groups.py` & `HABApp-1.1.0/src/HABApp/util/listener_groups/listener_groups.py`

 * *Files identical despite different names*

### Comparing `HABApp-1.0.8/src/HABApp/util/multimode/item.py` & `HABApp-1.1.0/src/HABApp/util/multimode/item.py`

 * *Files identical despite different names*

### Comparing `HABApp-1.0.8/src/HABApp/util/multimode/mode_base.py` & `HABApp-1.1.0/src/HABApp/util/multimode/mode_base.py`

 * *Files identical despite different names*

### Comparing `HABApp-1.0.8/src/HABApp/util/multimode/mode_switch.py` & `HABApp-1.1.0/src/HABApp/util/multimode/mode_switch.py`

 * *Files identical despite different names*

### Comparing `HABApp-1.0.8/src/HABApp/util/multimode/mode_value.py` & `HABApp-1.1.0/src/HABApp/util/multimode/mode_value.py`

 * *Files identical despite different names*

### Comparing `HABApp-1.0.8/src/HABApp/util/statistics.py` & `HABApp-1.1.0/src/HABApp/util/statistics.py`

 * *Files identical despite different names*

### Comparing `HABApp-1.0.8/src/HABApp/util/threshold.py` & `HABApp-1.1.0/src/HABApp/util/threshold.py`

 * *Files identical despite different names*

### Comparing `HABApp-1.0.8/src/HABApp.egg-info/PKG-INFO` & `HABApp-1.1.0/src/HABApp.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HABApp
-Version: 1.0.8
+Version: 1.1.0
 Summary: Easy automation with MQTT and/or openHAB. Create home automation rules in python.
 Home-page: https://github.com/spacemanspiff2007/HABApp
 Author: spaceman_spiff
 Project-URL: Documentation, https://habapp.readthedocs.io/
 Project-URL: GitHub, https://github.com/spacemanspiff2007/HABApp
 Keywords: mqtt,openhab,habapp,home automation
 Classifier: Development Status :: 4 - Beta
@@ -42,14 +42,25 @@
 ## Goals
 The goal of this application is to provide a simple way to create home automation rules in python.
 With full syntax highlighting and descriptive names it should almost never be required to look something up in the documentation
 
 ## Documentation
 [The documentation can be found at here](https://habapp.readthedocs.io)
 
+## Help out
+HABApp was created for my own use, but I wanted others to profit from it, too.
+Creating, maintaining and developing it takes a lot of time.
+If you think this is a great tool and want to support it you can donate,
+so I can buy some more coffee to keep development going. :wink:
+
+[![Donate with PayPal](https://img.shields.io/badge/Donate-PayPal-informational?logo=paypal)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=YU5U9YQN56JVA)
+
+All donations are greatly appreciated!
+
+
 ## Examples
 
 ### MQTT Rule example
 ```python
 import datetime
 import random
 
@@ -93,25 +104,25 @@
 ```
 
 ### openHAB rule example
 
 ```python
 import HABApp
 from HABApp.core.events import ValueUpdateEvent, ValueChangeEvent, ValueChangeEventFilter, ValueUpdateEventFilter
-from HABApp.openhab.events import ItemCommandEvent, ItemStateEventFilter, ItemCommandEventFilter, \
+from HABApp.openhab.events import ItemCommandEvent, ItemStateUpdatedEventFilter, ItemCommandEventFilter, \
   ItemStateChangedEventFilter
 
 
 class MyOpenhabRule(HABApp.Rule):
 
   def __init__(self):
     super().__init__()
 
     # Trigger on item updates
-    self.listen_event('TestContact', self.item_state_update, ItemStateEventFilter())
+    self.listen_event('TestContact', self.item_state_update, ItemStateUpdatedEventFilter())
     self.listen_event('TestDateTime', self.item_state_update, ValueUpdateEventFilter())
 
     # Trigger on item changes
     self.listen_event('TestDateTime', self.item_state_change, ItemStateChangedEventFilter())
     self.listen_event('TestSwitch', self.item_state_change, ValueChangeEventFilter())
 
     # Trigger on item commands
@@ -136,14 +147,31 @@
     self.oh.post_update('TestItemUpdate', 123)
 
 
 MyOpenhabRule()
 ```
 
 # Changelog
+#### 1.1.0 (2023-06-15)
+- This is a breaking change!
+- Renamed `GroupItemStateChangedEvent` to `GroupStateChangedEvent`
+- Groups issue a `GroupStateUpdateEvent` when the state updates on OH3 (consistent with OH4 behavior)
+- Groups work now with `ValueUpdateEvent` and `ValueChangedEvent` as expected
+- Renamed `ItemStateEvent` to `ItemStateUpdatedEvent`
+- Ignored ItemStateEvent on OH4
+- Fewer warnings for long-running functions (execution of <FUNC_NAME> took too long)
+- `Thing` status and status_detail are now an Enum
+- Added `status_detail` to `Thing`
+- `LocationItem` now provides the location as a tuple
+- Added support for `Point` events
+- Improved item sync from openHAB (no more false item state `None` after startup)
+- Improved startup behavior when openHAB and HABApp get started together (e.g. after reboot)
+- Fixed an issue with short tracebacks for HABApp internal files
+- Doc improvements
+
 #### 1.0.8 (2023-02-09)
 - Fixed an issue when using token based authentication with openHAB
 - Fixed an issue with the asyncio event loop under Python < 3.10
 
 #### 1.0.7 (2023-02-09)
 - ``ContactItem`` has ``open()``/``closed()`` methods
 - Setting persistence values now works for some persistence services
```

### Comparing `HABApp-1.0.8/src/HABApp.egg-info/SOURCES.txt` & `HABApp-1.1.0/src/HABApp.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 src/HABApp/__cmd_args__.py
 src/HABApp/__debug_info__.py
 src/HABApp/__init__.py
 src/HABApp/__main__.py
 src/HABApp/__setup_packages__.py
 src/HABApp/__splash_screen__.py
 src/HABApp/__version__.py
+src/HABApp/py.typed
 src/HABApp.egg-info/PKG-INFO
 src/HABApp.egg-info/SOURCES.txt
 src/HABApp.egg-info/dependency_links.txt
 src/HABApp.egg-info/entry_points.txt
 src/HABApp.egg-info/requires.txt
 src/HABApp.egg-info/top_level.txt
 src/HABApp/config/__init__.py
@@ -39,14 +40,15 @@
 src/HABApp/core/errors.py
 src/HABApp/core/logger.py
 src/HABApp/core/wrapper.py
 src/HABApp/core/const/__init__.py
 src/HABApp/core/const/const.py
 src/HABApp/core/const/hints.py
 src/HABApp/core/const/json.py
+src/HABApp/core/const/log.py
 src/HABApp/core/const/loop.py
 src/HABApp/core/const/topics.py
 src/HABApp/core/const/yml.py
 src/HABApp/core/events/__init__.py
 src/HABApp/core/events/events.py
 src/HABApp/core/events/habapp_events.py
 src/HABApp/core/events/filter/__init__.py
@@ -143,29 +145,31 @@
 src/HABApp/openhab/connection_handler/sse_handler.py
 src/HABApp/openhab/connection_logic/__init__.py
 src/HABApp/openhab/connection_logic/_plugin.py
 src/HABApp/openhab/connection_logic/connection.py
 src/HABApp/openhab/connection_logic/plugin_load_items.py
 src/HABApp/openhab/connection_logic/plugin_ping.py
 src/HABApp/openhab/connection_logic/plugin_thing_overview.py
+src/HABApp/openhab/connection_logic/wait_startup.py
 src/HABApp/openhab/connection_logic/plugin_things/__init__.py
 src/HABApp/openhab/connection_logic/plugin_things/_log.py
 src/HABApp/openhab/connection_logic/plugin_things/cfg_validator.py
 src/HABApp/openhab/connection_logic/plugin_things/filters.py
 src/HABApp/openhab/connection_logic/plugin_things/item_worker.py
 src/HABApp/openhab/connection_logic/plugin_things/plugin_things.py
 src/HABApp/openhab/connection_logic/plugin_things/str_builder.py
 src/HABApp/openhab/connection_logic/plugin_things/thing_config.py
 src/HABApp/openhab/connection_logic/plugin_things/thing_worker.py
 src/HABApp/openhab/connection_logic/plugin_things/file_writer/__init__.py
 src/HABApp/openhab/connection_logic/plugin_things/file_writer/formatter.py
 src/HABApp/openhab/connection_logic/plugin_things/file_writer/formatter_builder.py
 src/HABApp/openhab/connection_logic/plugin_things/file_writer/writer.py
 src/HABApp/openhab/definitions/__init__.py
-src/HABApp/openhab/definitions/definitions.py
+src/HABApp/openhab/definitions/items.py
+src/HABApp/openhab/definitions/things.py
 src/HABApp/openhab/definitions/topics.py
 src/HABApp/openhab/definitions/values.py
 src/HABApp/openhab/definitions/helpers/__init__.py
 src/HABApp/openhab/definitions/helpers/log_table.py
 src/HABApp/openhab/definitions/helpers/persistence_data.py
 src/HABApp/openhab/definitions/rest/__init__.py
 src/HABApp/openhab/definitions/rest/base.py
@@ -177,27 +181,27 @@
 src/HABApp/openhab/events/base_event.py
 src/HABApp/openhab/events/channel_events.py
 src/HABApp/openhab/events/event_filters.py
 src/HABApp/openhab/events/item_events.py
 src/HABApp/openhab/events/thing_events.py
 src/HABApp/openhab/items/__init__.py
 src/HABApp/openhab/items/base_item.py
-src/HABApp/openhab/items/call_item.py
 src/HABApp/openhab/items/color_item.py
 src/HABApp/openhab/items/commands.py
 src/HABApp/openhab/items/contact_item.py
 src/HABApp/openhab/items/datetime_item.py
 src/HABApp/openhab/items/dimmer_item.py
 src/HABApp/openhab/items/group_item.py
 src/HABApp/openhab/items/image_item.py
 src/HABApp/openhab/items/number_item.py
 src/HABApp/openhab/items/rollershutter_item.py
 src/HABApp/openhab/items/string_item.py
 src/HABApp/openhab/items/switch_item.py
 src/HABApp/openhab/items/thing_item.py
+src/HABApp/openhab/items/tuple_items.py
 src/HABApp/parameters/__init__.py
 src/HABApp/parameters/parameter.py
 src/HABApp/parameters/parameter_files.py
 src/HABApp/parameters/parameters.py
 src/HABApp/rule/__init__.py
 src/HABApp/rule/rule.py
 src/HABApp/rule/rule_hook.py
```

### Comparing `HABApp-1.0.8/tests/test_cmd_args.py` & `HABApp-1.1.0/tests/test_cmd_args.py`

 * *Files identical despite different names*

### Comparing `HABApp-1.0.8/tests/test_docs.py` & `HABApp-1.1.0/tests/test_docs.py`

 * *Files identical despite different names*

### Comparing `HABApp-1.0.8/tests/test_packages.py` & `HABApp-1.1.0/tests/test_packages.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import re
 from pathlib import Path
-
+from packaging.version import VERSION_PATTERN
 import HABApp.__check_dependency_packages__
+from HABApp import __version__
 
 
 def test_installation_check():
     re_name = re.compile(r'^([A-Za-z_-]{3,})')
     requirements = Path(__file__).parent.parent / 'requirements_setup.txt'
     assert requirements.is_file()
 
@@ -15,7 +16,12 @@
         if not line or line.startswith('#'):
             continue
         found.add(re_name.search(line).group(1))
 
     coded = set(HABApp.__check_dependency_packages__.get_dependencies())
 
     assert coded == found
+
+
+def test_version():
+    check = re.compile(VERSION_PATTERN, re.VERBOSE | re.IGNORECASE)
+    assert check.fullmatch(__version__)
```

