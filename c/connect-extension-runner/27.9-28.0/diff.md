# Comparing `tmp/connect_extension_runner-27.9.tar.gz` & `tmp/connect_extension_runner-28.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "connect_extension_runner-27.9.tar", max compression
+gzip compressed data, was "connect_extension_runner-28.0.tar", max compression
```

## Comparing `connect_extension_runner-27.9.tar` & `connect_extension_runner-28.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0    11357 2023-03-22 15:22:15.174830 connect_extension_runner-27.9/LICENSE
--rw-r--r--   0        0        0     1422 2023-03-22 15:22:15.174830 connect_extension_runner-27.9/README.md
--rw-r--r--   0        0        0       55 2023-03-22 15:22:15.174830 connect_extension_runner-27.9/connect/eaas/dataclasses.py
--rw-r--r--   0        0        0      405 2023-03-22 15:22:15.174830 connect_extension_runner-27.9/connect/eaas/extension.py
--rw-r--r--   0        0        0      143 2023-03-22 15:22:15.174830 connect_extension_runner-27.9/connect/eaas/runner/__init__.py
--rw-r--r--   0        0        0        0 2023-03-22 15:22:15.174830 connect_extension_runner-27.9/connect/eaas/runner/artworks/__init__.py
--rw-r--r--   0        0        0     9409 2023-03-22 15:22:15.174830 connect_extension_runner-27.9/connect/eaas/runner/artworks/ansi_regular.flf
--rw-r--r--   0        0        0      950 2023-03-22 15:22:15.174830 connect_extension_runner-27.9/connect/eaas/runner/artworks/banner.py
--rw-r--r--   0        0        0    11425 2023-03-22 15:22:15.178830 connect_extension_runner-27.9/connect/eaas/runner/artworks/bloody.flf
--rw-r--r--   0        0        0     6483 2023-03-22 15:22:15.178830 connect_extension_runner-27.9/connect/eaas/runner/config.py
--rw-r--r--   0        0        0     5633 2023-03-22 15:22:15.178830 connect_extension_runner-27.9/connect/eaas/runner/constants.py
--rw-r--r--   0        0        0      320 2023-03-22 15:22:15.178830 connect_extension_runner-27.9/connect/eaas/runner/exceptions.py
--rw-r--r--   0        0        0        0 2023-03-22 15:22:15.178830 connect_extension_runner-27.9/connect/eaas/runner/handlers/__init__.py
--rw-r--r--   0        0        0     2692 2023-03-22 15:22:15.178830 connect_extension_runner-27.9/connect/eaas/runner/handlers/anvil.py
--rw-r--r--   0        0        0     4392 2023-03-22 15:22:15.178830 connect_extension_runner-27.9/connect/eaas/runner/handlers/base.py
--rw-r--r--   0        0        0     3751 2023-03-22 15:22:15.178830 connect_extension_runner-27.9/connect/eaas/runner/handlers/events.py
--rw-r--r--   0        0        0     2444 2023-03-22 15:22:15.178830 connect_extension_runner-27.9/connect/eaas/runner/handlers/transformations.py
--rw-r--r--   0        0        0     5793 2023-03-22 15:22:15.178830 connect_extension_runner-27.9/connect/eaas/runner/handlers/web.py
--rw-r--r--   0        0        0    18982 2023-03-22 15:22:15.178830 connect_extension_runner-27.9/connect/eaas/runner/helpers.py
--rw-r--r--   0        0        0     1989 2023-03-22 15:22:15.178830 connect_extension_runner-27.9/connect/eaas/runner/main.py
--rw-r--r--   0        0        0      340 2023-03-22 15:22:15.178830 connect_extension_runner-27.9/connect/eaas/runner/managers/__init__.py
--rw-r--r--   0        0        0     3191 2023-03-22 15:22:15.178830 connect_extension_runner-27.9/connect/eaas/runner/managers/background.py
--rw-r--r--   0        0        0     8101 2023-03-22 15:22:15.178830 connect_extension_runner-27.9/connect/eaas/runner/managers/base.py
--rw-r--r--   0        0        0     2225 2023-03-22 15:22:15.178830 connect_extension_runner-27.9/connect/eaas/runner/managers/interactive.py
--rw-r--r--   0        0        0     1931 2023-03-22 15:22:15.178830 connect_extension_runner-27.9/connect/eaas/runner/managers/scheduled.py
--rw-r--r--   0        0        0    14441 2023-03-22 15:22:15.178830 connect_extension_runner-27.9/connect/eaas/runner/managers/transformation.py
--rw-r--r--   0        0        0      533 2023-03-22 15:22:15.178830 connect_extension_runner-27.9/connect/eaas/runner/managers/utils.py
--rw-r--r--   0        0        0     7917 2023-03-22 15:22:15.178830 connect_extension_runner-27.9/connect/eaas/runner/master.py
--rw-r--r--   0        0        0        0 2023-03-22 15:22:15.178830 connect_extension_runner-27.9/connect/eaas/runner/workers/__init__.py
--rw-r--r--   0        0        0     2549 2023-03-22 15:22:15.178830 connect_extension_runner-27.9/connect/eaas/runner/workers/anvil.py
--rw-r--r--   0        0        0    11320 2023-03-22 15:22:15.178830 connect_extension_runner-27.9/connect/eaas/runner/workers/base.py
--rw-r--r--   0        0        0     8834 2023-03-22 15:22:15.178830 connect_extension_runner-27.9/connect/eaas/runner/workers/events.py
--rw-r--r--   0        0        0     6545 2023-03-22 15:22:15.178830 connect_extension_runner-27.9/connect/eaas/runner/workers/transformations.py
--rw-r--r--   0        0        0     6846 2023-03-22 15:22:15.178830 connect_extension_runner-27.9/connect/eaas/runner/workers/web.py
--rw-r--r--   0        0        0     2802 2023-03-22 15:23:39.386584 connect_extension_runner-27.9/pyproject.toml
--rw-r--r--   0        0        0     3026 1970-01-01 00:00:00.000000 connect_extension_runner-27.9/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-15 15:55:12.711196 connect_extension_runner-28.0/LICENSE
+-rw-r--r--   0        0        0     1422 2023-06-15 15:55:12.711196 connect_extension_runner-28.0/README.md
+-rw-r--r--   0        0        0       55 2023-06-15 15:55:12.711196 connect_extension_runner-28.0/connect/eaas/dataclasses.py
+-rw-r--r--   0        0        0      405 2023-06-15 15:55:12.711196 connect_extension_runner-28.0/connect/eaas/extension.py
+-rw-r--r--   0        0        0      143 2023-06-15 15:55:12.711196 connect_extension_runner-28.0/connect/eaas/runner/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-15 15:55:12.711196 connect_extension_runner-28.0/connect/eaas/runner/artworks/__init__.py
+-rw-r--r--   0        0        0     9409 2023-06-15 15:55:12.711196 connect_extension_runner-28.0/connect/eaas/runner/artworks/ansi_regular.flf
+-rw-r--r--   0        0        0      950 2023-06-15 15:55:12.711196 connect_extension_runner-28.0/connect/eaas/runner/artworks/banner.py
+-rw-r--r--   0        0        0    11425 2023-06-15 15:55:12.711196 connect_extension_runner-28.0/connect/eaas/runner/artworks/bloody.flf
+-rw-r--r--   0        0        0     6483 2023-06-15 15:55:12.711196 connect_extension_runner-28.0/connect/eaas/runner/config.py
+-rw-r--r--   0        0        0     5708 2023-06-15 15:55:12.711196 connect_extension_runner-28.0/connect/eaas/runner/constants.py
+-rw-r--r--   0        0        0      320 2023-06-15 15:55:12.711196 connect_extension_runner-28.0/connect/eaas/runner/exceptions.py
+-rw-r--r--   0        0        0        0 2023-06-15 15:55:12.711196 connect_extension_runner-28.0/connect/eaas/runner/handlers/__init__.py
+-rw-r--r--   0        0        0     2692 2023-06-15 15:55:12.711196 connect_extension_runner-28.0/connect/eaas/runner/handlers/anvil.py
+-rw-r--r--   0        0        0     4391 2023-06-15 15:55:12.711196 connect_extension_runner-28.0/connect/eaas/runner/handlers/base.py
+-rw-r--r--   0        0        0     3751 2023-06-15 15:55:12.711196 connect_extension_runner-28.0/connect/eaas/runner/handlers/events.py
+-rw-r--r--   0        0        0     2444 2023-06-15 15:55:12.711196 connect_extension_runner-28.0/connect/eaas/runner/handlers/transformations.py
+-rw-r--r--   0        0        0     6881 2023-06-15 15:55:12.711196 connect_extension_runner-28.0/connect/eaas/runner/handlers/web.py
+-rw-r--r--   0        0        0    18982 2023-06-15 15:55:12.715196 connect_extension_runner-28.0/connect/eaas/runner/helpers.py
+-rw-r--r--   0        0        0     1989 2023-06-15 15:55:12.715196 connect_extension_runner-28.0/connect/eaas/runner/main.py
+-rw-r--r--   0        0        0      340 2023-06-15 15:55:12.715196 connect_extension_runner-28.0/connect/eaas/runner/managers/__init__.py
+-rw-r--r--   0        0        0     3190 2023-06-15 15:55:12.715196 connect_extension_runner-28.0/connect/eaas/runner/managers/background.py
+-rw-r--r--   0        0        0     8100 2023-06-15 15:55:12.715196 connect_extension_runner-28.0/connect/eaas/runner/managers/base.py
+-rw-r--r--   0        0        0     2225 2023-06-15 15:55:12.715196 connect_extension_runner-28.0/connect/eaas/runner/managers/interactive.py
+-rw-r--r--   0        0        0     1931 2023-06-15 15:55:12.715196 connect_extension_runner-28.0/connect/eaas/runner/managers/scheduled.py
+-rw-r--r--   0        0        0    20464 2023-06-15 15:55:12.715196 connect_extension_runner-28.0/connect/eaas/runner/managers/transformation.py
+-rw-r--r--   0        0        0      533 2023-06-15 15:55:12.715196 connect_extension_runner-28.0/connect/eaas/runner/managers/utils.py
+-rw-r--r--   0        0        0     7917 2023-06-15 15:55:12.715196 connect_extension_runner-28.0/connect/eaas/runner/master.py
+-rw-r--r--   0        0        0        0 2023-06-15 15:55:12.715196 connect_extension_runner-28.0/connect/eaas/runner/workers/__init__.py
+-rw-r--r--   0        0        0     2549 2023-06-15 15:55:12.715196 connect_extension_runner-28.0/connect/eaas/runner/workers/anvil.py
+-rw-r--r--   0        0        0    11320 2023-06-15 15:55:12.715196 connect_extension_runner-28.0/connect/eaas/runner/workers/base.py
+-rw-r--r--   0        0        0     8834 2023-06-15 15:55:12.715196 connect_extension_runner-28.0/connect/eaas/runner/workers/events.py
+-rw-r--r--   0        0        0     6545 2023-06-15 15:55:12.715196 connect_extension_runner-28.0/connect/eaas/runner/workers/transformations.py
+-rw-r--r--   0        0        0     6916 2023-06-15 15:55:12.715196 connect_extension_runner-28.0/connect/eaas/runner/workers/web.py
+-rw-r--r--   0        0        0     2870 2023-06-15 15:56:19.568483 connect_extension_runner-28.0/pyproject.toml
+-rw-r--r--   0        0        0     2909 1970-01-01 00:00:00.000000 connect_extension_runner-28.0/PKG-INFO
```

### Comparing `connect_extension_runner-27.9/LICENSE` & `connect_extension_runner-28.0/LICENSE`

 * *Files identical despite different names*

### Comparing `connect_extension_runner-27.9/README.md` & `connect_extension_runner-28.0/README.md`

 * *Files identical despite different names*

### Comparing `connect_extension_runner-27.9/connect/eaas/runner/artworks/ansi_regular.flf` & `connect_extension_runner-28.0/connect/eaas/runner/artworks/ansi_regular.flf`

 * *Files identical despite different names*

### Comparing `connect_extension_runner-27.9/connect/eaas/runner/artworks/banner.py` & `connect_extension_runner-28.0/connect/eaas/runner/artworks/banner.py`

 * *Files identical despite different names*

### Comparing `connect_extension_runner-27.9/connect/eaas/runner/artworks/bloody.flf` & `connect_extension_runner-28.0/connect/eaas/runner/artworks/bloody.flf`

 * *Files identical despite different names*

### Comparing `connect_extension_runner-27.9/connect/eaas/runner/config.py` & `connect_extension_runner-28.0/connect/eaas/runner/config.py`

 * *Files identical despite different names*

### Comparing `connect_extension_runner-27.9/connect/eaas/runner/constants.py` & `connect_extension_runner-28.0/connect/eaas/runner/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -150,7 +150,10 @@
 PROCESS_CHECK_INTERVAL_SECS = 1
 
 LEVEL_TO_FONT_COLOR = {
     'INFO': ('ansi_regular', 'BLUE'),
     'WARNING': ('bloody', 'YELLOW'),
     'ERROR': ('bloody', 'RED'),
 }
