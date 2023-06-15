# Comparing `tmp/tomodachi-0.9.4.tar.gz` & `tmp/tomodachi-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tomodachi-0.9.4.tar", last modified: Tue Mar  6 16:52:43 2018, max compression
+gzip compressed data, was "dist/tomodachi-0.9.5.tar", last modified: Fri Mar 16 07:42:10 2018, max compression
```

## Comparing `tomodachi-0.9.4.tar` & `tomodachi-0.9.5.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 kalaspuff   (501) staff       (20)        0 2018-03-06 16:52:43.000000 tomodachi-0.9.4/
--rw-r--r--   0 kalaspuff   (501) staff       (20)    13792 2018-03-06 16:52:27.000000 tomodachi-0.9.4/CHANGES.rst
--rw-r--r--   0 kalaspuff   (501) staff       (20)     1060 2018-02-28 17:06:05.000000 tomodachi-0.9.4/LICENSE
--rw-r--r--   0 kalaspuff   (501) staff       (20)      163 2018-02-28 17:06:05.000000 tomodachi-0.9.4/MANIFEST.in
--rw-r--r--   0 kalaspuff   (501) staff       (20)    27445 2018-03-06 16:52:43.000000 tomodachi-0.9.4/PKG-INFO
--rw-r--r--   0 kalaspuff   (501) staff       (20)     7113 2018-03-06 07:27:51.000000 tomodachi-0.9.4/README.rst
--rw-r--r--   0 kalaspuff   (501) staff       (20)       38 2018-03-06 16:52:43.000000 tomodachi-0.9.4/setup.cfg
--rw-r--r--   0 kalaspuff   (501) staff       (20)     2122 2018-03-04 14:32:42.000000 tomodachi-0.9.4/setup.py
-drwxr-xr-x   0 kalaspuff   (501) staff       (20)        0 2018-03-06 16:52:43.000000 tomodachi-0.9.4/tomodachi/
--rw-r--r--   0 kalaspuff   (501) staff       (20)     1702 2018-03-02 20:32:46.000000 tomodachi-0.9.4/tomodachi/__init__.py
--rw-r--r--   0 kalaspuff   (501) staff       (20)      106 2018-02-28 17:06:05.000000 tomodachi-0.9.4/tomodachi/__main__.py
--rw-r--r--   0 kalaspuff   (501) staff       (20)      245 2018-03-06 16:51:53.000000 tomodachi-0.9.4/tomodachi/__version__.py
-drwxr-xr-x   0 kalaspuff   (501) staff       (20)        0 2018-03-06 16:52:43.000000 tomodachi-0.9.4/tomodachi/cli/
--rw-r--r--   0 kalaspuff   (501) staff       (20)     4904 2018-02-28 17:06:05.000000 tomodachi-0.9.4/tomodachi/cli/__init__.py
--rw-r--r--   0 kalaspuff   (501) staff       (20)      977 2018-02-28 17:06:05.000000 tomodachi-0.9.4/tomodachi/config.py
--rw-r--r--   0 kalaspuff   (501) staff       (20)     8362 2018-03-02 20:32:46.000000 tomodachi-0.9.4/tomodachi/container.py
-drwxr-xr-x   0 kalaspuff   (501) staff       (20)        0 2018-03-06 16:52:43.000000 tomodachi-0.9.4/tomodachi/discovery/
--rw-r--r--   0 kalaspuff   (501) staff       (20)      184 2018-03-04 13:59:48.000000 tomodachi-0.9.4/tomodachi/discovery/__init__.py
--rw-r--r--   0 kalaspuff   (501) staff       (20)     1523 2018-03-04 13:59:48.000000 tomodachi-0.9.4/tomodachi/discovery/aws_sns_registration.py
--rw-r--r--   0 kalaspuff   (501) staff       (20)     1012 2018-02-28 17:06:05.000000 tomodachi-0.9.4/tomodachi/discovery/dummy_registry.py
-drwxr-xr-x   0 kalaspuff   (501) staff       (20)        0 2018-03-06 16:52:43.000000 tomodachi-0.9.4/tomodachi/helpers/
--rw-r--r--   0 kalaspuff   (501) staff       (20)        0 2018-02-28 17:06:05.000000 tomodachi-0.9.4/tomodachi/helpers/__init__.py
--rw-r--r--   0 kalaspuff   (501) staff       (20)    11678 2018-02-28 17:06:05.000000 tomodachi-0.9.4/tomodachi/helpers/crontab.py
--rw-r--r--   0 kalaspuff   (501) staff       (20)     2867 2018-03-02 20:32:46.000000 tomodachi-0.9.4/tomodachi/helpers/logging.py
--rw-r--r--   0 kalaspuff   (501) staff       (20)     2336 2018-03-02 20:32:46.000000 tomodachi-0.9.4/tomodachi/importer.py
-drwxr-xr-x   0 kalaspuff   (501) staff       (20)        0 2018-03-06 16:52:43.000000 tomodachi-0.9.4/tomodachi/invoker/
--rw-r--r--   0 kalaspuff   (501) staff       (20)       71 2018-02-28 17:06:05.000000 tomodachi-0.9.4/tomodachi/invoker/__init__.py
--rw-r--r--   0 kalaspuff   (501) staff       (20)     1517 2018-02-28 17:06:05.000000 tomodachi-0.9.4/tomodachi/invoker/base.py
--rw-r--r--   0 kalaspuff   (501) staff       (20)     6992 2018-03-05 17:29:54.000000 tomodachi-0.9.4/tomodachi/launcher.py
-drwxr-xr-x   0 kalaspuff   (501) staff       (20)        0 2018-03-06 16:52:43.000000 tomodachi-0.9.4/tomodachi/protocol/
--rw-r--r--   0 kalaspuff   (501) staff       (20)       74 2018-03-04 13:59:48.000000 tomodachi-0.9.4/tomodachi/protocol/__init__.py
--rw-r--r--   0 kalaspuff   (501) staff       (20)     2705 2018-02-28 17:06:05.000000 tomodachi-0.9.4/tomodachi/protocol/json_base.py
-drwxr-xr-x   0 kalaspuff   (501) staff       (20)        0 2018-03-06 16:52:43.000000 tomodachi-0.9.4/tomodachi/transport/
--rw-r--r--   0 kalaspuff   (501) staff       (20)        0 2018-02-28 17:06:05.000000 tomodachi-0.9.4/tomodachi/transport/__init__.py
--rw-r--r--   0 kalaspuff   (501) staff       (20)    16094 2018-03-06 07:34:20.000000 tomodachi-0.9.4/tomodachi/transport/amqp.py
--rw-r--r--   0 kalaspuff   (501) staff       (20)    34699 2018-03-06 09:08:30.000000 tomodachi-0.9.4/tomodachi/transport/aws_sns_sqs.py
--rw-r--r--   0 kalaspuff   (501) staff       (20)    34093 2018-03-06 16:48:33.000000 tomodachi-0.9.4/tomodachi/transport/http.py
--rw-r--r--   0 kalaspuff   (501) staff       (20)    16943 2018-03-06 09:43:49.000000 tomodachi-0.9.4/tomodachi/transport/schedule.py
--rw-r--r--   0 kalaspuff   (501) staff       (20)     4811 2018-03-05 20:50:11.000000 tomodachi-0.9.4/tomodachi/watcher.py
-drwxr-xr-x   0 kalaspuff   (501) staff       (20)        0 2018-03-06 16:52:43.000000 tomodachi-0.9.4/tomodachi.egg-info/
--rw-r--r--   0 kalaspuff   (501) staff       (20)        1 2018-03-06 16:52:43.000000 tomodachi-0.9.4/tomodachi.egg-info/dependency_links.txt
--rw-r--r--   0 kalaspuff   (501) staff       (20)       60 2018-03-06 16:52:43.000000 tomodachi-0.9.4/tomodachi.egg-info/entry_points.txt
--rw-r--r--   0 kalaspuff   (501) staff       (20)        1 2018-02-28 17:11:38.000000 tomodachi-0.9.4/tomodachi.egg-info/not-zip-safe
--rw-r--r--   0 kalaspuff   (501) staff       (20)    27445 2018-03-06 16:52:43.000000 tomodachi-0.9.4/tomodachi.egg-info/PKG-INFO
--rw-r--r--   0 kalaspuff   (501) staff       (20)      146 2018-03-06 16:52:43.000000 tomodachi-0.9.4/tomodachi.egg-info/requires.txt
--rw-r--r--   0 kalaspuff   (501) staff       (20)      962 2018-03-06 16:52:43.000000 tomodachi-0.9.4/tomodachi.egg-info/SOURCES.txt
--rw-r--r--   0 kalaspuff   (501) staff       (20)       10 2018-03-06 16:52:43.000000 tomodachi-0.9.4/tomodachi.egg-info/top_level.txt
+drwxr-xr-x   0 kalaspuff   (501) staff       (20)        0 2018-03-16 07:42:10.000000 tomodachi-0.9.5/
+-rw-r--r--   0 kalaspuff   (501) staff       (20)    13923 2018-03-16 07:41:42.000000 tomodachi-0.9.5/CHANGES.rst
+-rw-r--r--   0 kalaspuff   (501) staff       (20)     1060 2018-02-28 17:06:05.000000 tomodachi-0.9.5/LICENSE
+-rw-r--r--   0 kalaspuff   (501) staff       (20)      163 2018-02-28 17:06:05.000000 tomodachi-0.9.5/MANIFEST.in
+-rw-r--r--   0 kalaspuff   (501) staff       (20)    27624 2018-03-16 07:42:10.000000 tomodachi-0.9.5/PKG-INFO
+-rw-r--r--   0 kalaspuff   (501) staff       (20)     7113 2018-03-13 21:47:23.000000 tomodachi-0.9.5/README.rst
+-rw-r--r--   0 kalaspuff   (501) staff       (20)       38 2018-03-16 07:42:10.000000 tomodachi-0.9.5/setup.cfg
+-rw-r--r--   0 kalaspuff   (501) staff       (20)     2122 2018-03-13 21:47:23.000000 tomodachi-0.9.5/setup.py
+drwxr-xr-x   0 kalaspuff   (501) staff       (20)        0 2018-03-16 07:42:10.000000 tomodachi-0.9.5/tomodachi/
+-rw-r--r--   0 kalaspuff   (501) staff       (20)     1702 2018-03-02 20:32:46.000000 tomodachi-0.9.5/tomodachi/__init__.py
+-rw-r--r--   0 kalaspuff   (501) staff       (20)      106 2018-02-28 17:06:05.000000 tomodachi-0.9.5/tomodachi/__main__.py
+-rw-r--r--   0 kalaspuff   (501) staff       (20)      245 2018-03-16 07:40:20.000000 tomodachi-0.9.5/tomodachi/__version__.py
+drwxr-xr-x   0 kalaspuff   (501) staff       (20)        0 2018-03-16 07:42:10.000000 tomodachi-0.9.5/tomodachi/cli/
+-rw-r--r--   0 kalaspuff   (501) staff       (20)     4904 2018-02-28 17:06:05.000000 tomodachi-0.9.5/tomodachi/cli/__init__.py
+-rw-r--r--   0 kalaspuff   (501) staff       (20)      977 2018-02-28 17:06:05.000000 tomodachi-0.9.5/tomodachi/config.py
+-rw-r--r--   0 kalaspuff   (501) staff       (20)     8362 2018-03-02 20:32:46.000000 tomodachi-0.9.5/tomodachi/container.py
+drwxr-xr-x   0 kalaspuff   (501) staff       (20)        0 2018-03-16 07:42:10.000000 tomodachi-0.9.5/tomodachi/discovery/
+-rw-r--r--   0 kalaspuff   (501) staff       (20)      184 2018-03-13 21:47:23.000000 tomodachi-0.9.5/tomodachi/discovery/__init__.py
+-rw-r--r--   0 kalaspuff   (501) staff       (20)     1523 2018-03-13 21:47:23.000000 tomodachi-0.9.5/tomodachi/discovery/aws_sns_registration.py
+-rw-r--r--   0 kalaspuff   (501) staff       (20)     1012 2018-02-28 17:06:05.000000 tomodachi-0.9.5/tomodachi/discovery/dummy_registry.py
+drwxr-xr-x   0 kalaspuff   (501) staff       (20)        0 2018-03-16 07:42:10.000000 tomodachi-0.9.5/tomodachi/helpers/
+-rw-r--r--   0 kalaspuff   (501) staff       (20)        0 2018-02-28 17:06:05.000000 tomodachi-0.9.5/tomodachi/helpers/__init__.py
+-rw-r--r--   0 kalaspuff   (501) staff       (20)    11678 2018-02-28 17:06:05.000000 tomodachi-0.9.5/tomodachi/helpers/crontab.py
+-rw-r--r--   0 kalaspuff   (501) staff       (20)     2867 2018-03-02 20:32:46.000000 tomodachi-0.9.5/tomodachi/helpers/logging.py
+-rw-r--r--   0 kalaspuff   (501) staff       (20)     2791 2018-03-15 23:26:36.000000 tomodachi-0.9.5/tomodachi/importer.py
+drwxr-xr-x   0 kalaspuff   (501) staff       (20)        0 2018-03-16 07:42:10.000000 tomodachi-0.9.5/tomodachi/invoker/
+-rw-r--r--   0 kalaspuff   (501) staff       (20)       71 2018-02-28 17:06:05.000000 tomodachi-0.9.5/tomodachi/invoker/__init__.py
+-rw-r--r--   0 kalaspuff   (501) staff       (20)     1517 2018-02-28 17:06:05.000000 tomodachi-0.9.5/tomodachi/invoker/base.py
+-rw-r--r--   0 kalaspuff   (501) staff       (20)     6992 2018-03-13 21:47:23.000000 tomodachi-0.9.5/tomodachi/launcher.py
+drwxr-xr-x   0 kalaspuff   (501) staff       (20)        0 2018-03-16 07:42:10.000000 tomodachi-0.9.5/tomodachi/protocol/
+-rw-r--r--   0 kalaspuff   (501) staff       (20)       74 2018-03-13 21:47:23.000000 tomodachi-0.9.5/tomodachi/protocol/__init__.py
+-rw-r--r--   0 kalaspuff   (501) staff       (20)     2705 2018-02-28 17:06:05.000000 tomodachi-0.9.5/tomodachi/protocol/json_base.py
+drwxr-xr-x   0 kalaspuff   (501) staff       (20)        0 2018-03-16 07:42:10.000000 tomodachi-0.9.5/tomodachi/transport/
+-rw-r--r--   0 kalaspuff   (501) staff       (20)        0 2018-02-28 17:06:05.000000 tomodachi-0.9.5/tomodachi/transport/__init__.py
+-rw-r--r--   0 kalaspuff   (501) staff       (20)    16094 2018-03-13 21:47:23.000000 tomodachi-0.9.5/tomodachi/transport/amqp.py
+-rw-r--r--   0 kalaspuff   (501) staff       (20)    34699 2018-03-13 21:47:23.000000 tomodachi-0.9.5/tomodachi/transport/aws_sns_sqs.py
+-rw-r--r--   0 kalaspuff   (501) staff       (20)    34093 2018-03-13 21:47:23.000000 tomodachi-0.9.5/tomodachi/transport/http.py
+-rw-r--r--   0 kalaspuff   (501) staff       (20)    16943 2018-03-13 21:47:23.000000 tomodachi-0.9.5/tomodachi/transport/schedule.py
+-rw-r--r--   0 kalaspuff   (501) staff       (20)     4811 2018-03-13 21:47:23.000000 tomodachi-0.9.5/tomodachi/watcher.py
+drwxr-xr-x   0 kalaspuff   (501) staff       (20)        0 2018-03-16 07:42:10.000000 tomodachi-0.9.5/tomodachi.egg-info/
+-rw-r--r--   0 kalaspuff   (501) staff       (20)        1 2018-03-16 07:42:10.000000 tomodachi-0.9.5/tomodachi.egg-info/dependency_links.txt
+-rw-r--r--   0 kalaspuff   (501) staff       (20)       60 2018-03-16 07:42:10.000000 tomodachi-0.9.5/tomodachi.egg-info/entry_points.txt
+-rw-r--r--   0 kalaspuff   (501) staff       (20)        1 2018-02-28 17:11:38.000000 tomodachi-0.9.5/tomodachi.egg-info/not-zip-safe
+-rw-r--r--   0 kalaspuff   (501) staff       (20)    27624 2018-03-16 07:42:10.000000 tomodachi-0.9.5/tomodachi.egg-info/PKG-INFO
+-rw-r--r--   0 kalaspuff   (501) staff       (20)      146 2018-03-16 07:42:10.000000 tomodachi-0.9.5/tomodachi.egg-info/requires.txt
+-rw-r--r--   0 kalaspuff   (501) staff       (20)      962 2018-03-16 07:42:10.000000 tomodachi-0.9.5/tomodachi.egg-info/SOURCES.txt
+-rw-r--r--   0 kalaspuff   (501) staff       (20)       10 2018-03-16 07:42:10.000000 tomodachi-0.9.5/tomodachi.egg-info/top_level.txt
```

### Comparing `tomodachi-0.9.4/CHANGES.rst` & `tomodachi-0.9.5/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 Changes
 =======
 
