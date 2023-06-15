# Comparing `tmp/poplar_logging-1.2.2.tar.gz` & `tmp/poplar_logging-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poplar_logging-1.2.2.tar", last modified: Wed Jun 14 20:11:15 2023, max compression
+gzip compressed data, was "poplar_logging-1.2.3.tar", last modified: Thu Jun 15 00:18:36 2023, max compression
```

## Comparing `poplar_logging-1.2.2.tar` & `poplar_logging-1.2.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 odai       (501) staff       (20)        0 2023-06-14 20:11:15.816734 poplar_logging-1.2.2/
--rw-r--r--   0 odai       (501) staff       (20)     1070 2023-06-12 04:45:07.000000 poplar_logging-1.2.2/LICENSE
--rw-r--r--   0 odai       (501) staff       (20)      861 2023-06-14 20:11:15.816601 poplar_logging-1.2.2/PKG-INFO
--rw-r--r--   0 odai       (501) staff       (20)      427 2023-06-14 19:59:52.000000 poplar_logging-1.2.2/README.md
--rw-r--r--   0 odai       (501) staff       (20)      427 2023-06-14 20:09:38.000000 poplar_logging-1.2.2/pyproject.toml
--rw-r--r--   0 odai       (501) staff       (20)       38 2023-06-14 20:11:15.816769 poplar_logging-1.2.2/setup.cfg
-drwxr-xr-x   0 odai       (501) staff       (20)        0 2023-06-14 20:11:15.814608 poplar_logging-1.2.2/src/
-drwxr-xr-x   0 odai       (501) staff       (20)        0 2023-06-14 20:11:15.815609 poplar_logging-1.2.2/src/poplar_logging/
--rw-r--r--   0 odai       (501) staff       (20)       40 2023-06-14 20:05:23.000000 poplar_logging-1.2.2/src/poplar_logging/__init__.py
--rw-r--r--   0 odai       (501) staff       (20)     1507 2023-06-14 19:58:23.000000 poplar_logging-1.2.2/src/poplar_logging/logger.py
-drwxr-xr-x   0 odai       (501) staff       (20)        0 2023-06-14 20:11:15.816424 poplar_logging-1.2.2/src/poplar_logging.egg-info/
--rw-r--r--   0 odai       (501) staff       (20)      861 2023-06-14 20:11:15.000000 poplar_logging-1.2.2/src/poplar_logging.egg-info/PKG-INFO
--rw-r--r--   0 odai       (501) staff       (20)      260 2023-06-14 20:11:15.000000 poplar_logging-1.2.2/src/poplar_logging.egg-info/SOURCES.txt
--rw-r--r--   0 odai       (501) staff       (20)        1 2023-06-14 20:11:15.000000 poplar_logging-1.2.2/src/poplar_logging.egg-info/dependency_links.txt
--rw-r--r--   0 odai       (501) staff       (20)       15 2023-06-14 20:11:15.000000 poplar_logging-1.2.2/src/poplar_logging.egg-info/top_level.txt
+drwxr-xr-x   0 odai       (501) staff       (20)        0 2023-06-15 00:18:36.399218 poplar_logging-1.2.3/
+-rw-r--r--   0 odai       (501) staff       (20)     1070 2023-06-12 04:45:07.000000 poplar_logging-1.2.3/LICENSE
+-rw-r--r--   0 odai       (501) staff       (20)      861 2023-06-15 00:18:36.399081 poplar_logging-1.2.3/PKG-INFO
+-rw-r--r--   0 odai       (501) staff       (20)      427 2023-06-14 19:59:52.000000 poplar_logging-1.2.3/README.md
+-rw-r--r--   0 odai       (501) staff       (20)      427 2023-06-15 00:18:29.000000 poplar_logging-1.2.3/pyproject.toml
+-rw-r--r--   0 odai       (501) staff       (20)       38 2023-06-15 00:18:36.399254 poplar_logging-1.2.3/setup.cfg
+drwxr-xr-x   0 odai       (501) staff       (20)        0 2023-06-15 00:18:36.397608 poplar_logging-1.2.3/src/
+drwxr-xr-x   0 odai       (501) staff       (20)        0 2023-06-15 00:18:36.398365 poplar_logging-1.2.3/src/poplar_logging/
+-rw-r--r--   0 odai       (501) staff       (20)       40 2023-06-14 20:05:23.000000 poplar_logging-1.2.3/src/poplar_logging/__init__.py
+-rw-r--r--   0 odai       (501) staff       (20)     1458 2023-06-15 00:17:54.000000 poplar_logging-1.2.3/src/poplar_logging/logger.py
+drwxr-xr-x   0 odai       (501) staff       (20)        0 2023-06-15 00:18:36.398945 poplar_logging-1.2.3/src/poplar_logging.egg-info/
+-rw-r--r--   0 odai       (501) staff       (20)      861 2023-06-15 00:18:36.000000 poplar_logging-1.2.3/src/poplar_logging.egg-info/PKG-INFO
+-rw-r--r--   0 odai       (501) staff       (20)      260 2023-06-15 00:18:36.000000 poplar_logging-1.2.3/src/poplar_logging.egg-info/SOURCES.txt
+-rw-r--r--   0 odai       (501) staff       (20)        1 2023-06-15 00:18:36.000000 poplar_logging-1.2.3/src/poplar_logging.egg-info/dependency_links.txt
+-rw-r--r--   0 odai       (501) staff       (20)       15 2023-06-15 00:18:36.000000 poplar_logging-1.2.3/src/poplar_logging.egg-info/top_level.txt
```

### Comparing `poplar_logging-1.2.2/LICENSE` & `poplar_logging-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `poplar_logging-1.2.2/PKG-INFO` & `poplar_logging-1.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poplar_logging
-Version: 1.2.2
+Version: 1.2.3
 Summary: Simple Python logging library
 Author-email: Odai Athamneh <heyodai@gmail.com>
 Project-URL: Homepage, https://github.com/heyodai/poplar
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `poplar_logging-1.2.2/src/poplar_logging/logger.py` & `poplar_logging-1.2.3/src/poplar_logging/logger.py`

 * *Files 23% similar despite different names*

```diff
@@ -14,19 +14,19 @@
 
         stream_handler = logging.StreamHandler()
         stream_handler.setLevel(logging.INFO)
         stream_handler.setFormatter(self.formatter)
         self.logger.addHandler(stream_handler)
 
         log_file = os.path.join(self.log_directory, f'{datetime.utcnow().strftime("%Y%m%d%H%M%S")}.log')