+
+EXCEL_NULL_MARKER = '#N/A'
+ROW_DELETED_MARKER = '#INSTRUCTION/DELETE_ROW'
```

### Comparing `connect_extension_runner-27.9/connect/eaas/runner/handlers/anvil.py` & `connect_extension_runner-28.0/connect/eaas/runner/handlers/anvil.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 # This file is part of the Ingram Micro CloudBlue Connect EaaS Extension Runner.
 #
 # Copyright (c) 2022 Ingram Micro. All Rights Reserved.
 #
 import logging
 
 import anvil.server
+
 from connect.client import (
     ConnectClient,
 )
-
 from connect.eaas.core.logging import (
     RequestLogger,
 )
 from connect.eaas.runner.config import (
     ConfigHelper,
 )
 from connect.eaas.runner.handlers.base import (
```

### Comparing `connect_extension_runner-27.9/connect/eaas/runner/handlers/base.py` & `connect_extension_runner-28.0/connect/eaas/runner/handlers/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,14 @@
     abstractmethod,
 )
 
 from connect.client import (
     AsyncConnectClient,
     ConnectClient,
 )
-
 from connect.eaas.core.logging import (
     ExtensionLogHandler,
     RequestLogger,
 )
 from connect.eaas.runner.helpers import (
     iter_entry_points,
 )
