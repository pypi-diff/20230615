# Comparing `tmp/rajesh_cli-2.0.1.tar.gz` & `tmp/rajesh_cli-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rajesh_cli-2.0.1.tar", last modified: Thu Jun 15 06:15:43 2023, max compression
+gzip compressed data, was "rajesh_cli-2.0.2.tar", last modified: Thu Jun 15 06:22:25 2023, max compression
```

## Comparing `rajesh_cli-2.0.1.tar` & `rajesh_cli-2.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 rajesh    (1000) rajesh    (1000)        0 2023-06-15 06:15:43.920008 rajesh_cli-2.0.1/
--rw-rw-r--   0 rajesh    (1000) rajesh    (1000)       54 2023-06-15 06:15:43.916008 rajesh_cli-2.0.1/PKG-INFO
-drwxrwxr-x   0 rajesh    (1000) rajesh    (1000)        0 2023-06-15 06:15:43.916008 rajesh_cli-2.0.1/rajesh_cli.egg-info/
--rw-rw-r--   0 rajesh    (1000) rajesh    (1000)       54 2023-06-15 06:15:43.000000 rajesh_cli-2.0.1/rajesh_cli.egg-info/PKG-INFO
--rw-rw-r--   0 rajesh    (1000) rajesh    (1000)      241 2023-06-15 06:15:43.000000 rajesh_cli-2.0.1/rajesh_cli.egg-info/SOURCES.txt
--rw-rw-r--   0 rajesh    (1000) rajesh    (1000)        1 2023-06-15 06:15:43.000000 rajesh_cli-2.0.1/rajesh_cli.egg-info/dependency_links.txt
--rw-rw-r--   0 rajesh    (1000) rajesh    (1000)       52 2023-06-15 06:15:43.000000 rajesh_cli-2.0.1/rajesh_cli.egg-info/entry_points.txt
--rw-rw-r--   0 rajesh    (1000) rajesh    (1000)        9 2023-06-15 06:15:43.000000 rajesh_cli-2.0.1/rajesh_cli.egg-info/requires.txt
--rw-rw-r--   0 rajesh    (1000) rajesh    (1000)        4 2023-06-15 06:15:43.000000 rajesh_cli-2.0.1/rajesh_cli.egg-info/top_level.txt
--rw-rw-r--   0 rajesh    (1000) rajesh    (1000)       38 2023-06-15 06:15:43.920008 rajesh_cli-2.0.1/setup.cfg
--rw-rw-r--   0 rajesh    (1000) rajesh    (1000)      291 2023-06-15 06:15:43.000000 rajesh_cli-2.0.1/setup.py
-drwxrwxr-x   0 rajesh    (1000) rajesh    (1000)        0 2023-06-15 06:15:43.916008 rajesh_cli-2.0.1/src/
--rw-rw-r--   0 rajesh    (1000) rajesh    (1000)        0 2023-06-14 11:10:06.000000 rajesh_cli-2.0.1/src/__init__.py
--rw-rw-r--   0 rajesh    (1000) rajesh    (1000)     1223 2023-06-15 06:14:25.000000 rajesh_cli-2.0.1/src/cli.py
+drwxrwxr-x   0 rajesh    (1000) rajesh    (1000)        0 2023-06-15 06:22:25.016009 rajesh_cli-2.0.2/
+-rw-rw-r--   0 rajesh    (1000) rajesh    (1000)       54 2023-06-15 06:22:25.016009 rajesh_cli-2.0.2/PKG-INFO
+drwxrwxr-x   0 rajesh    (1000) rajesh    (1000)        0 2023-06-15 06:22:25.016009 rajesh_cli-2.0.2/rajesh_cli.egg-info/
+-rw-rw-r--   0 rajesh    (1000) rajesh    (1000)       54 2023-06-15 06:22:25.000000 rajesh_cli-2.0.2/rajesh_cli.egg-info/PKG-INFO
+-rw-rw-r--   0 rajesh    (1000) rajesh    (1000)      241 2023-06-15 06:22:25.000000 rajesh_cli-2.0.2/rajesh_cli.egg-info/SOURCES.txt
+-rw-rw-r--   0 rajesh    (1000) rajesh    (1000)        1 2023-06-15 06:22:25.000000 rajesh_cli-2.0.2/rajesh_cli.egg-info/dependency_links.txt
+-rw-rw-r--   0 rajesh    (1000) rajesh    (1000)       52 2023-06-15 06:22:25.000000 rajesh_cli-2.0.2/rajesh_cli.egg-info/entry_points.txt
+-rw-rw-r--   0 rajesh    (1000) rajesh    (1000)        9 2023-06-15 06:22:25.000000 rajesh_cli-2.0.2/rajesh_cli.egg-info/requires.txt
+-rw-rw-r--   0 rajesh    (1000) rajesh    (1000)        4 2023-06-15 06:22:25.000000 rajesh_cli-2.0.2/rajesh_cli.egg-info/top_level.txt
+-rw-rw-r--   0 rajesh    (1000) rajesh    (1000)       38 2023-06-15 06:22:25.016009 rajesh_cli-2.0.2/setup.cfg
+-rw-rw-r--   0 rajesh    (1000) rajesh    (1000)      291 2023-06-15 06:22:22.000000 rajesh_cli-2.0.2/setup.py
+drwxrwxr-x   0 rajesh    (1000) rajesh    (1000)        0 2023-06-15 06:22:25.016009 rajesh_cli-2.0.2/src/
+-rw-rw-r--   0 rajesh    (1000) rajesh    (1000)        0 2023-06-14 11:10:06.000000 rajesh_cli-2.0.2/src/__init__.py
+-rw-rw-r--   0 rajesh    (1000) rajesh    (1000)     1191 2023-06-15 06:22:01.000000 rajesh_cli-2.0.2/src/cli.py
```

### Comparing `rajesh_cli-2.0.1/src/cli.py` & `rajesh_cli-2.0.2/src/cli.py`

 * *Files 11% similar despite different names*

```diff
@@ -35,17 +35,13 @@
         elif command.startswith("add "):
             numbers = list(map(int, command[4:].split(",")))
             add_numbers(numbers)
         else:
             print("Invalid command. Please try again.")
 
 
-def main():
+def activate_cli():
     parser = argparse.ArgumentParser(prog="rajesh_login")
     parser.set_defaults(func=login)
 
     args = parser.parse_args()
     args.func()
-
-
-if __name__ == "__main__":
-    main()
```

