# Comparing `tmp/aslooper-1.1.4.tar.gz` & `tmp/aslooper-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aslooper-1.1.4.tar", last modified: Sat Dec  3 16:24:51 2022, max compression
+gzip compressed data, was "aslooper-1.2.1.tar", max compression
```

## Comparing `aslooper-1.1.4.tar` & `aslooper-1.2.1.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0       72 2022-05-31 11:36:32.266107 aslooper-1.1.4/.gitignore
--rw-r--r--   0        0        0     1075 2022-05-31 11:36:32.266107 aslooper-1.1.4/LICENSE
--rw-r--r--   0        0        0      802 2022-09-18 04:35:36.407702 aslooper-1.1.4/README.md
--rw-r--r--   0        0        0      936 2022-11-24 13:02:20.629690 aslooper-1.1.4/README_zh.md
--rw-r--r--   0        0        0     6168 2022-12-03 16:22:46.526483 aslooper-1.1.4/aslooper.py
--rw-r--r--   0        0        0      510 2022-10-20 11:28:30.326364 aslooper-1.1.4/pyproject.toml
--rw-r--r--   0        0        0     1124 1970-01-01 00:00:00.000000 aslooper-1.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1075 2022-05-31 11:36:32.266107 aslooper-1.2.1/LICENSE
+-rw-r--r--   0        0        0      802 2022-09-18 04:35:36.407702 aslooper-1.2.1/README.md
+-rw-r--r--   0        0        0      936 2022-11-24 13:02:20.629690 aslooper-1.2.1/README_zh.md
+-rw-r--r--   0        0        0     6462 2023-06-15 14:21:21.775265 aslooper-1.2.1/aslooper.py
+-rw-r--r--   0        0        0      715 2023-06-15 14:52:40.058392 aslooper-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1258 1970-01-01 00:00:00.000000 aslooper-1.2.1/PKG-INFO
```

### Comparing `aslooper-1.1.4/LICENSE` & `aslooper-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aslooper-1.1.4/README.md` & `aslooper-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `aslooper-1.1.4/README_zh.md` & `aslooper-1.2.1/README_zh.md`

 * *Files identical despite different names*

### Comparing `aslooper-1.1.4/aslooper.py` & `aslooper-1.2.1/aslooper.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,23 +32,22 @@
         await asyncio.sleep(1)
 
 
 uvloop.install()
 asyncio.run(main())
 """
 
-__version__ = "1.1.4"
-
 __all__ = ["looper"]
 
 
 import asyncio
 import functools
 from signal import SIGINT, SIGTERM
-from typing import Callable
+from typing import Callable, Awaitable
+from typing import TypeVar, ParamSpec
 # from types import FunctionType
 
 
 # def __cancel_all_tasks():
 #     """取消所有任务
 #
 #     :return:
@@ -112,14 +111,18 @@
 #             return await func(*args, **kwargs)
 #         except asyncio.CancelledError:
 #             print("Exit!")
 #
 #     return loop_signal_handler
 
 
+FuncReturnType = TypeVar('FuncReturnType')
+FuncParamType = ParamSpec('FuncParamType')
+
+
 class Looper:
     """装饰器对象，用来装饰异步函数，用于取消异步任务。"""
 
     def __init__(self, call: Callable = None, *,
                  debug: bool = True):
         """（call 暂时只能支持同步函数，异步函数没研究出来 - -！）"""
         self.call = call
@@ -149,39 +152,41 @@
             # elif isinstance(self.call, FunctionType):
             #     self.call()
             # elif callable(self.call):
             self.call()
         else:
             self.print(f"[Error Call] {self.call}")
 
-    async def run_func(self):
+    async def run_func(self) -> FuncReturnType:
         """用于__await__执行"""
         try:
             return await self.func_coroutine
         except asyncio.CancelledError:
             self.print("Exit!")
 
     def __await__(self):
         """
         必须定义这个方法才能直接 await 这个类的对象
         并且，返回值必须是一个 iterator，这里直接
         使用 async 函数的内置方法 __await__()
         """
         return self.run_func().__await__()
 
-    def __call__(self, func):
+    def __call__(self,
+                 func: Callable[FuncParamType, FuncReturnType]
+                 ) -> Callable[..., Awaitable[FuncReturnType]]:
         """异步函数装饰器:
         用来捕获 SIGINT, SIGTERM 信号后取消所有运行任务，退出运行不报错。
         """
         if not asyncio.iscoroutinefunction(func):
             raise TypeError(f"{func} is not coroutine function.")
         self.func = func
 
         @functools.wraps(func)
-        async def loop_signal_handler(*args, **kwargs):
+        async def loop_signal_handler(*args: FuncParamType.args, **kwargs: FuncParamType.kwargs):
             loop = asyncio.get_running_loop()
             # Add signal
             for signal in (SIGINT, SIGTERM):
                 try:
                     loop.add_signal_handler(
                         signal,
                         # lambda: asyncio.create_task(__cancel_all_tasks(), name="signal_handler_call")
```

### Comparing `aslooper-1.1.4/PKG-INFO` & `aslooper-1.2.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 Metadata-Version: 2.1
 Name: aslooper
-Version: 1.1.4
-Summary: looper-佛跳墙活套
+Version: 1.2.1
+Summary: looper-佛跳墙活套：捕获asyncio报错。
+Home-page: https://vastxiao.github.io/
+License: MIT
 Keywords: async,asyncio,loop
-Author-email: vastxiao <vastxiao@gmail.com>
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
+Author: vastxiao
+Author-email: vastxiao@gmail.com
+Requires-Python: >=3.11
 Classifier: License :: OSI Approved :: MIT License
-Project-URL: Author, https://vastxiao.github.io/
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.11
+Description-Content-Type: text/markdown
 
 # aslooper
 
 > looper
 > Used to cancel all running tasks after catching SIGINT, SIGTERM signals,
 > Quit running without raise asyncio cancelled error.
```

