# Comparing `tmp/packtivity-0.9.4.tar.gz` & `tmp/packtivity-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/packtivity-0.9.4.tar", last modified: Sat Nov 25 14:50:07 2017, max compression
+gzip compressed data, was "dist/packtivity-0.9.6.tar", last modified: Wed Dec  6 02:03:10 2017, max compression
```

## Comparing `packtivity-0.9.4.tar` & `packtivity-0.9.6.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-11-25 14:50:07.000000 packtivity-0.9.4/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-11-25 14:50:07.000000 packtivity-0.9.4/packtivity/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1334 2017-11-25 14:48:52.000000 packtivity-0.9.4/packtivity/utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2039 2017-11-25 14:48:52.000000 packtivity-0.9.4/packtivity/logutils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7324 2017-11-25 14:48:52.000000 packtivity-0.9.4/packtivity/asyncbackends.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-11-25 14:50:07.000000 packtivity-0.9.4/packtivity/statecontexts/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1019 2017-11-25 14:48:52.000000 packtivity-0.9.4/packtivity/statecontexts/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3516 2017-11-25 14:48:52.000000 packtivity-0.9.4/packtivity/statecontexts/posixfs_context.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-11-25 14:50:07.000000 packtivity-0.9.4/packtivity/handlers/
--rw-rw-r--   0 travis    (2000) travis    (2000)     4159 2017-11-25 14:48:52.000000 packtivity-0.9.4/packtivity/handlers/publisher_handlers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1140 2017-11-25 14:48:52.000000 packtivity-0.9.4/packtivity/handlers/process_handlers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12234 2017-11-25 14:48:52.000000 packtivity-0.9.4/packtivity/handlers/execution_handlers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      168 2017-11-25 14:48:52.000000 packtivity-0.9.4/packtivity/handlers/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      133 2017-11-25 14:48:52.000000 packtivity-0.9.4/packtivity/handlers/environment_handlers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4377 2017-11-25 14:48:52.000000 packtivity-0.9.4/packtivity/cli.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4177 2017-11-25 14:48:52.000000 packtivity-0.9.4/packtivity/syncbackends.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1434 2017-11-25 14:48:52.000000 packtivity-0.9.4/packtivity/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3982 2017-11-25 14:48:52.000000 packtivity-0.9.4/packtivity/backendutils.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-11-25 14:50:07.000000 packtivity-0.9.4/packtivity.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)      128 2017-11-25 14:50:07.000000 packtivity-0.9.4/packtivity.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      661 2017-11-25 14:50:07.000000 packtivity-0.9.4/packtivity.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      157 2017-11-25 14:50:07.000000 packtivity-0.9.4/packtivity.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2017-11-25 14:50:07.000000 packtivity-0.9.4/packtivity.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      265 2017-11-25 14:50:07.000000 packtivity-0.9.4/packtivity.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)       11 2017-11-25 14:50:07.000000 packtivity-0.9.4/packtivity.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2017-11-25 14:50:07.000000 packtivity-0.9.4/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)      962 2017-11-25 14:48:52.000000 packtivity-0.9.4/setup.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      265 2017-11-25 14:50:07.000000 packtivity-0.9.4/PKG-INFO
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-12-06 02:03:10.000000 packtivity-0.9.6/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-12-06 02:03:10.000000 packtivity-0.9.6/packtivity/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1334 2017-12-06 02:01:48.000000 packtivity-0.9.6/packtivity/utils.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2039 2017-12-06 02:01:48.000000 packtivity-0.9.6/packtivity/logutils.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7324 2017-12-06 02:01:48.000000 packtivity-0.9.6/packtivity/asyncbackends.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-12-06 02:03:10.000000 packtivity-0.9.6/packtivity/statecontexts/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1019 2017-12-06 02:01:48.000000 packtivity-0.9.6/packtivity/statecontexts/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3516 2017-12-06 02:01:48.000000 packtivity-0.9.6/packtivity/statecontexts/posixfs_context.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-12-06 02:03:10.000000 packtivity-0.9.6/packtivity/handlers/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4225 2017-12-06 02:01:48.000000 packtivity-0.9.6/packtivity/handlers/publisher_handlers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1140 2017-12-06 02:01:48.000000 packtivity-0.9.6/packtivity/handlers/process_handlers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12234 2017-12-06 02:01:48.000000 packtivity-0.9.6/packtivity/handlers/execution_handlers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      168 2017-12-06 02:01:48.000000 packtivity-0.9.6/packtivity/handlers/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      133 2017-12-06 02:01:48.000000 packtivity-0.9.6/packtivity/handlers/environment_handlers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4377 2017-12-06 02:01:48.000000 packtivity-0.9.6/packtivity/cli.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4177 2017-12-06 02:01:48.000000 packtivity-0.9.6/packtivity/syncbackends.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1434 2017-12-06 02:01:48.000000 packtivity-0.9.6/packtivity/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3982 2017-12-06 02:01:48.000000 packtivity-0.9.6/packtivity/backendutils.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-12-06 02:03:10.000000 packtivity-0.9.6/packtivity.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      128 2017-12-06 02:03:10.000000 packtivity-0.9.6/packtivity.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      661 2017-12-06 02:03:10.000000 packtivity-0.9.6/packtivity.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      157 2017-12-06 02:03:10.000000 packtivity-0.9.6/packtivity.egg-info/entry_points.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2017-12-06 02:03:10.000000 packtivity-0.9.6/packtivity.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      265 2017-12-06 02:03:10.000000 packtivity-0.9.6/packtivity.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)       11 2017-12-06 02:03:10.000000 packtivity-0.9.6/packtivity.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       38 2017-12-06 02:03:10.000000 packtivity-0.9.6/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)      962 2017-12-06 02:01:48.000000 packtivity-0.9.6/setup.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      265 2017-12-06 02:03:10.000000 packtivity-0.9.6/PKG-INFO
```

### Comparing `packtivity-0.9.4/packtivity/utils.py` & `packtivity-0.9.6/packtivity/utils.py`

 * *Files identical despite different names*

### Comparing `packtivity-0.9.4/packtivity/logutils.py` & `packtivity-0.9.6/packtivity/logutils.py`

 * *Files identical despite different names*

### Comparing `packtivity-0.9.4/packtivity/asyncbackends.py` & `packtivity-0.9.6/packtivity/asyncbackends.py`

 * *Files identical despite different names*

### Comparing `packtivity-0.9.4/packtivity/statecontexts/__init__.py` & `packtivity-0.9.6/packtivity/statecontexts/__init__.py`

 * *Files identical despite different names*

### Comparing `packtivity-0.9.4/packtivity/statecontexts/posixfs_context.py` & `packtivity-0.9.6/packtivity/statecontexts/posixfs_context.py`

 * *Files identical despite different names*

### Comparing `packtivity-0.9.4/packtivity/handlers/publisher_handlers.py` & `packtivity-0.9.6/packtivity/handlers/publisher_handlers.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,21 +67,22 @@
         elif state.readonly and len(state.readonly)==1:
             globdir = state.readonly[0]
         else: break
 
         searchval = value
         if publisher['relative_paths'] and not os.path.isabs(searchval):
             searchval = os.path.join(globdir,value)
