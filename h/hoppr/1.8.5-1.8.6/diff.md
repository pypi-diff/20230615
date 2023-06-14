# Comparing `tmp/hoppr-1.8.5.tar.gz` & `tmp/hoppr-1.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hoppr-1.8.5.tar", max compression
+gzip compressed data, was "hoppr-1.8.6.tar", max compression
```

## Comparing `hoppr-1.8.5.tar` & `hoppr-1.8.6.tar`

### file list

```diff
@@ -1,61 +1,61 @@
--rw-r--r--   0        0        0     1084 2023-05-24 23:07:22.000000 hoppr-1.8.5/LICENSE
--rw-r--r--   0        0        0     1214 2023-05-24 23:07:22.000000 hoppr-1.8.5/README.md
--rw-r--r--   0        0        0     1035 2023-05-24 23:07:22.000000 hoppr-1.8.5/hoppr/__init__.py
--rw-r--r--   0        0        0      161 2023-05-24 23:07:22.000000 hoppr-1.8.5/hoppr/__main__.py
--rw-r--r--   0        0        0        0 2023-05-24 23:07:22.000000 hoppr-1.8.5/hoppr/base_plugins/__init__.py
--rw-r--r--   0        0        0    11010 2023-05-24 23:07:22.000000 hoppr-1.8.5/hoppr/base_plugins/collector.py
--rw-r--r--   0        0        0    10707 2023-05-24 23:07:22.000000 hoppr-1.8.5/hoppr/base_plugins/hoppr.py
--rw-r--r--   0        0        0        0 2023-05-24 23:07:22.000000 hoppr-1.8.5/hoppr/base_plugins/py.typed
--rw-r--r--   0        0        0        0 2023-05-24 23:07:22.000000 hoppr-1.8.5/hoppr/cli/__init__.py
--rw-r--r--   0        0        0     6256 2023-05-24 23:07:22.000000 hoppr-1.8.5/hoppr/cli/hopctl.py
--rw-r--r--   0        0        0      563 2023-05-24 23:07:22.000000 hoppr-1.8.5/hoppr/constants.py
--rw-r--r--   0        0        0        0 2023-05-24 23:07:22.000000 hoppr-1.8.5/hoppr/core_plugins/__init__.py
--rw-r--r--   0        0        0     3046 2023-05-24 23:07:22.000000 hoppr-1.8.5/hoppr/core_plugins/bundle_tar.py
--rw-r--r--   0        0        0    12943 2023-05-24 23:07:22.000000 hoppr-1.8.5/hoppr/core_plugins/collect_apt_plugin.py
--rw-r--r--   0        0        0    10272 2023-05-24 23:07:22.000000 hoppr-1.8.5/hoppr/core_plugins/collect_dnf_plugin.py
--rw-r--r--   0        0        0     3840 2023-05-24 23:07:22.000000 hoppr-1.8.5/hoppr/core_plugins/collect_docker_plugin.py
--rw-r--r--   0        0        0     4664 2023-05-24 23:07:22.000000 hoppr-1.8.5/hoppr/core_plugins/collect_git_plugin.py
--rw-r--r--   0        0        0     4113 2023-05-24 23:07:22.000000 hoppr-1.8.5/hoppr/core_plugins/collect_helm_plugin.py
--rw-r--r--   0        0        0     6369 2023-05-24 23:07:22.000000 hoppr-1.8.5/hoppr/core_plugins/collect_maven_plugin.py
--rw-r--r--   0        0        0     7961 2023-05-24 23:07:22.000000 hoppr-1.8.5/hoppr/core_plugins/collect_nexus_search.py
--rw-r--r--   0        0        0     4418 2023-05-24 23:07:22.000000 hoppr-1.8.5/hoppr/core_plugins/collect_pypi_plugin.py
--rw-r--r--   0        0        0     3043 2023-05-24 23:07:22.000000 hoppr-1.8.5/hoppr/core_plugins/collect_raw_plugin.py
--rw-r--r--   0        0        0     3739 2023-05-24 23:07:22.000000 hoppr-1.8.5/hoppr/core_plugins/collect_yum_plugin.py
--rw-r--r--   0        0        0     4278 2023-05-24 23:07:22.000000 hoppr-1.8.5/hoppr/core_plugins/composite_collector.py
--rw-r--r--   0        0        0     5673 2023-05-24 23:07:22.000000 hoppr-1.8.5/hoppr/core_plugins/delta_sbom.py
--rw-r--r--   0        0        0     6885 2023-05-24 23:07:22.000000 hoppr-1.8.5/hoppr/core_plugins/oras_bundle.py
--rw-r--r--   0        0        0     5301 2023-05-24 23:07:22.000000 hoppr-1.8.5/hoppr/core_plugins/oras_registry.py
--rw-r--r--   0        0        0        0 2023-05-24 23:07:22.000000 hoppr-1.8.5/hoppr/core_plugins/py.typed
--rw-r--r--   0        0        0      202 2023-05-24 23:07:22.000000 hoppr-1.8.5/hoppr/core_plugins/report_generator/__init__.py
--rw-r--r--   0        0        0   126749 2023-05-24 23:07:22.000000 hoppr-1.8.5/hoppr/core_plugins/report_generator/assets/hoppr_hippo.png
--rw-r--r--   0        0        0     4606 2023-05-24 23:07:22.000000 hoppr-1.8.5/hoppr/core_plugins/report_generator/report_generator.py
--rw-r--r--   0        0        0    60554 2023-05-24 23:07:22.000000 hoppr-1.8.5/hoppr/core_plugins/report_generator/scripts/bootstrap.min.js
--rw-r--r--   0        0        0      518 2023-05-24 23:07:22.000000 hoppr-1.8.5/hoppr/core_plugins/report_generator/scripts/custom.js
--rw-r--r--   0        0        0   220780 2023-05-24 23:07:22.000000 hoppr-1.8.5/hoppr/core_plugins/report_generator/styles/bootstrap.min.css
--rw-r--r--   0        0        0     3562 2023-05-24 23:07:22.000000 hoppr-1.8.5/hoppr/core_plugins/report_generator/styles/custom.css
--rw-r--r--   0        0        0     5052 2023-05-24 23:07:22.000000 hoppr-1.8.5/hoppr/core_plugins/report_generator/templates/component_card.jinja2
--rw-r--r--   0        0        0     1230 2023-05-24 23:07:22.000000 hoppr-1.8.5/hoppr/core_plugins/report_generator/templates/general_summary.jinja2
--rw-r--r--   0        0        0     7246 2023-05-24 23:07:22.000000 hoppr-1.8.5/hoppr/core_plugins/report_generator/templates/index.jinja2
--rw-r--r--   0        0        0      458 2023-05-24 23:07:22.000000 hoppr-1.8.5/hoppr/exceptions.py
--rw-r--r--   0        0        0     6847 2023-05-24 23:07:22.000000 hoppr-1.8.5/hoppr/in_toto.py
--rw-r--r--   0        0        0     3074 2023-05-24 23:07:22.000000 hoppr-1.8.5/hoppr/main.py
--rw-r--r--   0        0        0     4106 2023-05-24 23:07:22.000000 hoppr-1.8.5/hoppr/mem_logger.py
--rw-r--r--   0        0        0     1708 2023-05-24 23:07:22.000000 hoppr-1.8.5/hoppr/models/__init__.py
--rw-r--r--   0        0        0     1602 2023-05-24 23:07:22.000000 hoppr-1.8.5/hoppr/models/__main__.py
--rw-r--r--   0        0        0     1409 2023-05-24 23:07:22.000000 hoppr-1.8.5/hoppr/models/base.py
--rw-r--r--   0        0        0     4001 2023-05-24 23:07:22.000000 hoppr-1.8.5/hoppr/models/credentials.py
--rw-r--r--   0        0        0    17448 2023-05-24 23:07:22.000000 hoppr-1.8.5/hoppr/models/manifest.py
--rw-r--r--   0        0        0        0 2023-05-24 23:07:22.000000 hoppr-1.8.5/hoppr/models/py.typed
--rw-r--r--   0        0        0     3975 2023-05-24 23:07:22.000000 hoppr-1.8.5/hoppr/models/transfer.py
--rw-r--r--   0        0        0     5023 2023-05-24 23:07:22.000000 hoppr-1.8.5/hoppr/models/types.py
--rw-r--r--   0        0        0     2335 2023-05-24 23:07:22.000000 hoppr-1.8.5/hoppr/net.py
--rw-r--r--   0        0        0     4323 2023-05-24 23:07:22.000000 hoppr-1.8.5/hoppr/oci_artifacts.py
--rw-r--r--   0        0        0     1332 2023-05-24 23:07:22.000000 hoppr-1.8.5/hoppr/plugin_utils.py
--rw-r--r--   0        0        0    26282 2023-05-24 23:07:22.000000 hoppr-1.8.5/hoppr/processor.py
--rw-r--r--   0        0        0        0 2023-05-24 23:07:22.000000 hoppr-1.8.5/hoppr/py.typed
--rw-r--r--   0        0        0    22579 2023-05-24 23:07:22.000000 hoppr-1.8.5/hoppr/resources/hoppr-hippo-large.ansi
--rw-r--r--   0        0        0    10419 2023-05-24 23:07:22.000000 hoppr-1.8.5/hoppr/resources/hoppr-hippo.ansi
--rw-r--r--   0        0        0     4036 2023-05-24 23:07:22.000000 hoppr-1.8.5/hoppr/result.py
--rw-r--r--   0        0        0     5791 2023-05-24 23:07:22.000000 hoppr-1.8.5/hoppr/utils.py
--rw-r--r--   0        0        0     3614 2023-05-24 23:07:22.000000 hoppr-1.8.5/pyproject.toml
--rw-r--r--   0        0        0     2686 1970-01-01 00:00:00.000000 hoppr-1.8.5/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-06-14 22:06:45.000000 hoppr-1.8.6/LICENSE
+-rw-r--r--   0        0        0     1214 2023-06-14 22:06:45.000000 hoppr-1.8.6/README.md
+-rw-r--r--   0        0        0     1035 2023-06-14 22:06:45.000000 hoppr-1.8.6/hoppr/__init__.py
+-rw-r--r--   0        0        0      161 2023-06-14 22:06:45.000000 hoppr-1.8.6/hoppr/__main__.py
+-rw-r--r--   0        0        0        0 2023-06-14 22:06:45.000000 hoppr-1.8.6/hoppr/base_plugins/__init__.py
+-rw-r--r--   0        0        0    11010 2023-06-14 22:06:45.000000 hoppr-1.8.6/hoppr/base_plugins/collector.py
+-rw-r--r--   0        0        0    10697 2023-06-14 22:06:45.000000 hoppr-1.8.6/hoppr/base_plugins/hoppr.py
+-rw-r--r--   0        0        0        0 2023-06-14 22:06:45.000000 hoppr-1.8.6/hoppr/base_plugins/py.typed
+-rw-r--r--   0        0        0        0 2023-06-14 22:06:45.000000 hoppr-1.8.6/hoppr/cli/__init__.py
+-rw-r--r--   0        0        0     6256 2023-06-14 22:06:45.000000 hoppr-1.8.6/hoppr/cli/hopctl.py
+-rw-r--r--   0        0        0      563 2023-06-14 22:06:45.000000 hoppr-1.8.6/hoppr/constants.py
+-rw-r--r--   0        0        0        0 2023-06-14 22:06:45.000000 hoppr-1.8.6/hoppr/core_plugins/__init__.py
+-rw-r--r--   0        0        0     3046 2023-06-14 22:06:45.000000 hoppr-1.8.6/hoppr/core_plugins/bundle_tar.py
+-rw-r--r--   0        0        0    12943 2023-06-14 22:06:45.000000 hoppr-1.8.6/hoppr/core_plugins/collect_apt_plugin.py
+-rw-r--r--   0        0        0    10272 2023-06-14 22:06:45.000000 hoppr-1.8.6/hoppr/core_plugins/collect_dnf_plugin.py
+-rw-r--r--   0        0        0     4387 2023-06-14 22:06:45.000000 hoppr-1.8.6/hoppr/core_plugins/collect_docker_plugin.py
+-rw-r--r--   0        0        0     4664 2023-06-14 22:06:45.000000 hoppr-1.8.6/hoppr/core_plugins/collect_git_plugin.py
+-rw-r--r--   0        0        0     4113 2023-06-14 22:06:45.000000 hoppr-1.8.6/hoppr/core_plugins/collect_helm_plugin.py
+-rw-r--r--   0        0        0     6368 2023-06-14 22:06:45.000000 hoppr-1.8.6/hoppr/core_plugins/collect_maven_plugin.py
+-rw-r--r--   0        0        0     7961 2023-06-14 22:06:45.000000 hoppr-1.8.6/hoppr/core_plugins/collect_nexus_search.py
+-rw-r--r--   0        0        0     4418 2023-06-14 22:06:45.000000 hoppr-1.8.6/hoppr/core_plugins/collect_pypi_plugin.py
+-rw-r--r--   0        0        0     3043 2023-06-14 22:06:45.000000 hoppr-1.8.6/hoppr/core_plugins/collect_raw_plugin.py
+-rw-r--r--   0        0        0     3739 2023-06-14 22:06:45.000000 hoppr-1.8.6/hoppr/core_plugins/collect_yum_plugin.py
+-rw-r--r--   0        0        0     4278 2023-06-14 22:06:45.000000 hoppr-1.8.6/hoppr/core_plugins/composite_collector.py
+-rw-r--r--   0        0        0     5673 2023-06-14 22:06:45.000000 hoppr-1.8.6/hoppr/core_plugins/delta_sbom.py
+-rw-r--r--   0        0        0     6885 2023-06-14 22:06:45.000000 hoppr-1.8.6/hoppr/core_plugins/oras_bundle.py
+-rw-r--r--   0        0        0     5301 2023-06-14 22:06:45.000000 hoppr-1.8.6/hoppr/core_plugins/oras_registry.py
+-rw-r--r--   0        0        0        0 2023-06-14 22:06:45.000000 hoppr-1.8.6/hoppr/core_plugins/py.typed
+-rw-r--r--   0        0        0      202 2023-06-14 22:06:45.000000 hoppr-1.8.6/hoppr/core_plugins/report_generator/__init__.py
+-rw-r--r--   0        0        0   126749 2023-06-14 22:06:45.000000 hoppr-1.8.6/hoppr/core_plugins/report_generator/assets/hoppr_hippo.png
+-rw-r--r--   0        0        0     4606 2023-06-14 22:06:45.000000 hoppr-1.8.6/hoppr/core_plugins/report_generator/report_generator.py
+-rw-r--r--   0        0        0    60554 2023-06-14 22:06:45.000000 hoppr-1.8.6/hoppr/core_plugins/report_generator/scripts/bootstrap.min.js
+-rw-r--r--   0        0        0      518 2023-06-14 22:06:45.000000 hoppr-1.8.6/hoppr/core_plugins/report_generator/scripts/custom.js
+-rw-r--r--   0        0        0   220780 2023-06-14 22:06:45.000000 hoppr-1.8.6/hoppr/core_plugins/report_generator/styles/bootstrap.min.css
+-rw-r--r--   0        0        0     3562 2023-06-14 22:06:45.000000 hoppr-1.8.6/hoppr/core_plugins/report_generator/styles/custom.css
+-rw-r--r--   0        0        0     5052 2023-06-14 22:06:45.000000 hoppr-1.8.6/hoppr/core_plugins/report_generator/templates/component_card.jinja2
+-rw-r--r--   0        0        0     1230 2023-06-14 22:06:45.000000 hoppr-1.8.6/hoppr/core_plugins/report_generator/templates/general_summary.jinja2
+-rw-r--r--   0        0        0     7246 2023-06-14 22:06:45.000000 hoppr-1.8.6/hoppr/core_plugins/report_generator/templates/index.jinja2
+-rw-r--r--   0        0        0      458 2023-06-14 22:06:45.000000 hoppr-1.8.6/hoppr/exceptions.py
+-rw-r--r--   0        0        0     6847 2023-06-14 22:06:45.000000 hoppr-1.8.6/hoppr/in_toto.py
+-rw-r--r--   0        0        0     3357 2023-06-14 22:06:45.000000 hoppr-1.8.6/hoppr/main.py
+-rw-r--r--   0        0        0     4106 2023-06-14 22:06:45.000000 hoppr-1.8.6/hoppr/mem_logger.py
+-rw-r--r--   0        0        0     1708 2023-06-14 22:06:45.000000 hoppr-1.8.6/hoppr/models/__init__.py
+-rw-r--r--   0        0        0     1602 2023-06-14 22:06:45.000000 hoppr-1.8.6/hoppr/models/__main__.py
+-rw-r--r--   0        0        0     1409 2023-06-14 22:06:45.000000 hoppr-1.8.6/hoppr/models/base.py
+-rw-r--r--   0        0        0     4001 2023-06-14 22:06:45.000000 hoppr-1.8.6/hoppr/models/credentials.py
+-rw-r--r--   0        0        0    17448 2023-06-14 22:06:45.000000 hoppr-1.8.6/hoppr/models/manifest.py
+-rw-r--r--   0        0        0        0 2023-06-14 22:06:45.000000 hoppr-1.8.6/hoppr/models/py.typed
+-rw-r--r--   0        0        0     4018 2023-06-14 22:06:45.000000 hoppr-1.8.6/hoppr/models/transfer.py
+-rw-r--r--   0        0        0     5023 2023-06-14 22:06:45.000000 hoppr-1.8.6/hoppr/models/types.py
+-rw-r--r--   0        0        0     2335 2023-06-14 22:06:45.000000 hoppr-1.8.6/hoppr/net.py
+-rw-r--r--   0        0        0     4323 2023-06-14 22:06:45.000000 hoppr-1.8.6/hoppr/oci_artifacts.py
+-rw-r--r--   0        0        0     1332 2023-06-14 22:06:45.000000 hoppr-1.8.6/hoppr/plugin_utils.py
+-rw-r--r--   0        0        0    27309 2023-06-14 22:06:45.000000 hoppr-1.8.6/hoppr/processor.py
+-rw-r--r--   0        0        0        0 2023-06-14 22:06:45.000000 hoppr-1.8.6/hoppr/py.typed
+-rw-r--r--   0        0        0    22579 2023-06-14 22:06:45.000000 hoppr-1.8.6/hoppr/resources/hoppr-hippo-large.ansi
+-rw-r--r--   0        0        0    10419 2023-06-14 22:06:45.000000 hoppr-1.8.6/hoppr/resources/hoppr-hippo.ansi
+-rw-r--r--   0        0        0     4036 2023-06-14 22:06:45.000000 hoppr-1.8.6/hoppr/result.py
+-rw-r--r--   0        0        0     5791 2023-06-14 22:06:45.000000 hoppr-1.8.6/hoppr/utils.py
+-rw-r--r--   0        0        0     3614 2023-06-14 22:06:45.000000 hoppr-1.8.6/pyproject.toml
+-rw-r--r--   0        0        0     2686 1970-01-01 00:00:00.000000 hoppr-1.8.6/PKG-INFO
```

### Comparing `hoppr-1.8.5/LICENSE` & `hoppr-1.8.6/LICENSE`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.5/README.md` & `hoppr-1.8.6/README.md`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.5/hoppr/__init__.py` & `hoppr-1.8.6/hoppr/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,8 +29,8 @@
     "Property",
     "PurlType",
     "Result",
     "Sbom",
     "Transfer",
 ]
 