-        with open(log_file, mode='w') as file:
-            file_handler = logging.FileHandler(filename=log_file)
-            file_handler.setLevel(logging.INFO)
-            file_handler.setFormatter(self.formatter)
-            self.logger.addHandler(file_handler)
+
+        self.file_handler = logging.FileHandler(filename=log_file)  # Store file handler as instance variable
+        self.file_handler.setLevel(logging.INFO)
+        self.file_handler.setFormatter(self.formatter)
+        self.logger.addHandler(self.file_handler)
 
     def info(self, message):
         self.logger.info(message)
 
     def error(self, message):
         self.logger.error(message)
 
@@ -36,12 +36,9 @@
     def warning(self, message):
         self.logger.warning(message)
 
     def critical(self, message):
         self.logger.critical(message)
 
     def save(self):
-        for handler in self.logger.handlers:
-            if isinstance(handler, logging.FileHandler):
-                handler.flush()
-
-poplar = PoplarLogger()
+        self.file_handler.flush()
+        self.file_handler.close()  # Close the file handler after flushing
```

### Comparing `poplar_logging-1.2.2/src/poplar_logging.egg-info/PKG-INFO` & `poplar_logging-1.2.3/src/poplar_logging.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poplar-logging
-Version: 1.2.2
+Version: 1.2.3
 Summary: Simple Python logging library
 Author-email: Odai Athamneh <heyodai@gmail.com>
 Project-URL: Homepage, https://github.com/heyodai/poplar
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

