# Comparing `tmp/botboy-3.0.1.tar.gz` & `tmp/botboy-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botboy-3.0.1.tar", last modified: Fri Jan 20 17:36:17 2023, max compression
+gzip compressed data, was "botboy-3.0.2.tar", last modified: Thu Jun 15 13:11:54 2023, max compression
```

## Comparing `botboy-3.0.1.tar` & `botboy-3.0.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1823 2023-01-18 18:08:20.701074 botboy-3.0.1/.gitignore
--rw-r--r--   0        0        0     1082 2022-11-02 20:37:39.058145 botboy-3.0.1/LICENSE
--rw-r--r--   0        0        0      343 2023-01-18 18:06:07.620557 botboy-3.0.1/Makefile
--rw-r--r--   0        0        0     1884 2023-01-18 18:06:07.621706 botboy-3.0.1/README.md
--rw-r--r--   0        0        0       78 2023-01-20 17:35:39.607974 botboy-3.0.1/botboy/__init__.py
--rw-r--r--   0        0        0     5596 2023-01-20 17:34:38.973915 botboy-3.0.1/botboy/core.py
--rw-r--r--   0        0        0        0 2023-01-18 18:06:07.622882 botboy-3.0.1/botboy/tests/__init__.py
--rw-r--r--   0        0        0     2731 2023-01-19 14:37:48.322761 botboy-3.0.1/botboy/tests/botboy_tests.py
--rw-r--r--   0        0        0      390 2023-01-18 18:06:07.624153 botboy-3.0.1/pyproject.toml
--rw-r--r--   0        0        0     2194 1970-01-01 00:00:00.000000 botboy-3.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1823 2023-01-20 17:37:21.046449 botboy-3.0.2/.gitignore
+-rw-r--r--   0        0        0     1082 2022-11-02 20:37:39.058145 botboy-3.0.2/LICENSE
+-rw-r--r--   0        0        0      343 2023-01-18 18:06:07.620557 botboy-3.0.2/Makefile
+-rw-r--r--   0        0        0     1867 2023-06-15 13:08:28.802558 botboy-3.0.2/README.md
+-rw-r--r--   0        0        0       78 2023-06-15 13:09:42.111472 botboy-3.0.2/botboy/__init__.py
+-rw-r--r--   0        0        0     5596 2023-01-20 17:37:21.048633 botboy-3.0.2/botboy/core.py
+-rw-r--r--   0        0        0        0 2023-01-18 18:06:07.622882 botboy-3.0.2/botboy/tests/__init__.py
+-rw-r--r--   0        0        0     2731 2023-01-20 17:37:21.049609 botboy-3.0.2/botboy/tests/botboy_tests.py
+-rw-r--r--   0        0        0      390 2023-01-18 18:06:07.624153 botboy-3.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2177 1970-01-01 00:00:00.000000 botboy-3.0.2/PKG-INFO
```

### Comparing `botboy-3.0.1/.gitignore` & `botboy-3.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `botboy-3.0.1/LICENSE` & `botboy-3.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `botboy-3.0.1/README.md` & `botboy-3.0.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 # BotBoy
 Multithreading &amp; processing worker that executes functions and prints the
 result
 
-**Version 3 Release**
-
 ## Installation
 ```
 pip install botboy
 ```
 
 ## Usage
 ### Instantiation
 ```
-from botboy import BotBoy
+from botboy.core import BotBoy
 
 name = 'Adder' # Name of thread/process
 task = lambda x, y: x + y # Function to run on separate thread/process
 params = [1, 2] # Task arguments
 verbose = True # Logging
 
 bot = BotBoy(name=name, task=task, params=params, verbose=verbose)
@@ -37,15 +35,14 @@
 
 # Turn logging off
 bot.silent()
 
 ```
 
 ### Execute task