```

### Comparing `connect_extension_runner-27.9/connect/eaas/runner/handlers/events.py` & `connect_extension_runner-28.0/connect/eaas/runner/handlers/events.py`

 * *Files identical despite different names*

### Comparing `connect_extension_runner-27.9/connect/eaas/runner/handlers/transformations.py` & `connect_extension_runner-28.0/connect/eaas/runner/handlers/transformations.py`

 * *Files identical despite different names*

### Comparing `connect_extension_runner-27.9/connect/eaas/runner/handlers/web.py` & `connect_extension_runner-28.0/connect/eaas/runner/handlers/web.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,15 @@
+#
+# Copyright (c) 2023 Ingram Micro. All Rights Reserved.
+#
+
 import functools
 import inspect
 import logging
 
-from connect.client import (
-    ClientError,
-)
 from fastapi import (
     FastAPI,
 )
 from fastapi.middleware.cors import (
     CORSMiddleware,
 )
 from fastapi.openapi.utils import (
@@ -18,14 +19,17 @@
 from fastapi.staticfiles import (
     StaticFiles,
 )
 from starlette.middleware.base import (
     BaseHTTPMiddleware,
 )
 
+from connect.client import (
+    ClientError,
+)
 from connect.eaas.core.decorators import (
     router as root_router,
 )
 from connect.eaas.core.utils import (
     client_error_exception_handler,
 )
 from connect.eaas.runner.config import (
@@ -44,14 +48,30 @@
         if scope['type'] != 'http' or scope['path'] != '/openapi/spec.json':  # pragma: no cover
             await self.app(scope, receive, send)
             return
 
         await super().__call__(scope, receive, send)  # pragma: no cover
 
 
+class _ProxyHeadersMiddleware:
+    def __init__(self, app):
+        self.app = app
+
+    async def __call__(self, scope, receive, send):
+        if scope['type'] == 'http':  # pragma: no branch
+            headers = dict(scope['headers'])
+            if b'x-forwarded-host' in headers:
+                headers[b'host'] = headers[b'x-forwarded-host']
+                scope['headers'] = list(headers.items())
+            if b'x-forwarded-proto' in headers:
+                scope['scheme'] = headers[b'x-forwarded-proto'].decode('ascii')
+
+        await self.app(scope, receive, send)
+
+
 class WebApp(ApplicationHandlerBase):
     """
     Handle the lifecycle of an extension.
     """
 
     LOGGER_NAME = 'eaas.webapp'
 
@@ -61,14 +81,18 @@
         self._app = None
 
     @property
     def ui_modules(self):
         return self.get_application().get_ui_modules()
 
     @property
+    def proxied_connect_api(self):
+        return self.get_application().get_proxied_connect_api()
+
+    @property
     def app(self):
         if not self._app:
             self._app = self.get_asgi_application()
         return self._app
 
     def get_application(self):
         return self.load_application('webapp')
@@ -123,30 +147,37 @@
                         'summary': generate_operation_summary(route=route, method=method),
                         'method': method,
                         'path': route.path,
                     })
         return endpoints
 
     def get_asgi_application(self):
