# Comparing `tmp/django_access_inspector-0.1.0.tar.gz` & `tmp/django_access_inspector-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_access_inspector-0.1.0.tar", max compression
+gzip compressed data, was "django_access_inspector-0.2.0.tar", max compression
```

## Comparing `django_access_inspector-0.1.0.tar` & `django_access_inspector-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      661 2023-06-06 10:13:09.817673 django_access_inspector-0.1.0/README.md
--rw-r--r--   0        0        0       80 2023-06-06 08:59:56.214457 django_access_inspector-0.1.0/django_access_inspector/__init__.py
--rw-r--r--   0        0        0      214 2023-06-06 08:59:35.358727 django_access_inspector-0.1.0/django_access_inspector/apps.py
--rw-r--r--   0        0        0        0 2023-05-12 07:44:26.702861 django_access_inspector-0.1.0/django_access_inspector/management/commands/__init__.py
--rw-r--r--   0        0        0    11452 2023-06-06 09:15:25.583484 django_access_inspector-0.1.0/django_access_inspector/management/commands/inspect_access_control.py
--rw-r--r--   0        0        0        0 2023-05-12 07:44:26.697168 django_access_inspector-0.1.0/django_access_inspector/migrations/__init__.py
--rw-r--r--   0        0        0       27 2023-05-12 14:52:13.253924 django_access_inspector-0.1.0/django_access_inspector/models.py
--rw-r--r--   0        0        0        0 2023-05-12 13:53:16.305989 django_access_inspector-0.1.0/django_access_inspector/permissions.py
--rw-r--r--   0        0        0     3531 2023-06-06 09:14:44.250249 django_access_inspector-0.1.0/django_access_inspector/settings.py
--rw-r--r--   0        0        0     1176 2023-06-06 09:07:57.365718 django_access_inspector-0.1.0/django_access_inspector/tests/management/command/test_scan_access_control.py
--rw-r--r--   0        0        0      195 2023-05-12 16:47:21.310700 django_access_inspector-0.1.0/django_access_inspector/tests/mocks/permissions.py
--rw-r--r--   0        0        0     2627 2023-06-06 08:58:22.193482 django_access_inspector-0.1.0/django_access_inspector/tests/mocks/views.py
--rw-r--r--   0        0        0        0 2023-05-12 09:15:50.318163 django_access_inspector-0.1.0/django_access_inspector/urls.py
--rw-r--r--   0        0        0        0 2023-05-12 09:15:38.338344 django_access_inspector-0.1.0/django_access_inspector/views.py
--rw-r--r--   0        0        0      679 2023-06-06 12:25:49.187582 django_access_inspector-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1322 1970-01-01 00:00:00.000000 django_access_inspector-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1570 2023-06-15 14:20:56.592805 django_access_inspector-0.2.0/README.md
+-rw-r--r--   0        0        0       80 2023-06-06 08:59:56.214457 django_access_inspector-0.2.0/django_access_inspector/__init__.py
+-rw-r--r--   0        0        0      214 2023-06-06 08:59:35.358727 django_access_inspector-0.2.0/django_access_inspector/apps.py
+-rw-r--r--   0        0        0        0 2023-05-12 07:44:26.702861 django_access_inspector-0.2.0/django_access_inspector/management/commands/__init__.py
+-rw-r--r--   0        0        0    12785 2023-06-15 13:59:22.368908 django_access_inspector-0.2.0/django_access_inspector/management/commands/inspect_access_control.py
+-rw-r--r--   0        0        0        0 2023-05-12 07:44:26.697168 django_access_inspector-0.2.0/django_access_inspector/migrations/__init__.py
+-rw-r--r--   0        0        0       27 2023-05-12 14:52:13.253924 django_access_inspector-0.2.0/django_access_inspector/models.py
+-rw-r--r--   0        0        0        0 2023-05-12 13:53:16.305989 django_access_inspector-0.2.0/django_access_inspector/permissions.py
+-rw-r--r--   0        0        0     3531 2023-06-06 09:14:44.250249 django_access_inspector-0.2.0/django_access_inspector/settings.py
+-rw-r--r--   0        0        0     1176 2023-06-06 09:07:57.365718 django_access_inspector-0.2.0/django_access_inspector/tests/management/command/test_scan_access_control.py
+-rw-r--r--   0        0        0      195 2023-05-12 16:47:21.310700 django_access_inspector-0.2.0/django_access_inspector/tests/mocks/permissions.py
+-rw-r--r--   0        0        0     2627 2023-06-06 08:58:22.193482 django_access_inspector-0.2.0/django_access_inspector/tests/mocks/views.py
+-rw-r--r--   0        0        0        0 2023-05-12 09:15:50.318163 django_access_inspector-0.2.0/django_access_inspector/urls.py
+-rw-r--r--   0        0        0        0 2023-05-12 09:15:38.338344 django_access_inspector-0.2.0/django_access_inspector/views.py
+-rw-r--r--   0        0        0      679 2023-06-15 14:22:35.015780 django_access_inspector-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2231 1970-01-01 00:00:00.000000 django_access_inspector-0.2.0/PKG-INFO
```

### Comparing `django_access_inspector-0.1.0/django_access_inspector/management/commands/inspect_access_control.py` & `django_access_inspector-0.2.0/django_access_inspector/management/commands/inspect_access_control.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from django.core.exceptions import ViewDoesNotExist
 from django.core.management.base import BaseCommand, CommandError
 from django.urls import URLPattern, URLResolver  # type: ignore
 from django.utils import translation
 from rich.console import Console
 from rich.table import Table
 from rich.text import Text