-__version__ = "1.8.5"
+__version__ = "1.8.6"
```

### Comparing `hoppr-1.8.5/hoppr/base_plugins/collector.py` & `hoppr-1.8.6/hoppr/base_plugins/collector.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.5/hoppr/base_plugins/hoppr.py` & `hoppr-1.8.6/hoppr/base_plugins/hoppr.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,25 +14,21 @@
 
 from hoppr import plugin_utils
 from hoppr.mem_logger import MemoryLogger
 from hoppr.models import HopprContext
 from hoppr.models.transfer import ComponentCoverage
 from hoppr.models.types import BomAccess
 from hoppr.result import Result
-from hoppr.utils import obscure_passwords, get_package_url
+from hoppr.utils import get_package_url, obscure_passwords
 
 
 def _get_component(*args, **kwargs) -> Optional[Any]:
     # TODO: This will only utilize the first Component found in 1) args, 2) kwargs  # pylint: disable=fixme
     # and assumes all plugins operate this way
-    comp = None
-    for arg in args:
-        if type(arg).__name__ == "Component":
-            comp = arg
-            break
+    comp = next((arg for arg in args if type(arg).__name__ == "Component"), None)
 
     if comp is None:
         for value in kwargs.values():
             if type(value).__name__ == "Component":
                 comp = value
                 break
 
