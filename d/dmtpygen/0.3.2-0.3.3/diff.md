# Comparing `tmp/dmtpygen-0.3.2.tar.gz` & `tmp/dmtpygen-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dmtpygen-0.3.2.tar", last modified: Mon Nov 14 11:28:36 2022, max compression
+gzip compressed data, was "dmtpygen-0.3.3.tar", last modified: Thu Jun 15 13:45:00 2023, max compression
```

## Comparing `dmtpygen-0.3.2.tar` & `dmtpygen-0.3.3.tar`

### file list

```diff
@@ -1,42 +1,43 @@
-drwxrwxrwx   0        0        0        0 2022-11-14 11:28:36.199993 dmtpygen-0.3.2/
--rw-rw-rw-   0        0        0      523 2022-11-14 11:28:36.198992 dmtpygen-0.3.2/PKG-INFO
--rw-rw-rw-   0        0        0       82 2021-10-22 10:16:42.000000 dmtpygen-0.3.2/README.md
--rw-rw-rw-   0        0        0       42 2022-11-14 11:28:36.199993 dmtpygen-0.3.2/setup.cfg
--rw-rw-rw-   0        0        0     1148 2022-11-14 11:28:12.000000 dmtpygen-0.3.2/setup.py
-drwxrwxrwx   0        0        0        0 2022-11-14 11:28:36.072995 dmtpygen-0.3.2/src/
-drwxrwxrwx   0        0        0        0 2022-11-14 11:28:36.082992 dmtpygen-0.3.2/src/dmtpygen/
--rw-rw-rw-   0        0        0        0 2022-02-22 08:02:43.000000 dmtpygen-0.3.2/src/dmtpygen/__init__.py
--rw-rw-rw-   0        0        0      745 2022-10-19 05:33:40.000000 dmtpygen-0.3.2/src/dmtpygen/generator.py
-drwxrwxrwx   0        0        0        0 2022-11-14 11:28:36.121993 dmtpygen-0.3.2/src/dmtpygen/generators/
--rw-rw-rw-   0        0        0      295 2022-02-22 08:02:43.000000 dmtpygen-0.3.2/src/dmtpygen/generators/__init__.py
--rw-rw-rw-   0        0        0     5825 2022-10-19 05:34:41.000000 dmtpygen-0.3.2/src/dmtpygen/generators/blueprint_generator.py
--rw-rw-rw-   0        0        0     1712 2022-10-19 05:34:48.000000 dmtpygen-0.3.2/src/dmtpygen/generators/entity_generator.py
--rw-rw-rw-   0        0        0     9367 2022-11-14 11:27:46.000000 dmtpygen-0.3.2/src/dmtpygen/generators/entity_model.py
--rw-rw-rw-   0        0        0     2131 2022-10-19 05:35:03.000000 dmtpygen-0.3.2/src/dmtpygen/generators/enum_generator.py
--rw-rw-rw-   0        0        0     2441 2022-10-19 05:35:13.000000 dmtpygen-0.3.2/src/dmtpygen/generators/init_generator.py
--rw-rw-rw-   0        0        0     1257 2022-10-19 05:34:20.000000 dmtpygen-0.3.2/src/dmtpygen/generators/package_info_generator.py
--rw-rw-rw-   0        0        0     2034 2022-10-19 07:38:43.000000 dmtpygen-0.3.2/src/dmtpygen/generators/runtime_generator.py
--rw-rw-rw-   0        0        0      660 2022-10-19 05:35:49.000000 dmtpygen-0.3.2/src/dmtpygen/generators/setup_generator.py
-drwxrwxrwx   0        0        0        0 2022-11-14 11:28:36.162992 dmtpygen-0.3.2/src/dmtpygen/templates/
--rw-rw-rw-   0        0        0      358 2022-02-22 08:02:43.000000 dmtpygen-0.3.2/src/dmtpygen/templates/Dockerfile.jinja
--rw-rw-rw-   0        0        0       64 2022-02-22 08:02:43.000000 dmtpygen-0.3.2/src/dmtpygen/templates/README.md
--rw-rw-rw-   0        0        0      109 2022-02-22 08:02:43.000000 dmtpygen-0.3.2/src/dmtpygen/templates/docker-compose.yml..jinja
--rw-rw-rw-   0        0        0      244 2022-02-22 08:02:43.000000 dmtpygen-0.3.2/src/dmtpygen/templates/publish.sh
--rw-rw-rw-   0        0        0       63 2022-02-22 08:02:43.000000 dmtpygen-0.3.2/src/dmtpygen/templates/requirements-dev.txt
--rw-rw-rw-   0        0        0        5 2022-02-22 08:02:43.000000 dmtpygen-0.3.2/src/dmtpygen/templates/requirements.txt
--rw-rw-rw-   0        0        0     1015 2022-02-22 08:02:43.000000 dmtpygen-0.3.2/src/dmtpygen/templates/setup.py.jinja
-drwxrwxrwx   0        0        0        0 2022-11-14 11:28:36.195993 dmtpygen-0.3.2/src/dmtpygen/templates/src/
--rw-rw-rw-   0        0        0        0 2022-02-22 08:02:43.000000 dmtpygen-0.3.2/src/dmtpygen/templates/src/__init__.py
--rw-rw-rw-   0        0        0       88 2022-02-22 08:02:43.000000 dmtpygen-0.3.2/src/dmtpygen/templates/src/__init__.py.jinja
--rw-rw-rw-   0        0        0     1609 2022-10-19 06:34:37.000000 dmtpygen-0.3.2/src/dmtpygen/templates/src/blueprint.py.jinja
--rw-rw-rw-   0        0        0     2405 2022-09-30 10:47:16.000000 dmtpygen-0.3.2/src/dmtpygen/templates/src/entity.py.jinja
--rw-rw-rw-   0        0        0      398 2022-02-22 08:02:43.000000 dmtpygen-0.3.2/src/dmtpygen/templates/src/enum.py.jinja
--rw-rw-rw-   0        0        0       26 2022-02-22 08:02:43.000000 dmtpygen-0.3.2/src/dmtpygen/templates/src/package_info.py.jinja
-drwxrwxrwx   0        0        0        0 2022-11-14 11:28:36.196992 dmtpygen-0.3.2/src/dmtpygen/templates/tests/
--rw-rw-rw-   0        0        0        0 2022-02-22 08:02:43.000000 dmtpygen-0.3.2/src/dmtpygen/templates/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-14 11:28:36.106990 dmtpygen-0.3.2/src/dmtpygen.egg-info/
--rw-rw-rw-   0        0        0      523 2022-11-14 11:28:35.000000 dmtpygen-0.3.2/src/dmtpygen.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1219 2022-11-14 11:28:36.000000 dmtpygen-0.3.2/src/dmtpygen.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-14 11:28:35.000000 dmtpygen-0.3.2/src/dmtpygen.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2022-11-14 11:28:35.000000 dmtpygen-0.3.2/src/dmtpygen.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2022-11-14 11:28:35.000000 dmtpygen-0.3.2/src/dmtpygen.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-15 13:45:00.729077 dmtpygen-0.3.3/
+-rw-rw-rw-   0        0        0     1093 2022-03-22 09:36:53.000000 dmtpygen-0.3.3/LICENSE
+-rw-rw-rw-   0        0        0      523 2023-06-15 13:45:00.727082 dmtpygen-0.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0       82 2021-10-22 10:16:42.000000 dmtpygen-0.3.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-15 13:45:00.731076 dmtpygen-0.3.3/setup.cfg
+-rw-rw-rw-   0        0        0     1148 2023-06-15 13:44:22.000000 dmtpygen-0.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 13:45:00.585075 dmtpygen-0.3.3/src/
+drwxrwxrwx   0        0        0        0 2023-06-15 13:45:00.601077 dmtpygen-0.3.3/src/dmtpygen/
+-rw-rw-rw-   0        0        0        0 2022-02-22 08:02:43.000000 dmtpygen-0.3.3/src/dmtpygen/__init__.py
+-rw-rw-rw-   0        0        0      745 2023-04-27 11:30:41.000000 dmtpygen-0.3.3/src/dmtpygen/generator.py
+drwxrwxrwx   0        0        0        0 2023-06-15 13:45:00.670075 dmtpygen-0.3.3/src/dmtpygen/generators/
+-rw-rw-rw-   0        0        0      295 2022-02-22 08:02:43.000000 dmtpygen-0.3.3/src/dmtpygen/generators/__init__.py
+-rw-rw-rw-   0        0        0     7091 2023-06-13 12:10:31.000000 dmtpygen-0.3.3/src/dmtpygen/generators/blueprint_generator.py
+-rw-rw-rw-   0        0        0     1712 2022-10-19 05:34:48.000000 dmtpygen-0.3.3/src/dmtpygen/generators/entity_generator.py
+-rw-rw-rw-   0        0        0    10211 2023-06-13 12:10:31.000000 dmtpygen-0.3.3/src/dmtpygen/generators/entity_model.py
+-rw-rw-rw-   0        0        0     2131 2022-10-19 05:35:03.000000 dmtpygen-0.3.3/src/dmtpygen/generators/enum_generator.py
+-rw-rw-rw-   0        0        0     2441 2022-10-19 05:35:13.000000 dmtpygen-0.3.3/src/dmtpygen/generators/init_generator.py
+-rw-rw-rw-   0        0        0     1257 2022-10-19 05:34:20.000000 dmtpygen-0.3.3/src/dmtpygen/generators/package_info_generator.py
+-rw-rw-rw-   0        0        0     2034 2022-10-19 07:38:43.000000 dmtpygen-0.3.3/src/dmtpygen/generators/runtime_generator.py
+-rw-rw-rw-   0        0        0      660 2022-10-19 05:35:49.000000 dmtpygen-0.3.3/src/dmtpygen/generators/setup_generator.py
+drwxrwxrwx   0        0        0        0 2023-06-15 13:45:00.696077 dmtpygen-0.3.3/src/dmtpygen/templates/
+-rw-rw-rw-   0        0        0      358 2022-02-22 08:02:43.000000 dmtpygen-0.3.3/src/dmtpygen/templates/Dockerfile.jinja
+-rw-rw-rw-   0        0        0       64 2022-02-22 08:02:43.000000 dmtpygen-0.3.3/src/dmtpygen/templates/README.md
+-rw-rw-rw-   0        0        0      109 2022-02-22 08:02:43.000000 dmtpygen-0.3.3/src/dmtpygen/templates/docker-compose.yml..jinja
+-rw-rw-rw-   0        0        0      244 2022-02-22 08:02:43.000000 dmtpygen-0.3.3/src/dmtpygen/templates/publish.sh
+-rw-rw-rw-   0        0        0       63 2023-03-01 11:39:52.000000 dmtpygen-0.3.3/src/dmtpygen/templates/requirements-dev.txt
+-rw-rw-rw-   0        0        0        5 2022-02-22 08:02:43.000000 dmtpygen-0.3.3/src/dmtpygen/templates/requirements.txt
+-rw-rw-rw-   0        0        0     1015 2022-02-22 08:02:43.000000 dmtpygen-0.3.3/src/dmtpygen/templates/setup.py.jinja
+drwxrwxrwx   0        0        0        0 2023-06-15 13:45:00.720079 dmtpygen-0.3.3/src/dmtpygen/templates/src/
+-rw-rw-rw-   0        0        0        0 2022-02-22 08:02:43.000000 dmtpygen-0.3.3/src/dmtpygen/templates/src/__init__.py
+-rw-rw-rw-   0        0        0       88 2022-02-22 08:02:43.000000 dmtpygen-0.3.3/src/dmtpygen/templates/src/__init__.py.jinja
+-rw-rw-rw-   0        0        0     1609 2022-10-19 06:34:37.000000 dmtpygen-0.3.3/src/dmtpygen/templates/src/blueprint.py.jinja
+-rw-rw-rw-   0        0        0     2635 2023-06-03 07:51:26.000000 dmtpygen-0.3.3/src/dmtpygen/templates/src/entity.py.jinja
+-rw-rw-rw-   0        0        0      398 2022-02-22 08:02:43.000000 dmtpygen-0.3.3/src/dmtpygen/templates/src/enum.py.jinja
+-rw-rw-rw-   0        0        0       26 2022-02-22 08:02:43.000000 dmtpygen-0.3.3/src/dmtpygen/templates/src/package_info.py.jinja
+drwxrwxrwx   0        0        0        0 2023-06-15 13:45:00.723081 dmtpygen-0.3.3/src/dmtpygen/templates/tests/
+-rw-rw-rw-   0        0        0        0 2022-02-22 08:02:43.000000 dmtpygen-0.3.3/src/dmtpygen/templates/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-15 13:45:00.636074 dmtpygen-0.3.3/src/dmtpygen.egg-info/
+-rw-rw-rw-   0        0        0      523 2023-06-15 13:45:00.000000 dmtpygen-0.3.3/src/dmtpygen.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1227 2023-06-15 13:45:00.000000 dmtpygen-0.3.3/src/dmtpygen.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 13:45:00.000000 dmtpygen-0.3.3/src/dmtpygen.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2023-06-15 13:45:00.000000 dmtpygen-0.3.3/src/dmtpygen.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-15 13:45:00.000000 dmtpygen-0.3.3/src/dmtpygen.egg-info/top_level.txt
```

### Comparing `dmtpygen-0.3.2/PKG-INFO` & `dmtpygen-0.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dmtpygen
-Version: 0.3.2
+Version: 0.3.3
 Summary: Python generator for SIMOS based DMT models
 Home-page: UNKNOWN
 Author: SINTEF Ocean
 License: UNKNOWN
 Description: # Python runtime generators