+from rich.panel import Panel
 
 
 class RegexURLPattern:  # type: ignore
     pass
 
 
 class RegexURLResolver:  # type: ignore
@@ -56,16 +57,21 @@
         except Exception as e:
             raise CommandError(
                 "Error occurred while trying to load %s: %s"
                 % (getattr(settings, urlconf), str(e))
             )
 
         view_functions = self.extract_views_from_urlpatterns(urlconf.urlpatterns)
+        admin_views = []
 
         for func, _, url_name in view_functions:
+            if hasattr(func, "model_admin"):
+                admin_views.append(url_name)
+                continue
+
             permissions = []
             authentications = []
             if url_name is not None and hasattr(views, url_name):
                 permissions = views[url_name].get("permission_classes", [])
 
             if hasattr(func, "view_class"):
                 permissions.extend(
@@ -124,134 +130,149 @@
                     func_name = func.__name__
                 elif hasattr(func, "__class__"):
                     func_name = "%s()" % func.__class__.__name__
                 else:
                     func_name = re.sub(r" at 0x[0-9a-f]+", "", repr(func))
 
                 unchecked_views.append(f"{url_name} / {func_name}")
+                continue
 
             views[url_name] = {
-                "permissions_classes": list(set(permissions)),
+                "permission_classes": list(set(permissions)),
                 "authentication_classes": list(set(authentications)),
             }
 
         split_views = self.split_views(views)
 
         if options["output"] == "json":
             print(
-                json.dumps({"views": split_views, "unchecked_views": unchecked_views})
+                json.dumps(
+                    {
+                        "views": split_views,
+                        "model_admin_views": admin_views,
+                        "unchecked_views": unchecked_views,
+                    }
+                )
             )
         else:
-            self.print_views_in_terminal(views, unchecked_views)
+            self.print_views_in_terminal(views, unchecked_views, admin_views)
 
     def get_default_classes(self):
-        default_classes = {"authentication": [], "permission": []}
+        default_classes = {
+            "authentication": ["BasicAuthentication"],
+            "permission": ["AllowAny"],
+        }
         if getattr(settings, "REST_FRAMEWORK", None) is None:
             return default_classes
         default_classes["permission"] = [
             c.split(".")[-1]
             for c in settings.REST_FRAMEWORK.get("DEFAULT_PERMISSION_CLASSES", [])
         ]
         default_classes["authentication"] = [
             c.split(".")[-1]
             for c in settings.REST_FRAMEWORK.get("DEFAULT_AUTHENTICATION_CLASSES", [])
         ]
         return default_classes
 
-    def _render_class_cell(
-        self, classes, default_classes, number_of_no, number_of_default
-    ):
+    def _render_class_cell(self, classes, default_classes):
         if len(classes) == 0:
-            return (Text("None", style="bold red"), number_of_no + 1, number_of_default)
+            return Text("None", style="bold red")
         if len(classes) == 1 and classes[0] in default_classes:
-            return (
-                Text(classes[0], style="bold yellow"),
-                number_of_no,
-                number_of_default + 1,
-            )
-        return (Text(", ".join(classes)), number_of_no, number_of_default)
+            return Text(classes[0], style="bold yellow")
+        return Text(", ".join(classes))
 
-    def print_views_in_terminal(self, views, unchecked_views):
+    def count_ko_and_default(self, classes_list, default_classes):
+        number_of_no, number_of_default = 0, 0
+        for classes in classes_list:
+            if len(classes) == 0:
+                number_of_no = number_of_no + 1
+            if len(classes) == 1 and classes[0] in default_classes:
+                number_of_default = number_of_default + 1
+        return number_of_no, number_of_default
+
+    def _set_color(self, count):
+        if count == 0:
+            return "green"
+        return "red"
+
+    def print_views_in_terminal(self, views, unchecked_views, admin_views):
         console = Console()
 
         table = Table(show_header=True, header_style="bold magenta")
-        table.add_column("View")
-        table.add_column("Permission Classes")
-        table.add_column("Authentication Classes")
+        table.add_column(f"Unchecked: {len(unchecked_views)} views")
+        for view in unchecked_views:
+            table.add_row(Text(view, style="bold red"))
+        console.print(table)
+
+        table = Table(show_header=True, header_style="bold magenta")
+        table.add_column(f"Model admin: {len(admin_views)} views")
+        for view in admin_views:
+            if view is not None:
+                table.add_row(Text(view, style="bold grey"))
+        console.print(table)
+
         default_classes = self.get_default_classes()
-        no_authentication, authentication_default, no_permission, permission_default = (
-            0,
-            0,
-            0,
-            0,
+
+        table = Table(show_header=True, header_style="bold magenta")
+        table.add_column("Views")
+
+        no_authentication, authentication_default = self.count_ko_and_default(
+            [perm.get("authentication_classes", []) for perm in views.values()],
+            default_classes["authentication"],
+        )
+        table.add_column("Authentication Classes")
+        no_permission, permission_default = self.count_ko_and_default(
+            [perm.get("permission_classes", []) for perm in views.values()],
+            default_classes["permission"],
         )
+        table.add_column("Permission Classes")
+
         for url, perm in views.items():
             if url is not None:
-                (
-                    permissions,
-                    no_permission,
-                    permission_default,
-                ) = self._render_class_cell(
-                    perm.get("permissions_classes", []),
+                permissions = self._render_class_cell(
+                    perm.get("permission_classes", []),
                     default_classes["permission"],
-                    no_permission,
-                    permission_default,
                 )
-                (
-                    authentications,
-                    no_authentication,
-                    authentication_default,
-                ) = self._render_class_cell(
+                authentications = self._render_class_cell(
                     perm.get("authentication_classes", []),
                     default_classes["authentication"],
-                    no_authentication,
-                    authentication_default,
                 )
                 table.add_row(
                     Text(url, style="bold blue"), permissions, authentications
                 )
 
         number_of_views = len(views.keys())
         console.print(table)
 
         console.print(
-            Text(
-                f"Default authentication: {authentication_default} / {number_of_views}",
-                style="bold yellow",
+            Panel(
+                f"Number of views: {number_of_views}\nUnchecked views: {len(unchecked_views)}\nModel admin views: {len(admin_views)}",
+                title="Details views",
             )
         )
         console.print(
-            Text(
-                f"No authentication: {no_authentication} / {number_of_views}",
-                style="bold red",
+            Panel(
+                f"Default: [{self._set_color(authentication_default)}]{authentication_default}/{number_of_views}[/{self._set_color(authentication_default)}]\nNo authentication: [{self._set_color(no_authentication)}]{no_authentication}/{number_of_views}[/{self._set_color(no_authentication)}]",
+                title="Authentication",
             )
         )
         console.print(
-            Text(
-                f"Default permission: {permission_default} / {number_of_views}",
-                style="bold yellow",
+            Panel(
+                f"Default: [{self._set_color(permission_default)}]{permission_default}/{number_of_views}[/{self._set_color(permission_default)}]\nNo permission: [{self._set_color(no_permission)}]{no_permission}/{number_of_views}[/{self._set_color(no_permission)}]",
+                title="Permission",
             )
         )
-        console.print(
-            Text(
-                f"No permission: {no_permission} / {number_of_views}",
-                style="bold red",
-            )
-        )
-        console.print(
-            Text(f"Unchecked views: {len(unchecked_views)}", style="bold red")
-        )
 
     def split_views(self, views):
         authenticated = {}
         unauthenticated = {}
         for url, perm in views.items():
             if (
                 len(perm.get("authentication_classes", 0)) > 0
-                or len(perm.get("permissions_classes", 0)) > 0
+                or len(perm.get("permission_classes", 0)) > 0
             ):
                 authenticated[url] = perm
             else:
                 unauthenticated[url] = perm
         return {"authenticated": authenticated, "unauthenticated": unauthenticated}
 
     def extract_views_from_urlpatterns(self, urlpatterns, base="", namespace=None):
```

### Comparing `django_access_inspector-0.1.0/django_access_inspector/settings.py` & `django_access_inspector-0.2.0/django_access_inspector/settings.py`

 * *Files identical despite different names*

### Comparing `django_access_inspector-0.1.0/django_access_inspector/tests/management/command/test_scan_access_control.py` & `django_access_inspector-0.2.0/django_access_inspector/tests/management/command/test_scan_access_control.py`

 * *Files identical despite different names*

### Comparing `django_access_inspector-0.1.0/django_access_inspector/tests/mocks/views.py` & `django_access_inspector-0.2.0/django_access_inspector/tests/mocks/views.py`

 * *Files identical despite different names*

### Comparing `django_access_inspector-0.1.0/pyproject.toml` & `django_access_inspector-0.2.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-access-inspector"
-version = "0.1.0"
+version = "0.2.0"
 license='MIT License'
 repository="https://github.com/BastienTeissier/django-access-inspector"
 description='A tool to analyze your Django app access control'
 authors = ["Bastien Teissier <bastient@theodo.fr>"]
 readme = "README.md"
 packages = [{include = "django_access_inspector"}]
```

### Comparing `django_access_inspector-0.1.0/PKG-INFO` & `django_access_inspector-0.2.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-access-inspector
-Version: 0.1.0
+Version: 0.2.0
 Summary: A tool to analyze your Django app access control
 Home-page: https://github.com/BastienTeissier/django-access-inspector
 License: MIT
 Author: Bastien Teissier
 Author-email: bastient@theodo.fr
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -17,30 +17,50 @@
 
 # Django Access Inspector
 
 Django Access Inspector is a comprehensive access control app for Django that helps you enforce fine-grained access control on your views. It provides a flexible and easy-to-use interface to check and analyze authentication and permission classes for each view in your Django project.
 
 ## Installation
 
-Run one of the following command:
+To install Django Access Inspector, you can use either `pip` or `poetry`. Here are the commands:
 
-```
+```shell
 pip install django-access-inspector
 ```
 
-```
+```shell
 poetry add django-access-inspector
 ```
 
-Add "django_access_inspector" to your INSTALLED_APPS setting like this:
+After installing, make sure to add `"django_access_inspector"` to your `INSTALLED_APPS` setting in your Django project's `settings.py` file:
+
+```python
+INSTALLED_APPS = [
+    ...,
+    "django_access_inspector",
+]
+```
 
-    INSTALLED_APPS = [
-        ...,
-        "django_access_inspector",
-    ]
+## Usage
 
-## Run
+To run Django Access Inspector, use the following command:
 
-```
+```shell
 python manage.py inspect_access_control
 ```
 
+By default, it will provide a human-readable output. If you prefer a JSON output, you can use the `--output json` flag:
+
+```shell
+python manage.py inspect_access_control --output json
+```
+
+## Example
+
+![cli example output](/assets/cli_output.png)
+
+Here's an interpretation of the output:
+
+- **Unchecked views**: Views that Django Access Inspector was not able to check. As the tool is still a work in progress, we aim to make it check all views in the future.
+- **Model Admin views**: Views generated by Django Admin that are checked with the Django Admin permission system.
+- **Views**: All views that Django Access Inspector was able to check, including their authentication and permission classes.
+
```

