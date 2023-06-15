# Comparing `tmp/oxalis-0.6.2.tar.gz` & `tmp/oxalis-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oxalis-0.6.2.tar", max compression
+gzip compressed data, was "oxalis-0.6.3.tar", max compression
```

## Comparing `oxalis-0.6.2.tar` & `oxalis-0.6.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1065 2022-06-07 12:05:40.532331 oxalis-0.6.2/LICENSE
--rw-r--r--   0        0        0     6896 2023-04-20 05:15:02.504528 oxalis-0.6.2/README.md
--rw-r--r--   0        0        0       22 2022-06-03 10:29:06.678568 oxalis-0.6.2/oxalis/__init__.py
--rw-r--r--   0        0        0    11615 2023-05-12 06:41:48.719578 oxalis-0.6.2/oxalis/amqp.py
--rw-r--r--   0        0        0     7310 2023-05-12 06:41:48.719578 oxalis-0.6.2/oxalis/base.py
--rw-r--r--   0        0        0     1978 2023-04-28 02:27:00.905636 oxalis-0.6.2/oxalis/beater.py
--rw-r--r--   0        0        0     5917 2023-06-14 07:44:58.843783 oxalis-0.6.2/oxalis/kafka.py
--rw-r--r--   0        0        0     3538 2023-05-12 06:41:48.719578 oxalis-0.6.2/oxalis/pool.py
--rw-r--r--   0        0        0     7448 2023-05-12 06:41:48.719578 oxalis-0.6.2/oxalis/redis.py
--rw-r--r--   0        0        0      884 2023-06-14 07:19:57.315599 oxalis-0.6.2/pyproject.toml
--rw-r--r--   0        0        0     7653 1970-01-01 00:00:00.000000 oxalis-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0     1065 2022-06-07 12:05:40.532331 oxalis-0.6.3/LICENSE
+-rw-r--r--   0        0        0     6896 2023-04-20 05:15:02.504528 oxalis-0.6.3/README.md
+-rw-r--r--   0        0        0       22 2022-06-03 10:29:06.678568 oxalis-0.6.3/oxalis/__init__.py
+-rw-r--r--   0        0        0    11619 2023-06-15 05:50:52.211402 oxalis-0.6.3/oxalis/amqp.py
+-rw-r--r--   0        0        0     7314 2023-06-15 05:41:22.005127 oxalis-0.6.3/oxalis/base.py
+-rw-r--r--   0        0        0     1978 2023-04-28 02:27:00.905636 oxalis-0.6.3/oxalis/beater.py
+-rw-r--r--   0        0        0     5917 2023-06-14 07:44:58.843783 oxalis-0.6.3/oxalis/kafka.py
+-rw-r--r--   0        0        0     3542 2023-06-15 05:41:58.004260 oxalis-0.6.3/oxalis/pool.py
+-rw-r--r--   0        0        0     7448 2023-05-12 06:41:48.719578 oxalis-0.6.3/oxalis/redis.py
+-rw-r--r--   0        0        0      884 2023-06-15 05:50:57.851266 oxalis-0.6.3/pyproject.toml
+-rw-r--r--   0        0        0     7653 1970-01-01 00:00:00.000000 oxalis-0.6.3/PKG-INFO
```

### Comparing `oxalis-0.6.2/LICENSE` & `oxalis-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `oxalis-0.6.2/README.md` & `oxalis-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `oxalis-0.6.2/oxalis/amqp.py` & `oxalis-0.6.3/oxalis/amqp.py`

 * *Files 0% similar despite different names*

```diff
@@ -281,15 +281,15 @@
     async def exec_task(self, task: Task, *args, **task_kwargs):
         message: aio_pika.IncomingMessage = args[0]
         task_args = args[1:]
         if not task.ack_later:
             await message.ack()
         try:
             await super().exec_task(task, *task_args, **task_kwargs)
-        except Exception as e:
+        except BaseException as e:
             if task.reject:
                 await message.reject(requeue=task.reject_requeue)
             elif task.ack_always and task.ack_later:
                 await message.ack()
             raise e from None
         if task.ack_later:
             await message.ack()
```

### Comparing `oxalis-0.6.2/oxalis/base.py` & `oxalis-0.6.3/oxalis/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -229,15 +229,15 @@
             timeout=self.pool.timeout if task.timeout == -1 else task.timeout,
         )
 
     async def on_message_receive(self, content: bytes, *_):
         """should not raise exception"""
         try:
             return await self.load_and_execute_task(content, *_)
-        except Exception as e:
+        except BaseException as e:
             logger.exception(e)
 
     def close(self, *_):
         """Close self but wait pool"""
         if not self.is_worker:
             return
         self._on_close_signal_count += 1
```

### Comparing `oxalis-0.6.2/oxalis/beater.py` & `oxalis-0.6.3/oxalis/beater.py`

 * *Files identical despite different names*

### Comparing `oxalis-0.6.2/oxalis/kafka.py` & `oxalis-0.6.3/oxalis/kafka.py`

 * *Files identical despite different names*

### Comparing `oxalis-0.6.2/oxalis/pool.py` & `oxalis-0.6.3/oxalis/pool.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,15 +88,15 @@
         self.close(force=True)
 
     def check_future(self, f: asyncio.Future):
         e = f.exception()
         if e:
             try:
                 raise e
-            except Exception:
+            except BaseException:
                 logger.exception(e)
 
     def on_future_done(self, f: asyncio.Future):
         self.running_count -= 1
         self.done_queue.put_nowait(f)
         self.check_future(f)
         self.futures.remove(f)
```

### Comparing `oxalis-0.6.2/oxalis/redis.py` & `oxalis-0.6.3/oxalis/redis.py`

 * *Files identical despite different names*

### Comparing `oxalis-0.6.2/pyproject.toml` & `oxalis-0.6.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "oxalis"
-version = "0.6.2"
+version = "0.6.3"
 description = "Distributed async task/job queue"
 authors = ["strongbugman <strongbugman@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 classifiers=[
     "Environment :: Console",
     "Programming Language :: Python :: 3.10",
```

### Comparing `oxalis-0.6.2/PKG-INFO` & `oxalis-0.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oxalis
-Version: 0.6.2
+Version: 0.6.3
 Summary: Distributed async task/job queue
 License: MIT
 Author: strongbugman
 Author-email: strongbugman@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
```