+        exception_handlers = {ClientError: client_error_exception_handler}
+        if hasattr(self.get_application(), 'get_exception_handlers'):
+            exception_handlers = self.get_application().get_exception_handlers(
+                exception_handlers,
+            )
+
         app = FastAPI(
             openapi_url='/openapi/spec.json',
-            exception_handlers={
-                ClientError: client_error_exception_handler,
-            },
+            exception_handlers=exception_handlers,
         )
         app.add_middleware(
             _OpenApiCORSMiddleware,
             allow_origins=['*'],
         )
+        app.add_middleware(_ProxyHeadersMiddleware)
+
         if hasattr(self.get_application(), 'get_middlewares'):
             self.setup_middlewares(app, self.get_application().get_middlewares() or [])
 
         auth, no_auth = self.get_application().get_routers()
         app.include_router(auth, prefix='/api')
         app.include_router(no_auth, prefix='/guest')
+        app.include_router(no_auth, prefix='/unauthorized')
         app.openapi = functools.partial(self.get_api_schema, app)
         static_root = self.get_application().get_static_root()
         if static_root:
             app.mount('/static', StaticFiles(directory=static_root), name='static')
 
         return app
```

### Comparing `connect_extension_runner-27.9/connect/eaas/runner/helpers.py` & `connect_extension_runner-28.0/connect/eaas/runner/helpers.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -14,18 +14,14 @@
     version,
 )
 from uuid import (
     uuid4,
 )
 
 import requests