+0.9.5 (2018-03-16)
+------------------
+- More robust handling of invoking service files that aren't a part of a
+  Python package.
+
+
 0.9.4 (2018-03-06)
 ------------------
 - Fixes an issue affecting websocket connections where the receive function
   was invalidly called twice of which one time were without error handling.
 
 
 0.9.3 (2018-03-06)
```

### Comparing `tomodachi-0.9.4/LICENSE` & `tomodachi-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tomodachi-0.9.4/PKG-INFO` & `tomodachi-0.9.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tomodachi
-Version: 0.9.4
+Version: 0.9.5
 Summary: Python 3 microservice library / framework using asyncio with HTTP, websockets, RabbitMQ / AMQP and AWS SNS+SQS support.
 Home-page: https://github.com/kalaspuff/tomodachi
 Author: Carl Oscar Aaro
 Author-email: hello@carloscar.com
 License: MIT
 Download-URL: https://pypi.python.org/pypi/tomodachi
 Description-Content-Type: UNKNOWN
@@ -199,14 +199,20 @@
         
         Who built this and why?
           My name is **Carl Oscar Aaro** and I'm a coder from Sweden. I simply wanted to learn more about asyncio and needed a constructive off-work project to experiment with – and here we are. 🎉
         
         Changes
         =======
         
