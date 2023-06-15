# Comparing `tmp/hopeit.apps-visualizer-0.9.3.tar.gz` & `tmp/hopeit.apps-visualizer-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hopeit.apps-visualizer-0.9.3.tar", last modified: Mon Jul 12 23:34:18 2021, max compression
+gzip compressed data, was "hopeit.apps-visualizer-0.9.4.tar", last modified: Wed Jul 14 00:52:00 2021, max compression
```

## Comparing `hopeit.apps-visualizer-0.9.3.tar` & `hopeit.apps-visualizer-0.9.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-12 23:34:18.918186 hopeit.apps-visualizer-0.9.3/
--rw-r--r--   0 runner    (1001) docker     (121)     3479 2021-07-12 23:34:18.918186 hopeit.apps-visualizer-0.9.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2175 2021-07-12 23:27:48.000000 hopeit.apps-visualizer-0.9.3/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-07-12 23:34:18.918186 hopeit.apps-visualizer-0.9.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2348 2021-07-12 23:27:48.000000 hopeit.apps-visualizer-0.9.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-12 23:34:18.914186 hopeit.apps-visualizer-0.9.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-12 23:34:18.914186 hopeit.apps-visualizer-0.9.3/src/hopeit/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-12 23:34:18.914186 hopeit.apps-visualizer-0.9.3/src/hopeit/apps_visualizer/
--rw-r--r--   0 runner    (1001) docker     (121)     1179 2021-07-12 23:27:48.000000 hopeit.apps-visualizer-0.9.3/src/hopeit/apps_visualizer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-12 23:34:18.914186 hopeit.apps-visualizer-0.9.3/src/hopeit/apps_visualizer/apps/
--rw-r--r--   0 runner    (1001) docker     (121)     1269 2021-07-12 23:27:48.000000 hopeit.apps-visualizer-0.9.3/src/hopeit/apps_visualizer/apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4933 2021-07-12 23:27:48.000000 hopeit.apps-visualizer-0.9.3/src/hopeit/apps_visualizer/apps/events_graph.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-12 23:34:18.918186 hopeit.apps-visualizer-0.9.3/src/hopeit/apps_visualizer/event_stats/
--rw-r--r--   0 runner    (1001) docker     (121)     2787 2021-07-12 23:27:48.000000 hopeit.apps-visualizer-0.9.3/src/hopeit/apps_visualizer/event_stats/collect.py
--rw-r--r--   0 runner    (1001) docker     (121)     3651 2021-07-12 23:27:48.000000 hopeit.apps-visualizer-0.9.3/src/hopeit/apps_visualizer/event_stats/live.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-12 23:34:18.918186 hopeit.apps-visualizer-0.9.3/src/hopeit/apps_visualizer/graphs/
--rw-r--r--   0 runner    (1001) docker     (121)     5702 2021-07-12 23:27:48.000000 hopeit.apps-visualizer-0.9.3/src/hopeit/apps_visualizer/graphs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-12 23:34:18.918186 hopeit.apps-visualizer-0.9.3/src/hopeit/apps_visualizer/site/
--rw-r--r--   0 runner    (1001) docker     (121)     3756 2021-07-12 23:27:48.000000 hopeit.apps-visualizer-0.9.3/src/hopeit/apps_visualizer/site/main.py
--rw-r--r--   0 runner    (1001) docker     (121)     1385 2021-07-12 23:27:48.000000 hopeit.apps-visualizer-0.9.3/src/hopeit/apps_visualizer/site/visualization.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-12 23:34:18.914186 hopeit.apps-visualizer-0.9.3/src/hopeit.apps_visualizer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3479 2021-07-12 23:34:18.000000 hopeit.apps-visualizer-0.9.3/src/hopeit.apps_visualizer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      630 2021-07-12 23:34:18.000000 hopeit.apps-visualizer-0.9.3/src/hopeit.apps_visualizer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-07-12 23:34:18.000000 hopeit.apps-visualizer-0.9.3/src/hopeit.apps_visualizer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       54 2021-07-12 23:34:18.000000 hopeit.apps-visualizer-0.9.3/src/hopeit.apps_visualizer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2021-07-12 23:34:18.000000 hopeit.apps-visualizer-0.9.3/src/hopeit.apps_visualizer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-14 00:52:00.080905 hopeit.apps-visualizer-0.9.4/
+-rw-r--r--   0 runner    (1001) docker     (121)     3479 2021-07-14 00:52:00.080905 hopeit.apps-visualizer-0.9.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2175 2021-07-14 00:45:26.000000 hopeit.apps-visualizer-0.9.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-07-14 00:52:00.080905 hopeit.apps-visualizer-0.9.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2348 2021-07-14 00:45:26.000000 hopeit.apps-visualizer-0.9.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-14 00:52:00.076905 hopeit.apps-visualizer-0.9.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-14 00:52:00.076905 hopeit.apps-visualizer-0.9.4/src/hopeit/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-14 00:52:00.076905 hopeit.apps-visualizer-0.9.4/src/hopeit/apps_visualizer/
+-rw-r--r--   0 runner    (1001) docker     (121)     1179 2021-07-14 00:45:26.000000 hopeit.apps-visualizer-0.9.4/src/hopeit/apps_visualizer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-14 00:52:00.080905 hopeit.apps-visualizer-0.9.4/src/hopeit/apps_visualizer/apps/
+-rw-r--r--   0 runner    (1001) docker     (121)     1384 2021-07-14 00:45:26.000000 hopeit.apps-visualizer-0.9.4/src/hopeit/apps_visualizer/apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4733 2021-07-14 00:45:26.000000 hopeit.apps-visualizer-0.9.4/src/hopeit/apps_visualizer/apps/events_graph.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-14 00:52:00.080905 hopeit.apps-visualizer-0.9.4/src/hopeit/apps_visualizer/event_stats/
+-rw-r--r--   0 runner    (1001) docker     (121)     2787 2021-07-14 00:45:26.000000 hopeit.apps-visualizer-0.9.4/src/hopeit/apps_visualizer/event_stats/collect.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3651 2021-07-14 00:45:26.000000 hopeit.apps-visualizer-0.9.4/src/hopeit/apps_visualizer/event_stats/live.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-14 00:52:00.080905 hopeit.apps-visualizer-0.9.4/src/hopeit/apps_visualizer/graphs/
+-rw-r--r--   0 runner    (1001) docker     (121)     5702 2021-07-14 00:45:26.000000 hopeit.apps-visualizer-0.9.4/src/hopeit/apps_visualizer/graphs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-14 00:52:00.080905 hopeit.apps-visualizer-0.9.4/src/hopeit/apps_visualizer/site/
+-rw-r--r--   0 runner    (1001) docker     (121)     3786 2021-07-14 00:45:26.000000 hopeit.apps-visualizer-0.9.4/src/hopeit/apps_visualizer/site/main.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1385 2021-07-14 00:45:26.000000 hopeit.apps-visualizer-0.9.4/src/hopeit/apps_visualizer/site/visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-14 00:52:00.076905 hopeit.apps-visualizer-0.9.4/src/hopeit.apps_visualizer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3479 2021-07-14 00:52:00.000000 hopeit.apps-visualizer-0.9.4/src/hopeit.apps_visualizer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      630 2021-07-14 00:52:00.000000 hopeit.apps-visualizer-0.9.4/src/hopeit.apps_visualizer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-07-14 00:52:00.000000 hopeit.apps-visualizer-0.9.4/src/hopeit.apps_visualizer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       54 2021-07-14 00:52:00.000000 hopeit.apps-visualizer-0.9.4/src/hopeit.apps_visualizer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        7 2021-07-14 00:52:00.000000 hopeit.apps-visualizer-0.9.4/src/hopeit.apps_visualizer.egg-info/top_level.txt
```

### Comparing `hopeit.apps-visualizer-0.9.3/PKG-INFO` & `hopeit.apps-visualizer-0.9.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hopeit.apps-visualizer
-Version: 0.9.3
+Version: 0.9.4
 Summary: Hopeit Engine Apps Visualizer Plugin
 Home-page: https://github.com/hopeit-git/hopeit.engine
 Author: Leo Smerling and Pablo Canto
 Author-email: contact@hopeit.com.ar
 License: Apache 2
 Project-URL: CI: GitHub Actions, https://github.com/hopeit-git/hopeit.engine/actions?query=workflow
 Project-URL: Docs: RTD, https://hopeitengine.readthedocs.io/en/latest/
