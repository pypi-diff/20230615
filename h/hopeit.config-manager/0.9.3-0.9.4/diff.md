# Comparing `tmp/hopeit.config-manager-0.9.3.tar.gz` & `tmp/hopeit.config-manager-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hopeit.config-manager-0.9.3.tar", last modified: Mon Jul 12 23:34:16 2021, max compression
+gzip compressed data, was "hopeit.config-manager-0.9.4.tar", last modified: Wed Jul 14 00:51:57 2021, max compression
```

## Comparing `hopeit.config-manager-0.9.3.tar` & `hopeit.config-manager-0.9.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-12 23:34:16.330172 hopeit.config-manager-0.9.3/
--rw-r--r--   0 runner    (1001) docker     (121)     2005 2021-07-12 23:34:16.330172 hopeit.config-manager-0.9.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      703 2021-07-12 23:27:48.000000 hopeit.config-manager-0.9.3/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-07-12 23:34:16.330172 hopeit.config-manager-0.9.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1920 2021-07-12 23:27:48.000000 hopeit.config-manager-0.9.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-12 23:34:16.330172 hopeit.config-manager-0.9.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-12 23:34:16.330172 hopeit.config-manager-0.9.3/src/hopeit/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-12 23:34:16.330172 hopeit.config-manager-0.9.3/src/hopeit/config_manager/
--rw-r--r--   0 runner    (1001) docker     (121)      870 2021-07-12 23:27:48.000000 hopeit.config-manager-0.9.3/src/hopeit/config_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3158 2021-07-12 23:27:48.000000 hopeit.config-manager-0.9.3/src/hopeit/config_manager/client.py
--rw-r--r--   0 runner    (1001) docker     (121)      988 2021-07-12 23:27:48.000000 hopeit.config-manager-0.9.3/src/hopeit/config_manager/cluster_apps_config.py
--rw-r--r--   0 runner    (1001) docker     (121)      727 2021-07-12 23:27:48.000000 hopeit.config-manager-0.9.3/src/hopeit/config_manager/runtime.py
--rw-r--r--   0 runner    (1001) docker     (121)      972 2021-07-12 23:27:48.000000 hopeit.config-manager-0.9.3/src/hopeit/config_manager/runtime_apps_config.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-12 23:34:16.330172 hopeit.config-manager-0.9.3/src/hopeit.config_manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2005 2021-07-12 23:34:16.000000 hopeit.config-manager-0.9.3/src/hopeit.config_manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      471 2021-07-12 23:34:16.000000 hopeit.config-manager-0.9.3/src/hopeit.config_manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-07-12 23:34:16.000000 hopeit.config-manager-0.9.3/src/hopeit.config_manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       26 2021-07-12 23:34:16.000000 hopeit.config-manager-0.9.3/src/hopeit.config_manager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2021-07-12 23:34:16.000000 hopeit.config-manager-0.9.3/src/hopeit.config_manager.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-14 00:51:57.688907 hopeit.config-manager-0.9.4/
+-rw-r--r--   0 runner    (1001) docker     (121)     2005 2021-07-14 00:51:57.684907 hopeit.config-manager-0.9.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      703 2021-07-14 00:45:26.000000 hopeit.config-manager-0.9.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-07-14 00:51:57.688907 hopeit.config-manager-0.9.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1920 2021-07-14 00:45:26.000000 hopeit.config-manager-0.9.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-14 00:51:57.684907 hopeit.config-manager-0.9.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-14 00:51:57.684907 hopeit.config-manager-0.9.4/src/hopeit/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-14 00:51:57.684907 hopeit.config-manager-0.9.4/src/hopeit/config_manager/
+-rw-r--r--   0 runner    (1001) docker     (121)      936 2021-07-14 00:45:26.000000 hopeit.config-manager-0.9.4/src/hopeit/config_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3265 2021-07-14 00:45:26.000000 hopeit.config-manager-0.9.4/src/hopeit/config_manager/client.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1198 2021-07-14 00:45:26.000000 hopeit.config-manager-0.9.4/src/hopeit/config_manager/cluster_apps_config.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1547 2021-07-14 00:45:26.000000 hopeit.config-manager-0.9.4/src/hopeit/config_manager/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1201 2021-07-14 00:45:26.000000 hopeit.config-manager-0.9.4/src/hopeit/config_manager/runtime_apps_config.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-14 00:51:57.684907 hopeit.config-manager-0.9.4/src/hopeit.config_manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     2005 2021-07-14 00:51:57.000000 hopeit.config-manager-0.9.4/src/hopeit.config_manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      471 2021-07-14 00:51:57.000000 hopeit.config-manager-0.9.4/src/hopeit.config_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-07-14 00:51:57.000000 hopeit.config-manager-0.9.4/src/hopeit.config_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       26 2021-07-14 00:51:57.000000 hopeit.config-manager-0.9.4/src/hopeit.config_manager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        7 2021-07-14 00:51:57.000000 hopeit.config-manager-0.9.4/src/hopeit.config_manager.egg-info/top_level.txt
```

### Comparing `hopeit.config-manager-0.9.3/PKG-INFO` & `hopeit.config-manager-0.9.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hopeit.config-manager
-Version: 0.9.3
+Version: 0.9.4
 Summary: Hopeit Engine Config Manager Plugin
 Home-page: https://github.com/hopeit-git/hopeit.engine
 Author: Leo Smerling and Pablo Canto
 Author-email: contact@hopeit.com.ar
 License: Apache 2
 Project-URL: CI: GitHub Actions, https://github.com/hopeit-git/hopeit.engine/actions?query=workflow
 Project-URL: Docs: RTD, https://hopeitengine.readthedocs.io/en/latest/