-from connect.client import (
-    ClientError,
-    ConnectClient,
-)
 from rich import (
     box,
 )
 from rich.align import (
     Align,
 )
 from rich.markdown import (
@@ -34,14 +30,18 @@
 from rich.syntax import (
     Syntax,
 )
 from rich.table import (
     Table,
 )
 
+from connect.client import (
+    ClientError,
+    ConnectClient,
+)
 from connect.eaas.core.validation.models import (
     ValidationItem,
     ValidationResult,
 )
 from connect.eaas.core.validation.validators import (
     get_validators,
 )
```

### Comparing `connect_extension_runner-27.9/connect/eaas/runner/main.py` & `connect_extension_runner-28.0/connect/eaas/runner/main.py`

 * *Files identical despite different names*

### Comparing `connect_extension_runner-27.9/connect/eaas/runner/managers/background.py` & `connect_extension_runner-28.0/connect/eaas/runner/managers/background.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 
 from connect.client import (
     AsyncConnectClient,
 )
 from connect.client.models import (
     AsyncResource,
 )
-
 from connect.eaas.core.enums import (
     ResultType,
 )
 from connect.eaas.core.proto import (
     Task,
     TaskOutput,
 )
```

### Comparing `connect_extension_runner-27.9/connect/eaas/runner/managers/base.py` & `connect_extension_runner-28.0/connect/eaas/runner/managers/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 from connect.client import (
     AsyncConnectClient,
     ClientError,
 )
 from connect.client.models import (
     AsyncCollection,
 )
-
 from connect.eaas.core.enums import (
     TaskCategory,
 )
 from connect.eaas.runner.config import (
     ConfigHelper,
 )
 from connect.eaas.runner.handlers.events import (
```

### Comparing `connect_extension_runner-27.9/connect/eaas/runner/managers/interactive.py` & `connect_extension_runner-28.0/connect/eaas/runner/managers/interactive.py`

 * *Files identical despite different names*

### Comparing `connect_extension_runner-27.9/connect/eaas/runner/managers/scheduled.py` & `connect_extension_runner-28.0/connect/eaas/runner/managers/scheduled.py`

 * *Files identical despite different names*

### Comparing `connect_extension_runner-27.9/connect/eaas/runner/managers/utils.py` & `connect_extension_runner-28.0/connect/eaas/runner/managers/utils.py`

 * *Files identical despite different names*

### Comparing `connect_extension_runner-27.9/connect/eaas/runner/master.py` & `connect_extension_runner-28.0/connect/eaas/runner/master.py`

 * *Files identical despite different names*

### Comparing `connect_extension_runner-27.9/connect/eaas/runner/workers/anvil.py` & `connect_extension_runner-28.0/connect/eaas/runner/workers/anvil.py`

 * *Files identical despite different names*

### Comparing `connect_extension_runner-27.9/connect/eaas/runner/workers/base.py` & `connect_extension_runner-28.0/connect/eaas/runner/workers/base.py`

 * *Files identical despite different names*

### Comparing `connect_extension_runner-27.9/connect/eaas/runner/workers/events.py` & `connect_extension_runner-28.0/connect/eaas/runner/workers/events.py`

 * *Files identical despite different names*

### Comparing `connect_extension_runner-27.9/connect/eaas/runner/workers/transformations.py` & `connect_extension_runner-28.0/connect/eaas/runner/workers/transformations.py`

 * *Files identical despite different names*

### Comparing `connect_extension_runner-27.9/connect/eaas/runner/workers/web.py` & `connect_extension_runner-28.0/connect/eaas/runner/workers/web.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,14 +56,15 @@
                 repository={
                     'readme_url': self.handler.readme,
                     'changelog_url': self.handler.changelog,
                 },
                 icon=self.handler.icon,
                 audience=self.handler.audience,
                 runner_version=get_version(),
+                proxied_connect_api=self.handler.proxied_connect_api,
             ),
         )
         logger.debug(f'Sending setup request: {pformat(msg)}')
         return msg.dict()
 
     async def stopping(self):
         pass