```

### Comparing `dmtpygen-0.3.2/setup.py` & `dmtpygen-0.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 long_description = (here / 'README.md').read_text(encoding='utf-8')
 
 with open('requirements.txt',encoding='utf8') as f:
     required = f.read().splitlines()
 
 setup(
     name='dmtpygen',
-    version='0.3.2',
+    version='0.3.3',
     author="SINTEF Ocean",
     description="Python generator for SIMOS based DMT models",
     long_description=long_description,
     long_description_content_type="text/markdown",
     package_dir={"": "src"},
     packages= find_packages(where="src"),
     package_data={'dmtpygen':  ['templates/*','templates/src/*','templates/tests/*']},
```

### Comparing `dmtpygen-0.3.2/src/dmtpygen/generator.py` & `dmtpygen-0.3.3/src/dmtpygen/generator.py`

 * *Files identical despite different names*

### Comparing `dmtpygen-0.3.2/src/dmtpygen/generators/blueprint_generator.py` & `dmtpygen-0.3.3/src/dmtpygen/generators/blueprint_generator.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """blueprint generator"""
 import codecs
+import os
 from pathlib import Path
 from typing import Dict, Sequence
 from collections import OrderedDict
 from jinja2.environment import Template
 from dmtgen.common.package import Blueprint
 from dmtgen.package_generator import PackageGenerator
 from dmtgen import TemplateBasedGenerator
@@ -84,16 +85,24 @@
                 default = find_default_value(attribute)
                 if default is not None:
                     named_args.append(f"default={default}")
             else:
                 a_dict["contained"]=attribute.contained
                 a_dict["constructor"]="BlueprintAttribute"
                 atype = a_dict["attributeType"]
+                idx = atype.find(":")
+                if idx > 0:
+                    alias = atype[:idx]
+                    adress = package.get_root().aliases[alias]
+                    atype = adress + "/" + atype[idx+1:]
+
                 if not atype.startswith("system/SIMOS"):
                     a_dict["attributeType"]=root_name+atype
+                else:
+                    a_dict["attributeType"]=atype
 
             if len(named_args) > 0:
                 a_dict["named_args"] = ",".join(named_args)
 
             a_dicts.append(a_dict)
 
         model["attributes"] = a_dicts
@@ -117,24 +126,45 @@
             return ",".join(types)
         return "Blueprint"
 
     def __to__imports(self,package: Package, blueprints: Sequence[Blueprint]) -> Sequence[str]:
         imports = []
         for blueprint in blueprints:
             import_package: Package = blueprint.get_parent()
-            paths=import_package.get_paths()
             if import_package != package:
-                bp_path = ".".join(paths) + ".blueprints." + blueprint.name.lower()
-                if bp_path.startswith("system.SIMOS"):
+                relative_path =self._to_relative_import_path(package, blueprint)
+                if relative_path.startswith("system.SIMOS"):
                     bp_path = "dmt.blueprints."+ blueprint.name.lower()
+                else:
+                    bp_path = "." + relative_path + ".blueprints." + blueprint.name.lower()
+
             else:
                 bp_path = "." + blueprint.name.lower()
 
             bp_name = self.__to_type_string(blueprint)
             imports.append(f"from {bp_path} import {bp_name}")
         return imports
 
     def __find_super_classes(self, bp: Blueprint) -> Sequence[Blueprint]:
         base_classes: OrderedDict[Blueprint] = OrderedDict()
         for extension in bp.extensions:
-                base_classes[extension.name]=extension
+            base_classes[extension.name]=extension
         return base_classes.values()
+
+    def _to_relative_import_path(self, pkg: Package, blueprint: Blueprint) -> str:
+        import_package = blueprint.get_parent()
+        name = blueprint.name.lower()
+        if pkg == import_package:
+            return "."+name
+        current_dir = pkg.package_dir
+        import_dir = import_package.package_dir
+        import_module = import_package.package_dir / name
+        # Get me the relative path from current_dir to import_dir
+        root_dir = pkg.get_root().package_dir
+        if import_module.is_relative_to(root_dir) and current_dir.is_relative_to(root_dir):
+            # Find the relative path from current_dir to import_dir
+            relative = os.path.relpath(import_dir, current_dir)
+            ret = "".join(Path(relative).parts)
+            return ret
+
+        paths = import_package.get_paths()
+        return ".".join(paths)
```

### Comparing `dmtpygen-0.3.2/src/dmtpygen/generators/entity_generator.py` & `dmtpygen-0.3.3/src/dmtpygen/generators/entity_generator.py`

 * *Files identical despite different names*

### Comparing `dmtpygen-0.3.2/src/dmtpygen/generators/entity_model.py` & `dmtpygen-0.3.3/src/dmtpygen/generators/entity_model.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import keyword
 from collections import OrderedDict
+import os
+from pathlib import Path
 from typing import Dict, Sequence, Set
 
 from dmtgen.common.blueprint_attribute import BlueprintAttribute
 from dmtgen.common.package import Blueprint, Package
 
 types = {"number": "float", "double": "float", "string": "str", "char": "str",
          "integer": "int", "short": "int", "boolean": "bool"}
@@ -62,17 +64,17 @@
             for attribute  in import_type.all_attributes.values():
                 if not attribute.is_primitive and not attribute.is_enum:
                     imp_bp = pkg.get_blueprint(attribute.type)
                     if blueprint == imp_bp:
                         cross_references[import_type.name] = import_type
                         import_types.remove(import_type)
 
-    model["imports"] = __to__imports(import_types)
+    model["imports"] = __to__imports(pkg,import_types)
     model["has_cross_references"] = len(cross_references) > 0
-    model["cross_references"] = __to__import_infos(cross_references.values())
+    model["cross_references"] = __to__import_infos(pkg,cross_references.values())
     model["has_array"] = has_array
     model["needs_numpy"] = needs_numpy
     model["fields"] = fields
     model["arguments"]=__create_named_arguments(fields)
     return model
 
 def __first_to_upper(string):
@@ -92,46 +94,49 @@
     a_type: str = attribute.get("attributeType")
     if a_type not in types:
         blueprint = package.get_blueprint(a_type)
         if attribute.contained:
             imports[a_type]=blueprint
         else:
             cross_references[a_type]=blueprint
-        return __create_blueprint_field(field, blueprint, is_array, attribute)
+        return __create_blueprint_field(field, blueprint, is_array)
 
     enum_type = attribute.get("enumType",None)
     if enum_type:
         return __create_enum_field(field,attribute,package,enum_type, imports)
 
     ftype = __map_type(a_type)
     field["is_entity"] = False
     field["type"] = ftype
+    field["type_description"] = ftype
 
     if is_array:
         dims=dimension.split(",")
-        ndims = len(dims)
-        # Multidimensional array
         field["type"] = "ndarray"
-        field["init"] = f"ndarray({ndims})"
-        field["setter"] = f"ndarray({ndims})"
+        field["type_description"] = "ndarray of " + ftype
+        field["ftype"] = ftype
+        field["init"] = "[]"
+        field["setter"] = f"asarray(value, dtype={ftype})"
+        field["ndim"] = len(dims)
+
     else:
         field["setter"] = __map(ftype, setters)
         field["default"] = __find_default_value(attribute, ftype)
         field["init"] = field["default"]
 
     return field
 
 def __rename_if_reserved(name):
     if keyword.iskeyword(name):
         return name + "_"
     return name
 
 
 
-def __create_blueprint_field(field, blueprint: Blueprint, is_array, attribute: BlueprintAttribute) -> Dict:
+def __create_blueprint_field(field, blueprint: Blueprint, is_array) -> Dict:
     field["is_entity"] = True
     import_package: Package = blueprint.get_parent()
     paths=import_package.get_paths()
     bp_path = ".".join(paths) + "." + blueprint.name.lower()
     field["module"] = bp_path
     if is_array:
         field["type"] = "List["+blueprint.name+"]"
@@ -192,44 +197,61 @@
         else:
             return "'" + default_value + "'"
     return default_value
 
 def __to_type_string(string: str) -> str:
     return string[:1].upper() + string[1:]
 
-def __to__imports(blueprints: Set[Blueprint]) -> Sequence[str]:
-    imports = __to__import_infos(blueprints)
+def __to__imports(pkg: Package,  blueprints: Set[Blueprint]) -> Sequence[str]:
+    imports = __to__import_infos(pkg, blueprints)
     statements = [__to_import_statement(x) for x in imports]
     statements.sort()
     return statements
 
 def __to_import_statement(import_info: Dict) -> str:
     module=import_info["module"]
     name=import_info["name"]
     return f"from {module} import {name}"
 
 
-def __to__import_infos(blueprints: Set[Blueprint]) -> Sequence[Dict]:
+def __to__import_infos(pkg: Package,blueprints: Set[Blueprint]) -> Sequence[Dict]:
     imports = []
     for blueprint in blueprints:
-        import_package: Package = blueprint.get_parent()
-        paths=import_package.get_paths()
+        bp_path=_to_relative_import_path(pkg,blueprint)
         name = blueprint.name
-        bp_path = ".".join(paths) + "." + name.lower()
         if bp_path.startswith("system.SIMOS"):
             bp_path = "dmt."+ name.lower()
         bp_name = __to_type_string(name)
         import_info = {
             "module": bp_path,
             "name": bp_name
         }
         imports.append(import_info)
 
     return imports
 
+def _to_relative_import_path(pkg: Package, blueprint: Blueprint) -> str:
+    import_package = blueprint.get_parent()
+    name = blueprint.name.lower()
+    if pkg == import_package:
+        return "."+name
+    current_dir = pkg.package_dir
+    import_dir = import_package.package_dir
+    import_module = import_package.package_dir / name
+    # Get me the relative path from current_dir to import_dir
+    root_dir = pkg.get_root().package_dir
+    if import_module.is_relative_to(root_dir) and current_dir.is_relative_to(root_dir):
+        # Find the relative path from current_dir to import_dir
+        relative = os.path.relpath(import_dir, current_dir)
+        ret = "".join(Path(relative).parts)
+        return ret
+
+    paths = import_package.get_paths()
+    return ".".join(paths)
+
 def __refers_to(blueprint: Blueprint, imports: Dict) -> bool:
     return blueprint in imports.values()
 
 def __create_named_arguments(fields: Sequence[Dict]) -> str:
     args = []
     for field in fields:
         if not field["is_entity"] and not field["is_array"]:
```

### Comparing `dmtpygen-0.3.2/src/dmtpygen/generators/enum_generator.py` & `dmtpygen-0.3.3/src/dmtpygen/generators/enum_generator.py`

 * *Files identical despite different names*

### Comparing `dmtpygen-0.3.2/src/dmtpygen/generators/init_generator.py` & `dmtpygen-0.3.3/src/dmtpygen/generators/init_generator.py`

 * *Files identical despite different names*

### Comparing `dmtpygen-0.3.2/src/dmtpygen/generators/package_info_generator.py` & `dmtpygen-0.3.3/src/dmtpygen/generators/package_info_generator.py`

 * *Files identical despite different names*

### Comparing `dmtpygen-0.3.2/src/dmtpygen/generators/runtime_generator.py` & `dmtpygen-0.3.3/src/dmtpygen/generators/runtime_generator.py`

 * *Files identical despite different names*

### Comparing `dmtpygen-0.3.2/src/dmtpygen/generators/setup_generator.py` & `dmtpygen-0.3.3/src/dmtpygen/generators/setup_generator.py`

 * *Files identical despite different names*

### Comparing `dmtpygen-0.3.2/src/dmtpygen/templates/setup.py.jinja` & `dmtpygen-0.3.3/src/dmtpygen/templates/setup.py.jinja`

 * *Files identical despite different names*

### Comparing `dmtpygen-0.3.2/src/dmtpygen/templates/src/blueprint.py.jinja` & `dmtpygen-0.3.3/src/dmtpygen/templates/src/blueprint.py.jinja`

 * *Files identical despite different names*

### Comparing `dmtpygen-0.3.2/src/dmtpygen/templates/src/entity.py.jinja` & `dmtpygen-0.3.3/src/dmtpygen/templates/src/entity.py.jinja`

 * *Files 11% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     """
 {%-if description %}
     {{description}}
 {%-endif %}
     Keyword arguments
     -----------------
     {%-for field in fields %}
-    {{ field.name }} : {{ field.type }}
+    {{ field.name }} : {{ field.get("type_description",field.get("type")) }}
 {%-if field.description or "default" in field %}
          {{ field.description | escape_string }} {%- if "default" in field %}(default {{ field["default"] }}){%- endif %}
 {%-endif %}
     {%-endfor %}
     """
 
     def __init__(self {{ arguments }}, **kwargs):
@@ -62,17 +62,20 @@
 
     @{{ field.name }}.setter
     def {{ field.name }}(self, value: {{ field.type }}):
         """Set {{field.name}}"""
         {%- if field.is_array %}
             {%- if field.is_entity %}
         if not isinstance(value, Sequence):
-            raise Exception("Expected sequense, but was " , type(value))
+            raise ValueError("Expected sequense, but was " , type(value))
         self.__{{ field.name }} = value
             {%- else %}
-        self.__{{ field.name }} = asarray(value)
+        array = asarray(value, dtype={{ field.ftype }})
+        if len(array) > 0 and array.ndim != {{ field.ndim }}:
+            raise ValueError("Expected array with {{ field.ndim }} dimensions")
+        self.__{{ field.name }} = array
             {%- endif %}
         {%- else %}
         self.__{{ field.name }} = {{ field.setter }}
         {%- endif %}
     {%- endif %}
 {% endfor %}
```

### Comparing `dmtpygen-0.3.2/src/dmtpygen.egg-info/PKG-INFO` & `dmtpygen-0.3.3/src/dmtpygen.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dmtpygen
-Version: 0.3.2
+Version: 0.3.3
 Summary: Python generator for SIMOS based DMT models
 Home-page: UNKNOWN
 Author: SINTEF Ocean
 License: UNKNOWN
 Description: # Python runtime generators
```

### Comparing `dmtpygen-0.3.2/src/dmtpygen.egg-info/SOURCES.txt` & `dmtpygen-0.3.3/src/dmtpygen.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.py
 src/dmtpygen/__init__.py
 src/dmtpygen/generator.py
 src/dmtpygen.egg-info/PKG-INFO
 src/dmtpygen.egg-info/SOURCES.txt
 src/dmtpygen.egg-info/dependency_links.txt
```

