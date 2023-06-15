# Comparing `tmp/api-reflector-0.7.0.tar.gz` & `tmp/api_reflector-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "api-reflector-0.7.0.tar", max compression
+gzip compressed data, was "api_reflector-0.8.0.tar", max compression
```

## Comparing `api-reflector-0.7.0.tar` & `api_reflector-0.8.0.tar`

### file list

```diff
@@ -1,30 +1,29 @@
--rw-r--r--   0        0        0     1061 2023-01-06 16:10:23.615163 api-reflector-0.7.0/LICENSE
--rw-r--r--   0        0        0        0 2023-01-06 16:10:23.615163 api-reflector-0.7.0/api_reflector/__init__.py
--rw-r--r--   0        0        0     2019 2023-01-06 16:10:23.615163 api-reflector-0.7.0/api_reflector/actions.py
--rw-r--r--   0        0        0     3625 2023-01-06 16:10:23.615163 api-reflector-0.7.0/api_reflector/admin.py
--rw-r--r--   0        0        0     2069 2023-01-06 16:10:23.615163 api-reflector-0.7.0/api_reflector/api.py
--rw-r--r--   0        0        0     1644 2023-01-06 16:10:23.615163 api-reflector-0.7.0/api_reflector/auth.py
--rw-r--r--   0        0        0      196 2023-01-06 16:10:23.615163 api-reflector-0.7.0/api_reflector/db.py
--rw-r--r--   0        0        0      643 2023-01-06 16:10:23.615163 api-reflector-0.7.0/api_reflector/endpoint.py
--rw-r--r--   0        0        0       38 2023-01-06 16:10:23.615163 api-reflector-0.7.0/api_reflector/migrations/README
--rw-r--r--   0        0        0        0 2023-01-06 16:10:23.615163 api-reflector-0.7.0/api_reflector/migrations/__init__.py
--rw-r--r--   0        0        0       37 2023-01-06 16:10:23.615163 api-reflector-0.7.0/api_reflector/migrations/alembic.ini
--rw-r--r--   0        0        0     1525 2023-01-06 16:10:23.615163 api-reflector-0.7.0/api_reflector/migrations/env.py
--rw-r--r--   0        0        0      594 2023-01-06 16:10:23.615163 api-reflector-0.7.0/api_reflector/migrations/run_migrations.py
--rw-r--r--   0        0        0      494 2023-01-06 16:10:23.615163 api-reflector-0.7.0/api_reflector/migrations/script.py.mako
--rw-r--r--   0        0        0      652 2023-01-06 16:10:23.615163 api-reflector-0.7.0/api_reflector/migrations/versions/76feeb81949a_callback_action.py
--rw-r--r--   0        0        0     3386 2023-01-06 16:10:23.615163 api-reflector-0.7.0/api_reflector/migrations/versions/7b4efa0dd5ea_initial.py
--rw-r--r--   0        0        0      475 2023-01-06 16:10:23.615163 api-reflector-0.7.0/api_reflector/migrations/versions/d42bddfac4f1_.py
--rw-r--r--   0        0        0     5123 2023-01-06 16:10:23.615163 api-reflector-0.7.0/api_reflector/models.py
--rw-r--r--   0        0        0     1625 2023-01-06 16:10:23.615163 api-reflector-0.7.0/api_reflector/reporting.py
--rw-r--r--   0        0        0     3558 2023-01-06 16:10:23.615163 api-reflector-0.7.0/api_reflector/rules_engine.py
--rw-r--r--   0        0        0   180327 2023-01-06 16:10:23.619163 api-reflector-0.7.0/api_reflector/static/bootstrap.min.css
--rw-r--r--   0        0        0     2764 2023-01-06 16:10:23.619163 api-reflector-0.7.0/api_reflector/static/filter.js
--rw-r--r--   0        0        0      138 2023-01-06 16:10:23.619163 api-reflector-0.7.0/api_reflector/templates/admin/index.html
--rw-r--r--   0        0        0     3260 2023-01-06 16:10:23.619163 api-reflector-0.7.0/api_reflector/templates/home.html
--rw-r--r--   0        0        0     1844 2023-01-06 16:10:23.619163 api-reflector-0.7.0/api_reflector/templating.py
--rw-r--r--   0        0        0     4690 2023-01-06 16:10:23.619163 api-reflector-0.7.0/api_reflector/views.py
--rw-r--r--   0        0        0     1455 2023-01-06 16:10:51.599313 api-reflector-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     1465 2023-01-06 16:10:23.619163 api-reflector-0.7.0/settings.py
--rw-r--r--   0        0        0     1436 1970-01-01 00:00:00.000000 api-reflector-0.7.0/setup.py
--rw-r--r--   0        0        0     1103 1970-01-01 00:00:00.000000 api-reflector-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-06-15 17:13:18.271103 api_reflector-0.8.0/LICENSE
+-rw-r--r--   0        0        0        0 2023-06-15 17:13:18.271103 api_reflector-0.8.0/api_reflector/__init__.py
+-rw-r--r--   0        0        0     2019 2023-06-15 17:13:18.271103 api_reflector-0.8.0/api_reflector/actions.py
+-rw-r--r--   0        0        0     3625 2023-06-15 17:13:18.271103 api_reflector-0.8.0/api_reflector/admin.py
+-rw-r--r--   0        0        0     2069 2023-06-15 17:13:18.271103 api_reflector-0.8.0/api_reflector/api.py
+-rw-r--r--   0        0        0     1644 2023-06-15 17:13:18.271103 api_reflector-0.8.0/api_reflector/auth.py
+-rw-r--r--   0        0        0      196 2023-06-15 17:13:18.271103 api_reflector-0.8.0/api_reflector/db.py
+-rw-r--r--   0        0        0      643 2023-06-15 17:13:18.271103 api_reflector-0.8.0/api_reflector/endpoint.py
+-rw-r--r--   0        0        0       38 2023-06-15 17:13:18.271103 api_reflector-0.8.0/api_reflector/migrations/README
+-rw-r--r--   0        0        0        0 2023-06-15 17:13:18.271103 api_reflector-0.8.0/api_reflector/migrations/__init__.py
+-rw-r--r--   0        0        0       37 2023-06-15 17:13:18.271103 api_reflector-0.8.0/api_reflector/migrations/alembic.ini
+-rw-r--r--   0        0        0     1525 2023-06-15 17:13:18.271103 api_reflector-0.8.0/api_reflector/migrations/env.py
+-rw-r--r--   0        0        0      594 2023-06-15 17:13:18.271103 api_reflector-0.8.0/api_reflector/migrations/run_migrations.py
+-rw-r--r--   0        0        0      494 2023-06-15 17:13:18.271103 api_reflector-0.8.0/api_reflector/migrations/script.py.mako
+-rw-r--r--   0        0        0      652 2023-06-15 17:13:18.271103 api_reflector-0.8.0/api_reflector/migrations/versions/76feeb81949a_callback_action.py
+-rw-r--r--   0        0        0     3386 2023-06-15 17:13:18.271103 api_reflector-0.8.0/api_reflector/migrations/versions/7b4efa0dd5ea_initial.py
+-rw-r--r--   0        0        0      475 2023-06-15 17:13:18.271103 api_reflector-0.8.0/api_reflector/migrations/versions/d42bddfac4f1_.py
+-rw-r--r--   0        0        0     5482 2023-06-15 17:13:18.271103 api_reflector-0.8.0/api_reflector/models.py
+-rw-r--r--   0        0        0     1625 2023-06-15 17:13:18.271103 api_reflector-0.8.0/api_reflector/reporting.py
+-rw-r--r--   0        0        0     3558 2023-06-15 17:13:18.271103 api_reflector-0.8.0/api_reflector/rules_engine.py
+-rw-r--r--   0        0        0   180327 2023-06-15 17:13:18.271103 api_reflector-0.8.0/api_reflector/static/bootstrap.min.css
+-rw-r--r--   0        0        0     2764 2023-06-15 17:13:18.271103 api_reflector-0.8.0/api_reflector/static/filter.js
+-rw-r--r--   0        0        0      138 2023-06-15 17:13:18.271103 api_reflector-0.8.0/api_reflector/templates/admin/index.html
+-rw-r--r--   0        0        0     3260 2023-06-15 17:13:18.271103 api_reflector-0.8.0/api_reflector/templates/home.html
+-rw-r--r--   0        0        0     1844 2023-06-15 17:13:18.271103 api_reflector-0.8.0/api_reflector/templating.py
+-rw-r--r--   0        0        0     4693 2023-06-15 17:13:18.271103 api_reflector-0.8.0/api_reflector/views.py
+-rw-r--r--   0        0        0     1430 2023-06-15 17:13:33.495456 api_reflector-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     1465 2023-06-15 17:13:18.275103 api_reflector-0.8.0/settings.py
+-rw-r--r--   0        0        0     1154 1970-01-01 00:00:00.000000 api_reflector-0.8.0/PKG-INFO
```

### Comparing `api-reflector-0.7.0/LICENSE` & `api_reflector-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `api-reflector-0.7.0/api_reflector/actions.py` & `api_reflector-0.8.0/api_reflector/actions.py`

 * *Files identical despite different names*