```

### Comparing `connect_extension_runner-27.9/pyproject.toml` & `connect_extension_runner-28.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "connect-extension-runner"
-version = "27.9"
+version = "28.0"
 description = "CloudBlue Connect EaaS Extension Runner"
 authors = ["CloudBlue LLC"]
 license = "Apache-2.0"
 packages = [
     { include = "connect" },
 ]
 readme = "./README.md"
@@ -25,24 +25,26 @@
 [tool.poetry.scripts]
 cextrun = 'connect.eaas.runner.main:main'
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4"
 websockets = "10.*"
 connect-openapi-client = ">=25.16"
-logzio-python-handler = "^3.0.0"
-backoff = "^1.11.1"
-uvloop = "^0.16.0"
-connect-eaas-core = ">=27.7,<28"
-httpx = "^0.23.0"
-rich = "^12.5.1"
+logzio-python-handler = "^3.1.1"
+backoff = "^2.2.1"
+connect-eaas-core = ">=28.3,<29"
+httpx = ">=0.23,<0.25"
+rich = ">=12"
 pyfiglet = "^0.8.post1"
-devtools = "^0.9.0"
-watchfiles = "^0.17.0"
-openpyxl = "^3.0.10"
+devtools = "^0.10.0"
+watchfiles = "^0.19.0"
+openpyxl = ">=3.0.0,<4"
+lxml = "^4.9.2"
+uvloop = "^0.17.0"
+urllib3 = "<2"
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.2.1"
 pytest-cov = "^4.0.0"
 pytest-mock = "^3.3.1"
 pytest-randomly = "^3.12.0"
 coverage = {extras = ["toml"], version = "^5.3"}
@@ -51,15 +53,15 @@
 flake8-cognitive-complexity = "^0.1"
 flake8-commas = "^2.1.0"
 flake8-future-import = "~0.4"
 flake8-broken-line = "^0.6"
 flake8-pyproject = "^1.2.2"
 pytest-asyncio = "0.20.*"
 pytest-httpx = ">=0.20"
-responses = "^0.21.0"
+responses = "^0.23.0"
 freezegun = "^1.2.1"
 flaky = "^3.7.0"
 flake8-isort = "^6.0.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