+        0.9.5 (2018-03-16)
+        ------------------
+        - More robust handling of invoking service files that aren't a part of a
+          Python package.
+        
+        
         0.9.4 (2018-03-06)
         ------------------
         - Fixes an issue affecting websocket connections where the receive function
           was invalidly called twice of which one time were without error handling.
         
         
         0.9.3 (2018-03-06)
```

### Comparing `tomodachi-0.9.4/README.rst` & `tomodachi-0.9.5/README.rst`

 * *Files identical despite different names*

### Comparing `tomodachi-0.9.4/setup.py` & `tomodachi-0.9.5/setup.py`

 * *Files identical despite different names*

### Comparing `tomodachi-0.9.4/tomodachi/__init__.py` & `tomodachi-0.9.5/tomodachi/__init__.py`

 * *Files identical despite different names*

### Comparing `tomodachi-0.9.4/tomodachi/cli/__init__.py` & `tomodachi-0.9.5/tomodachi/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `tomodachi-0.9.4/tomodachi/config.py` & `tomodachi-0.9.5/tomodachi/config.py`

 * *Files identical despite different names*

### Comparing `tomodachi-0.9.4/tomodachi/container.py` & `tomodachi-0.9.5/tomodachi/container.py`

 * *Files identical despite different names*

### Comparing `tomodachi-0.9.4/tomodachi/discovery/aws_sns_registration.py` & `tomodachi-0.9.5/tomodachi/discovery/aws_sns_registration.py`

 * *Files identical despite different names*