### Comparing `api-reflector-0.7.0/api_reflector/admin.py` & `api_reflector-0.8.0/api_reflector/admin.py`

 * *Files identical despite different names*

### Comparing `api-reflector-0.7.0/api_reflector/api.py` & `api_reflector-0.8.0/api_reflector/api.py`

 * *Files identical despite different names*

### Comparing `api-reflector-0.7.0/api_reflector/auth.py` & `api_reflector-0.8.0/api_reflector/auth.py`

 * *Files identical despite different names*

### Comparing `api-reflector-0.7.0/api_reflector/endpoint.py` & `api_reflector-0.8.0/api_reflector/endpoint.py`

 * *Files identical despite different names*

### Comparing `api-reflector-0.7.0/api_reflector/migrations/env.py` & `api_reflector-0.8.0/api_reflector/migrations/env.py`

 * *Files identical despite different names*

### Comparing `api-reflector-0.7.0/api_reflector/migrations/run_migrations.py` & `api_reflector-0.8.0/api_reflector/migrations/run_migrations.py`

 * *Files identical despite different names*

### Comparing `api-reflector-0.7.0/api_reflector/migrations/versions/76feeb81949a_callback_action.py` & `api_reflector-0.8.0/api_reflector/migrations/versions/76feeb81949a_callback_action.py`

 * *Files identical despite different names*

