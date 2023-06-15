# Comparing `tmp/concurrent-executor-1.1.1.tar.gz` & `tmp/concurrent-executor-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "concurrent-executor-1.1.1.tar", last modified: Wed Mar  1 02:37:28 2023, max compression
+gzip compressed data, was "concurrent-executor-1.1.2.tar", last modified: Thu Jun 15 01:02:12 2023, max compression
```

## Comparing `concurrent-executor-1.1.1.tar` & `concurrent-executor-1.1.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 02:37:28.371112 concurrent-executor-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-03-01 02:37:21.000000 concurrent-executor-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4641 2023-03-01 02:37:28.371112 concurrent-executor-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4019 2023-03-01 02:37:21.000000 concurrent-executor-1.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 02:37:28.367112 concurrent-executor-1.1.1/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)      850 2023-03-01 02:37:21.000000 concurrent-executor-1.1.1/bin/cexec
--rwxr-xr-x   0 runner    (1001) docker     (123)      848 2023-03-01 02:37:21.000000 concurrent-executor-1.1.1/bin/cssh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 02:37:28.371112 concurrent-executor-1.1.1/concurrent_executor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-01 02:37:21.000000 concurrent-executor-1.1.1/concurrent_executor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-01 02:37:21.000000 concurrent-executor-1.1.1/concurrent_executor/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5673 2023-03-01 02:37:21.000000 concurrent-executor-1.1.1/concurrent_executor/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-03-01 02:37:21.000000 concurrent-executor-1.1.1/concurrent_executor/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-03-01 02:37:21.000000 concurrent-executor-1.1.1/concurrent_executor/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-03-01 02:37:21.000000 concurrent-executor-1.1.1/concurrent_executor/signal_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 02:37:28.371112 concurrent-executor-1.1.1/concurrent_executor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4641 2023-03-01 02:37:28.000000 concurrent-executor-1.1.1/concurrent_executor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-03-01 02:37:28.000000 concurrent-executor-1.1.1/concurrent_executor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-01 02:37:28.000000 concurrent-executor-1.1.1/concurrent_executor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-03-01 02:37:28.000000 concurrent-executor-1.1.1/concurrent_executor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-03-01 02:37:28.000000 concurrent-executor-1.1.1/concurrent_executor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-01 02:37:28.371112 concurrent-executor-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-03-01 02:37:21.000000 concurrent-executor-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 01:02:12.501823 concurrent-executor-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-15 01:02:03.000000 concurrent-executor-1.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4641 2023-06-15 01:02:12.501823 concurrent-executor-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4019 2023-06-15 01:02:03.000000 concurrent-executor-1.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 01:02:12.501823 concurrent-executor-1.1.2/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      850 2023-06-15 01:02:03.000000 concurrent-executor-1.1.2/bin/cexec
+-rwxr-xr-x   0 runner    (1001) docker     (123)      848 2023-06-15 01:02:03.000000 concurrent-executor-1.1.2/bin/cssh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 01:02:12.501823 concurrent-executor-1.1.2/concurrent_executor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 01:02:03.000000 concurrent-executor-1.1.2/concurrent_executor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-15 01:02:03.000000 concurrent-executor-1.1.2/concurrent_executor/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6518 2023-06-15 01:02:03.000000 concurrent-executor-1.1.2/concurrent_executor/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-06-15 01:02:03.000000 concurrent-executor-1.1.2/concurrent_executor/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-06-15 01:02:03.000000 concurrent-executor-1.1.2/concurrent_executor/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-06-15 01:02:03.000000 concurrent-executor-1.1.2/concurrent_executor/signal_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 01:02:12.501823 concurrent-executor-1.1.2/concurrent_executor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4641 2023-06-15 01:02:12.000000 concurrent-executor-1.1.2/concurrent_executor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-15 01:02:12.000000 concurrent-executor-1.1.2/concurrent_executor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 01:02:12.000000 concurrent-executor-1.1.2/concurrent_executor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-15 01:02:12.000000 concurrent-executor-1.1.2/concurrent_executor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-15 01:02:12.000000 concurrent-executor-1.1.2/concurrent_executor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 01:02:12.501823 concurrent-executor-1.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-06-15 01:02:03.000000 concurrent-executor-1.1.2/setup.py
```

### Comparing `concurrent-executor-1.1.1/LICENSE` & `concurrent-executor-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `concurrent-executor-1.1.1/PKG-INFO` & `concurrent-executor-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: concurrent-executor
-Version: 1.1.1
+Version: 1.1.2
 Summary: Executing commands using SSH concurrently on multiple hosts
 Home-page: https://github.com/DCsunset/concurrent-executor
 Author: DCsunset
 Author-email: DCsunset@protonmail.com
 License: AGPL-3.0
 Classifier: Environment :: Console
 Classifier: Topic :: System :: Networking
```

### Comparing `concurrent-executor-1.1.1/README.md` & `concurrent-executor-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `concurrent-executor-1.1.1/bin/cexec` & `concurrent-executor-1.1.2/bin/cexec`

 * *Files identical despite different names*

### Comparing `concurrent-executor-1.1.1/bin/cssh` & `concurrent-executor-1.1.2/bin/cssh`

 * *Files identical despite different names*

