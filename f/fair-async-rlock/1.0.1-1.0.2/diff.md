# Comparing `tmp/fair_async_rlock-1.0.1.tar.gz` & `tmp/fair_async_rlock-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fair_async_rlock-1.0.1.tar", last modified: Thu Jun 15 00:13:40 2023, max compression
+gzip compressed data, was "fair_async_rlock-1.0.2.tar", last modified: Thu Jun 15 00:21:19 2023, max compression
```

## Comparing `fair_async_rlock-1.0.1.tar` & `fair_async_rlock-1.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-06-15 00:13:39.998697 fair_async_rlock-1.0.1/
--rw-rw-r--   0 albert    (1000) albert    (1000)     1077 2023-06-14 11:40:02.000000 fair_async_rlock-1.0.1/LICENSE
--rw-rw-r--   0 albert    (1000) albert    (1000)     4862 2023-06-15 00:13:39.998697 fair_async_rlock-1.0.1/PKG-INFO
--rw-rw-r--   0 albert    (1000) albert    (1000)     4340 2023-06-15 00:12:42.000000 fair_async_rlock-1.0.1/README.md
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-06-15 00:13:39.994697 fair_async_rlock-1.0.1/fair_async_rlock/
--rw-rw-r--   0 albert    (1000) albert    (1000)        0 2023-06-14 11:43:19.000000 fair_async_rlock-1.0.1/fair_async_rlock/__init__.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     1969 2023-06-14 11:44:15.000000 fair_async_rlock-1.0.1/fair_async_rlock/fair_async_rlock.py
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-06-15 00:13:39.998697 fair_async_rlock-1.0.1/fair_async_rlock/tests/
--rw-rw-r--   0 albert    (1000) albert    (1000)        0 2023-06-14 11:43:19.000000 fair_async_rlock-1.0.1/fair_async_rlock/tests/__init__.py
--rw-rw-r--   0 albert    (1000) albert    (1000)    12069 2023-06-14 11:51:23.000000 fair_async_rlock-1.0.1/fair_async_rlock/tests/test_fair_async_rlock.py
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-06-15 00:13:39.994697 fair_async_rlock-1.0.1/fair_async_rlock.egg-info/
--rw-rw-r--   0 albert    (1000) albert    (1000)     4862 2023-06-15 00:13:39.000000 fair_async_rlock-1.0.1/fair_async_rlock.egg-info/PKG-INFO
--rw-rw-r--   0 albert    (1000) albert    (1000)      366 2023-06-15 00:13:39.000000 fair_async_rlock-1.0.1/fair_async_rlock.egg-info/SOURCES.txt
--rw-rw-r--   0 albert    (1000) albert    (1000)        1 2023-06-15 00:13:39.000000 fair_async_rlock-1.0.1/fair_async_rlock.egg-info/dependency_links.txt
--rw-rw-r--   0 albert    (1000) albert    (1000)       17 2023-06-15 00:13:39.000000 fair_async_rlock-1.0.1/fair_async_rlock.egg-info/top_level.txt
--rw-rw-r--   0 albert    (1000) albert    (1000)      103 2022-10-13 02:52:05.000000 fair_async_rlock-1.0.1/pyproject.toml
--rw-rw-r--   0 albert    (1000) albert    (1000)       38 2023-06-15 00:13:39.998697 fair_async_rlock-1.0.1/setup.cfg
--rwxrwxr-x   0 albert    (1000) albert    (1000)      953 2023-06-14 23:58:07.000000 fair_async_rlock-1.0.1/setup.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-06-15 00:21:19.467517 fair_async_rlock-1.0.2/
+-rw-rw-r--   0 albert    (1000) albert    (1000)     1077 2023-06-14 11:40:02.000000 fair_async_rlock-1.0.2/LICENSE
+-rw-rw-r--   0 albert    (1000) albert    (1000)     4980 2023-06-15 00:21:19.467517 fair_async_rlock-1.0.2/PKG-INFO
+-rw-rw-r--   0 albert    (1000) albert    (1000)     4457 2023-06-15 00:19:33.000000 fair_async_rlock-1.0.2/README.md
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-06-15 00:21:19.467517 fair_async_rlock-1.0.2/fair_async_rlock/
+-rw-rw-r--   0 albert    (1000) albert    (1000)       48 2023-06-15 00:14:55.000000 fair_async_rlock-1.0.2/fair_async_rlock/__init__.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     1998 2023-06-15 00:14:55.000000 fair_async_rlock-1.0.2/fair_async_rlock/fair_async_rlock.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-06-15 00:21:19.467517 fair_async_rlock-1.0.2/fair_async_rlock/tests/
+-rw-rw-r--   0 albert    (1000) albert    (1000)        0 2023-06-14 11:43:19.000000 fair_async_rlock-1.0.2/fair_async_rlock/tests/__init__.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)    12053 2023-06-15 00:19:33.000000 fair_async_rlock-1.0.2/fair_async_rlock/tests/test_fair_async_rlock.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-06-15 00:21:19.467517 fair_async_rlock-1.0.2/fair_async_rlock.egg-info/
+-rw-rw-r--   0 albert    (1000) albert    (1000)     4980 2023-06-15 00:21:19.000000 fair_async_rlock-1.0.2/fair_async_rlock.egg-info/PKG-INFO
+-rw-rw-r--   0 albert    (1000) albert    (1000)      366 2023-06-15 00:21:19.000000 fair_async_rlock-1.0.2/fair_async_rlock.egg-info/SOURCES.txt
+-rw-rw-r--   0 albert    (1000) albert    (1000)        1 2023-06-15 00:21:19.000000 fair_async_rlock-1.0.2/fair_async_rlock.egg-info/dependency_links.txt
+-rw-rw-r--   0 albert    (1000) albert    (1000)       17 2023-06-15 00:21:19.000000 fair_async_rlock-1.0.2/fair_async_rlock.egg-info/top_level.txt
+-rw-rw-r--   0 albert    (1000) albert    (1000)      103 2022-10-13 02:52:05.000000 fair_async_rlock-1.0.2/pyproject.toml
+-rw-rw-r--   0 albert    (1000) albert    (1000)       38 2023-06-15 00:21:19.467517 fair_async_rlock-1.0.2/setup.cfg
+-rwxrwxr-x   0 albert    (1000) albert    (1000)      953 2023-06-15 00:16:05.000000 fair_async_rlock-1.0.2/setup.py
```

### Comparing `fair_async_rlock-1.0.1/LICENSE` & `fair_async_rlock-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fair_async_rlock-1.0.1/PKG-INFO` & `fair_async_rlock-1.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 Metadata-Version: 2.1
 Name: fair_async_rlock
