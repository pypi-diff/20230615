# Comparing `tmp/toml_to_requirements-0.1.0-py2.py3-none-any.whl.zip` & `tmp/toml_to_requirements-0.2.0-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 2423 bytes, number of entries: 6
--rw-r--r--  2.0 unx     1022 b- defN 23-Apr-05 20:19 toml_to_requirements/main.py
--rw-r--r--  2.0 unx     1043 b- defN 23-Apr-05 20:22 toml_to_requirements-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Apr-05 20:22 toml_to_requirements-0.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       63 b- defN 23-Apr-05 20:22 toml_to_requirements-0.1.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       21 b- defN 23-Apr-05 20:22 toml_to_requirements-0.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      544 b- defN 23-Apr-05 20:22 toml_to_requirements-0.1.0.dist-info/RECORD
-6 files, 2803 bytes uncompressed, 1423 bytes compressed:  49.2%
+Zip file size: 2613 bytes, number of entries: 6
+-rw-r--r--  2.0 unx     1451 b- defN 23-Jun-15 13:00 toml_to_requirements/main.py
+-rw-r--r--  2.0 unx     1251 b- defN 23-Jun-15 13:05 toml_to_requirements-0.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Jun-15 13:05 toml_to_requirements-0.2.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       63 b- defN 23-Jun-15 13:05 toml_to_requirements-0.2.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       21 b- defN 23-Jun-15 13:05 toml_to_requirements-0.2.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      544 b- defN 23-Jun-15 13:05 toml_to_requirements-0.2.0.dist-info/RECORD
+6 files, 3440 bytes uncompressed, 1613 bytes compressed:  53.1%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: toml_to_requirements/main.py
 Comment: 
 
-Filename: toml_to_requirements-0.1.0.dist-info/METADATA
+Filename: toml_to_requirements-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: toml_to_requirements-0.1.0.dist-info/WHEEL
+Filename: toml_to_requirements-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: toml_to_requirements-0.1.0.dist-info/entry_points.txt
+Filename: toml_to_requirements-0.2.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: toml_to_requirements-0.1.0.dist-info/top_level.txt
+Filename: toml_to_requirements-0.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: toml_to_requirements-0.1.0.dist-info/RECORD
+Filename: toml_to_requirements-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## toml_to_requirements/main.py

```diff
@@ -5,14 +5,17 @@
 import argparse
 
 
 def main():
     argparser = argparse.ArgumentParser()
     argparser.add_argument("--toml-file", type=str, default="pyproject.toml")
     argparser.add_argument("--include-optional", action="store_true")
+    argparser.add_argument(
+        "-o", "--optional-lists", help="Optional dependency lists to include."
+    )
 
     args = argparser.parse_args()
 
     data = toml.load(args.toml_file)
 
     project = data.get("project")
 
@@ -20,16 +23,25 @@
         print("project section is missing from the toml file. Exiting...")
         sys.exit(1)
 
     dependencies = set(project.get("dependencies", []))
 
     if args.include_optional:
         optional_dependency_list = project.get("optional-dependencies", [])
+        optional_lists_to_include = (
+            None if args.optional_lists is None else str(args.optional_lists).split(",")
+        )
 
         for optional_list in optional_dependency_list:
+            if (
+                optional_lists_to_include is not None
+                and optional_list not in optional_lists_to_include
+            ):
+                continue
+
             optional_dependencies = optional_dependency_list[optional_list]
             dependencies.update(optional_dependencies)
 
     requirements_content = "\n".join(sorted(dependencies))
 
     with open("requirements.txt", "w") as f:
         f.write(requirements_content)
```

## Comparing `toml_to_requirements-0.1.0.dist-info/METADATA` & `toml_to_requirements-0.2.0.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: toml-to-requirements
-Version: 0.1.0
+Version: 0.2.0
 Summary: Convert a pyproject.toml file to a requirements.txt file
 Author-email: Jake Cyr <cyrjake@gmail.com>
 License: MIT
 Keywords: toml,requirements,converter,parser
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: toml
+Provides-Extra: dev
+Requires-Dist: black ; extra == 'dev'
 
 # TOML to Requirements
 
 Simple script to convert a pyproject.toml file to a requirements.txt file.
 
 Does not support poetry projects! They have their own converter tools.
 
@@ -35,7 +37,13 @@
 ```
 
 To include optional dependencies, include the `--include-optional` flag in the above command:
 
 ```bash
 toml-to-req --toml-file pyproject.toml --include-optional
 ```
+
+The optional lists to include can also be specified
+
+```bash
+toml-to-req --toml-file pyproject.toml --include-optional --optional-lists dev,test
+```
```