@@ -71,15 +67,14 @@
                 component_header = f"{comp.name}" + (f"@{comp.version}" if comp.version is not None else "")
 
                 self.get_logger().info(
                     msg=f"{'-' * 4} Component: {component_header} {'-' * 50}",
                 )
 
         if result is None:
-
             # Only check for missing commands if func has been overridden
             if func.__module__ != HopprPlugin.__module__:
                 command_result = plugin_utils.check_for_missing_commands(self.required_commands)
                 if command_result.is_fail():
                     self.get_logger().error(command_result.message)
                     return command_result
 
@@ -112,15 +107,14 @@
     """
     Runs a method (assumed to return a Result object) a number of times,
     or until the result type is not RETRY
     """
 
     @functools.wraps(method)
     def wrapper(self, *args, **kwargs) -> Result:
-
         log = self.get_logger()
 
         result = Result.fail(message="Context max_attempts must be a positive integer.")
 
         for attempt in range(self.context.max_attempts):
             log.info(msg=f"Processing component [attempt {attempt + 1} of {self.context.max_attempts}]", indent_level=1)
 
@@ -156,17 +150,19 @@
 def hoppr_ignore_excluded(func: Callable) -> Callable:
     """
     Decorator to ignore components which have a scope of `excluded`
     """
 
     @functools.wraps(func)
     def wrapper(self, *args, **kwargs) -> Result:
