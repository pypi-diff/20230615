# Comparing `tmp/ascall-0.1.1.tar.gz` & `tmp/ascall-0.1.2a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ascall-0.1.1.tar", last modified: Tue Sep 20 15:14:47 2022, max compression
+gzip compressed data, was "ascall-0.1.2a0.tar", max compression
```

## Comparing `ascall-0.1.1.tar` & `ascall-0.1.2a0.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0       72 2022-09-19 13:12:25.013470 ascall-0.1.1/.gitignore
--rw-r--r--   0        0        0     1075 2022-09-19 12:40:14.117382 ascall-0.1.1/LICENSE
--rw-r--r--   0        0        0      593 2022-09-20 15:10:44.614240 ascall-0.1.1/README.md
--rw-r--r--   0        0        0     1865 2022-09-20 15:09:19.642236 ascall-0.1.1/ascall.py
--rw-r--r--   0        0        0      492 2022-09-20 15:05:58.954227 ascall-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1012 1970-01-01 00:00:00.000000 ascall-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1075 2022-09-19 12:40:14.117382 ascall-0.1.2a0/LICENSE
+-rw-r--r--   0        0        0      593 2022-09-20 15:10:44.614240 ascall-0.1.2a0/README.md
+-rw-r--r--   0        0        0     1895 2023-03-14 13:45:56.272709 ascall-0.1.2a0/ascall.py
+-rw-r--r--   0        0        0      425 2023-06-15 09:49:08.286979 ascall-0.1.2a0/pyproject.toml
+-rw-r--r--   0        0        0     1162 1970-01-01 00:00:00.000000 ascall-0.1.2a0/PKG-INFO
```

### Comparing `ascall-0.1.1/LICENSE` & `ascall-0.1.2a0/LICENSE`

 * *Files identical despite different names*

### Comparing `ascall-0.1.1/README.md` & `ascall-0.1.2a0/README.md`

 * *Files identical despite different names*

### Comparing `ascall-0.1.1/ascall.py` & `ascall-0.1.2a0/ascall.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,15 +44,16 @@
 
     def __call__(self, func):
         """同步函数装饰器: 装饰同步函数
         """
 
         @functools.wraps(func)
         async def func_magic_async(*args, **kwargs):
-            assert not self.call, f"使用 @{self.__class__.__name__}() 则不允许传 call 参数。"
+            if not self.call:
+                raise ValueError(f"使用 @{self.__class__.__name__}() 则不允许传 call 参数。")
             self.call = func
             self.set_func_coroutine(*args, **kwargs)
             await self
         return func_magic_async
 
 
 ascall = AsCall
```

### Comparing `ascall-0.1.1/PKG-INFO` & `ascall-0.1.2a0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,23 @@
 Metadata-Version: 2.1
 Name: ascall
-Version: 0.1.1
-Summary: ascall用于自动识别同步或异步的可调用对象，然后进行转换并执行异步调用返回结果。
+Version: 0.1.2a0
+Summary: ascall用于将可调用对象自动异步执行。
+Home-page: https://vastxiao.github.io/
+License: MIT
 Keywords: async,asyncio,func,function
-Author-email: vastxiao <vastxiao@gmail.com>
+Author: vastxiao
+Author-email: vastxiao@gmail.com
 Requires-Python: >=3.9
-Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
-Project-URL: Home, https://vastxiao.github.io/
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Description-Content-Type: text/markdown
 
 # ascall
 
 > ascall用于自动识别同步或异步的可调用对象，
 > 然后进行转换并执行异步调用返回结果。
 > 
 > ascall可作为函数运行，也可作为装饰器。
```