### Comparing `concurrent-executor-1.1.1/concurrent_executor/cli.py` & `concurrent-executor-1.1.2/concurrent_executor/cli.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,18 +21,29 @@
 from rich.console import Console
 import argparse
 import asyncio
 import sys
 
 console = Console(highlight=False)
 err_console = Console(highlight=False, stderr=True)
+
+async def output_messages(output_queue: asyncio.Queue, stdout_transformer, stderr_transformer):
+	while True:
+		msg = await output_queue.get()
+		if msg == None:
+			break
+		index, out, is_stdout = msg
+		if is_stdout:
+			console.print(stdout_transformer(index, out))
+		else:
+			err_console.print(stderr_transformer(index, out))
+
 	
 # handle I/O, signals and return codes
-async def handle_executor(executor: Executor, stdout_transformer, stderr_transformer):
-	
+async def handle_executor(executor: Executor, output_queue: asyncio.Queue()):
 	def signal_callback(counter):
 		if counter == 1:
 			console.print(f"[bright_yellow]Terminating all processes...[/bright_yellow]")
 			executor.terminate()
 		else:
 			# send more than twice to kill all processes
 			console.print(f"[bright_red]Killing all processes...[/bright_red]")
@@ -48,18 +59,18 @@
 	stderr = stream.map(executor.get_stderr(), lambda v: (v, False))
 	
 	# use async with to ensure it is cleaned up correctly
 	async with stream.merge(stdout, stderr).stream() as s:
 		async for output, is_stdout in s:
 			index, out = output
 			out = out.decode().rstrip()
-			if is_stdout:
-				console.print(stdout_transformer(index, out))
-			else:
-				err_console.print(stderr_transformer(index, out))
+			await output_queue.put((index, out, is_stdout))
+			
+	# end of output
+	await output_queue.put(None)
 	
 	# return code
 	ret = 0
 	# wait until all finished
 	ret_codes = await executor.wait()
 	if not stdin_task.done():
 		stdin_task.cancel()
@@ -108,23 +119,28 @@
 			host_len = len(h)
 
 	executor = SshExecutor(
 		hosts,
 		sshOptions=args.options,
 		sshBin=args.bin
 	)
-
 	await executor.run(" ".join(args.cmd))
-
-	return await handle_executor(
-		executor,
+	
+	# use another task for output to preventing non-blocking IO error
+	# (store it quickly in the queue to prevent output from overflowing)
+	output_queue = asyncio.Queue()
+	output_task = asyncio.create_task(output_messages(
+		output_queue,
 		stdout_transformer=lambda i, out: f"[bright_black]{hosts[i]:{host_len}} |[/bright_black] {out}",
 		stderr_transformer=lambda i, out: f"[bright_black]{hosts[i]:{host_len}}[/bright_black] [bright_red]|[/bright_red] {out}",
-	)
-	
+	))
+
+	ret = await handle_executor(executor, output_queue)
+	await output_task
+	return ret
 
 # concurrent exec
 async def cexec_main():
 	parser = argparse.ArgumentParser(
 		formatter_class=argparse.ArgumentDefaultsHelpFormatter,
 		description="Executing multiple commands concurrently using template command",
 	)
@@ -153,16 +169,22 @@
 	# The max var length (for padding)
 	var_len = 0
 	for v in variables:
 		if len(v) > var_len:
 			var_len = len(v)
 
 	executor = Executor(variables)
-
 	await executor.run(" ".join(args.template))
 
-	return await handle_executor(
-		executor,
+	# use another task for output to preventing non-blocking IO error
+	# (store it quickly in the queue to prevent output from overflowing)
+	output_queue = asyncio.Queue()
+	output_task = asyncio.create_task(output_messages(
+		output_queue,
 		stdout_transformer=lambda i, out: f"[bright_black]{variables[i]:{var_len}} |[/bright_black] {out}",
 		stderr_transformer=lambda i, out: f"[bright_black]{variables[i]:{var_len}}[/bright_black] [bright_red]|[/bright_red] {out}",
-	)
-		
+	))
+	
+	ret = await handle_executor(executor, output_queue)
+	await output_task
+	return ret
+
```

### Comparing `concurrent-executor-1.1.1/concurrent_executor/executor.py` & `concurrent-executor-1.1.2/concurrent_executor/executor.py`

 * *Files identical despite different names*

### Comparing `concurrent-executor-1.1.1/concurrent_executor/io.py` & `concurrent-executor-1.1.2/concurrent_executor/io.py`

 * *Files identical despite different names*

### Comparing `concurrent-executor-1.1.1/concurrent_executor/signal_handler.py` & `concurrent-executor-1.1.2/concurrent_executor/signal_handler.py`

 * *Files identical despite different names*

### Comparing `concurrent-executor-1.1.1/concurrent_executor.egg-info/PKG-INFO` & `concurrent-executor-1.1.2/concurrent_executor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: concurrent-executor
-Version: 1.1.1
+Version: 1.1.2
 Summary: Executing commands using SSH concurrently on multiple hosts
 Home-page: https://github.com/DCsunset/concurrent-executor
 Author: DCsunset
 Author-email: DCsunset@protonmail.com
 License: AGPL-3.0
 Classifier: Environment :: Console
 Classifier: Topic :: System :: Networking
```

### Comparing `concurrent-executor-1.1.1/setup.py` & `concurrent-executor-1.1.2/setup.py`

 * *Files identical despite different names*