-
         comp = _get_component(*args, **kwargs)
-        if comp is not None and str(comp.scope) in ('excluded', 'Scope.excluded'):
+        if comp is not None and str(comp.scope) in {
+            'excluded',
+            'Scope.excluded',
+        }:
             return Result.excluded()
         return func(self, *args, **kwargs)
 
     return wrapper
 
 
 class HopprPlugin(ABC):
```

### Comparing `hoppr-1.8.5/hoppr/cli/hopctl.py` & `hoppr-1.8.6/hoppr/cli/hopctl.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.5/hoppr/constants.py` & `hoppr-1.8.6/hoppr/constants.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.5/hoppr/core_plugins/bundle_tar.py` & `hoppr-1.8.6/hoppr/core_plugins/bundle_tar.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.5/hoppr/core_plugins/collect_apt_plugin.py` & `hoppr-1.8.6/hoppr/core_plugins/collect_apt_plugin.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.5/hoppr/core_plugins/collect_dnf_plugin.py` & `hoppr-1.8.6/hoppr/core_plugins/collect_dnf_plugin.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.5/hoppr/core_plugins/collect_docker_plugin.py` & `hoppr-1.8.6/hoppr/core_plugins/collect_docker_plugin.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 from __future__ import annotations
 
 import re
 import urllib.parse
 
 from typing import Any