@@ -102,14 +104,15 @@
 python_files = "test_*.py"
 junit_family = "xunit2"
 asyncio_mode = "strict"
 
 [tool.isort]
 src_paths = "*"
 sections = ["FUTURE", "STDLIB", "THIRDPARTY", "FIRSTPARTY", "LOCALFOLDER"]
+known_first_party = ["connect"]
 group_by_package = true
 multi_line_output = 3
 force_grid_wrap = 1
 combine_as_imports = true
 use_parentheses = true
 include_trailing_comma = true
 line_length = 100
```

### Comparing `connect_extension_runner-27.9/PKG-INFO` & `connect_extension_runner-28.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: connect-extension-runner
-Version: 27.9
+Version: 28.0
 Summary: CloudBlue Connect EaaS Extension Runner
 Home-page: https://connect.cloudblue.com
 License: Apache-2.0
 Author: CloudBlue LLC
 Requires-Python: >=3.8,<4
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -12,31 +12,30 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Utilities
-Requires-Dist: backoff (>=1.11.1,<2.0.0)
-Requires-Dist: connect-eaas-core (>=27.7,<28)
+Requires-Dist: backoff (>=2.2.1,<3.0.0)
+Requires-Dist: connect-eaas-core (>=28.3,<29)
 Requires-Dist: connect-openapi-client (>=25.16)
-Requires-Dist: devtools (>=0.9.0,<0.10.0)
-Requires-Dist: httpx (>=0.23.0,<0.24.0)
-Requires-Dist: logzio-python-handler (>=3.0.0,<4.0.0)
-Requires-Dist: openpyxl (>=3.0.10,<4.0.0)
+Requires-Dist: devtools (>=0.10.0,<0.11.0)
+Requires-Dist: httpx (>=0.23,<0.25)
+Requires-Dist: logzio-python-handler (>=3.1.1,<4.0.0)
+Requires-Dist: lxml (>=4.9.2,<5.0.0)
+Requires-Dist: openpyxl (>=3.0.0,<4)
 Requires-Dist: pyfiglet (>=0.8.post1,<0.9)
-Requires-Dist: rich (>=12.5.1,<13.0.0)
-Requires-Dist: uvloop (>=0.16.0,<0.17.0)
-Requires-Dist: watchfiles (>=0.17.0,<0.18.0)
-Requires-Dist: websockets (>=10.0.0,<11.0.0)
+Requires-Dist: rich (>=12)
+Requires-Dist: urllib3 (<2)
+Requires-Dist: uvloop (>=0.17.0,<0.18.0)
+Requires-Dist: watchfiles (>=0.19.0,<0.20.0)
+Requires-Dist: websockets (==10.*)
 Project-URL: Repository, https://github.com/cloudblue/connect-extension-runner
 Description-Content-Type: text/markdown
 
 # CloudBlue Connect EaaS Extension Runner
 
 
 ![pyversions](https://img.shields.io/pypi/pyversions/connect-extension-runner.svg) [![PyPi Status](https://img.shields.io/pypi/v/connect-extension-runner.svg)](https://pypi.org/project/connect-extension-runner/) [![Build Connect Reports Core](https://github.com/cloudblue/connect-extension-runner/actions/workflows/build.yml/badge.svg)](https://github.com/cloudblue/connect-extension-runner/actions/workflows/build.yml) [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=connect-extension-runner&metric=alert_status)](https://sonarcloud.io/dashboard?id=connect-extension-runner) [![Coverage](https://sonarcloud.io/api/project_badges/measure?project=connect-extension-runner&metric=coverage)](https://sonarcloud.io/dashboard?id=connect-extension-runner) [![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=connect-extension-runner&metric=sqale_rating)](https://sonarcloud.io/dashboard?id=connect-extension-runner)![Docker Image Version (latest semver)](https://img.shields.io/docker/v/cloudblueconnect/connect-extension-runner?label=docker%20version&sort=semver)![Docker Image Size (latest semver)](https://img.shields.io/docker/image-size/cloudblueconnect/connect-extension-runner?label=docker%20image%20size&sort=semver)![Docker Pulls](https://img.shields.io/docker/pulls/cloudblueconnect/connect-extension-runner)
```