```

### Comparing `hopeit.apps-visualizer-0.9.3/README.md` & `hopeit.apps-visualizer-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `hopeit.apps-visualizer-0.9.3/setup.py` & `hopeit.apps-visualizer-0.9.4/setup.py`

 * *Files identical despite different names*

### Comparing `hopeit.apps-visualizer-0.9.3/src/hopeit/apps_visualizer/__init__.py` & `hopeit.apps-visualizer-0.9.4/src/hopeit/apps_visualizer/__init__.py`

 * *Files identical despite different names*

### Comparing `hopeit.apps-visualizer-0.9.3/src/hopeit/apps_visualizer/apps/__init__.py` & `hopeit.apps-visualizer-0.9.4/src/hopeit/apps_visualizer/apps/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,24 +16,26 @@
 logger, extra = engine_extra_logger()
 
 _lock = asyncio.Lock()
 _apps: Optional[RuntimeApps] = None
 _expire: float = 0.0
 
 
-async def get_runtime_apps(context: EventContext, refresh: bool = False) -> RuntimeApps:
+async def get_runtime_apps(context: EventContext,
+                           *, refresh: bool = False,
+                           expand_events: bool = False) -> RuntimeApps:
     """
     Extract current runtime app_config objects
     """
     global _apps, _expire
     if not refresh and _lock.locked():
         raise RuntimeError("Events graph request in process. Ignoring")
     env = AppsVisualizerEnv.from_context(context)
     now_ts = datetime.now(tz=timezone.utc).timestamp()
     async with _lock:
         if _apps is None or refresh or now_ts > _expire:
             logger.info(context, "Contacting hosts config-manager...")