+from packageurl import PackageURL
 
 import hoppr.utils
 
 from hoppr import __version__
 from hoppr.base_plugins.collector import SerialCollectorPlugin
 from hoppr.base_plugins.hoppr import hoppr_rerunner
 from hoppr.models import HopprContext
@@ -36,14 +37,31 @@
     def get_version(self) -> str:  # pylint: disable=duplicate-code
         return __version__
 
     def __init__(self, context: HopprContext, config: dict | None = None) -> None:
         super().__init__(context=context, config=config)
         self.required_commands = (self.config or {}).get("skopeo_command", self.required_commands)
 
+    def get_image(self, url: str, purl: PackageURL, image_name: str) -> RepositoryUrl:
+        """
+        Return the image details for skopeo to process
+
+        Args:
+            url (str): Repository URL
+            purl (PackageURL): Purl of component to operate on
+            image_name (str): Name of image with tag
+
+        Returns:
+            RepositoryUrl: Image information
+        """
+        source_image = RepositoryUrl(url=url) / (purl.namespace or "") / urllib.parse.quote_plus(image_name)
+        if source_image.scheme != "docker":
+            source_image = RepositoryUrl(url="docker://" + re.sub(r"^(.*://)", "", str(source_image)))
+        return source_image
+
     @hoppr_rerunner
     def collect(self, comp: Any, repo_url: str, creds: CredentialRequiredService | None = None):
         """
         Copy a component to the local collection directory structure
         """
         purl = hoppr.utils.get_package_url(comp.purl)
         version_path = purl.version
@@ -54,23 +72,20 @@
 
         elif purl.version.startswith("sha256:"):
             image_name = f"{purl.name}@{purl.version}"
         else:
             image_name = f"{purl.name}@sha256:{purl.version}"
             version_path = f"sha256:{purl.version}"
 
-        source_image = RepositoryUrl(url=repo_url) / (purl.namespace or "") / urllib.parse.quote_plus(image_name)
-
         version_path = urllib.parse.quote_plus(re.sub(r'^https?://', '', version_path))
         target_dir = self.directory_for(purl.type, repo_url, subdir=purl.namespace)
         target_path = target_dir / f"{urllib.parse.unquote(purl.name)}_{purl.version}"
-        destination = f"docker-archive:{target_dir / purl.name}_{version_path}"
+        destination = f"docker-archive:{target_dir / purl.name}@{version_path}"
 
-        if source_image.scheme != "docker":
-            source_image = RepositoryUrl(url=re.sub(r"^.+(?=://)", "docker", str(source_image)))
+        source_image = self.get_image(url=repo_url, purl=purl, image_name=image_name)
 
         self.get_logger().info(msg="Copying docker image:", indent_level=2)
         self.get_logger().info(msg=f"source: {source_image}", indent_level=3)
         self.get_logger().info(msg=f"destination: {destination}", indent_level=3)
 
         command = [self.required_commands[0], "copy"]