```

### Comparing `hopeit.config-manager-0.9.3/README.md` & `hopeit.config-manager-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `hopeit.config-manager-0.9.3/setup.py` & `hopeit.config-manager-0.9.4/setup.py`

 * *Files identical despite different names*

### Comparing `hopeit.config-manager-0.9.3/src/hopeit/config_manager/client.py` & `hopeit.config-manager-0.9.4/src/hopeit/config_manager/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,28 +13,28 @@
 
 from hopeit.config_manager import RuntimeAppInfo, RuntimeApps, ServerStatus
 from hopeit.config_manager.runtime import get_in_process_config
 
 logger, extra = engine_extra_logger()
 
 
-async def get_apps_config(hosts: str, context: Optional[EventContext] = None) -> RuntimeApps:
+async def get_apps_config(hosts: str, context: Optional[EventContext] = None, **kwargs) -> RuntimeApps:
     """
     Gathers RuntimeApps (runtime apps config) from a given list of hosts running
     `hopeit.config-manager` plugins and returns a combined RuntimeApps
     specifiying for each app_key its configuration and description of hosts where
     it is avalable.
 
     :param: hosts, str: comma-separated list of the form `http://host:port` where to reach
         servers running hopeit.engine with enabled `config-manager` plugin.
     :return: RuntimeApps, combined from all requested hosts
     """
     responses = await asyncio.gather(
         *[
-            _get_host_config(host, context)
+            _get_host_config(host, context, **kwargs)
             for host in hosts.split(',')
         ]
     )
 
     apps: Dict[str, RuntimeAppInfo] = {}
     server_status: Dict[str, ServerStatus] = {}
     for host, runtime_apps_response in responses:
@@ -44,26 +44,29 @@
         elif isinstance(runtime_apps_response, ServerStatus):
             server_status[host] = runtime_apps_response
 
     return RuntimeApps(apps=apps, server_status=server_status)
 
 
 async def _get_host_config(host: str,
-                           context: Optional[EventContext] = None
-                           ) -> Tuple[str, Union[RuntimeApps, ServerStatus]]:
+                           context: Optional[EventContext] = None,
+                           **kwargs) -> Tuple[str, Union[RuntimeApps, ServerStatus]]:
     """
     Invokes config-manager runtime-apps-config endpoint in a given host
     """
     if host == "in-process":
-        return host, get_in_process_config(host)
+        return host, get_in_process_config(host, **kwargs)
 
     # Random <1 sec pause to prevent network overload
     await asyncio.sleep(random.random())
 
     url = f"{host}/api/config-manager/{APPS_ROUTE_VERSION}/runtime-apps-config?url={host}"
+    for k, v in kwargs.items():
+        url += f"&{k}={v}".lower()
+
     logger.info(context or __name__, "Invoking config-manager on host: %s...", host, extra=extra(
         host=host, url=url
     ))
 
     try:
         async with aiohttp.ClientSession() as client:
             async with client.get(url) as response:
```

### Comparing `hopeit.config-manager-0.9.3/src/hopeit/config_manager/cluster_apps_config.py` & `hopeit.config-manager-0.9.4/src/hopeit/config_manager/cluster_apps_config.py`

 * *Files 19% similar despite different names*

```diff
@@ -12,16 +12,25 @@
 logger, extra = app_extra_logger()
 
 __steps__ = ['get_hosts_apps_config']
 
 __api__ = event_api(
     summary="Config Manager: Cluster Apps Config",
     description="Handle remote access to runtime configuration for a group of hosts",
-    query_args=[("hosts", str, "Comma-separated list of http://host:port strings")],
+    query_args=[
+        ("hosts", str, "Comma-separated list of http://host:port strings"),
+        ("expand_events", bool, "Extract effective events from event steps")
+    ],
     responses={
         200: (RuntimeApps, "Combined config info about running apps in provided list of hosts")
     }
 )
 
 
-async def get_hosts_apps_config(payload: None, context: EventContext, *, hosts: str) -> RuntimeApps:
-    return await client.get_apps_config(hosts, context)
+async def get_hosts_apps_config(
+    payload: None, context: EventContext,
+    *, hosts: str, expand_events: bool = False
+) -> RuntimeApps:
+
+    return await client.get_apps_config(
+        hosts, context, expand_events=expand_events is True or expand_events == "true"
+    )
```

### Comparing `hopeit.config-manager-0.9.3/src/hopeit.config_manager.egg-info/PKG-INFO` & `hopeit.config-manager-0.9.4/src/hopeit.config_manager.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hopeit.config-manager
-Version: 0.9.3
+Version: 0.9.4
 Summary: Hopeit Engine Config Manager Plugin
 Home-page: https://github.com/hopeit-git/hopeit.engine
 Author: Leo Smerling and Pablo Canto
 Author-email: contact@hopeit.com.ar
 License: Apache 2
 Project-URL: CI: GitHub Actions, https://github.com/hopeit-git/hopeit.engine/actions?query=workflow
 Project-URL: Docs: RTD, https://hopeitengine.readthedocs.io/en/latest/
```