-            _apps = await get_apps_config(env.hosts, context)
+            _apps = await get_apps_config(env.hosts, context, expand_events=expand_events)
             _expire = now_ts + env.refresh_hosts_seconds
         else:
             logger.info(context, "Using cached runtime apps information.")
         return _apps
```

### Comparing `hopeit.apps-visualizer-0.9.3/src/hopeit/apps_visualizer/apps/events_graph.py` & `hopeit.apps-visualizer-0.9.4/src/hopeit/apps_visualizer/apps/events_graph.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 """
 Events graph showing events, stream and dependencies for specified apps
 """
 from typing import Optional
 
 from hopeit.app.context import EventContext
 
-from hopeit.server.imports import find_event_handler
-from hopeit.server.steps import split_event_stages
 from hopeit.app.api import event_api
 from hopeit.dataobjects import dataclass, dataobject
 from hopeit.app.events import collector_step, Collector
 from hopeit.app.logger import app_extra_logger
 
 from hopeit.config_manager import RuntimeApps, RuntimeAppInfo
 
@@ -50,15 +48,16 @@
 )
 
 
 async def runtime_apps(collector: Collector, context: EventContext) -> RuntimeApps:
     """
     Extract current runtime app_config objects
     """
-    return await get_runtime_apps(context)
+    options: VisualizationOptions = await collector['payload']
+    return await get_runtime_apps(context, expand_events=options.expanded_view)
 
 
 def _filter_apps(runtime_info: RuntimeAppInfo, options: VisualizationOptions) -> bool:
     return (
         options.app_prefix == '' or (
             runtime_info.app_config.app.name[0:len(options.app_prefix)] == options.app_prefix
         )
@@ -75,33 +74,34 @@
 
 async def config_graph(collector: Collector, context: EventContext) -> Optional[Graph]:
     """
     Generates Graph object with nodes and edges from server runtime active configuration
     """
     options: VisualizationOptions = await collector['payload']
     all_apps: RuntimeApps = await collector['runtime_apps']
-    filterd_apps = (
-        runtime_info.app_config
+
+    filtered_apps = [
+        (app_key, runtime_info)
         for app_key, runtime_info in all_apps.apps.items()
         if _filter_apps(runtime_info, options) and _filter_hosts(runtime_info, options)
-    )
+    ]
 
-    events = {}
-    app_connections = {}
-    for app_config in filterd_apps:
-        app_key = app_config.app_key()
-        for event_name, event_info in app_config.events.items():
-            impl = find_event_handler(app_config=app_config, event_name=event_name)
-            splits = split_event_stages(app_config.app, event_name, event_info, impl)
-            for name, info in splits.items():
-                events[f"{app_key}.{name}"] = info
-        for app_conn_key, app_connection in app_config.app_connections.items():
-            app_connections[f"{app_key}.{app_conn_key}"] = app_connection
+    events = {
+        f"{app_key}.{event_name}": event_info
+        for app_key, app_info in filtered_apps
+        for event_name, event_info in app_info.effective_events.items()
+    }
+
+    app_connections = {
+        f"{app_key}.{app_conn_key}": app_connection
+        for app_key, app_info in filtered_apps
+        for app_conn_key, app_connection in app_info.app_config.app_connections.items()
+    }
 
-    nodes = get_nodes(events, expand_queues=options.expand_queues)
+    nodes = get_nodes(events, expanded_view=options.expanded_view)
     add_app_connections(nodes, app_connections=app_connections, events=events)
     edges = get_edges(nodes)
     return Graph(nodes=list(nodes.values()), edges=edges)
 
 
 async def cytoscape_data(collector: Collector, context: EventContext) -> CytoscapeGraph:
     """
```

### Comparing `hopeit.apps-visualizer-0.9.3/src/hopeit/apps_visualizer/event_stats/collect.py` & `hopeit.apps-visualizer-0.9.4/src/hopeit/apps_visualizer/event_stats/collect.py`

 * *Files identical despite different names*

### Comparing `hopeit.apps-visualizer-0.9.3/src/hopeit/apps_visualizer/event_stats/live.py` & `hopeit.apps-visualizer-0.9.4/src/hopeit/apps_visualizer/event_stats/live.py`

 * *Files identical despite different names*

### Comparing `hopeit.apps-visualizer-0.9.3/src/hopeit/apps_visualizer/graphs/__init__.py` & `hopeit.apps-visualizer-0.9.4/src/hopeit/apps_visualizer/graphs/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,20 +40,20 @@
 @dataclass
 class Graph:
     nodes: List[Node]
     edges: List[Edge]
 
 
 def get_nodes(events: Dict[str, EventDescriptor],
-              *, expand_queues: bool = False) -> Dict[str, Node]:
+              *, expanded_view: bool = False) -> Dict[str, Node]:
     """
     Create Node metadata from EventDescriptors from app_config,
     expanding effective events using engine functionallity.
 
-    :param expand_queues: bool, if True, stream queues are shown as separate streams,
+    :param expanded_view: bool, if True, stream queues are shown as separate streams,
         otherwise they are shown in a single node with multiple input/outputs.
     """
     nodes = {}
     for event_name, event_info in events.items():
         inputs, outputs = [], []
         if event_info.type in (EventType.GET, EventType.POST, EventType.MULTIPART):
             port_name = f"{event_name}.{event_info.type.value}"
@@ -61,50 +61,50 @@
             request_node = Node(
                 id=port_name, label=event_info.type.value, type=NodeType.REQUEST, outputs=[port_name]
             )
             nodes[port_name] = request_node
 
         if event_info.read_stream:
             queues = event_info.read_stream.queues
-            for qid, queue in zip(queues, queues) if expand_queues else [("", "|".join(queues))]:
+            for qid, queue in zip(queues, queues) if expanded_view else [("", "|".join(queues))]:
                 stream_id = f">{event_info.read_stream.name}.{qid}".strip('.')
                 stream_name = f"{event_info.read_stream.name}"
                 if qid not in ("", "AUTO"):
                     stream_name += f".{qid}"
                 stream_node = nodes.get(stream_id, Node(
                     id=stream_id, label=stream_name, type=NodeType.STREAM
                 ))
                 stream_node.slots = sorted(set([*stream_node.slots, *queue.split("|")]))
                 nodes[stream_id] = stream_node
 
-                for q in [queue] if expand_queues else queues:
+                for q in [queue] if expanded_view else queues:
                     port_name = f"{event_name}.{stream_name}.{q}"
                     inputs.append(port_name)
                     stream_node.outputs.append(port_name)
 
         if event_info.write_stream:
             queues = event_info.write_stream.queues
             if event_info.read_stream and event_info.write_stream.queue_strategy == StreamQueueStrategy.PROPAGATE:
                 queues = [
                     qx if qy == "AUTO" else qy
                     for qx in event_info.read_stream.queues
                     for qy in queues
                 ]
-            for qid, queue in zip(queues, queues) if expand_queues else [("", "|".join(queues))]:
+            for qid, queue in zip(queues, queues) if expanded_view else [("", "|".join(queues))]:
                 stream_id = f">{event_info.write_stream.name}.{qid}".strip('.')
                 stream_name = f"{event_info.write_stream.name}"
                 if qid not in ("", "AUTO"):
                     stream_name += f".{qid}"
                 stream_node = nodes.get(stream_id, Node(
                     id=stream_id, label=stream_name, type=NodeType.STREAM
                 ))
                 stream_node.slots = sorted(set([*stream_node.slots, *queue.split("|")]))
                 nodes[stream_id] = stream_node
 
-                for q in [queue] if expand_queues else queues:
+                for q in [queue] if expanded_view else queues:
                     port_name = f"{event_name}.{stream_name}.{q}"
                     stream_node.inputs.append(port_name)
                     outputs.append(port_name)
 
         nodes[event_name] = Node(
             id=event_name, label=event_name, type=NodeType.EVENT, inputs=inputs, outputs=outputs
         )
```

### Comparing `hopeit.apps-visualizer-0.9.3/src/hopeit/apps_visualizer/site/main.py` & `hopeit.apps-visualizer-0.9.4/src/hopeit/apps_visualizer/site/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -47,49 +47,49 @@
 
 
 async def runtime_apps_config(options: VisualizationOptions, context: EventContext) -> EventsGraphResult:
     """
     Extract current runtime app_config objects
     """
     return EventsGraphResult(
-        runtime_apps=await get_runtime_apps(context, refresh=True),
+        runtime_apps=await get_runtime_apps(context, refresh=True, expand_events=options.expanded_view),
         options=options
     )
 
 
 async def __postprocess__(result: EventsGraphResult, context: EventContext, response: PostprocessHook) -> str:
     """
     Renders html from template, using cytospace data json
     """
     response.set_content_type("text/html")
 
     app_prefix = result.options.app_prefix
 
     view_link = f"apps-visualizer?app_prefix={result.options.app_prefix}"
     view_link += f"&host_filter={result.options.host_filter}"
-    view_link += f"&expand_queues={str(not result.options.expand_queues).lower()}"
+    view_link += f"&expanded_view={str(not result.options.expanded_view).lower()}"
     view_link += f"&live={str(result.options.live).lower()}"
 
     live_link = f"apps-visualizer?app_prefix={result.options.app_prefix}"
     live_link += f"&host_filter={result.options.host_filter}"
-    live_link += f"&expand_queues={str(result.options.expand_queues).lower()}"
+    live_link += f"&expanded_view={str(result.options.expanded_view).lower()}"
     live_link += f"&live={str(not result.options.live).lower()}"
 
     app_prefix = f"{result.options.app_prefix}*" if result.options.app_prefix else 'All running apps'
     host_filter = f"*{result.options.host_filter}*" if result.options.host_filter else 'All servers'
-    view_type = "Expanded queues view" if result.options.expand_queues else "Standard view"
+    view_type = "Expanded view" if result.options.expanded_view else "Standard view"
     live_type = "Live!" if result.options.live else "Static"
 
     refresh_endpoint_comps = (
         ['event-stats', 'live'] if result.options.live else ['apps', 'events-graph']
     )
     refresh_endpoint = route_name("api", context.app.name, context.app.version, *refresh_endpoint_comps)
     refresh_endpoint += f"?app_prefix={result.options.app_prefix}"
     refresh_endpoint += f"&host_filter={result.options.host_filter}"
-    refresh_endpoint += f"&expand_queues={str(result.options.expand_queues).lower()}"
+    refresh_endpoint += f"&expanded_view={str(result.options.expanded_view).lower()}"
     refresh_endpoint += f"&live={str(result.options.live).lower()}"
 
     with open(_dir_path / 'events_graph_template.html') as f:
         template = f.read()
         template = template.replace("{{ app_prefix }}", app_prefix)
         template = template.replace("{{ host_filter }}", host_filter)
         template = template.replace("{{ view_link }}", view_link)
```

### Comparing `hopeit.apps-visualizer-0.9.3/src/hopeit/apps_visualizer/site/visualization.py` & `hopeit.apps-visualizer-0.9.4/src/hopeit/apps_visualizer/site/visualization.py`

 * *Files 19% similar despite different names*

```diff
@@ -15,31 +15,31 @@
 
 
 @dataobject
 @dataclass
 class VisualizationOptions:
     app_prefix: str = ''
     host_filter: str = ''
-    expand_queues: bool = False
+    expanded_view: bool = False
     live: bool = False
 
 
 def visualization_options_api_args():
     return [
         ("app_prefix", Optional[str], "app name prefix to filter"),
         ("host_filter", Optional[str], "host name filter substring"),
-        ("expand_queues", Optional[bool], "if `true` shows each stream queue as a separated stream"),
+        ("expanded_view", Optional[bool], "if `true` shows each stream queue as a separated stream"),
         ("live", Optional[bool], "if `true` enable live stats refreshing")
     ]
 
 
 async def visualization_options(payload: None, context: EventContext,
                                 *, app_prefix: str = '',
                                 host_filter: str = '',
-                                expand_queues: bool = False,
+                                expanded_view: bool = False,
                                 live: bool = False) -> VisualizationOptions:
     return VisualizationOptions(
         app_prefix=app_prefix,
         host_filter=host_filter,
-        expand_queues=expand_queues is True or expand_queues == 'true',
+        expanded_view=expanded_view is True or expanded_view == 'true',
         live=live is True or live == 'true'
     )
```

### Comparing `hopeit.apps-visualizer-0.9.3/src/hopeit.apps_visualizer.egg-info/PKG-INFO` & `hopeit.apps-visualizer-0.9.4/src/hopeit.apps_visualizer.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hopeit.apps-visualizer
-Version: 0.9.3
+Version: 0.9.4
 Summary: Hopeit Engine Apps Visualizer Plugin
 Home-page: https://github.com/hopeit-git/hopeit.engine
 Author: Leo Smerling and Pablo Canto
 Author-email: contact@hopeit.com.ar
 License: Apache 2
 Project-URL: CI: GitHub Actions, https://github.com/hopeit-git/hopeit.engine/actions?query=workflow
 Project-URL: Docs: RTD, https://hopeitengine.readthedocs.io/en/latest/
```

### Comparing `hopeit.apps-visualizer-0.9.3/src/hopeit.apps_visualizer.egg-info/SOURCES.txt` & `hopeit.apps-visualizer-0.9.4/src/hopeit.apps_visualizer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