```

### Comparing `hoppr-1.8.5/hoppr/core_plugins/collect_git_plugin.py` & `hoppr-1.8.6/hoppr/core_plugins/collect_git_plugin.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.5/hoppr/core_plugins/collect_helm_plugin.py` & `hoppr-1.8.6/hoppr/core_plugins/collect_helm_plugin.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.5/hoppr/core_plugins/collect_maven_plugin.py` & `hoppr-1.8.6/hoppr/core_plugins/collect_maven_plugin.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,14 @@
             self.required_commands = self.config.get("maven_command", self.required_commands)
             self.extra_opts = self.config.get("maven_opts", self.extra_opts)
 
         system_settings_file = Path("/") / "etc" / "maven" / "settings.xml"
         user_settings_file = Path.home() / ".m2" / "settings.xml"
 
         if not self.context.strict_repos:
-
             # Identify system repositories
             for settings_file in [system_settings_file, user_settings_file]:
                 if settings_file.is_file():
                     settings_dict: OrderedDict[str, Any] = xmltodict.parse(
                         settings_file.read_text(encoding="utf-8"),
                         encoding="utf-8",
                         force_list={"profile", "repository"},
```

### Comparing `hoppr-1.8.5/hoppr/core_plugins/collect_nexus_search.py` & `hoppr-1.8.6/hoppr/core_plugins/collect_nexus_search.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.5/hoppr/core_plugins/collect_pypi_plugin.py` & `hoppr-1.8.6/hoppr/core_plugins/collect_pypi_plugin.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.5/hoppr/core_plugins/collect_raw_plugin.py` & `hoppr-1.8.6/hoppr/core_plugins/collect_raw_plugin.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.5/hoppr/core_plugins/collect_yum_plugin.py` & `hoppr-1.8.6/hoppr/core_plugins/collect_yum_plugin.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.5/hoppr/core_plugins/composite_collector.py` & `hoppr-1.8.6/hoppr/core_plugins/composite_collector.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.5/hoppr/core_plugins/delta_sbom.py` & `hoppr-1.8.6/hoppr/core_plugins/delta_sbom.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.5/hoppr/core_plugins/oras_bundle.py` & `hoppr-1.8.6/hoppr/core_plugins/oras_bundle.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.5/hoppr/core_plugins/oras_registry.py` & `hoppr-1.8.6/hoppr/core_plugins/oras_registry.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.5/hoppr/core_plugins/report_generator/assets/hoppr_hippo.png` & `hoppr-1.8.6/hoppr/core_plugins/report_generator/assets/hoppr_hippo.png`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.5/hoppr/core_plugins/report_generator/report_generator.py` & `hoppr-1.8.6/hoppr/core_plugins/report_generator/report_generator.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.5/hoppr/core_plugins/report_generator/scripts/bootstrap.min.js` & `hoppr-1.8.6/hoppr/core_plugins/report_generator/scripts/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.5/hoppr/core_plugins/report_generator/scripts/custom.js` & `hoppr-1.8.6/hoppr/core_plugins/report_generator/scripts/custom.js`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.5/hoppr/core_plugins/report_generator/styles/bootstrap.min.css` & `hoppr-1.8.6/hoppr/core_plugins/report_generator/styles/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.5/hoppr/core_plugins/report_generator/styles/custom.css` & `hoppr-1.8.6/hoppr/core_plugins/report_generator/styles/custom.css`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.5/hoppr/core_plugins/report_generator/templates/component_card.jinja2` & `hoppr-1.8.6/hoppr/core_plugins/report_generator/templates/component_card.jinja2`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.5/hoppr/core_plugins/report_generator/templates/general_summary.jinja2` & `hoppr-1.8.6/hoppr/core_plugins/report_generator/templates/general_summary.jinja2`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.5/hoppr/core_plugins/report_generator/templates/index.jinja2` & `hoppr-1.8.6/hoppr/core_plugins/report_generator/templates/index.jinja2`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.5/hoppr/in_toto.py` & `hoppr-1.8.6/hoppr/in_toto.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.5/hoppr/main.py` & `hoppr-1.8.6/hoppr/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 Framework for manipulating bundles for airgapped transfers.
 """
 import logging
 import sys
 
 from pathlib import Path
+from posixpath import sep
 from typing import List, Optional
 
 from typer import Exit, echo, prompt
 
 from hoppr import __version__
 from hoppr.in_toto import generate_in_toto_layout
 from hoppr.models.credentials import Credentials
@@ -30,17 +31,22 @@
     functionary_key_password: Optional[str] = None,
     previous_delivery: Optional[Path] = None,
 ):
     """
     Run the stages specified in the transfer config
     file on the content specified in the manifest
     """
+    echo(
+        f"Loading {str(manifest_file).rsplit(str(sep), maxsplit=1)[-1]} and"
+        f"{str(transfer_file).rsplit(str(sep), maxsplit=1)[-1]} files..."
+    )
     metadata_files = [manifest_file, transfer_file]
 
     if credentials_file is not None:
+        echo(f"Loading {str(credentials_file).rsplit(str(sep), maxsplit=1)[-1]} file...")
         metadata_files.append(credentials_file)
 
     log_level = logging.DEBUG if verbose else logging.INFO
 
     if create_attestations and functionary_key_path is None:
         echo("To create attestations both the `--attest` option and a functionary private key need to be provided.")
         raise Exit(code=1)
```

### Comparing `hoppr-1.8.5/hoppr/mem_logger.py` & `hoppr-1.8.6/hoppr/mem_logger.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.5/hoppr/models/__init__.py` & `hoppr-1.8.6/hoppr/models/__init__.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.5/hoppr/models/__main__.py` & `hoppr-1.8.6/hoppr/models/__main__.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.5/hoppr/models/base.py` & `hoppr-1.8.6/hoppr/models/base.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.5/hoppr/models/credentials.py` & `hoppr-1.8.6/hoppr/models/credentials.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.5/hoppr/models/manifest.py` & `hoppr-1.8.6/hoppr/models/manifest.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.5/hoppr/models/transfer.py` & `hoppr-1.8.6/hoppr/models/transfer.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,15 +21,16 @@
 
 
 class StageName(ConstrainedStr):
     """
     Constrained string type for stage key name
     """
 
-    regex: Pattern[str] = re.compile(pattern=r"^[A-Za-z_][\w\s]*$")
+    # Match any string without whitespace for stagenames
+    regex: Pattern[str] = re.compile(pattern=r"^\S+")
     min_length: int = 1
 
 
 class Plugin(HopprBaseModel):
     """
     Plugin data model
     """
```

### Comparing `hoppr-1.8.5/hoppr/models/types.py` & `hoppr-1.8.6/hoppr/models/types.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.5/hoppr/net.py` & `hoppr-1.8.6/hoppr/net.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.5/hoppr/oci_artifacts.py` & `hoppr-1.8.6/hoppr/oci_artifacts.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.5/hoppr/plugin_utils.py` & `hoppr-1.8.6/hoppr/plugin_utils.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.5/hoppr/processor.py` & `hoppr-1.8.6/hoppr/processor.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import shutil
 import socket
 import sys
 import tempfile
 import time
 import uuid
 
-from concurrent.futures import Future, ProcessPoolExecutor
+from concurrent.futures import Future, ThreadPoolExecutor, as_completed
 from copy import deepcopy
 from datetime import datetime
 from multiprocessing import cpu_count
 from os import PathLike
 from pathlib import Path
 from threading import _RLock as RLock
 from typing import Any, MutableMapping
@@ -115,91 +115,117 @@
         # Each sub-stage must complete before the next can begin
         result.merge(self._run_all(HopprPlugin.pre_stage_process.__name__))
         result.merge(self._run_all(HopprPlugin.process_component.__name__))
         result.merge(self._run_all(HopprPlugin.post_stage_process.__name__))
 
         return result
 
-    def _run_all(self, method_name: str):
+    def _populate_futures(self, method_name: str) -> tuple[int, int]:
         """
         Run the named method for all plugins.  If appropriate to the method, run it for
         all components for all plug-ins.
         """
-
-        # Map to allow access to the arguments that went into a future call
         future_argument_map: dict[Future[Result], tuple[Plugin, Component | None]] = {}
 
-        with ProcessPoolExecutor(max_workers=self.context.max_processes) as executor:
+        with ThreadPoolExecutor(max_workers=self.context.max_processes) as executor:
+            failures = 0
+            retries = 0
             for plugin in self.plugin_ref_list:
-
                 plugin_cls = plugin_class(plugin.name)
 
                 if getattr(plugin_cls, method_name) == getattr(HopprPlugin, method_name):
                     continue
 
                 if method_name in self.component_based_methods:
                     # Create one concurrent future object to run this method for each component
                     for component in self.context.delivered_sbom.components or []:
-                        future_proc = executor.submit(
-                            _run_plugin,
-                            plugin_name=plugin.name,
-                            context=self.context,
-                            config=plugin.config,
-                            method_name=method_name,
-                            component=component,
-                        )
-                        future_argument_map[future_proc] = (plugin, component)
+                        if component.purl:
+                            instance = plugin_instance(plugin.name, self.context, plugin.config)
+                            if instance.supports_purl_type(PackageURL.from_string(component.purl).type):
+                                future_proc = executor.submit(
+                                    _run_plugin,
+                                    plugin_name=plugin.name,
+                                    context=self.context,
+                                    config=plugin.config,
+                                    method_name=method_name,
+                                    component=component,
+                                )
+                                future_argument_map[future_proc] = (plugin, component)
                 else:
                     # Create a concurrent future object to run this method
                     future_proc = executor.submit(
                         _run_plugin,
                         plugin_name=plugin.name,
                         context=self.context,
                         config=plugin.config,
                         method_name=method_name,
                         component=None,
                     )
                     future_argument_map[future_proc] = (plugin, None)
 
-            # Save all the results, count failures and retries
-            # Note: future.results() blocks until the process is complete
-            need_method_label = True
-            failures = 0
-            retries = 0
+            fail, retry = self.process_status(
+                future_argument_map=future_argument_map, method_name=method_name, failures=failures, retries=retries
+            )
+
+            failures += fail
+            retries += retry
+
+        return failures, retries
+
+    def process_status(
+        self,
+        future_argument_map: dict[Future[Result], tuple[Plugin, Component | None]],
+        method_name: str,
+        failures: int,
+        retries: int,
+    ) -> tuple[int, int]:
+        """
+        Print processing results.
+        """
+        need_method_label = True
+        for future in as_completed(future_argument_map):
+            # retrieve the result
+            (plugin, comp) = future_argument_map[future]
+            future_result: Result = future.result()
+            if not future_result.is_skip():
+                if need_method_label:
+                    echo(f"   Beginning method {method_name}")
+                    need_method_label = False
 
-            for future_proc, (plugin, comp) in future_argument_map.items():
-                future_result: Result = future_proc.result()
-                if not future_result.is_skip():
-                    if need_method_label:
-                        echo(f"   Beginning method {method_name}")
-                        need_method_label = False
-
-                    plugin_cls = plugin_class(plugin.name)
-
-                    if not future_result.is_excluded():
-                        self._save_result(method_name, plugin_cls.__name__, future_result, comp)
-                        self._update_bom(future_result.return_obj, comp)
-                    self._report_result(plugin_cls.__name__, comp, future_result)
-
-                    ReportGenerator.report_gen_list.append(
-                        Report(
-                            uuid.uuid4(),
-                            plugin_cls.__name__,
-                            self.stage_id,
-                            future_result.status,
-                            future_result.message,
-                            method_name,
-                            comp,
-                        )
+                plugin_cls = plugin_class(plugin.name)
+
+                if not future_result.is_excluded():
+                    self._save_result(method_name, plugin_cls.__name__, future_result, comp)
+                    self._update_bom(future_result.return_obj, comp)
+                self._report_result(plugin_cls.__name__, comp, future_result)
+
+                ReportGenerator.report_gen_list.append(
+                    Report(
+                        uuid.uuid4(),
+                        plugin_cls.__name__,
+                        self.stage_id,
+                        future_result.status,
+                        future_result.message,
+                        method_name,
+                        comp,
                     )
+                )
+
+                if future_result.is_fail():
+                    failures += 1
+                if future_result.is_retry():
+                    retries += 1
+        return failures, retries
+
+    def _run_all(self, method_name: str):
+        """
+        Run the named method for all plugins and process results
+        """
 
-                    if future_result.is_fail():
-                        failures += 1
-                    if future_result.is_retry():
-                        retries += 1
+        failures, retries = self._populate_futures(method_name)
 
         if method_name in self.component_based_methods:
             failures += self._check_component_coverage(method_name)
 
         return self._get_stage_result(method_name, failures, retries)
 
     def _get_stage_result(self, method_name: str, failures: int, retries: int) -> Result:
@@ -229,15 +255,15 @@
                     "component coverage values. The value may be overridden in transfer file."
                 )
 
         return coverage
 
     def _check_component_coverage(self, method_name: str) -> int:
         result_count: dict[str | None, int] = {}
-        for (_, purl, _) in self.results.get(method_name, []):
+        for _, purl, _ in self.results.get(method_name, []):
             result_count[purl] = result_count.get(purl, 0) + 1
 
         additional_failures = 0
         for component in self.context.delivered_sbom.components or []:
             count = result_count.get(component.purl, 0)
             if not self.required_coverage.accepts_count(count) and str(component.scope) not in {
                 'excluded',
@@ -406,28 +432,30 @@
         self.get_logger().info(f"Collecting metadata file {file_name}")
         abs_path = Path(file_name).absolute()
 
         target = Path(target_dir, quote_plus(f"{abs_path}"))
         shutil.copyfile(file_name, f"{target}")
 
     def _collect_manifest_metadata(self, manifest: ManifestFile, target_dir: str | PathLike[str]) -> None:
+        echo(f"Loading {len(manifest.includes)} includes from manifest...")
         for include_ref in manifest.includes:
             include = Manifest.loaded_manifests[include_ref]
             include_dict = include_ref.dict()
 
             if "local" in include_dict:
                 url = str(include_dict["local"])
             else:
                 url = str(include_dict["url"])
 
             target_file = Path(target_dir) / quote_plus(url)
 
             with target_file.open(mode="w+", encoding="utf-8") as output_file:
                 output_file.write(include.yaml(by_alias=True, exclude_unset=True, indent=True))
 
+        echo(f"Loading {len(manifest.sboms)} sboms from manifest...")
         for sbom_ref in manifest.sboms:
             sbom = Sbom.loaded_sboms[sbom_ref]
             sbom_dict = sbom_ref.dict()
 
             if "local" in sbom_dict:
                 url = str(sbom_dict["local"])
             elif "oci" in sbom_dict:
```

### Comparing `hoppr-1.8.5/hoppr/resources/hoppr-hippo-large.ansi` & `hoppr-1.8.6/hoppr/resources/hoppr-hippo-large.ansi`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.5/hoppr/resources/hoppr-hippo.ansi` & `hoppr-1.8.6/hoppr/resources/hoppr-hippo.ansi`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.5/hoppr/result.py` & `hoppr-1.8.6/hoppr/result.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.5/hoppr/utils.py` & `hoppr-1.8.6/hoppr/utils.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.5/pyproject.toml` & `hoppr-1.8.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hoppr"
-version = "1.8.5"
+version = "1.8.6"
 description = "A tool for defining, verifying, and transferring software dependencies between environments."
 authors = ["LMCO Open Source <open.source@lmco.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://hoppr.dev"
 repository = "https://gitlab.com/hoppr/hoppr"
```

### Comparing `hoppr-1.8.5/PKG-INFO` & `hoppr-1.8.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hoppr
-Version: 1.8.5
+Version: 1.8.6
 Summary: A tool for defining, verifying, and transferring software dependencies between environments.
 Home-page: https://hoppr.dev
 License: MIT
 Keywords: packaging,reports,build dependencies,software bill of materials
 Author: LMCO Open Source
 Author-email: open.source@lmco.com
 Requires-Python: >=3.10,<4.0
```