-
         # if requested try first exact match and then try glob (if requested)
         if publisher['tryExact'] and os.path.exists(searchval):
             #if it's a string and the full path exists replace relative path
             value = searchval
         elif publisher['glob']:
-            value = glob2.glob(searchval)
+            globresult = glob2.glob(searchval)
+            if globresult:
+                value = globresult
         path.set(result,value)
     return result
 
 @publisher('fromglob-pub')
 def glob_pub_handler(publisher,parameters,state):
     workdir = state.readwrite[0]
     globexpr =  publisher['globexpression']
```

### Comparing `packtivity-0.9.4/packtivity/handlers/process_handlers.py` & `packtivity-0.9.6/packtivity/handlers/process_handlers.py`

 * *Files identical despite different names*

### Comparing `packtivity-0.9.4/packtivity/handlers/execution_handlers.py` & `packtivity-0.9.6/packtivity/handlers/execution_handlers.py`

 * *Files identical despite different names*

### Comparing `packtivity-0.9.4/packtivity/cli.py` & `packtivity-0.9.6/packtivity/cli.py`

 * *Files identical despite different names*

### Comparing `packtivity-0.9.4/packtivity/syncbackends.py` & `packtivity-0.9.6/packtivity/syncbackends.py`

 * *Files identical despite different names*

### Comparing `packtivity-0.9.4/packtivity/__init__.py` & `packtivity-0.9.6/packtivity/__init__.py`

 * *Files identical despite different names*

### Comparing `packtivity-0.9.4/packtivity/backendutils.py` & `packtivity-0.9.6/packtivity/backendutils.py`

 * *Files identical despite different names*

### Comparing `packtivity-0.9.4/packtivity.egg-info/SOURCES.txt` & `packtivity-0.9.6/packtivity.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `packtivity-0.9.4/setup.py` & `packtivity-0.9.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 if not 'READTHEDOCS' in os.environ:
   deps += ['jq']
 
 
 
 setup(
   name = 'packtivity',
-  version = '0.9.4',
+  version = '0.9.6',
   description = 'packtivity - general purpose schema + bindings for PROV activities',
   url = '',
   author = 'Lukas Heinrich',
   author_email = 'lukas.heinrich@cern.ch',
   packages = find_packages(),
   include_package_data = True,
   install_requires = deps,
```