### Comparing `api-reflector-0.7.0/api_reflector/migrations/versions/7b4efa0dd5ea_initial.py` & `api_reflector-0.8.0/api_reflector/migrations/versions/7b4efa0dd5ea_initial.py`

 * *Files identical despite different names*

### Comparing `api-reflector-0.7.0/api_reflector/models.py` & `api_reflector-0.8.0/api_reflector/models.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # model classes are inherently just data structures, so pylint's warning here isn't particularly useful.
 # pylint: disable=too-few-public-methods
 
 """
 Contains definitions of SQLAlchemy database models.
 """
-from typing import Any, Mapping
+from typing import TYPE_CHECKING, Any, Mapping, cast
 
 from sqlalchemy import (
     ARRAY,
     Boolean,
     Column,
     Enum,
     ForeignKey,
@@ -19,15 +19,21 @@
     UniqueConstraint,
 )
 from sqlalchemy.orm import DeclarativeMeta, relationship
 
 from api_reflector import actions, db, endpoint, rules_engine
 from api_reflector.reporting import get_logger
 
-Model = db.Model  # type: DeclarativeMeta
+if TYPE_CHECKING:
+
+    class Model(db.Model):
+        """Dummy base class for type checking"""
+
+else:
+    Model = db.Model  # type: DeclarativeMeta
 
 
 log = get_logger(__name__)
 
 
 class Endpoint(Model):
     """
@@ -36,15 +42,15 @@
 
     __tablename__ = "endpoint"
 
     id = Column(Integer, primary_key=True)
 
     name = Column(String, nullable=False)
 
-    method = Column(Enum(endpoint.Method), nullable=False)
+    method: Column[endpoint.Method] = Column(Enum(endpoint.Method), nullable=False)
     path = Column(String, nullable=False)
 
     UniqueConstraint(method, path)
 
     responses = relationship("Response", back_populates="endpoint")
 
     def __str__(self) -> str:
@@ -84,15 +90,15 @@
     tags = relationship("Tag", secondary=response_tag, back_populates="responses")
 
     def __str__(self) -> str:
         max_body_length = 20
         if len(self.content) > max_body_length:
             body = f"{self.content[:max_body_length]}..."
         else:
-            body = self.content
+            body = cast(str, self.content)
 
         return f"{self.status_code} {body}" if body else str(self.status_code)
 
     def execute_actions(self, req_json: Mapping[str, Any], content: str):
         """
         Executes all response actions for the given response.
         """
@@ -110,56 +116,58 @@
 
     __tablename__ = "response_rule"
 
     id = Column(Integer, primary_key=True)
 
     response_id = Column(Integer, ForeignKey("response.id"), nullable=False)
 
-    operator = Column(Enum(rules_engine.Operator), nullable=False)
-    arguments = Column(ARRAY(String), nullable=False)
+    operator: Column[rules_engine.Operator] = Column(Enum(rules_engine.Operator), nullable=False)
+    arguments: Column[list[str]] = Column(ARRAY(String), nullable=False)
 
     response = relationship("Response", back_populates="rules")
 
     def __str__(self) -> str:
+        operator = cast(rules_engine.Operator, self.operator)
         rule_str = {
             rules_engine.Operator.EQUAL: "{} == {}",
             rules_engine.Operator.NOT_EQUAL: "{} != {}",
             rules_engine.Operator.LESS_THAN: "{} < {}",
             rules_engine.Operator.LESS_THAN_EQUAL: "{} <= {}",
             rules_engine.Operator.GREATER_THAN: "{} > {}",
             rules_engine.Operator.GREATER_THAN_EQUAL: "{} >= {}",
             rules_engine.Operator.IS_EMPTY: "{} is empty",
             rules_engine.Operator.IS_NOT_EMPTY: "{} is not empty",
             rules_engine.Operator.CONTAINS: "{} contains {}",
             rules_engine.Operator.NOT_CONTAINS: "{} does not contain {}",
-        }[self.operator]
+        }[operator]
         return rule_str.format(*self.arguments)
 
 
 class Action(Model):
     """
     Models an additional action to be taken when a response is chosen.
     """
 
     __tablename__ = "response_action"
 
     id = Column(Integer, primary_key=True)
 
     response_id = Column(Integer, ForeignKey("response.id"), nullable=False)
 
-    action = Column(Enum(actions.Action), nullable=False)
-    arguments = Column(ARRAY(String), nullable=False)
+    action: Column[actions.Action] = Column(Enum(actions.Action), nullable=False)
+    arguments: Column[list[str]] = Column(ARRAY(String), nullable=False)
 
     response = relationship("Response", back_populates="actions")
 
     def __str__(self) -> str:
+        action = cast(actions.Action, self.action)
         action_str = {
             actions.Action.DELAY: "Delay for {} second(s)",
             actions.Action.CALLBACK: "Do the callback",
-        }[self.action]
+        }[action]
         return action_str.format(*self.arguments)
 
 
 class Tag(Model):
     """
     Models a tag used for tagging responses to group related responses together.
     """
```

### Comparing `api-reflector-0.7.0/api_reflector/reporting.py` & `api_reflector-0.8.0/api_reflector/reporting.py`

 * *Files identical despite different names*

### Comparing `api-reflector-0.7.0/api_reflector/rules_engine.py` & `api_reflector-0.8.0/api_reflector/rules_engine.py`

 * *Files identical despite different names*

### Comparing `api-reflector-0.7.0/api_reflector/static/bootstrap.min.css` & `api_reflector-0.8.0/api_reflector/static/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `api-reflector-0.7.0/api_reflector/static/filter.js` & `api_reflector-0.8.0/api_reflector/static/filter.js`

 * *Files identical despite different names*

### Comparing `api-reflector-0.7.0/api_reflector/templates/home.html` & `api_reflector-0.8.0/api_reflector/templates/home.html`

 * *Files identical despite different names*

### Comparing `api-reflector-0.7.0/api_reflector/templating.py` & `api_reflector-0.8.0/api_reflector/templating.py`

 * *Files identical despite different names*

### Comparing `api-reflector-0.7.0/api_reflector/views.py` & `api_reflector-0.8.0/api_reflector/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 Defines the project's API endpoints.
 """