### Comparing `tomodachi-0.9.4/tomodachi/discovery/dummy_registry.py` & `tomodachi-0.9.5/tomodachi/discovery/dummy_registry.py`

 * *Files identical despite different names*

### Comparing `tomodachi-0.9.4/tomodachi/helpers/crontab.py` & `tomodachi-0.9.5/tomodachi/helpers/crontab.py`

 * *Files identical despite different names*

### Comparing `tomodachi-0.9.4/tomodachi/helpers/logging.py` & `tomodachi-0.9.5/tomodachi/helpers/logging.py`

 * *Files identical despite different names*

### Comparing `tomodachi-0.9.4/tomodachi/importer.py` & `tomodachi-0.9.5/tomodachi/importer.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,37 +13,47 @@
         cwd = os.getcwd()
         file_path = '{}/{}.py'.format(os.path.realpath(cwd), file_name)
         if file_path.endswith('.py.py'):
             file_path = file_path[:-3]
         try:
             sys.path.insert(0, cwd)
             sys.path.insert(0, os.path.dirname(os.path.dirname(file_path)))
-            spec = importlib.util.find_spec('.{}'.format(file_path.rsplit('/', 1)[1])[:-3], package=os.path.dirname(file_path).rsplit('/', 1)[1])  # type: Any
+            try:
+                spec = importlib.util.find_spec('.{}'.format(file_path.rsplit('/', 1)[1])[:-3], package=os.path.dirname(file_path).rsplit('/', 1)[1])  # type: Any
+                if not spec:
+                    spec = importlib.util.spec_from_file_location(file_name, file_path)
+            except AttributeError as e:
+                try:
+                    spec = importlib.util.spec_from_file_location(file_name, file_path)
+                except Exception:
+                    raise e
             if not spec:
                 raise OSError
             service_import = importlib.util.module_from_spec(spec)
             try:
                 importlib.reload(service_import)
                 service_import = importlib.util.module_from_spec(spec)
             except ImportError:
                 pass
             if not spec.loader:
                 raise OSError
             spec.loader.exec_module(service_import)
         except ImportError as e:
             if file_name.endswith('.py.py'):
                 return cls.import_service_file(file_name[:-3])
