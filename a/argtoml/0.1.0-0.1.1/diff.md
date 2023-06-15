# Comparing `tmp/argtoml-0.1.0.tar.gz` & `tmp/argtoml-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "argtoml-0.1.0.tar", last modified: Sat Jun 10 10:41:36 2023, max compression
+gzip compressed data, was "argtoml-0.1.1.tar", last modified: Thu Jun 15 19:37:43 2023, max compression
```

## Comparing `argtoml-0.1.0.tar` & `argtoml-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 gum       (1000) gum       (1000)        0 2023-06-10 10:41:36.147520 argtoml-0.1.0/
--rw-r--r--   0 gum       (1000) gum       (1000)     1069 2023-06-10 10:02:47.000000 argtoml-0.1.0/LICENSE
--rw-r--r--   0 gum       (1000) gum       (1000)     2052 2023-06-10 10:41:36.147520 argtoml-0.1.0/PKG-INFO
--rw-r--r--   0 gum       (1000) gum       (1000)     1522 2023-06-07 09:20:09.000000 argtoml-0.1.0/README.md
-drwxr-xr-x   0 gum       (1000) gum       (1000)        0 2023-06-10 10:41:36.140853 argtoml-0.1.0/argtoml/
--rw-r--r--   0 gum       (1000) gum       (1000)       92 2023-06-05 13:46:56.000000 argtoml-0.1.0/argtoml/__init__.py
--rw-r--r--   0 gum       (1000) gum       (1000)     5553 2023-06-09 12:30:22.000000 argtoml-0.1.0/argtoml/main.py
-drwxr-xr-x   0 gum       (1000) gum       (1000)        0 2023-06-10 10:41:36.144186 argtoml-0.1.0/argtoml/tests/
--rw-r--r--   0 gum       (1000) gum       (1000)       25 2023-06-09 12:19:14.000000 argtoml-0.1.0/argtoml/tests/__init__.py
--rw-r--r--   0 gum       (1000) gum       (1000)      245 2023-06-09 14:34:41.000000 argtoml-0.1.0/argtoml/tests/test_main.py
-drwxr-xr-x   0 gum       (1000) gum       (1000)        0 2023-06-10 10:41:36.144186 argtoml-0.1.0/argtoml.egg-info/
--rw-r--r--   0 gum       (1000) gum       (1000)     2052 2023-06-10 10:41:36.000000 argtoml-0.1.0/argtoml.egg-info/PKG-INFO
--rw-r--r--   0 gum       (1000) gum       (1000)      273 2023-06-10 10:41:36.000000 argtoml-0.1.0/argtoml.egg-info/SOURCES.txt
--rw-r--r--   0 gum       (1000) gum       (1000)        1 2023-06-10 10:41:36.000000 argtoml-0.1.0/argtoml.egg-info/dependency_links.txt
--rw-r--r--   0 gum       (1000) gum       (1000)        8 2023-06-10 10:41:36.000000 argtoml-0.1.0/argtoml.egg-info/top_level.txt
--rw-r--r--   0 gum       (1000) gum       (1000)      939 2023-06-10 10:41:24.000000 argtoml-0.1.0/pyproject.toml
--rw-r--r--   0 gum       (1000) gum       (1000)       38 2023-06-10 10:41:36.147520 argtoml-0.1.0/setup.cfg
--rw-r--r--   0 gum       (1000) gum       (1000)       61 2023-06-07 07:31:31.000000 argtoml-0.1.0/setup.py
-drwxr-xr-x   0 gum       (1000) gum       (1000)        0 2023-06-10 10:41:36.147520 argtoml-0.1.0/tests/
--rw-r--r--   0 gum       (1000) gum       (1000)      245 2023-06-09 14:34:41.000000 argtoml-0.1.0/tests/test_main.py
+drwxr-xr-x   0 gum       (1000) gum       (1000)        0 2023-06-15 19:37:43.578075 argtoml-0.1.1/
+-rw-r--r--   0 gum       (1000) gum       (1000)     1069 2023-06-10 10:02:47.000000 argtoml-0.1.1/LICENSE
+-rw-r--r--   0 gum       (1000) gum       (1000)     2052 2023-06-15 19:37:43.578075 argtoml-0.1.1/PKG-INFO
+-rw-r--r--   0 gum       (1000) gum       (1000)     1522 2023-06-07 09:20:09.000000 argtoml-0.1.1/README.md
+drwxr-xr-x   0 gum       (1000) gum       (1000)        0 2023-06-15 19:37:43.571408 argtoml-0.1.1/argtoml/
+-rw-r--r--   0 gum       (1000) gum       (1000)       92 2023-06-05 13:46:56.000000 argtoml-0.1.1/argtoml/__init__.py
+-rw-r--r--   0 gum       (1000) gum       (1000)     6630 2023-06-15 19:35:31.000000 argtoml-0.1.1/argtoml/main.py
+drwxr-xr-x   0 gum       (1000) gum       (1000)        0 2023-06-15 19:37:43.574742 argtoml-0.1.1/argtoml/tests/
+-rw-r--r--   0 gum       (1000) gum       (1000)       25 2023-06-09 12:19:14.000000 argtoml-0.1.1/argtoml/tests/__init__.py
+-rw-r--r--   0 gum       (1000) gum       (1000)      245 2023-06-09 14:34:41.000000 argtoml-0.1.1/argtoml/tests/test_main.py
+drwxr-xr-x   0 gum       (1000) gum       (1000)        0 2023-06-15 19:37:43.574742 argtoml-0.1.1/argtoml.egg-info/
+-rw-r--r--   0 gum       (1000) gum       (1000)     2052 2023-06-15 19:37:43.000000 argtoml-0.1.1/argtoml.egg-info/PKG-INFO
+-rw-r--r--   0 gum       (1000) gum       (1000)      273 2023-06-15 19:37:43.000000 argtoml-0.1.1/argtoml.egg-info/SOURCES.txt
+-rw-r--r--   0 gum       (1000) gum       (1000)        1 2023-06-15 19:37:43.000000 argtoml-0.1.1/argtoml.egg-info/dependency_links.txt
+-rw-r--r--   0 gum       (1000) gum       (1000)        8 2023-06-15 19:37:43.000000 argtoml-0.1.1/argtoml.egg-info/top_level.txt
+-rw-r--r--   0 gum       (1000) gum       (1000)      939 2023-06-15 19:37:25.000000 argtoml-0.1.1/pyproject.toml
+-rw-r--r--   0 gum       (1000) gum       (1000)       38 2023-06-15 19:37:43.578075 argtoml-0.1.1/setup.cfg
+-rw-r--r--   0 gum       (1000) gum       (1000)       61 2023-06-07 07:31:31.000000 argtoml-0.1.1/setup.py
+drwxr-xr-x   0 gum       (1000) gum       (1000)        0 2023-06-15 19:37:43.574742 argtoml-0.1.1/tests/
+-rw-r--r--   0 gum       (1000) gum       (1000)      245 2023-06-09 14:34:41.000000 argtoml-0.1.1/tests/test_main.py
```

### Comparing `argtoml-0.1.0/LICENSE` & `argtoml-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `argtoml-0.1.0/PKG-INFO` & `argtoml-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: argtoml
-Version: 0.1.0
+Version: 0.1.1
 Summary: Add the keys from a .toml file to your CLI as arguments. Their values default to the values in the .toml file.
 Author-email: Jochem Hölscher <jono-dev.6psuo@simplelogin.com>
 Project-URL: homepage, https://github.com/JJJHolscher/argtoml
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

### Comparing `argtoml-0.1.0/README.md` & `argtoml-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `argtoml-0.1.0/argtoml/main.py` & `argtoml-0.1.1/argtoml/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -73,14 +73,21 @@
                 f"--{prefix}{key}", required=False, type=str, help=f"map"
             )
             add_toml_args(parser, value, key + ".")
         elif type_ == list:
             parser.add_argument(
                 f"--{prefix}{key}", required=False, type=str, help=f"list"
             )
+        elif type_ == bool:
+            parser.add_argument(
+                f"--{prefix}{key}", required=False, action="store_const", const=True
+            )
+            parser.add_argument(
+                f"--{prefix}no-{key}", required=False, action="store_const", const=True
+            )
         else:
             parser.add_argument(
                 f"--{prefix}{key}",
                 required=False,
                 type=type_,
                 help=f"defaults to {value}",
             )
@@ -88,26 +95,36 @@
 
 def fill_toml_args(args, toml, prefix="", filled=False):
     namespace = SimpleNamespace()
     for raw_key, value in toml.items():
         # Check if the user provided the same key but with dashes instead of underscores.
         key = raw_key.replace("-", "_")
         key_str = prefix + "." + key if prefix else key
+        # Boolean variables have 2 arguments.
+        alt_key_str = prefix + ".no_" + key if prefix else "no_" + key
         if namespace.__dict__.get(key) is not None:
             dash_key = prefix + "." + raw_key if prefix else raw_key
             raise KeyError(
-                f"Because '-' is converted to '_', you cannot both have {key_str} and {dash_key} in {TOML_PATH}."
+                f"Because '-' is converted to '_', you cannot both have --{key_str} and --{dash_key} in {TOML_PATH}."
             )
 
         arg_value = args[key_str] if key_str in args else None
 
         # Fill in the default value from the toml file.
         if arg_value is None:
             if type(value) == dict:
                 setattr(namespace, key, fill_toml_args(args, value, key, filled))
+            # Check whether both boolean arguments are empty before filling in the default.
+            elif type(value) == bool:
+                if args[alt_key_str] is None:
+                    setattr(namespace, key, value)  # Fill in the default.
+                else:
+                    setattr(namespace, key, False)  # The anti-argument was called.
+                    del args[alt_key_str]
+                
             else:
                 setattr(namespace, key, value)
 
         # Fill in the value from the command line.
         else:
             if filled:
                 raise Exception(
@@ -127,20 +144,25 @@
                     case builtins.dict:
                         # Check if values are not filled twice.
                         fill_toml_args(args, value, key, True)
                         arg_value = literal_eval(arg_value)
                         assert type(arg_value) == dict
                         arg_value = fill_toml_args(args, arg_value, key, filled)
 
+                    case builtins.bool:
+                        assert type(arg_value) == bool
+                        if args[alt_key_str] is not None:
+                            raise ValueError(f"Do not call --{key_str} and --{alt_key_str} simultaneously.")
+
                     case _:
                         assert type(value) == type(arg_value)
 
             except AssertionError:
                 raise TypeError(
-                    f"Type mismatch for {key_str}. The type from {TOML_PATH} is {type(value)}, but the cli got an argument of type {type(arg_value)}"
+                    f"Type mismatch for {key_str}: the type from {TOML_PATH} is {type(value)}, but the CLI got a {type(arg_value)}"
                 )
 
             setattr(namespace, key, arg_value)
             del args[key_str]
 
     return namespace
```

### Comparing `argtoml-0.1.0/argtoml.egg-info/PKG-INFO` & `argtoml-0.1.1/argtoml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: argtoml
-Version: 0.1.0
+Version: 0.1.1
 Summary: Add the keys from a .toml file to your CLI as arguments. Their values default to the values in the .toml file.
 Author-email: Jochem Hölscher <jono-dev.6psuo@simplelogin.com>
 Project-URL: homepage, https://github.com/JJJHolscher/argtoml
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

### Comparing `argtoml-0.1.0/pyproject.toml` & `argtoml-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 [project]
 name = "argtoml"
-version = "0.1.0"
+version = "0.1.1"
 description = "Add the keys from a .toml file to your CLI as arguments. Their values default to the values in the .toml file."
 dynamic = ["readme"]
 requires-python = ">=3.11"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