-from typing import Any, Mapping, Union
+from typing import Any, Mapping, Union, cast
 
 import psycopg2
 from flask import Blueprint, Response, request
 from flask_admin.base import render_template
 from jinja2.exceptions import TemplateError, TemplateSyntaxError, UndefinedError
 from werkzeug.routing import Map, Rule
 
@@ -28,15 +28,15 @@
 
     log.debug(f"Matching path `{path}`")
 
     endpoints: list[models.Endpoint] = models.Endpoint.query.filter(
         models.Endpoint.method == request.method.upper()
     ).all()
 
-    rules = [Rule(endpoint.path, endpoint=endpoint, methods=[request.method]) for endpoint in endpoints]
+    rules = [Rule(cast(str, endpoint.path), endpoint=endpoint, methods=[request.method]) for endpoint in endpoints]
     urls = Map(rules).bind("localhost")
 
     # we're disabling mypy here because you're supposed to get strings back from `match`, not full endpoint objects.
     return urls.match(path, method=request.method)  # type: ignore
 
 
 def _process_error_response(ex: Union[UndefinedError, TemplateSyntaxError, TemplateError]) -> Response:
@@ -137,9 +137,8 @@
 
     except UndefinedError as ex:
         return _process_error_response(ex)
     except TemplateSyntaxError as ex:
         return _process_error_response(ex)
     except TemplateError as ex:
         return _process_error_response(ex)