-            logging.getLogger('import').warning('Invalid service, unable to load service file "{}"'.format(file_name))
+            logging.getLogger('import').warning('Invalid service, unable to load service file "{}.py"'.format(file_name))
             raise e
         except OSError:
             if file_name.endswith('.py'):
                 return cls.import_service_file(file_name[:-3])
-            logging.getLogger('import').warning('Invalid service, no such service file "{}"'.format(file_name))
+            logging.getLogger('import').warning('Invalid service, no such service file "{}.py"'.format(file_name))
             sys.exit(2)
         except Exception as e:
+            if not file_name.endswith('.py'):
+                file_name = '{}.py'.format(file_name)
             logging.getLogger('import').warning('Unable to load service file "{}"'.format(file_name))
             logging.getLogger('import').warning('Error: {}'.format(e))
             raise e
         return service_import
 
     @classmethod
     def import_module(cls, file_name: str) -> ModuleType:
```

### Comparing `tomodachi-0.9.4/tomodachi/invoker/base.py` & `tomodachi-0.9.5/tomodachi/invoker/base.py`

 * *Files identical despite different names*

### Comparing `tomodachi-0.9.4/tomodachi/launcher.py` & `tomodachi-0.9.5/tomodachi/launcher.py`

 * *Files identical despite different names*

### Comparing `tomodachi-0.9.4/tomodachi/protocol/json_base.py` & `tomodachi-0.9.5/tomodachi/protocol/json_base.py`

 * *Files identical despite different names*

### Comparing `tomodachi-0.9.4/tomodachi/transport/amqp.py` & `tomodachi-0.9.5/tomodachi/transport/amqp.py`

 * *Files identical despite different names*

### Comparing `tomodachi-0.9.4/tomodachi/transport/aws_sns_sqs.py` & `tomodachi-0.9.5/tomodachi/transport/aws_sns_sqs.py`

 * *Files identical despite different names*

### Comparing `tomodachi-0.9.4/tomodachi/transport/http.py` & `tomodachi-0.9.5/tomodachi/transport/http.py`

 * *Files identical despite different names*

### Comparing `tomodachi-0.9.4/tomodachi/transport/schedule.py` & `tomodachi-0.9.5/tomodachi/transport/schedule.py`

 * *Files identical despite different names*

### Comparing `tomodachi-0.9.4/tomodachi/watcher.py` & `tomodachi-0.9.5/tomodachi/watcher.py`

 * *Files identical despite different names*

### Comparing `tomodachi-0.9.4/tomodachi.egg-info/PKG-INFO` & `tomodachi-0.9.5/tomodachi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tomodachi
-Version: 0.9.4
+Version: 0.9.5
 Summary: Python 3 microservice library / framework using asyncio with HTTP, websockets, RabbitMQ / AMQP and AWS SNS+SQS support.
 Home-page: https://github.com/kalaspuff/tomodachi
 Author: Carl Oscar Aaro
 Author-email: hello@carloscar.com
 License: MIT
 Download-URL: https://pypi.python.org/pypi/tomodachi
 Description-Content-Type: UNKNOWN
@@ -199,14 +199,20 @@
         
         Who built this and why?
           My name is **Carl Oscar Aaro** and I'm a coder from Sweden. I simply wanted to learn more about asyncio and needed a constructive off-work project to experiment with – and here we are. 🎉
         
         Changes
         =======
         
+        0.9.5 (2018-03-16)
+        ------------------
+        - More robust handling of invoking service files that aren't a part of a
+          Python package.
+        
+        
         0.9.4 (2018-03-06)
         ------------------
         - Fixes an issue affecting websocket connections where the receive function
           was invalidly called twice of which one time were without error handling.
         
         
         0.9.3 (2018-03-06)
```

### Comparing `tomodachi-0.9.4/tomodachi.egg-info/SOURCES.txt` & `tomodachi-0.9.5/tomodachi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