-Version: 1.0.1
+Version: 1.0.2
 Summary: A well-tested implementation of a fair asynchronous RLock for concurrent programming.
 Home-page: https://github.com/Joshuaalbert/FairAsyncRLock
 Author: Joshua G. Albert
 Author-email: albert@strw.leidenuniv.nl
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # FairAsyncRLock
+
 [![Python](https://img.shields.io/pypi/pyversions/fair_async_rlock.svg)](https://badge.fury.io/py/fair_async_rlock)
 [![PyPI](https://badge.fury.io/py/fair_async_rlock.svg)](https://badge.fury.io/py/fair_async_rlock)
 
-Main Status: ![Workflow name](https://github.com/JoshuaAlbert/FairAsyncRLock/actions/workflows/unittests.yml/badge.svg?branch=main)
+Main
+Status: ![Workflow name](https://github.com/JoshuaAlbert/FairAsyncRLock/actions/workflows/unittests.yml/badge.svg?branch=main)
 
-Develop Status: ![Workflow name](https://github.com/JoshuaAlbert/FairAsyncRLock/actions/workflows/unittests.yml/badge.svg?branch=develop)
+Develop
+Status: ![Workflow name](https://github.com/JoshuaAlbert/FairAsyncRLock/actions/workflows/unittests.yml/badge.svg?branch=develop)
 
 This is a well-tested standalone implementation of a fair reentrant lock for conncurrent programming with asyncio.
 This was built
 because [python decided not to support RLock in asyncio](https://discuss.python.org/t/asyncio-rlock-reentrant-locks-for-async-python/21509),
 their [argument](https://discuss.python.org/t/asyncio-rlock-reentrant-locks-for-async-python/21509/2) being that every
 extra bit of functionality adds to maintenance cost.
 
@@ -51,15 +54,15 @@
 
 * **Task ownership**: If your code logic depends on which task owns a lock, reentrant locks can be
   helpful. They inherently track ownership since they are tied to the task that acquired them first.
 
 This code demonstrates the reentrant property:
 
 ```python
-from fair_async_rlock.fair_async_rlock import FairAsyncRLock
+from fair_async_rlock import FairAsyncRLock
 
 
 async def reentrant():
     lock = FairAsyncRLock()
     async with lock:
         async with lock:  # This will not block, whereas it would with asyncio.Lock
             assert True
@@ -71,15 +74,15 @@
 lock indefinitely while others after it acquire the lock, which can happen with standard asyncio Locks.
 
 This code demonstrates fairness:
 
 ```python
 import asyncio
 
-from fair_async_rlock.fair_async_rlock import FairAsyncRLock
+from fair_async_rlock import FairAsyncRLock
 
 
 async def fairness():
     lock = FairAsyncRLock()
     num_tasks = 1000
     order = []
 
@@ -103,7 +106,12 @@
 
 It's also important to note the potential downsides of using a reentrant lock.
 For one, they can hide bugs in code that isn't properly synchronized, since
 the same task can acquire a reentrant lock multiple times without issue.
 
 **_Non-reentrant locks are often simpler and can expose synchronization bugs more easily, so you should only use a
 reentrant lock if you have a specific need for it._**
+
+### Performance
+
+The performance is about 50% slower than `asyncio.Lock`, i.e. overhead of sequential locks is about 3/2 of same
+with `asyncio.Lock`.
```

### Comparing `fair_async_rlock-1.0.1/README.md` & `fair_async_rlock-1.0.2/fair_async_rlock.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,31 @@
+Metadata-Version: 2.1
+Name: fair-async-rlock
+Version: 1.0.2
+Summary: A well-tested implementation of a fair asynchronous RLock for concurrent programming.
+Home-page: https://github.com/Joshuaalbert/FairAsyncRLock
+Author: Joshua G. Albert
+Author-email: albert@strw.leidenuniv.nl
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # FairAsyncRLock
+
 [![Python](https://img.shields.io/pypi/pyversions/fair_async_rlock.svg)](https://badge.fury.io/py/fair_async_rlock)
 [![PyPI](https://badge.fury.io/py/fair_async_rlock.svg)](https://badge.fury.io/py/fair_async_rlock)
 
-Main Status: ![Workflow name](https://github.com/JoshuaAlbert/FairAsyncRLock/actions/workflows/unittests.yml/badge.svg?branch=main)
+Main
+Status: ![Workflow name](https://github.com/JoshuaAlbert/FairAsyncRLock/actions/workflows/unittests.yml/badge.svg?branch=main)
 
-Develop Status: ![Workflow name](https://github.com/JoshuaAlbert/FairAsyncRLock/actions/workflows/unittests.yml/badge.svg?branch=develop)
+Develop
+Status: ![Workflow name](https://github.com/JoshuaAlbert/FairAsyncRLock/actions/workflows/unittests.yml/badge.svg?branch=develop)
 
 This is a well-tested standalone implementation of a fair reentrant lock for conncurrent programming with asyncio.
 This was built
 because [python decided not to support RLock in asyncio](https://discuss.python.org/t/asyncio-rlock-reentrant-locks-for-async-python/21509),
 their [argument](https://discuss.python.org/t/asyncio-rlock-reentrant-locks-for-async-python/21509/2) being that every
 extra bit of functionality adds to maintenance cost.
 
@@ -37,15 +54,15 @@
 
 * **Task ownership**: If your code logic depends on which task owns a lock, reentrant locks can be
   helpful. They inherently track ownership since they are tied to the task that acquired them first.
 
 This code demonstrates the reentrant property:
 
 ```python
-from fair_async_rlock.fair_async_rlock import FairAsyncRLock
+from fair_async_rlock import FairAsyncRLock
 
 
 async def reentrant():
     lock = FairAsyncRLock()
     async with lock:
         async with lock:  # This will not block, whereas it would with asyncio.Lock
             assert True
@@ -57,15 +74,15 @@
 lock indefinitely while others after it acquire the lock, which can happen with standard asyncio Locks.
 
 This code demonstrates fairness:
 
 ```python
 import asyncio
 
-from fair_async_rlock.fair_async_rlock import FairAsyncRLock
+from fair_async_rlock import FairAsyncRLock
 
 
 async def fairness():
     lock = FairAsyncRLock()
     num_tasks = 1000
     order = []
 
@@ -89,7 +106,12 @@
 
 It's also important to note the potential downsides of using a reentrant lock.
 For one, they can hide bugs in code that isn't properly synchronized, since
 the same task can acquire a reentrant lock multiple times without issue.
 
 **_Non-reentrant locks are often simpler and can expose synchronization bugs more easily, so you should only use a
 reentrant lock if you have a specific need for it._**
+
+### Performance
+
+The performance is about 50% slower than `asyncio.Lock`, i.e. overhead of sequential locks is about 3/2 of same
+with `asyncio.Lock`.
```

### Comparing `fair_async_rlock-1.0.1/fair_async_rlock/fair_async_rlock.py` & `fair_async_rlock-1.0.2/fair_async_rlock/fair_async_rlock.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import asyncio
 from collections import deque
 
+__all__ = ['FairAsyncRLock']
 
 class FairAsyncRLock:
     """
     A fair reentrant lock for async programming. Fair means that it respects the order of acquisition.
     """
 
     def __init__(self):
```

### Comparing `fair_async_rlock-1.0.1/fair_async_rlock/tests/test_fair_async_rlock.py` & `fair_async_rlock-1.0.2/fair_async_rlock/tests/test_fair_async_rlock.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import asyncio
 from time import monotonic_ns, perf_counter
 
 import pytest
 
-from fair_async_rlock.fair_async_rlock import FairAsyncRLock
+from fair_async_rlock import FairAsyncRLock
 
 
 @pytest.mark.asyncio
 async def test_reentrant():
     lock = FairAsyncRLock()
     async with lock:
         async with lock:  # This should not block
@@ -250,15 +250,15 @@
     print(f"Time to complete {num_tasks} tasks with asyncio.Lock: {duration_asyncio} seconds")
     # We find that it's about the same performance as asyncio.Lock.
     perf_ratio = duration_fair / duration_asyncio
     if perf_ratio > 1:
         print(f"Relative performance: {(perf_ratio - 1) * 100:0.1f}% slower")
     else:
         print(f"Relative performance: {(1 - perf_ratio) * 100:0.1f}% faster")
-    assert perf_ratio < 2. # Solid upper bound
+    assert perf_ratio < 2.  # Solid upper bound
 
 
 @pytest.mark.asyncio
 async def test_lock_released_on_exception():
     lock = FairAsyncRLock()
     with pytest.raises(Exception):
         async with lock:
```

### Comparing `fair_async_rlock-1.0.1/fair_async_rlock.egg-info/PKG-INFO` & `fair_async_rlock-1.0.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,17 @@
-Metadata-Version: 2.1
-Name: fair-async-rlock
-Version: 1.0.1
-Summary: A well-tested implementation of a fair asynchronous RLock for concurrent programming.
-Home-page: https://github.com/Joshuaalbert/FairAsyncRLock
-Author: Joshua G. Albert
-Author-email: albert@strw.leidenuniv.nl
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # FairAsyncRLock
+
 [![Python](https://img.shields.io/pypi/pyversions/fair_async_rlock.svg)](https://badge.fury.io/py/fair_async_rlock)
 [![PyPI](https://badge.fury.io/py/fair_async_rlock.svg)](https://badge.fury.io/py/fair_async_rlock)
 
-Main Status: ![Workflow name](https://github.com/JoshuaAlbert/FairAsyncRLock/actions/workflows/unittests.yml/badge.svg?branch=main)
+Main
+Status: ![Workflow name](https://github.com/JoshuaAlbert/FairAsyncRLock/actions/workflows/unittests.yml/badge.svg?branch=main)
 
-Develop Status: ![Workflow name](https://github.com/JoshuaAlbert/FairAsyncRLock/actions/workflows/unittests.yml/badge.svg?branch=develop)
+Develop
+Status: ![Workflow name](https://github.com/JoshuaAlbert/FairAsyncRLock/actions/workflows/unittests.yml/badge.svg?branch=develop)
 
 This is a well-tested standalone implementation of a fair reentrant lock for conncurrent programming with asyncio.
 This was built
 because [python decided not to support RLock in asyncio](https://discuss.python.org/t/asyncio-rlock-reentrant-locks-for-async-python/21509),
 their [argument](https://discuss.python.org/t/asyncio-rlock-reentrant-locks-for-async-python/21509/2) being that every
 extra bit of functionality adds to maintenance cost.
 
@@ -51,15 +40,15 @@
 
 * **Task ownership**: If your code logic depends on which task owns a lock, reentrant locks can be
   helpful. They inherently track ownership since they are tied to the task that acquired them first.
 
 This code demonstrates the reentrant property:
 
 ```python
-from fair_async_rlock.fair_async_rlock import FairAsyncRLock
+from fair_async_rlock import FairAsyncRLock
 
 
 async def reentrant():
     lock = FairAsyncRLock()
     async with lock:
         async with lock:  # This will not block, whereas it would with asyncio.Lock
             assert True
@@ -71,15 +60,15 @@
 lock indefinitely while others after it acquire the lock, which can happen with standard asyncio Locks.
 
 This code demonstrates fairness:
 
 ```python
 import asyncio
 
-from fair_async_rlock.fair_async_rlock import FairAsyncRLock
+from fair_async_rlock import FairAsyncRLock
 
 
 async def fairness():
     lock = FairAsyncRLock()
     num_tasks = 1000
     order = []
 
@@ -103,7 +92,12 @@
 
 It's also important to note the potential downsides of using a reentrant lock.
 For one, they can hide bugs in code that isn't properly synchronized, since
 the same task can acquire a reentrant lock multiple times without issue.
 
 **_Non-reentrant locks are often simpler and can expose synchronization bugs more easily, so you should only use a
 reentrant lock if you have a specific need for it._**
+
+### Performance
+
+The performance is about 50% slower than `asyncio.Lock`, i.e. overhead of sequential locks is about 3/2 of same
+with `asyncio.Lock`.
```

### Comparing `fair_async_rlock-1.0.1/setup.py` & `fair_async_rlock-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import find_packages
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(name='fair_async_rlock',
-      version='1.0.1',
+      version='1.0.2',
       description='A well-tested implementation of a fair asynchronous RLock for concurrent programming.',
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/Joshuaalbert/FairAsyncRLock",
       author='Joshua G. Albert',
       author_email='albert@strw.leidenuniv.nl',
       setup_requires=[],
```