-    else:
-        return Response(content, status=response.status_code, mimetype=response.content_type)
+    return Response(content, status=response.status_code, mimetype=response.content_type)
```

### Comparing `api-reflector-0.7.0/pyproject.toml` & `api_reflector-0.8.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 [tool.poetry]
 name = "api-reflector"
-version = "0.7.0"
+version = "0.8.0"
 description = "A configurable API mocking service"
 authors = ["Chris Latham <cl@bink.com>"]
 license = "MIT"
-packages = [
-    { include = "api_reflector" },
-    { include = "settings.py" },
-]
+packages = [{ include = "api_reflector" }, { include = "settings.py" }]
 
 [tool.poetry.scripts]
 api-reflector-migrate = "api_reflector.migrations.run_migrations:main"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 Flask = "^2.2.2"
@@ -54,17 +51,13 @@
 line-length = 120
 
 [tool.isort]
 profile = "black"
 
 [tool.mypy]
 ignore_missing_imports = true
-plugins = [
-    "sqlalchemy.ext.mypy.plugin",
-]
+plugins = ["sqlalchemy.ext.mypy.plugin"]
 
 [tool.pylint.messages_control]
 max-line-length = 120
 ignore = ["settings.py", "wsgi.py"]
-disable = [
-    "logging-fstring-interpolation",
-]
+disable = ["logging-fstring-interpolation"]
```

### Comparing `api-reflector-0.7.0/settings.py` & `api_reflector-0.8.0/settings.py`

 * *Files identical despite different names*

### Comparing `api-reflector-0.7.0/PKG-INFO` & `api_reflector-0.8.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: api-reflector
-Version: 0.7.0
+Version: 0.8.0
 Summary: A configurable API mocking service
 License: MIT
 Author: Chris Latham
 Author-email: cl@bink.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Flask (>=2.2.2,<3.0.0)
 Requires-Dist: Flask-Admin (>=1.6.0,<2.0.0)
 Requires-Dist: Flask-Cors (>=3.0.10,<4.0.0)
 Requires-Dist: Flask-Dance (>=6.1.1,<7.0.0)
 Requires-Dist: Flask-SQLAlchemy (>=2.5.1,<3.0.0)
 Requires-Dist: Jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: alembic (>=1.8.1,<2.0.0)
```

