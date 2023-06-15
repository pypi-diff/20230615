# Comparing `tmp/pulumi_frontegg-0.2.25.tar.gz` & `tmp/pulumi_frontegg-0.2.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_frontegg-0.2.25.tar", last modified: Tue Dec  6 14:57:44 2022, max compression
+gzip compressed data, was "pulumi_frontegg-0.2.26.tar", last modified: Thu Jun 15 06:06:30 2023, max compression
```

## Comparing `pulumi_frontegg-0.2.25.tar` & `pulumi_frontegg-0.2.26.tar`

### file list

```diff
@@ -1,31 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 14:57:44.912010 pulumi_frontegg-0.2.25/
--rw-r--r--   0 runner    (1001) docker     (123)      805 2022-12-06 14:57:44.912010 pulumi_frontegg-0.2.25/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      438 2022-12-06 14:57:44.000000 pulumi_frontegg-0.2.25/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 14:57:44.912010 pulumi_frontegg-0.2.25/pulumi_frontegg/
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2022-12-06 14:57:44.000000 pulumi_frontegg-0.2.25/pulumi_frontegg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    63976 2022-12-06 14:57:44.000000 pulumi_frontegg-0.2.25/pulumi_frontegg/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8155 2022-12-06 14:57:44.000000 pulumi_frontegg-0.2.25/pulumi_frontegg/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 14:57:44.912010 pulumi_frontegg-0.2.25/pulumi_frontegg/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2022-12-06 14:57:44.000000 pulumi_frontegg-0.2.25/pulumi_frontegg/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2022-12-06 14:57:44.000000 pulumi_frontegg-0.2.25/pulumi_frontegg/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)     3969 2022-12-06 14:57:44.000000 pulumi_frontegg-0.2.25/pulumi_frontegg/get_permission.py
--rw-r--r--   0 runner    (1001) docker     (123)    63338 2022-12-06 14:57:44.000000 pulumi_frontegg-0.2.25/pulumi_frontegg/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    12391 2022-12-06 14:57:44.000000 pulumi_frontegg-0.2.25/pulumi_frontegg/permission.py
--rw-r--r--   0 runner    (1001) docker     (123)     8849 2022-12-06 14:57:44.000000 pulumi_frontegg-0.2.25/pulumi_frontegg/permission_category.py
--rw-r--r--   0 runner    (1001) docker     (123)     8292 2022-12-06 14:57:44.000000 pulumi_frontegg-0.2.25/pulumi_frontegg/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)      137 2022-12-06 14:57:44.000000 pulumi_frontegg-0.2.25/pulumi_frontegg/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-06 14:57:44.000000 pulumi_frontegg-0.2.25/pulumi_frontegg/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    19189 2022-12-06 14:57:44.000000 pulumi_frontegg-0.2.25/pulumi_frontegg/role.py
--rw-r--r--   0 runner    (1001) docker     (123)     9050 2022-12-06 14:57:44.000000 pulumi_frontegg-0.2.25/pulumi_frontegg/tenant.py
--rw-r--r--   0 runner    (1001) docker     (123)    15834 2022-12-06 14:57:44.000000 pulumi_frontegg-0.2.25/pulumi_frontegg/user.py
--rw-r--r--   0 runner    (1001) docker     (123)    18563 2022-12-06 14:57:44.000000 pulumi_frontegg-0.2.25/pulumi_frontegg/webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)    84582 2022-12-06 14:57:44.000000 pulumi_frontegg-0.2.25/pulumi_frontegg/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 14:57:44.912010 pulumi_frontegg-0.2.25/pulumi_frontegg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      805 2022-12-06 14:57:44.000000 pulumi_frontegg-0.2.25/pulumi_frontegg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      749 2022-12-06 14:57:44.000000 pulumi_frontegg-0.2.25/pulumi_frontegg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-06 14:57:44.000000 pulumi_frontegg-0.2.25/pulumi_frontegg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-06 14:57:44.000000 pulumi_frontegg-0.2.25/pulumi_frontegg.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2022-12-06 14:57:44.000000 pulumi_frontegg-0.2.25/pulumi_frontegg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2022-12-06 14:57:44.000000 pulumi_frontegg-0.2.25/pulumi_frontegg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-06 14:57:44.912010 pulumi_frontegg-0.2.25/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2022-12-06 14:57:44.000000 pulumi_frontegg-0.2.25/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:06:30.901745 pulumi_frontegg-0.2.26/
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-15 06:06:30.901745 pulumi_frontegg-0.2.26/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-15 06:06:30.000000 pulumi_frontegg-0.2.26/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:06:30.897745 pulumi_frontegg-0.2.26/pulumi_frontegg/
+-rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-06-15 06:06:30.000000 pulumi_frontegg-0.2.26/pulumi_frontegg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67966 2023-06-15 06:06:30.000000 pulumi_frontegg-0.2.26/pulumi_frontegg/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8155 2023-06-15 06:06:30.000000 pulumi_frontegg-0.2.26/pulumi_frontegg/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5785 2023-06-15 06:06:30.000000 pulumi_frontegg-0.2.26/pulumi_frontegg/allowed_origin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:06:30.897745 pulumi_frontegg-0.2.26/pulumi_frontegg/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-15 06:06:30.000000 pulumi_frontegg-0.2.26/pulumi_frontegg/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-06-15 06:06:30.000000 pulumi_frontegg-0.2.26/pulumi_frontegg/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-06-15 06:06:30.000000 pulumi_frontegg-0.2.26/pulumi_frontegg/get_permission.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66319 2023-06-15 06:06:30.000000 pulumi_frontegg-0.2.26/pulumi_frontegg/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12391 2023-06-15 06:06:30.000000 pulumi_frontegg-0.2.26/pulumi_frontegg/permission.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8849 2023-06-15 06:06:30.000000 pulumi_frontegg-0.2.26/pulumi_frontegg/permission_category.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8495 2023-06-15 06:06:30.000000 pulumi_frontegg-0.2.26/pulumi_frontegg/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-15 06:06:30.000000 pulumi_frontegg-0.2.26/pulumi_frontegg/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 06:06:30.000000 pulumi_frontegg-0.2.26/pulumi_frontegg/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     6474 2023-06-15 06:06:30.000000 pulumi_frontegg-0.2.26/pulumi_frontegg/redirect_uri.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19189 2023-06-15 06:06:30.000000 pulumi_frontegg-0.2.26/pulumi_frontegg/role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9050 2023-06-15 06:06:30.000000 pulumi_frontegg-0.2.26/pulumi_frontegg/tenant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16034 2023-06-15 06:06:30.000000 pulumi_frontegg-0.2.26/pulumi_frontegg/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19522 2023-06-15 06:06:30.000000 pulumi_frontegg-0.2.26/pulumi_frontegg/webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    84582 2023-06-15 06:06:30.000000 pulumi_frontegg-0.2.26/pulumi_frontegg/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:06:30.897745 pulumi_frontegg-0.2.26/pulumi_frontegg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-15 06:06:30.000000 pulumi_frontegg-0.2.26/pulumi_frontegg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-06-15 06:06:30.000000 pulumi_frontegg-0.2.26/pulumi_frontegg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 06:06:30.000000 pulumi_frontegg-0.2.26/pulumi_frontegg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 06:06:30.000000 pulumi_frontegg-0.2.26/pulumi_frontegg.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-15 06:06:30.000000 pulumi_frontegg-0.2.26/pulumi_frontegg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-15 06:06:30.000000 pulumi_frontegg-0.2.26/pulumi_frontegg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 06:06:30.901745 pulumi_frontegg-0.2.26/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-06-15 06:06:30.000000 pulumi_frontegg-0.2.26/setup.py
```

### Comparing `pulumi_frontegg-0.2.25/PKG-INFO` & `pulumi_frontegg-0.2.26/pulumi_frontegg.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
-Name: pulumi_frontegg
-Version: 0.2.25
+Name: pulumi-frontegg
+Version: 0.2.26
 Summary: A Pulumi package for creating and managing Frontegg resources.
 Home-page: https://github.com/MaterializeInc/pulumi-frontegg
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-frontegg
 Keywords: pulumi frontegg
 Platform: UNKNOWN
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # Frontegg Pulumi Provider
 
 A [Pulumi](https://pulumi.com) provider for the [Frontegg] user management
 platform.
```

### Comparing `pulumi_frontegg-0.2.25/pulumi_frontegg/__init__.py` & `pulumi_frontegg-0.2.26/pulumi_frontegg/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
 from . import _utilities
 import typing
 # Export this package's modules as members:
+from .allowed_origin import *
 from .get_permission import *
 from .permission import *
 from .permission_category import *
 from .provider import *
+from .redirect_uri import *
 from .role import *
 from .tenant import *
 from .user import *
 from .webhook import *
 from .workspace import *
 from ._inputs import *
 from . import outputs
@@ -25,14 +27,22 @@
     config = _utilities.lazy_import('pulumi_frontegg.config')
 
 _utilities.register(
     resource_modules="""
 [
  {
   "pkg": "frontegg",
+  "mod": "index/allowedOrigin",
+  "fqn": "pulumi_frontegg",
+  "classes": {
+   "frontegg:index/allowedOrigin:AllowedOrigin": "AllowedOrigin"
+  }
+ },
+ {
+  "pkg": "frontegg",
   "mod": "index/permission",
   "fqn": "pulumi_frontegg",
   "classes": {
    "frontegg:index/permission:Permission": "Permission"
   }
  },
  {
@@ -41,14 +51,22 @@
   "fqn": "pulumi_frontegg",
   "classes": {
    "frontegg:index/permissionCategory:PermissionCategory": "PermissionCategory"
   }
  },
  {
   "pkg": "frontegg",
+  "mod": "index/redirectUri",
+  "fqn": "pulumi_frontegg",
+  "classes": {
+   "frontegg:index/redirectUri:RedirectUri": "RedirectUri"
+  }
+ },
+ {
+  "pkg": "frontegg",
   "mod": "index/role",
   "fqn": "pulumi_frontegg",
   "classes": {
    "frontegg:index/role:Role": "Role"
   }
  },
  {
```

### Comparing `pulumi_frontegg-0.2.25/pulumi_frontegg/_inputs.py` & `pulumi_frontegg-0.2.26/pulumi_frontegg/_inputs.py`

 * *Files 6% similar despite different names*

```diff
@@ -54,29 +54,30 @@
                  enable_roles: pulumi.Input[bool],
                  enable_security: pulumi.Input[bool],
                  enable_sso: pulumi.Input[bool],
                  enable_subscriptions: pulumi.Input[bool],
                  enable_usage: pulumi.Input[bool],
                  enable_users: pulumi.Input[bool],
                  enable_webhooks: pulumi.Input[bool],
-                 palette: pulumi.Input['WorkspaceAdminPortalPaletteArgs']):
+                 palette: Optional[pulumi.Input['WorkspaceAdminPortalPaletteArgs']] = None):
         pulumi.set(__self__, "enable_account_settings", enable_account_settings)
         pulumi.set(__self__, "enable_api_tokens", enable_api_tokens)
         pulumi.set(__self__, "enable_audit_logs", enable_audit_logs)
         pulumi.set(__self__, "enable_personal_api_tokens", enable_personal_api_tokens)
         pulumi.set(__self__, "enable_privacy", enable_privacy)
         pulumi.set(__self__, "enable_profile", enable_profile)
         pulumi.set(__self__, "enable_roles", enable_roles)
         pulumi.set(__self__, "enable_security", enable_security)
         pulumi.set(__self__, "enable_sso", enable_sso)
         pulumi.set(__self__, "enable_subscriptions", enable_subscriptions)
         pulumi.set(__self__, "enable_usage", enable_usage)
         pulumi.set(__self__, "enable_users", enable_users)
         pulumi.set(__self__, "enable_webhooks", enable_webhooks)
-        pulumi.set(__self__, "palette", palette)
+        if palette is not None:
+            pulumi.set(__self__, "palette", palette)
 
     @property
     @pulumi.getter(name="enableAccountSettings")
     def enable_account_settings(self) -> pulumi.Input[bool]:
         return pulumi.get(self, "enable_account_settings")
 
     @enable_account_settings.setter
@@ -189,90 +190,96 @@
 
     @enable_webhooks.setter
     def enable_webhooks(self, value: pulumi.Input[bool]):
         pulumi.set(self, "enable_webhooks", value)
 
     @property
     @pulumi.getter
-    def palette(self) -> pulumi.Input['WorkspaceAdminPortalPaletteArgs']:
+    def palette(self) -> Optional[pulumi.Input['WorkspaceAdminPortalPaletteArgs']]:
         return pulumi.get(self, "palette")
 
     @palette.setter
-    def palette(self, value: pulumi.Input['WorkspaceAdminPortalPaletteArgs']):
+    def palette(self, value: Optional[pulumi.Input['WorkspaceAdminPortalPaletteArgs']]):
         pulumi.set(self, "palette", value)
 
 
 @pulumi.input_type
 class WorkspaceAdminPortalPaletteArgs:
     def __init__(__self__, *,
-                 errors: pulumi.Input[Sequence[pulumi.Input['WorkspaceAdminPortalPaletteErrorArgs']]],
-                 infos: pulumi.Input[Sequence[pulumi.Input['WorkspaceAdminPortalPaletteInfoArgs']]],
-                 primaries: pulumi.Input[Sequence[pulumi.Input['WorkspaceAdminPortalPalettePrimaryArgs']]],
-                 secondaries: pulumi.Input[Sequence[pulumi.Input['WorkspaceAdminPortalPaletteSecondaryArgs']]],
-                 successes: pulumi.Input[Sequence[pulumi.Input['WorkspaceAdminPortalPaletteSuccessArgs']]],
-                 warnings: pulumi.Input[Sequence[pulumi.Input['WorkspaceAdminPortalPaletteWarningArgs']]]):
-        pulumi.set(__self__, "errors", errors)
-        pulumi.set(__self__, "infos", infos)
-        pulumi.set(__self__, "primaries", primaries)
-        pulumi.set(__self__, "secondaries", secondaries)
-        pulumi.set(__self__, "successes", successes)
-        pulumi.set(__self__, "warnings", warnings)
+                 errors: Optional[pulumi.Input[Sequence[pulumi.Input['WorkspaceAdminPortalPaletteErrorArgs']]]] = None,
+                 infos: Optional[pulumi.Input[Sequence[pulumi.Input['WorkspaceAdminPortalPaletteInfoArgs']]]] = None,
+                 primaries: Optional[pulumi.Input[Sequence[pulumi.Input['WorkspaceAdminPortalPalettePrimaryArgs']]]] = None,
+                 secondaries: Optional[pulumi.Input[Sequence[pulumi.Input['WorkspaceAdminPortalPaletteSecondaryArgs']]]] = None,
+                 successes: Optional[pulumi.Input[Sequence[pulumi.Input['WorkspaceAdminPortalPaletteSuccessArgs']]]] = None,
+                 warnings: Optional[pulumi.Input[Sequence[pulumi.Input['WorkspaceAdminPortalPaletteWarningArgs']]]] = None):
+        if errors is not None:
+            pulumi.set(__self__, "errors", errors)
+        if infos is not None:
+            pulumi.set(__self__, "infos", infos)
+        if primaries is not None:
+            pulumi.set(__self__, "primaries", primaries)
+        if secondaries is not None:
+            pulumi.set(__self__, "secondaries", secondaries)
+        if successes is not None:
+            pulumi.set(__self__, "successes", successes)
+        if warnings is not None:
+            pulumi.set(__self__, "warnings", warnings)
 
     @property
     @pulumi.getter
-    def errors(self) -> pulumi.Input[Sequence[pulumi.Input['WorkspaceAdminPortalPaletteErrorArgs']]]:
+    def errors(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['WorkspaceAdminPortalPaletteErrorArgs']]]]:
         return pulumi.get(self, "errors")
 
     @errors.setter
-    def errors(self, value: pulumi.Input[Sequence[pulumi.Input['WorkspaceAdminPortalPaletteErrorArgs']]]):
+    def errors(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['WorkspaceAdminPortalPaletteErrorArgs']]]]):
         pulumi.set(self, "errors", value)
 
     @property
     @pulumi.getter
-    def infos(self) -> pulumi.Input[Sequence[pulumi.Input['WorkspaceAdminPortalPaletteInfoArgs']]]:
+    def infos(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['WorkspaceAdminPortalPaletteInfoArgs']]]]:
         return pulumi.get(self, "infos")
 
     @infos.setter
-    def infos(self, value: pulumi.Input[Sequence[pulumi.Input['WorkspaceAdminPortalPaletteInfoArgs']]]):
+    def infos(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['WorkspaceAdminPortalPaletteInfoArgs']]]]):
         pulumi.set(self, "infos", value)
 
     @property
     @pulumi.getter
-    def primaries(self) -> pulumi.Input[Sequence[pulumi.Input['WorkspaceAdminPortalPalettePrimaryArgs']]]:
+    def primaries(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['WorkspaceAdminPortalPalettePrimaryArgs']]]]:
         return pulumi.get(self, "primaries")
 
     @primaries.setter
-    def primaries(self, value: pulumi.Input[Sequence[pulumi.Input['WorkspaceAdminPortalPalettePrimaryArgs']]]):
+    def primaries(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['WorkspaceAdminPortalPalettePrimaryArgs']]]]):
         pulumi.set(self, "primaries", value)
 
     @property
     @pulumi.getter
-    def secondaries(self) -> pulumi.Input[Sequence[pulumi.Input['WorkspaceAdminPortalPaletteSecondaryArgs']]]:
+    def secondaries(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['WorkspaceAdminPortalPaletteSecondaryArgs']]]]:
         return pulumi.get(self, "secondaries")
 
     @secondaries.setter
-    def secondaries(self, value: pulumi.Input[Sequence[pulumi.Input['WorkspaceAdminPortalPaletteSecondaryArgs']]]):
+    def secondaries(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['WorkspaceAdminPortalPaletteSecondaryArgs']]]]):
         pulumi.set(self, "secondaries", value)
 
     @property
     @pulumi.getter
-    def successes(self) -> pulumi.Input[Sequence[pulumi.Input['WorkspaceAdminPortalPaletteSuccessArgs']]]:
+    def successes(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['WorkspaceAdminPortalPaletteSuccessArgs']]]]:
         return pulumi.get(self, "successes")
 
     @successes.setter
-    def successes(self, value: pulumi.Input[Sequence[pulumi.Input['WorkspaceAdminPortalPaletteSuccessArgs']]]):
+    def successes(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['WorkspaceAdminPortalPaletteSuccessArgs']]]]):
         pulumi.set(self, "successes", value)
 
     @property
     @pulumi.getter
-    def warnings(self) -> pulumi.Input[Sequence[pulumi.Input['WorkspaceAdminPortalPaletteWarningArgs']]]:
+    def warnings(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['WorkspaceAdminPortalPaletteWarningArgs']]]]:
         return pulumi.get(self, "warnings")
 
     @warnings.setter
-    def warnings(self, value: pulumi.Input[Sequence[pulumi.Input['WorkspaceAdminPortalPaletteWarningArgs']]]):
+    def warnings(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['WorkspaceAdminPortalPaletteWarningArgs']]]]):
         pulumi.set(self, "warnings", value)
 
 
 @pulumi.input_type
 class WorkspaceAdminPortalPaletteErrorArgs:
     def __init__(__self__, *,
                  contrast_text: pulumi.Input[str],
@@ -610,46 +617,60 @@
         pulumi.set(self, "main", value)
 
 
 @pulumi.input_type
 class WorkspaceAuthPolicyArgs:
     def __init__(__self__, *,
                  allow_signups: pulumi.Input[bool],
+                 allow_tenant_invitations: pulumi.Input[bool],
                  allow_unverified_users: pulumi.Input[bool],
                  auth_strategy: pulumi.Input[str],
                  enable_api_tokens: pulumi.Input[bool],
                  enable_roles: pulumi.Input[bool],
                  jwt_access_token_expiration: pulumi.Input[int],
                  jwt_refresh_token_expiration: pulumi.Input[int],
                  same_site_cookie_policy: pulumi.Input[str],
                  jwt_algorithm: Optional[pulumi.Input[str]] = None,
-                 jwt_public_key: Optional[pulumi.Input[str]] = None):
+                 jwt_public_key: Optional[pulumi.Input[str]] = None,
+                 machine_to_machine_auth_strategy: Optional[pulumi.Input[str]] = None):
         pulumi.set(__self__, "allow_signups", allow_signups)
+        pulumi.set(__self__, "allow_tenant_invitations", allow_tenant_invitations)
         pulumi.set(__self__, "allow_unverified_users", allow_unverified_users)
         pulumi.set(__self__, "auth_strategy", auth_strategy)
         pulumi.set(__self__, "enable_api_tokens", enable_api_tokens)
         pulumi.set(__self__, "enable_roles", enable_roles)
         pulumi.set(__self__, "jwt_access_token_expiration", jwt_access_token_expiration)
         pulumi.set(__self__, "jwt_refresh_token_expiration", jwt_refresh_token_expiration)
         pulumi.set(__self__, "same_site_cookie_policy", same_site_cookie_policy)
         if jwt_algorithm is not None:
             pulumi.set(__self__, "jwt_algorithm", jwt_algorithm)
         if jwt_public_key is not None:
             pulumi.set(__self__, "jwt_public_key", jwt_public_key)
+        if machine_to_machine_auth_strategy is not None:
+            pulumi.set(__self__, "machine_to_machine_auth_strategy", machine_to_machine_auth_strategy)
 
     @property
     @pulumi.getter(name="allowSignups")
     def allow_signups(self) -> pulumi.Input[bool]:
         return pulumi.get(self, "allow_signups")
 
     @allow_signups.setter
     def allow_signups(self, value: pulumi.Input[bool]):
         pulumi.set(self, "allow_signups", value)
 
     @property
+    @pulumi.getter(name="allowTenantInvitations")
+    def allow_tenant_invitations(self) -> pulumi.Input[bool]:
+        return pulumi.get(self, "allow_tenant_invitations")
+
+    @allow_tenant_invitations.setter
+    def allow_tenant_invitations(self, value: pulumi.Input[bool]):
+        pulumi.set(self, "allow_tenant_invitations", value)
+
+    @property
     @pulumi.getter(name="allowUnverifiedUsers")
     def allow_unverified_users(self) -> pulumi.Input[bool]:
         return pulumi.get(self, "allow_unverified_users")
 
     @allow_unverified_users.setter
     def allow_unverified_users(self, value: pulumi.Input[bool]):
         pulumi.set(self, "allow_unverified_users", value)
@@ -722,14 +743,23 @@
     def jwt_public_key(self) -> Optional[pulumi.Input[str]]:
         return pulumi.get(self, "jwt_public_key")
 
     @jwt_public_key.setter
     def jwt_public_key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "jwt_public_key", value)
 
+    @property
+    @pulumi.getter(name="machineToMachineAuthStrategy")
+    def machine_to_machine_auth_strategy(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "machine_to_machine_auth_strategy")
+
+    @machine_to_machine_auth_strategy.setter
+    def machine_to_machine_auth_strategy(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "machine_to_machine_auth_strategy", value)
+
 
 @pulumi.input_type
 class WorkspaceBulkTenantsInvitesEmailArgs:
     def __init__(__self__, *,
                  from_address: pulumi.Input[str],
                  from_name: pulumi.Input[str],
                  html_template: pulumi.Input[str],
@@ -849,122 +879,164 @@
     def ignored_emails(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "ignored_emails", value)
 
 
 @pulumi.input_type
 class WorkspaceFacebookSocialLoginArgs:
     def __init__(__self__, *,
-                 client_id: pulumi.Input[str],
                  redirect_url: pulumi.Input[str],
-                 secret: pulumi.Input[str]):
-        pulumi.set(__self__, "client_id", client_id)
+                 client_id: Optional[pulumi.Input[str]] = None,
+                 customised: Optional[pulumi.Input[bool]] = None,
+                 secret: Optional[pulumi.Input[str]] = None):
         pulumi.set(__self__, "redirect_url", redirect_url)
-        pulumi.set(__self__, "secret", secret)
+        if client_id is not None:
+            pulumi.set(__self__, "client_id", client_id)
+        if customised is not None:
+            pulumi.set(__self__, "customised", customised)
+        if secret is not None:
+            pulumi.set(__self__, "secret", secret)
+
+    @property
+    @pulumi.getter(name="redirectUrl")
+    def redirect_url(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "redirect_url")
+
+    @redirect_url.setter
+    def redirect_url(self, value: pulumi.Input[str]):
+        pulumi.set(self, "redirect_url", value)
 
     @property
     @pulumi.getter(name="clientId")
-    def client_id(self) -> pulumi.Input[str]:
+    def client_id(self) -> Optional[pulumi.Input[str]]:
         return pulumi.get(self, "client_id")
 
     @client_id.setter
-    def client_id(self, value: pulumi.Input[str]):
+    def client_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "client_id", value)
 
     @property
-    @pulumi.getter(name="redirectUrl")
-    def redirect_url(self) -> pulumi.Input[str]:
-        return pulumi.get(self, "redirect_url")
+    @pulumi.getter
+    def customised(self) -> Optional[pulumi.Input[bool]]:
+        return pulumi.get(self, "customised")
 
-    @redirect_url.setter
-    def redirect_url(self, value: pulumi.Input[str]):
-        pulumi.set(self, "redirect_url", value)
+    @customised.setter
+    def customised(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "customised", value)
 
     @property
     @pulumi.getter
-    def secret(self) -> pulumi.Input[str]:
+    def secret(self) -> Optional[pulumi.Input[str]]:
         return pulumi.get(self, "secret")
 
     @secret.setter
-    def secret(self, value: pulumi.Input[str]):
+    def secret(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret", value)
 
 
 @pulumi.input_type
 class WorkspaceGithubSocialLoginArgs:
     def __init__(__self__, *,
-                 client_id: pulumi.Input[str],
                  redirect_url: pulumi.Input[str],
-                 secret: pulumi.Input[str]):
-        pulumi.set(__self__, "client_id", client_id)
+                 client_id: Optional[pulumi.Input[str]] = None,
+                 customised: Optional[pulumi.Input[bool]] = None,
+                 secret: Optional[pulumi.Input[str]] = None):
         pulumi.set(__self__, "redirect_url", redirect_url)
-        pulumi.set(__self__, "secret", secret)
+        if client_id is not None:
+            pulumi.set(__self__, "client_id", client_id)
+        if customised is not None:
+            pulumi.set(__self__, "customised", customised)
+        if secret is not None:
+            pulumi.set(__self__, "secret", secret)
+
+    @property
+    @pulumi.getter(name="redirectUrl")
+    def redirect_url(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "redirect_url")
+
+    @redirect_url.setter
+    def redirect_url(self, value: pulumi.Input[str]):
+        pulumi.set(self, "redirect_url", value)
 
     @property
     @pulumi.getter(name="clientId")
-    def client_id(self) -> pulumi.Input[str]:
+    def client_id(self) -> Optional[pulumi.Input[str]]:
         return pulumi.get(self, "client_id")
 
     @client_id.setter
-    def client_id(self, value: pulumi.Input[str]):
+    def client_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "client_id", value)
 
     @property
-    @pulumi.getter(name="redirectUrl")
-    def redirect_url(self) -> pulumi.Input[str]:
-        return pulumi.get(self, "redirect_url")
+    @pulumi.getter
+    def customised(self) -> Optional[pulumi.Input[bool]]:
+        return pulumi.get(self, "customised")
 
-    @redirect_url.setter
-    def redirect_url(self, value: pulumi.Input[str]):
-        pulumi.set(self, "redirect_url", value)
+    @customised.setter
+    def customised(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "customised", value)
 
     @property
     @pulumi.getter
-    def secret(self) -> pulumi.Input[str]:
+    def secret(self) -> Optional[pulumi.Input[str]]:
         return pulumi.get(self, "secret")
 
     @secret.setter
-    def secret(self, value: pulumi.Input[str]):
+    def secret(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret", value)
 
 
 @pulumi.input_type
 class WorkspaceGoogleSocialLoginArgs:
     def __init__(__self__, *,
-                 client_id: pulumi.Input[str],
                  redirect_url: pulumi.Input[str],
-                 secret: pulumi.Input[str]):
-        pulumi.set(__self__, "client_id", client_id)
+                 client_id: Optional[pulumi.Input[str]] = None,
+                 customised: Optional[pulumi.Input[bool]] = None,
+                 secret: Optional[pulumi.Input[str]] = None):
         pulumi.set(__self__, "redirect_url", redirect_url)
-        pulumi.set(__self__, "secret", secret)
+        if client_id is not None:
+            pulumi.set(__self__, "client_id", client_id)
+        if customised is not None:
+            pulumi.set(__self__, "customised", customised)
+        if secret is not None:
+            pulumi.set(__self__, "secret", secret)
+
+    @property
+    @pulumi.getter(name="redirectUrl")
+    def redirect_url(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "redirect_url")
+
+    @redirect_url.setter
+    def redirect_url(self, value: pulumi.Input[str]):
+        pulumi.set(self, "redirect_url", value)
 
     @property
     @pulumi.getter(name="clientId")
-    def client_id(self) -> pulumi.Input[str]:
+    def client_id(self) -> Optional[pulumi.Input[str]]:
         return pulumi.get(self, "client_id")
 
     @client_id.setter
-    def client_id(self, value: pulumi.Input[str]):
+    def client_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "client_id", value)
 
     @property
-    @pulumi.getter(name="redirectUrl")
-    def redirect_url(self) -> pulumi.Input[str]:
-        return pulumi.get(self, "redirect_url")
+    @pulumi.getter
+    def customised(self) -> Optional[pulumi.Input[bool]]:
+        return pulumi.get(self, "customised")
 
-    @redirect_url.setter
-    def redirect_url(self, value: pulumi.Input[str]):
-        pulumi.set(self, "redirect_url", value)
+    @customised.setter
+    def customised(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "customised", value)
 
     @property
     @pulumi.getter
-    def secret(self) -> pulumi.Input[str]:
+    def secret(self) -> Optional[pulumi.Input[str]]:
         return pulumi.get(self, "secret")
 
     @secret.setter
-    def secret(self, value: pulumi.Input[str]):
+    def secret(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret", value)
 
 
 @pulumi.input_type
 class WorkspaceHostedLoginArgs:
     def __init__(__self__, *,
                  allowed_redirect_urls: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
@@ -1196,46 +1268,60 @@
     def enforce(self, value: pulumi.Input[str]):
         pulumi.set(self, "enforce", value)
 
 
 @pulumi.input_type
 class WorkspaceMicrosoftSocialLoginArgs:
     def __init__(__self__, *,
-                 client_id: pulumi.Input[str],
                  redirect_url: pulumi.Input[str],
-                 secret: pulumi.Input[str]):
-        pulumi.set(__self__, "client_id", client_id)
+                 client_id: Optional[pulumi.Input[str]] = None,
+                 customised: Optional[pulumi.Input[bool]] = None,
+                 secret: Optional[pulumi.Input[str]] = None):
         pulumi.set(__self__, "redirect_url", redirect_url)
-        pulumi.set(__self__, "secret", secret)
+        if client_id is not None:
+            pulumi.set(__self__, "client_id", client_id)
+        if customised is not None:
+            pulumi.set(__self__, "customised", customised)
+        if secret is not None:
+            pulumi.set(__self__, "secret", secret)
+
+    @property
+    @pulumi.getter(name="redirectUrl")
+    def redirect_url(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "redirect_url")
+
+    @redirect_url.setter
+    def redirect_url(self, value: pulumi.Input[str]):
+        pulumi.set(self, "redirect_url", value)
 
     @property
     @pulumi.getter(name="clientId")
-    def client_id(self) -> pulumi.Input[str]:
+    def client_id(self) -> Optional[pulumi.Input[str]]:
         return pulumi.get(self, "client_id")
 
     @client_id.setter
-    def client_id(self, value: pulumi.Input[str]):
+    def client_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "client_id", value)
 
     @property
-    @pulumi.getter(name="redirectUrl")
-    def redirect_url(self) -> pulumi.Input[str]:
-        return pulumi.get(self, "redirect_url")
+    @pulumi.getter
+    def customised(self) -> Optional[pulumi.Input[bool]]:
+        return pulumi.get(self, "customised")
 
-    @redirect_url.setter
-    def redirect_url(self, value: pulumi.Input[str]):
-        pulumi.set(self, "redirect_url", value)
+    @customised.setter
+    def customised(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "customised", value)
 
     @property
     @pulumi.getter
-    def secret(self) -> pulumi.Input[str]:
+    def secret(self) -> Optional[pulumi.Input[str]]:
         return pulumi.get(self, "secret")
 
     @secret.setter
-    def secret(self, value: pulumi.Input[str]):
+    def secret(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret", value)
 
 
 @pulumi.input_type
 class WorkspaceNewDeviceConnectedEmailArgs:
     def __init__(__self__, *,
                  from_address: pulumi.Input[str],
```

### Comparing `pulumi_frontegg-0.2.25/pulumi_frontegg/_utilities.py` & `pulumi_frontegg-0.2.26/pulumi_frontegg/_utilities.py`

 * *Files 0% similar despite different names*

```diff
@@ -243,8 +243,8 @@
         }).apply(lambda resolved_args: func(*resolved_args['args'],
                                             opts=opts,
                                             **resolved_args['kwargs']))
 
     return (lambda _: lifted_func)
 
 def get_plugin_download_url():
-	return "https://github.com/MaterializeInc/pulumi-frontegg/releases/download/v0.2.25/"
+	return "https://github.com/MaterializeInc/pulumi-frontegg/releases/download/v0.2.26/"
```

### Comparing `pulumi_frontegg-0.2.25/pulumi_frontegg/config/vars.py` & `pulumi_frontegg-0.2.26/pulumi_frontegg/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_frontegg-0.2.25/pulumi_frontegg/get_permission.py` & `pulumi_frontegg-0.2.26/pulumi_frontegg/get_permission.py`

 * *Files identical despite different names*

### Comparing `pulumi_frontegg-0.2.25/pulumi_frontegg/outputs.py` & `pulumi_frontegg-0.2.26/pulumi_frontegg/outputs.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,29 +96,30 @@
                  enable_roles: bool,
                  enable_security: bool,
                  enable_sso: bool,
                  enable_subscriptions: bool,
                  enable_usage: bool,
                  enable_users: bool,
                  enable_webhooks: bool,
-                 palette: 'outputs.WorkspaceAdminPortalPalette'):
+                 palette: Optional['outputs.WorkspaceAdminPortalPalette'] = None):
         pulumi.set(__self__, "enable_account_settings", enable_account_settings)
         pulumi.set(__self__, "enable_api_tokens", enable_api_tokens)
         pulumi.set(__self__, "enable_audit_logs", enable_audit_logs)
         pulumi.set(__self__, "enable_personal_api_tokens", enable_personal_api_tokens)
         pulumi.set(__self__, "enable_privacy", enable_privacy)
         pulumi.set(__self__, "enable_profile", enable_profile)
         pulumi.set(__self__, "enable_roles", enable_roles)
         pulumi.set(__self__, "enable_security", enable_security)
         pulumi.set(__self__, "enable_sso", enable_sso)
         pulumi.set(__self__, "enable_subscriptions", enable_subscriptions)
         pulumi.set(__self__, "enable_usage", enable_usage)
         pulumi.set(__self__, "enable_users", enable_users)
         pulumi.set(__self__, "enable_webhooks", enable_webhooks)
-        pulumi.set(__self__, "palette", palette)
+        if palette is not None:
+            pulumi.set(__self__, "palette", palette)
 
     @property
     @pulumi.getter(name="enableAccountSettings")
     def enable_account_settings(self) -> bool:
         return pulumi.get(self, "enable_account_settings")
 
     @property
@@ -179,62 +180,68 @@
     @property
     @pulumi.getter(name="enableWebhooks")
     def enable_webhooks(self) -> bool:
         return pulumi.get(self, "enable_webhooks")
 
     @property
     @pulumi.getter
-    def palette(self) -> 'outputs.WorkspaceAdminPortalPalette':
+    def palette(self) -> Optional['outputs.WorkspaceAdminPortalPalette']:
         return pulumi.get(self, "palette")
 
 
 @pulumi.output_type
 class WorkspaceAdminPortalPalette(dict):
     def __init__(__self__, *,
-                 errors: Sequence['outputs.WorkspaceAdminPortalPaletteError'],
-                 infos: Sequence['outputs.WorkspaceAdminPortalPaletteInfo'],
-                 primaries: Sequence['outputs.WorkspaceAdminPortalPalettePrimary'],
-                 secondaries: Sequence['outputs.WorkspaceAdminPortalPaletteSecondary'],
-                 successes: Sequence['outputs.WorkspaceAdminPortalPaletteSuccess'],
-                 warnings: Sequence['outputs.WorkspaceAdminPortalPaletteWarning']):
-        pulumi.set(__self__, "errors", errors)
-        pulumi.set(__self__, "infos", infos)
-        pulumi.set(__self__, "primaries", primaries)
-        pulumi.set(__self__, "secondaries", secondaries)
-        pulumi.set(__self__, "successes", successes)
-        pulumi.set(__self__, "warnings", warnings)
+                 errors: Optional[Sequence['outputs.WorkspaceAdminPortalPaletteError']] = None,
+                 infos: Optional[Sequence['outputs.WorkspaceAdminPortalPaletteInfo']] = None,
+                 primaries: Optional[Sequence['outputs.WorkspaceAdminPortalPalettePrimary']] = None,
+                 secondaries: Optional[Sequence['outputs.WorkspaceAdminPortalPaletteSecondary']] = None,
+                 successes: Optional[Sequence['outputs.WorkspaceAdminPortalPaletteSuccess']] = None,
+                 warnings: Optional[Sequence['outputs.WorkspaceAdminPortalPaletteWarning']] = None):
+        if errors is not None:
+            pulumi.set(__self__, "errors", errors)
+        if infos is not None:
+            pulumi.set(__self__, "infos", infos)
+        if primaries is not None:
+            pulumi.set(__self__, "primaries", primaries)
+        if secondaries is not None:
+            pulumi.set(__self__, "secondaries", secondaries)
+        if successes is not None:
+            pulumi.set(__self__, "successes", successes)
+        if warnings is not None:
+            pulumi.set(__self__, "warnings", warnings)
 
     @property
     @pulumi.getter
-    def errors(self) -> Sequence['outputs.WorkspaceAdminPortalPaletteError']:
+    def errors(self) -> Optional[Sequence['outputs.WorkspaceAdminPortalPaletteError']]:
         return pulumi.get(self, "errors")
 
     @property
     @pulumi.getter
-    def infos(self) -> Sequence['outputs.WorkspaceAdminPortalPaletteInfo']:
+    def infos(self) -> Optional[Sequence['outputs.WorkspaceAdminPortalPaletteInfo']]:
         return pulumi.get(self, "infos")
 
     @property
     @pulumi.getter
-    def primaries(self) -> Sequence['outputs.WorkspaceAdminPortalPalettePrimary']:
+    def primaries(self) -> Optional[Sequence['outputs.WorkspaceAdminPortalPalettePrimary']]:
         return pulumi.get(self, "primaries")
 
     @property
     @pulumi.getter
-    def secondaries(self) -> Sequence['outputs.WorkspaceAdminPortalPaletteSecondary']:
+    def secondaries(self) -> Optional[Sequence['outputs.WorkspaceAdminPortalPaletteSecondary']]:
         return pulumi.get(self, "secondaries")
 
     @property
     @pulumi.getter
-    def successes(self) -> Sequence['outputs.WorkspaceAdminPortalPaletteSuccess']:
+    def successes(self) -> Optional[Sequence['outputs.WorkspaceAdminPortalPaletteSuccess']]:
         return pulumi.get(self, "successes")
 
     @property
     @pulumi.getter
-    def warnings(self) -> Sequence['outputs.WorkspaceAdminPortalPaletteWarning']:
+    def warnings(self) -> Optional[Sequence['outputs.WorkspaceAdminPortalPaletteWarning']]:
         return pulumi.get(self, "warnings")
 
 
 @pulumi.output_type
 class WorkspaceAdminPortalPaletteError(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -565,14 +572,16 @@
 @pulumi.output_type
 class WorkspaceAuthPolicy(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
         if key == "allowSignups":
             suggest = "allow_signups"
+        elif key == "allowTenantInvitations":
+            suggest = "allow_tenant_invitations"
         elif key == "allowUnverifiedUsers":
             suggest = "allow_unverified_users"
         elif key == "authStrategy":
             suggest = "auth_strategy"
         elif key == "enableApiTokens":
             suggest = "enable_api_tokens"
         elif key == "enableRoles":
@@ -583,56 +592,68 @@
             suggest = "jwt_refresh_token_expiration"
         elif key == "sameSiteCookiePolicy":
             suggest = "same_site_cookie_policy"
         elif key == "jwtAlgorithm":
             suggest = "jwt_algorithm"
         elif key == "jwtPublicKey":
             suggest = "jwt_public_key"
+        elif key == "machineToMachineAuthStrategy":
+            suggest = "machine_to_machine_auth_strategy"
 
         if suggest:
             pulumi.log.warn(f"Key '{key}' not found in WorkspaceAuthPolicy. Access the value via the '{suggest}' property getter instead.")
 
     def __getitem__(self, key: str) -> Any:
         WorkspaceAuthPolicy.__key_warning(key)
         return super().__getitem__(key)
 
     def get(self, key: str, default = None) -> Any:
         WorkspaceAuthPolicy.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
                  allow_signups: bool,
+                 allow_tenant_invitations: bool,
                  allow_unverified_users: bool,
                  auth_strategy: str,
                  enable_api_tokens: bool,
                  enable_roles: bool,
                  jwt_access_token_expiration: int,
                  jwt_refresh_token_expiration: int,
                  same_site_cookie_policy: str,
                  jwt_algorithm: Optional[str] = None,
-                 jwt_public_key: Optional[str] = None):
+                 jwt_public_key: Optional[str] = None,
+                 machine_to_machine_auth_strategy: Optional[str] = None):
         pulumi.set(__self__, "allow_signups", allow_signups)
+        pulumi.set(__self__, "allow_tenant_invitations", allow_tenant_invitations)
         pulumi.set(__self__, "allow_unverified_users", allow_unverified_users)
         pulumi.set(__self__, "auth_strategy", auth_strategy)
         pulumi.set(__self__, "enable_api_tokens", enable_api_tokens)
         pulumi.set(__self__, "enable_roles", enable_roles)
         pulumi.set(__self__, "jwt_access_token_expiration", jwt_access_token_expiration)
         pulumi.set(__self__, "jwt_refresh_token_expiration", jwt_refresh_token_expiration)
         pulumi.set(__self__, "same_site_cookie_policy", same_site_cookie_policy)
         if jwt_algorithm is not None:
             pulumi.set(__self__, "jwt_algorithm", jwt_algorithm)
         if jwt_public_key is not None:
             pulumi.set(__self__, "jwt_public_key", jwt_public_key)
+        if machine_to_machine_auth_strategy is not None:
+            pulumi.set(__self__, "machine_to_machine_auth_strategy", machine_to_machine_auth_strategy)
 
     @property
     @pulumi.getter(name="allowSignups")
     def allow_signups(self) -> bool:
         return pulumi.get(self, "allow_signups")
 
     @property
+    @pulumi.getter(name="allowTenantInvitations")
+    def allow_tenant_invitations(self) -> bool:
+        return pulumi.get(self, "allow_tenant_invitations")
+
+    @property
     @pulumi.getter(name="allowUnverifiedUsers")
     def allow_unverified_users(self) -> bool:
         return pulumi.get(self, "allow_unverified_users")
 
     @property
     @pulumi.getter(name="authStrategy")
     def auth_strategy(self) -> str:
@@ -669,14 +690,19 @@
         return pulumi.get(self, "jwt_algorithm")
 
     @property
     @pulumi.getter(name="jwtPublicKey")
     def jwt_public_key(self) -> Optional[str]:
         return pulumi.get(self, "jwt_public_key")
 
+    @property
+    @pulumi.getter(name="machineToMachineAuthStrategy")
+    def machine_to_machine_auth_strategy(self) -> Optional[str]:
+        return pulumi.get(self, "machine_to_machine_auth_strategy")
+
 
 @pulumi.output_type
 class WorkspaceBulkTenantsInvitesEmail(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
         if key == "fromAddress":
@@ -806,141 +832,171 @@
 
 
 @pulumi.output_type
 class WorkspaceFacebookSocialLogin(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
-        if key == "clientId":
-            suggest = "client_id"
-        elif key == "redirectUrl":
+        if key == "redirectUrl":
             suggest = "redirect_url"
+        elif key == "clientId":
+            suggest = "client_id"
 
         if suggest:
             pulumi.log.warn(f"Key '{key}' not found in WorkspaceFacebookSocialLogin. Access the value via the '{suggest}' property getter instead.")
 
     def __getitem__(self, key: str) -> Any:
         WorkspaceFacebookSocialLogin.__key_warning(key)
         return super().__getitem__(key)
 
     def get(self, key: str, default = None) -> Any:
         WorkspaceFacebookSocialLogin.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
-                 client_id: str,
                  redirect_url: str,
-                 secret: str):
-        pulumi.set(__self__, "client_id", client_id)
+                 client_id: Optional[str] = None,
+                 customised: Optional[bool] = None,
+                 secret: Optional[str] = None):
         pulumi.set(__self__, "redirect_url", redirect_url)
-        pulumi.set(__self__, "secret", secret)
+        if client_id is not None:
+            pulumi.set(__self__, "client_id", client_id)
+        if customised is not None:
+            pulumi.set(__self__, "customised", customised)
+        if secret is not None:
+            pulumi.set(__self__, "secret", secret)
+
+    @property
+    @pulumi.getter(name="redirectUrl")
+    def redirect_url(self) -> str:
+        return pulumi.get(self, "redirect_url")
 
     @property
     @pulumi.getter(name="clientId")
-    def client_id(self) -> str:
+    def client_id(self) -> Optional[str]:
         return pulumi.get(self, "client_id")
 
     @property
-    @pulumi.getter(name="redirectUrl")
-    def redirect_url(self) -> str:
-        return pulumi.get(self, "redirect_url")
+    @pulumi.getter
+    def customised(self) -> Optional[bool]:
+        return pulumi.get(self, "customised")
 
     @property
     @pulumi.getter
-    def secret(self) -> str:
+    def secret(self) -> Optional[str]:
         return pulumi.get(self, "secret")
 
 
 @pulumi.output_type
 class WorkspaceGithubSocialLogin(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
-        if key == "clientId":
-            suggest = "client_id"
-        elif key == "redirectUrl":
+        if key == "redirectUrl":
             suggest = "redirect_url"
+        elif key == "clientId":
+            suggest = "client_id"
 
         if suggest:
             pulumi.log.warn(f"Key '{key}' not found in WorkspaceGithubSocialLogin. Access the value via the '{suggest}' property getter instead.")
 
     def __getitem__(self, key: str) -> Any:
         WorkspaceGithubSocialLogin.__key_warning(key)
         return super().__getitem__(key)
 
     def get(self, key: str, default = None) -> Any:
         WorkspaceGithubSocialLogin.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
-                 client_id: str,
                  redirect_url: str,
-                 secret: str):
-        pulumi.set(__self__, "client_id", client_id)
+                 client_id: Optional[str] = None,
+                 customised: Optional[bool] = None,
+                 secret: Optional[str] = None):
         pulumi.set(__self__, "redirect_url", redirect_url)
-        pulumi.set(__self__, "secret", secret)
+        if client_id is not None:
+            pulumi.set(__self__, "client_id", client_id)
+        if customised is not None:
+            pulumi.set(__self__, "customised", customised)
+        if secret is not None:
+            pulumi.set(__self__, "secret", secret)
+
+    @property
+    @pulumi.getter(name="redirectUrl")
+    def redirect_url(self) -> str:
+        return pulumi.get(self, "redirect_url")
 
     @property
     @pulumi.getter(name="clientId")
-    def client_id(self) -> str:
+    def client_id(self) -> Optional[str]:
         return pulumi.get(self, "client_id")
 
     @property
-    @pulumi.getter(name="redirectUrl")
-    def redirect_url(self) -> str:
-        return pulumi.get(self, "redirect_url")
+    @pulumi.getter
+    def customised(self) -> Optional[bool]:
+        return pulumi.get(self, "customised")
 
     @property
     @pulumi.getter
-    def secret(self) -> str:
+    def secret(self) -> Optional[str]:
         return pulumi.get(self, "secret")
 
 
 @pulumi.output_type
 class WorkspaceGoogleSocialLogin(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
-        if key == "clientId":
-            suggest = "client_id"
-        elif key == "redirectUrl":
+        if key == "redirectUrl":
             suggest = "redirect_url"
+        elif key == "clientId":
+            suggest = "client_id"
 
         if suggest:
             pulumi.log.warn(f"Key '{key}' not found in WorkspaceGoogleSocialLogin. Access the value via the '{suggest}' property getter instead.")
 
     def __getitem__(self, key: str) -> Any:
         WorkspaceGoogleSocialLogin.__key_warning(key)
         return super().__getitem__(key)
 
     def get(self, key: str, default = None) -> Any:
         WorkspaceGoogleSocialLogin.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
-                 client_id: str,
                  redirect_url: str,
-                 secret: str):
-        pulumi.set(__self__, "client_id", client_id)
+                 client_id: Optional[str] = None,
+                 customised: Optional[bool] = None,
+                 secret: Optional[str] = None):
         pulumi.set(__self__, "redirect_url", redirect_url)
-        pulumi.set(__self__, "secret", secret)
+        if client_id is not None:
+            pulumi.set(__self__, "client_id", client_id)
+        if customised is not None:
+            pulumi.set(__self__, "customised", customised)
+        if secret is not None:
+            pulumi.set(__self__, "secret", secret)
+
+    @property
+    @pulumi.getter(name="redirectUrl")
+    def redirect_url(self) -> str:
+        return pulumi.get(self, "redirect_url")
 
     @property
     @pulumi.getter(name="clientId")
-    def client_id(self) -> str:
+    def client_id(self) -> Optional[str]:
         return pulumi.get(self, "client_id")
 
     @property
-    @pulumi.getter(name="redirectUrl")
-    def redirect_url(self) -> str:
-        return pulumi.get(self, "redirect_url")
+    @pulumi.getter
+    def customised(self) -> Optional[bool]:
+        return pulumi.get(self, "customised")
 
     @property
     @pulumi.getter
-    def secret(self) -> str:
+    def secret(self) -> Optional[str]:
         return pulumi.get(self, "secret")
 
 
 @pulumi.output_type
 class WorkspaceHostedLogin(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -1222,51 +1278,61 @@
 
 
 @pulumi.output_type
 class WorkspaceMicrosoftSocialLogin(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
-        if key == "clientId":
-            suggest = "client_id"
-        elif key == "redirectUrl":
+        if key == "redirectUrl":
             suggest = "redirect_url"
+        elif key == "clientId":
+            suggest = "client_id"
 
         if suggest:
             pulumi.log.warn(f"Key '{key}' not found in WorkspaceMicrosoftSocialLogin. Access the value via the '{suggest}' property getter instead.")
 
     def __getitem__(self, key: str) -> Any:
         WorkspaceMicrosoftSocialLogin.__key_warning(key)
         return super().__getitem__(key)
 
     def get(self, key: str, default = None) -> Any:
         WorkspaceMicrosoftSocialLogin.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
-                 client_id: str,
                  redirect_url: str,
-                 secret: str):
-        pulumi.set(__self__, "client_id", client_id)
+                 client_id: Optional[str] = None,
+                 customised: Optional[bool] = None,
+                 secret: Optional[str] = None):
         pulumi.set(__self__, "redirect_url", redirect_url)
-        pulumi.set(__self__, "secret", secret)
+        if client_id is not None:
+            pulumi.set(__self__, "client_id", client_id)
+        if customised is not None:
+            pulumi.set(__self__, "customised", customised)
+        if secret is not None:
+            pulumi.set(__self__, "secret", secret)
+
+    @property
+    @pulumi.getter(name="redirectUrl")
+    def redirect_url(self) -> str:
+        return pulumi.get(self, "redirect_url")
 
     @property
     @pulumi.getter(name="clientId")
-    def client_id(self) -> str:
+    def client_id(self) -> Optional[str]:
         return pulumi.get(self, "client_id")
 
     @property
-    @pulumi.getter(name="redirectUrl")
-    def redirect_url(self) -> str:
-        return pulumi.get(self, "redirect_url")
+    @pulumi.getter
+    def customised(self) -> Optional[bool]:
+        return pulumi.get(self, "customised")
 
     @property
     @pulumi.getter
-    def secret(self) -> str:
+    def secret(self) -> Optional[str]:
         return pulumi.get(self, "secret")
 
 
 @pulumi.output_type
 class WorkspaceNewDeviceConnectedEmail(dict):
     @staticmethod
     def __key_warning(key: str):
```

### Comparing `pulumi_frontegg-0.2.25/pulumi_frontegg/permission.py` & `pulumi_frontegg-0.2.26/pulumi_frontegg/permission.py`

 * *Files identical despite different names*

### Comparing `pulumi_frontegg-0.2.25/pulumi_frontegg/permission_category.py` & `pulumi_frontegg-0.2.26/pulumi_frontegg/permission_category.py`

 * *Files identical despite different names*

### Comparing `pulumi_frontegg-0.2.25/pulumi_frontegg/provider.py` & `pulumi_frontegg-0.2.26/pulumi_frontegg/provider.py`

 * *Files 2% similar despite different names*

```diff
@@ -147,15 +147,17 @@
             __props__.__dict__["api_base_url"] = api_base_url
             if client_id is None and not opts.urn:
                 raise TypeError("Missing required property 'client_id'")
             __props__.__dict__["client_id"] = client_id
             __props__.__dict__["portal_base_url"] = portal_base_url
             if secret_key is None and not opts.urn:
                 raise TypeError("Missing required property 'secret_key'")
-            __props__.__dict__["secret_key"] = secret_key
+            __props__.__dict__["secret_key"] = None if secret_key is None else pulumi.Output.secret(secret_key)
+        secret_opts = pulumi.ResourceOptions(additional_secret_outputs=["secretKey"])
+        opts = pulumi.ResourceOptions.merge(opts, secret_opts)
         super(Provider, __self__).__init__(
             'frontegg',
             resource_name,
             __props__,
             opts)
 
     @property
```

### Comparing `pulumi_frontegg-0.2.25/pulumi_frontegg/role.py` & `pulumi_frontegg-0.2.26/pulumi_frontegg/role.py`

 * *Files identical despite different names*

### Comparing `pulumi_frontegg-0.2.25/pulumi_frontegg/tenant.py` & `pulumi_frontegg-0.2.26/pulumi_frontegg/tenant.py`

 * *Files identical despite different names*

### Comparing `pulumi_frontegg-0.2.25/pulumi_frontegg/user.py` & `pulumi_frontegg-0.2.26/pulumi_frontegg/user.py`

 * *Files 2% similar despite different names*

```diff
@@ -277,22 +277,24 @@
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = UserArgs.__new__(UserArgs)
 
             __props__.__dict__["automatically_verify"] = automatically_verify
             if email is None and not opts.urn:
                 raise TypeError("Missing required property 'email'")
             __props__.__dict__["email"] = email
-            __props__.__dict__["password"] = password
+            __props__.__dict__["password"] = None if password is None else pulumi.Output.secret(password)
             if role_ids is None and not opts.urn:
                 raise TypeError("Missing required property 'role_ids'")
             __props__.__dict__["role_ids"] = role_ids
             __props__.__dict__["skip_invite_email"] = skip_invite_email
             if tenant_id is None and not opts.urn:
                 raise TypeError("Missing required property 'tenant_id'")
             __props__.__dict__["tenant_id"] = tenant_id
+        secret_opts = pulumi.ResourceOptions(additional_secret_outputs=["password"])
+        opts = pulumi.ResourceOptions.merge(opts, secret_opts)
         super(User, __self__).__init__(
             'frontegg:index/user:User',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
```

### Comparing `pulumi_frontegg-0.2.25/pulumi_frontegg/webhook.py` & `pulumi_frontegg-0.2.26/pulumi_frontegg/webhook.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,29 +15,33 @@
 class WebhookArgs:
     def __init__(__self__, *,
                  description: pulumi.Input[str],
                  enabled: pulumi.Input[bool],
                  events: pulumi.Input[Sequence[pulumi.Input[str]]],
                  secret: pulumi.Input[str],
                  url: pulumi.Input[str],
+                 environment_id: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a Webhook resource.
         :param pulumi.Input[str] description: A human-readable description of the webhook.
         :param pulumi.Input[bool] enabled: Whether the webhook is enabled.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] events: The names of the events to subscribe to.
         :param pulumi.Input[str] secret: A secret to include with the event.
         :param pulumi.Input[str] url: The URL to send events to.
+        :param pulumi.Input[str] environment_id: The ID of the environment of webhook.
         :param pulumi.Input[str] name: A human-readable name for the webhook.
         """
         pulumi.set(__self__, "description", description)
         pulumi.set(__self__, "enabled", enabled)
         pulumi.set(__self__, "events", events)
         pulumi.set(__self__, "secret", secret)
         pulumi.set(__self__, "url", url)
+        if environment_id is not None:
+            pulumi.set(__self__, "environment_id", environment_id)
         if name is not None:
             pulumi.set(__self__, "name", name)
 
     @property
     @pulumi.getter
     def description(self) -> pulumi.Input[str]:
         """
@@ -94,14 +98,26 @@
         return pulumi.get(self, "url")
 
     @url.setter
     def url(self, value: pulumi.Input[str]):
         pulumi.set(self, "url", value)
 
     @property
+    @pulumi.getter(name="environmentId")
+    def environment_id(self) -> Optional[pulumi.Input[str]]:
+        """
+        The ID of the environment of webhook.
+        """
+        return pulumi.get(self, "environment_id")
+
+    @environment_id.setter
+    def environment_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "environment_id", value)
+
+    @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
         A human-readable name for the webhook.
         """
         return pulumi.get(self, "name")
 
@@ -112,48 +128,48 @@
 
 @pulumi.input_type
 class _WebhookState:
     def __init__(__self__, *,
                  created_at: Optional[pulumi.Input[str]] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  enabled: Optional[pulumi.Input[bool]] = None,
+                 environment_id: Optional[pulumi.Input[str]] = None,
                  events: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  secret: Optional[pulumi.Input[str]] = None,
-                 tenant_id: Optional[pulumi.Input[str]] = None,
                  type: Optional[pulumi.Input[str]] = None,
                  url: Optional[pulumi.Input[str]] = None,
                  vendor_id: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering Webhook resources.
         :param pulumi.Input[str] created_at: The timestamp at which the webhook was created.
         :param pulumi.Input[str] description: A human-readable description of the webhook.
         :param pulumi.Input[bool] enabled: Whether the webhook is enabled.
+        :param pulumi.Input[str] environment_id: The ID of the environment of webhook.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] events: The names of the events to subscribe to.
         :param pulumi.Input[str] name: A human-readable name for the webhook.
         :param pulumi.Input[str] secret: A secret to include with the event.
-        :param pulumi.Input[str] tenant_id: The ID of the tenant that owns the webhook.
         :param pulumi.Input[str] type: The type of the webhook.
         :param pulumi.Input[str] url: The URL to send events to.
         :param pulumi.Input[str] vendor_id: The ID of the vendor that owns the webhook.
         """
         if created_at is not None:
             pulumi.set(__self__, "created_at", created_at)
         if description is not None:
             pulumi.set(__self__, "description", description)
         if enabled is not None:
             pulumi.set(__self__, "enabled", enabled)
+        if environment_id is not None:
+            pulumi.set(__self__, "environment_id", environment_id)
         if events is not None:
             pulumi.set(__self__, "events", events)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if secret is not None:
             pulumi.set(__self__, "secret", secret)
-        if tenant_id is not None:
-            pulumi.set(__self__, "tenant_id", tenant_id)
         if type is not None:
             pulumi.set(__self__, "type", type)
         if url is not None:
             pulumi.set(__self__, "url", url)
         if vendor_id is not None:
             pulumi.set(__self__, "vendor_id", vendor_id)
 
@@ -190,14 +206,26 @@
         return pulumi.get(self, "enabled")
 
     @enabled.setter
     def enabled(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "enabled", value)
 
     @property
+    @pulumi.getter(name="environmentId")
+    def environment_id(self) -> Optional[pulumi.Input[str]]:
+        """
+        The ID of the environment of webhook.
+        """
+        return pulumi.get(self, "environment_id")
+
+    @environment_id.setter
+    def environment_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "environment_id", value)
+
+    @property
     @pulumi.getter
     def events(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
         The names of the events to subscribe to.
         """
         return pulumi.get(self, "events")
 
@@ -226,26 +254,14 @@
         return pulumi.get(self, "secret")
 
     @secret.setter
     def secret(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret", value)
 
     @property
-    @pulumi.getter(name="tenantId")
-    def tenant_id(self) -> Optional[pulumi.Input[str]]:
-        """
-        The ID of the tenant that owns the webhook.
-        """
-        return pulumi.get(self, "tenant_id")
-
-    @tenant_id.setter
-    def tenant_id(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "tenant_id", value)
-
-    @property
     @pulumi.getter
     def type(self) -> Optional[pulumi.Input[str]]:
         """
         The type of the webhook.
         """
         return pulumi.get(self, "type")
 
@@ -281,25 +297,27 @@
 class Webhook(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  enabled: Optional[pulumi.Input[bool]] = None,
+                 environment_id: Optional[pulumi.Input[str]] = None,
                  events: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  secret: Optional[pulumi.Input[str]] = None,
                  url: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Create a Webhook resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] description: A human-readable description of the webhook.
         :param pulumi.Input[bool] enabled: Whether the webhook is enabled.
+        :param pulumi.Input[str] environment_id: The ID of the environment of webhook.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] events: The names of the events to subscribe to.
         :param pulumi.Input[str] name: A human-readable name for the webhook.
         :param pulumi.Input[str] secret: A secret to include with the event.
         :param pulumi.Input[str] url: The URL to send events to.
         """
         ...
     @overload
@@ -322,14 +340,15 @@
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  enabled: Optional[pulumi.Input[bool]] = None,
+                 environment_id: Optional[pulumi.Input[str]] = None,
                  events: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  secret: Optional[pulumi.Input[str]] = None,
                  url: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
@@ -341,26 +360,26 @@
 
             if description is None and not opts.urn:
                 raise TypeError("Missing required property 'description'")
             __props__.__dict__["description"] = description
             if enabled is None and not opts.urn:
                 raise TypeError("Missing required property 'enabled'")
             __props__.__dict__["enabled"] = enabled
+            __props__.__dict__["environment_id"] = environment_id
             if events is None and not opts.urn:
                 raise TypeError("Missing required property 'events'")
             __props__.__dict__["events"] = events
             __props__.__dict__["name"] = name
             if secret is None and not opts.urn:
                 raise TypeError("Missing required property 'secret'")
             __props__.__dict__["secret"] = secret
             if url is None and not opts.urn:
                 raise TypeError("Missing required property 'url'")
             __props__.__dict__["url"] = url
             __props__.__dict__["created_at"] = None
-            __props__.__dict__["tenant_id"] = None
             __props__.__dict__["type"] = None
             __props__.__dict__["vendor_id"] = None
         super(Webhook, __self__).__init__(
             'frontegg:index/webhook:Webhook',
             resource_name,
             __props__,
             opts)
@@ -368,50 +387,50 @@
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
             created_at: Optional[pulumi.Input[str]] = None,
             description: Optional[pulumi.Input[str]] = None,
             enabled: Optional[pulumi.Input[bool]] = None,
+            environment_id: Optional[pulumi.Input[str]] = None,
             events: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
             name: Optional[pulumi.Input[str]] = None,
             secret: Optional[pulumi.Input[str]] = None,
-            tenant_id: Optional[pulumi.Input[str]] = None,
             type: Optional[pulumi.Input[str]] = None,
             url: Optional[pulumi.Input[str]] = None,
             vendor_id: Optional[pulumi.Input[str]] = None) -> 'Webhook':
         """
         Get an existing Webhook resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] created_at: The timestamp at which the webhook was created.
         :param pulumi.Input[str] description: A human-readable description of the webhook.
         :param pulumi.Input[bool] enabled: Whether the webhook is enabled.
+        :param pulumi.Input[str] environment_id: The ID of the environment of webhook.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] events: The names of the events to subscribe to.
         :param pulumi.Input[str] name: A human-readable name for the webhook.
         :param pulumi.Input[str] secret: A secret to include with the event.