-
 ```
 result = bot.execute()
 
 # Wait for execution to finish
 result = bot.execute(wait=True)
 
 # Execute on separate process
@@ -60,27 +57,26 @@
 print(bot.result()) # Result will be None unless task was executed
 
 # Or print all params together
 print(bot)
 ```
 
 ### Store result in a file or provide a path
-
 ```
 # Store result in a file at current directory
 bot.save('test.txt')
 
 # Store result at path
 import os
 bot.save(os.getcwd() + '/test2.txt')
 ```
 
 ### Run multiple tasks with Sequencer
 ```
-from botboy import BotBoy, Sequencer
+from botboy.core import BotBoy, Sequencer
 
 tasks = [lambda x, y: x + y, lambda x, y: x - y, lambda x, y: x * y]
 params = [[1, 2], [3, 4], [5, 6]]
 
 # Create list of BotBoys
 bots = Sequencer.pack(tasks=tasks, params=params, verbose=True)
 
@@ -88,16 +84,14 @@
 seq = Sequencer(bots)
 
 # Retrieve results
 results = seq()
 ```
 
 ## Test
-
 Runs the tests on the BotBoy Module
-
 ```
 make test-init: Test Initialization
 make test-wrapper: Test _wrapper method
 make test-client: Test client methods
 make test-sequencer: Test Sequencer
 ```
```

### Comparing `botboy-3.0.1/botboy/core.py` & `botboy-3.0.2/botboy/core.py`

 * *Files identical despite different names*

### Comparing `botboy-3.0.1/botboy/tests/botboy_tests.py` & `botboy-3.0.2/botboy/tests/botboy_tests.py`

 * *Files identical despite different names*

### Comparing `botboy-3.0.1/PKG-INFO` & `botboy-3.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 Metadata-Version: 2.1
 Name: botboy
-Version: 3.0.1
+Version: 3.0.2
 Summary: Multithreading & processing worker and Sequencer
 Author-email: Marques Traylor <traylorboy@proton.me>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Project-URL: Home, https://github.com/TraylorBoy/BotBoy
 
 # BotBoy
 Multithreading &amp; processing worker that executes functions and prints the
 result
 
-**Version 3 Release**
-
 ## Installation
 ```
 pip install botboy
 ```
 
 ## Usage
 ### Instantiation
 ```
-from botboy import BotBoy
+from botboy.core import BotBoy
 
 name = 'Adder' # Name of thread/process
 task = lambda x, y: x + y # Function to run on separate thread/process
 params = [1, 2] # Task arguments
 verbose = True # Logging
 
 bot = BotBoy(name=name, task=task, params=params, verbose=verbose)
@@ -46,15 +44,14 @@
 
 # Turn logging off
 bot.silent()
 
 ```
 
 ### Execute task
-
 ```
 result = bot.execute()
 
 # Wait for execution to finish
 result = bot.execute(wait=True)
 
 # Execute on separate process
@@ -69,27 +66,26 @@
 print(bot.result()) # Result will be None unless task was executed
 
 # Or print all params together
 print(bot)
 ```
 
 ### Store result in a file or provide a path
-
 ```
 # Store result in a file at current directory
 bot.save('test.txt')
 
 # Store result at path
 import os
 bot.save(os.getcwd() + '/test2.txt')
 ```
 
 ### Run multiple tasks with Sequencer
 ```
-from botboy import BotBoy, Sequencer
+from botboy.core import BotBoy, Sequencer
 
 tasks = [lambda x, y: x + y, lambda x, y: x - y, lambda x, y: x * y]
 params = [[1, 2], [3, 4], [5, 6]]
 
 # Create list of BotBoys
 bots = Sequencer.pack(tasks=tasks, params=params, verbose=True)
 
@@ -97,17 +93,15 @@
 seq = Sequencer(bots)
 
 # Retrieve results
 results = seq()
 ```
 
 ## Test
-
 Runs the tests on the BotBoy Module
-
 ```
 make test-init: Test Initialization
 make test-wrapper: Test _wrapper method
 make test-client: Test client methods
 make test-sequencer: Test Sequencer
 ```
```