-        :param pulumi.Input[str] tenant_id: The ID of the tenant that owns the webhook.
         :param pulumi.Input[str] type: The type of the webhook.
         :param pulumi.Input[str] url: The URL to send events to.
         :param pulumi.Input[str] vendor_id: The ID of the vendor that owns the webhook.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _WebhookState.__new__(_WebhookState)
 
         __props__.__dict__["created_at"] = created_at
         __props__.__dict__["description"] = description
         __props__.__dict__["enabled"] = enabled
+        __props__.__dict__["environment_id"] = environment_id
         __props__.__dict__["events"] = events
         __props__.__dict__["name"] = name
         __props__.__dict__["secret"] = secret
-        __props__.__dict__["tenant_id"] = tenant_id
         __props__.__dict__["type"] = type
         __props__.__dict__["url"] = url
         __props__.__dict__["vendor_id"] = vendor_id
         return Webhook(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter(name="createdAt")
@@ -434,14 +453,22 @@
     def enabled(self) -> pulumi.Output[bool]:
         """
         Whether the webhook is enabled.
         """
         return pulumi.get(self, "enabled")
 
     @property
+    @pulumi.getter(name="environmentId")
+    def environment_id(self) -> pulumi.Output[Optional[str]]:
+        """
+        The ID of the environment of webhook.
+        """
+        return pulumi.get(self, "environment_id")
+
+    @property
     @pulumi.getter
     def events(self) -> pulumi.Output[Sequence[str]]:
         """
         The names of the events to subscribe to.
         """
         return pulumi.get(self, "events")
 
@@ -458,22 +485,14 @@
     def secret(self) -> pulumi.Output[str]:
         """
         A secret to include with the event.
         """
         return pulumi.get(self, "secret")
 
     @property
-    @pulumi.getter(name="tenantId")
-    def tenant_id(self) -> pulumi.Output[str]:
-        """
-        The ID of the tenant that owns the webhook.
-        """
-        return pulumi.get(self, "tenant_id")
-
-    @property
     @pulumi.getter
     def type(self) -> pulumi.Output[str]:
         """
         The type of the webhook.
         """
         return pulumi.get(self, "type")
```

### Comparing `pulumi_frontegg-0.2.25/pulumi_frontegg/workspace.py` & `pulumi_frontegg-0.2.26/pulumi_frontegg/workspace.py`

 * *Files identical despite different names*

### Comparing `pulumi_frontegg-0.2.25/pulumi_frontegg.egg-info/PKG-INFO` & `pulumi_frontegg-0.2.26/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
-Name: pulumi-frontegg
-Version: 0.2.25
+Name: pulumi_frontegg
+Version: 0.2.26
 Summary: A Pulumi package for creating and managing Frontegg resources.
 Home-page: https://github.com/MaterializeInc/pulumi-frontegg
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-frontegg
 Keywords: pulumi frontegg
 Platform: UNKNOWN
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # Frontegg Pulumi Provider
 
 A [Pulumi](https://pulumi.com) provider for the [Frontegg] user management
 platform.
```

### Comparing `pulumi_frontegg-0.2.25/pulumi_frontegg.egg-info/SOURCES.txt` & `pulumi_frontegg-0.2.26/pulumi_frontegg.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 README.md
 setup.py
 pulumi_frontegg/__init__.py
 pulumi_frontegg/_inputs.py
 pulumi_frontegg/_utilities.py
+pulumi_frontegg/allowed_origin.py
 pulumi_frontegg/get_permission.py
 pulumi_frontegg/outputs.py
 pulumi_frontegg/permission.py
 pulumi_frontegg/permission_category.py
 pulumi_frontegg/provider.py
 pulumi_frontegg/pulumi-plugin.json
 pulumi_frontegg/py.typed
+pulumi_frontegg/redirect_uri.py
 pulumi_frontegg/role.py
 pulumi_frontegg/tenant.py
 pulumi_frontegg/user.py
 pulumi_frontegg/webhook.py
 pulumi_frontegg/workspace.py
 pulumi_frontegg.egg-info/PKG-INFO
 pulumi_frontegg.egg-info/SOURCES.txt
```

### Comparing `pulumi_frontegg-0.2.25/setup.py` & `pulumi_frontegg-0.2.26/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = '0.2.25'
-PLUGIN_VERSION = '0.2.25'
+VERSION = '0.2.26'
+PLUGIN_VERSION = '0.2.26'
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
-            check_call(['pulumi', 'plugin', 'install', 'resource', 'frontegg', PLUGIN_VERSION, '--server', 'https://github.com/MaterializeInc/pulumi-frontegg/releases/download/v0.2.25/'])
+            check_call(['pulumi', 'plugin', 'install', 'resource', 'frontegg', PLUGIN_VERSION, '--server', 'https://github.com/MaterializeInc/pulumi-frontegg/releases/download/v0.2.26/'])
         except OSError as error:
             if error.errno == errno.ENOENT:
                 print(f"""
                 There was an error installing the frontegg resource provider plugin.
                 It looks like `pulumi` is not installed on your system.
                 Please visit https://pulumi.com/ to install the Pulumi CLI.
                 You may try manually installing the plugin by running
@@ -34,14 +34,15 @@
         with open('README.md', encoding='utf-8') as f:
             return f.read()
     except FileNotFoundError:
         return "frontegg Pulumi Package - Development Version"
 
 
 setup(name='pulumi_frontegg',
+      python_requires='>=3.7',
       version=VERSION,
       description="A Pulumi package for creating and managing Frontegg resources.",
       long_description=readme(),
       long_description_content_type='text/markdown',
       cmdclass={
           'install': InstallPluginCommand,
       },
```

