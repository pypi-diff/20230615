# Comparing `tmp/casbin_redis_adapter-1.0.2.tar.gz` & `tmp/casbin_redis_adapter-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "casbin_redis_adapter-1.0.2.tar", last modified: Sun Jun 11 01:51:48 2023, max compression
+gzip compressed data, was "casbin_redis_adapter-1.1.0.tar", last modified: Thu Jun 15 14:20:32 2023, max compression
```

## Comparing `casbin_redis_adapter-1.0.2.tar` & `casbin_redis_adapter-1.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 01:51:48.359425 casbin_redis_adapter-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-11 01:51:16.000000 casbin_redis_adapter-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-06-11 01:51:48.359425 casbin_redis_adapter-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-06-11 01:51:16.000000 casbin_redis_adapter-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 01:51:48.359425 casbin_redis_adapter-1.0.2/casbin_redis_adapter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 01:51:16.000000 casbin_redis_adapter-1.0.2/casbin_redis_adapter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5381 2023-06-11 01:51:16.000000 casbin_redis_adapter-1.0.2/casbin_redis_adapter/adapter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 01:51:48.359425 casbin_redis_adapter-1.0.2/casbin_redis_adapter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-06-11 01:51:48.000000 casbin_redis_adapter-1.0.2/casbin_redis_adapter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-11 01:51:48.000000 casbin_redis_adapter-1.0.2/casbin_redis_adapter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 01:51:48.000000 casbin_redis_adapter-1.0.2/casbin_redis_adapter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-11 01:51:48.000000 casbin_redis_adapter-1.0.2/casbin_redis_adapter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-11 01:51:48.000000 casbin_redis_adapter-1.0.2/casbin_redis_adapter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-11 01:51:48.359425 casbin_redis_adapter-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-06-11 01:51:16.000000 casbin_redis_adapter-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 01:51:48.359425 casbin_redis_adapter-1.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 01:51:16.000000 casbin_redis_adapter-1.0.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8086 2023-06-11 01:51:16.000000 casbin_redis_adapter-1.0.2/tests/test_adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:20:32.955054 casbin_redis_adapter-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-15 14:20:02.000000 casbin_redis_adapter-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-06-15 14:20:32.955054 casbin_redis_adapter-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-06-15 14:20:02.000000 casbin_redis_adapter-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:20:32.955054 casbin_redis_adapter-1.1.0/casbin_redis_adapter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:20:02.000000 casbin_redis_adapter-1.1.0/casbin_redis_adapter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5450 2023-06-15 14:20:02.000000 casbin_redis_adapter-1.1.0/casbin_redis_adapter/adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:20:32.955054 casbin_redis_adapter-1.1.0/casbin_redis_adapter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-06-15 14:20:32.000000 casbin_redis_adapter-1.1.0/casbin_redis_adapter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-15 14:20:32.000000 casbin_redis_adapter-1.1.0/casbin_redis_adapter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 14:20:32.000000 casbin_redis_adapter-1.1.0/casbin_redis_adapter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-15 14:20:32.000000 casbin_redis_adapter-1.1.0/casbin_redis_adapter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-15 14:20:32.000000 casbin_redis_adapter-1.1.0/casbin_redis_adapter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-15 14:20:32.955054 casbin_redis_adapter-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-06-15 14:20:02.000000 casbin_redis_adapter-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:20:32.955054 casbin_redis_adapter-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:20:02.000000 casbin_redis_adapter-1.1.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8104 2023-06-15 14:20:02.000000 casbin_redis_adapter-1.1.0/tests/test_adapter.py
```

### Comparing `casbin_redis_adapter-1.0.2/LICENSE` & `casbin_redis_adapter-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `casbin_redis_adapter-1.0.2/PKG-INFO` & `casbin_redis_adapter-1.1.0/casbin_redis_adapter.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 Metadata-Version: 2.1
-Name: casbin_redis_adapter
-Version: 1.0.2
+Name: casbin-redis-adapter
+Version: 1.1.0
 Summary: Redis Adapter for PyCasbin
 Home-page: https://github.com/pycasbin/redis-adapter
 Author: BustDot
 Author-email: Bust.dev@outlook.com
 License: Apache 2.0
 Keywords: casbin,Redis,casbin-adapter,rbac,access control,abac,acl,permission
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.3
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-Redis Adapter for PyCasbin 
+Redis Adapter for PyCasbin
 ====
 
 [![GitHub Actions](https://github.com/pycasbin/redis-adapter/workflows/build/badge.svg?branch=master)](https://github.com/pycasbin/redis-adapter/actions)
 [![Coverage Status](https://coveralls.io/repos/github/pycasbin/redis-adapter/badge.svg?branch=master)](https://coveralls.io/github/pycasbin/redis-adapter?branch=master)
 [![Version](https://img.shields.io/pypi/v/casbin_redis_adapter.svg)](https://pypi.org/project/casbin_redis_adapter/)
 [![PyPI - Wheel](https://img.shields.io/pypi/wheel/casbin_redis_adapter.svg)](https://pypi.org/project/casbin_redis_adapter/)
 [![Pyversions](https://img.shields.io/pypi/pyversions/casbin_redis_adapter.svg)](https://pypi.org/project/casbin_redis_adapter/)
 [![Download](https://img.shields.io/pypi/dm/casbin_redis_adapter.svg)](https://pypi.org/project/casbin_redis_adapter/)
 [![License](https://img.shields.io/pypi/l/casbin_redis_adapter.svg)](https://pypi.org/project/casbin_redis_adapter/)
 
-Redis Adapter is the [redis](https://redis.io/) adapter for [PyCasbin](https://github.com/casbin/pycasbin). With this library, Casbin can load policy from redis or save policy to it.
+Redis Adapter is the [redis](https://redis.io/) adapter for [PyCasbin](https://github.com/casbin/pycasbin). With this
+library, Casbin can load policy from redis or save policy to it.
 
 ## Installation
 
 ```
 pip install casbin_redis_adapter
 ```
 
@@ -53,14 +54,33 @@
 if e.enforce(sub, obj, act):
     # permit alice to read data1casbin_sqlalchemy_adapter
     pass
 else:
     # deny the request, show an error
     pass
 ```
+
+## Configuration
+
+`Adapter()` enable decode_responses by default and supports any Redis parameter configuration.
+
+To use casbin_redis_adapter, you must provide the following parameter configuration
+
+- `host`: address of the redis service
+- `port`: redis service port
+
+The following parameters are provided by default
+
+- `db`: redis database, default is `0`
+- `username`: redis username, default is `None`
+- `password`: redis password, default is `None`
+- `key`: casbin rule to store key, default is `casbin_rules`
+
+For more parameters, please follow [redis-py](https://redis.readthedocs.io/en/stable/connections.html#redis.Redis)
+
 ### Getting Help
 
 - [PyCasbin](https://github.com/casbin/pycasbin)
 
 ### License
 
 This project is licensed under the [Apache 2.0 license](LICENSE).
```

### Comparing `casbin_redis_adapter-1.0.2/README.md` & `casbin_redis_adapter-1.1.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-Redis Adapter for PyCasbin 
+Redis Adapter for PyCasbin
 ====
 
 [![GitHub Actions](https://github.com/pycasbin/redis-adapter/workflows/build/badge.svg?branch=master)](https://github.com/pycasbin/redis-adapter/actions)
 [![Coverage Status](https://coveralls.io/repos/github/pycasbin/redis-adapter/badge.svg?branch=master)](https://coveralls.io/github/pycasbin/redis-adapter?branch=master)
 [![Version](https://img.shields.io/pypi/v/casbin_redis_adapter.svg)](https://pypi.org/project/casbin_redis_adapter/)
 [![PyPI - Wheel](https://img.shields.io/pypi/wheel/casbin_redis_adapter.svg)](https://pypi.org/project/casbin_redis_adapter/)
 [![Pyversions](https://img.shields.io/pypi/pyversions/casbin_redis_adapter.svg)](https://pypi.org/project/casbin_redis_adapter/)
 [![Download](https://img.shields.io/pypi/dm/casbin_redis_adapter.svg)](https://pypi.org/project/casbin_redis_adapter/)
 [![License](https://img.shields.io/pypi/l/casbin_redis_adapter.svg)](https://pypi.org/project/casbin_redis_adapter/)
 
-Redis Adapter is the [redis](https://redis.io/) adapter for [PyCasbin](https://github.com/casbin/pycasbin). With this library, Casbin can load policy from redis or save policy to it.
+Redis Adapter is the [redis](https://redis.io/) adapter for [PyCasbin](https://github.com/casbin/pycasbin). With this
+library, Casbin can load policy from redis or save policy to it.
 
 ## Installation
 
 ```
 pip install casbin_redis_adapter
 ```
 
@@ -34,14 +35,33 @@
 if e.enforce(sub, obj, act):
     # permit alice to read data1casbin_sqlalchemy_adapter
     pass
 else:
     # deny the request, show an error
     pass
 ```
+
+## Configuration
+
+`Adapter()` enable decode_responses by default and supports any Redis parameter configuration.
+
+To use casbin_redis_adapter, you must provide the following parameter configuration
+
+- `host`: address of the redis service
+- `port`: redis service port
+
+The following parameters are provided by default
+
+- `db`: redis database, default is `0`
+- `username`: redis username, default is `None`
+- `password`: redis password, default is `None`
+- `key`: casbin rule to store key, default is `casbin_rules`
+
+For more parameters, please follow [redis-py](https://redis.readthedocs.io/en/stable/connections.html#redis.Redis)
+
 ### Getting Help
 
 - [PyCasbin](https://github.com/casbin/pycasbin)
 
 ### License
 
-This project is licensed under the [Apache 2.0 license](LICENSE).
+This project is licensed under the [Apache 2.0 license](LICENSE).
```

### Comparing `casbin_redis_adapter-1.0.2/casbin_redis_adapter/adapter.py` & `casbin_redis_adapter-1.1.0/casbin_redis_adapter/adapter.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,24 +39,32 @@
         return '<CasbinRule :"{}">'.format(str(self))
 
 
 class Adapter(persist.Adapter):
     """the interface for Casbin adapters."""
 
     def __init__(
-        self, host, port, username=None, password=None, pool=None, key="casbin_rules"
+        self,
+        host,
+        port,
+        db=0,
+        username=None,
+        password=None,
+        key="casbin_rules",
+        **kwargs,
     ):
         self.key = key
         self.client = redis.Redis(
             host=host,
             port=port,
+            db=db,
             username=username,
             password=password,
-            connection_pool=pool,
             decode_responses=True,
+            **kwargs,
         )
 
     def drop_table(self):
         self.client.delete(self.key)
 
     def load_policy(self, model):
         """Implementing add Interface for casbin. Load all policy rules from redis
```

### Comparing `casbin_redis_adapter-1.0.2/casbin_redis_adapter.egg-info/PKG-INFO` & `casbin_redis_adapter-1.1.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 Metadata-Version: 2.1
-Name: casbin-redis-adapter
-Version: 1.0.2
+Name: casbin_redis_adapter
+Version: 1.1.0
 Summary: Redis Adapter for PyCasbin
 Home-page: https://github.com/pycasbin/redis-adapter
 Author: BustDot
 Author-email: Bust.dev@outlook.com
 License: Apache 2.0
 Keywords: casbin,Redis,casbin-adapter,rbac,access control,abac,acl,permission
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.3
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-Redis Adapter for PyCasbin 
+Redis Adapter for PyCasbin
 ====
 
 [![GitHub Actions](https://github.com/pycasbin/redis-adapter/workflows/build/badge.svg?branch=master)](https://github.com/pycasbin/redis-adapter/actions)
 [![Coverage Status](https://coveralls.io/repos/github/pycasbin/redis-adapter/badge.svg?branch=master)](https://coveralls.io/github/pycasbin/redis-adapter?branch=master)
 [![Version](https://img.shields.io/pypi/v/casbin_redis_adapter.svg)](https://pypi.org/project/casbin_redis_adapter/)
 [![PyPI - Wheel](https://img.shields.io/pypi/wheel/casbin_redis_adapter.svg)](https://pypi.org/project/casbin_redis_adapter/)
 [![Pyversions](https://img.shields.io/pypi/pyversions/casbin_redis_adapter.svg)](https://pypi.org/project/casbin_redis_adapter/)
 [![Download](https://img.shields.io/pypi/dm/casbin_redis_adapter.svg)](https://pypi.org/project/casbin_redis_adapter/)
 [![License](https://img.shields.io/pypi/l/casbin_redis_adapter.svg)](https://pypi.org/project/casbin_redis_adapter/)
 
-Redis Adapter is the [redis](https://redis.io/) adapter for [PyCasbin](https://github.com/casbin/pycasbin). With this library, Casbin can load policy from redis or save policy to it.
+Redis Adapter is the [redis](https://redis.io/) adapter for [PyCasbin](https://github.com/casbin/pycasbin). With this
+library, Casbin can load policy from redis or save policy to it.
 
 ## Installation
 
 ```
 pip install casbin_redis_adapter
 ```
 
@@ -53,14 +54,33 @@
 if e.enforce(sub, obj, act):
     # permit alice to read data1casbin_sqlalchemy_adapter
     pass
 else:
     # deny the request, show an error
     pass
 ```
+
+## Configuration
+
+`Adapter()` enable decode_responses by default and supports any Redis parameter configuration.
+
+To use casbin_redis_adapter, you must provide the following parameter configuration
+
+- `host`: address of the redis service
+- `port`: redis service port
+
+The following parameters are provided by default
+
+- `db`: redis database, default is `0`
+- `username`: redis username, default is `None`
+- `password`: redis password, default is `None`
+- `key`: casbin rule to store key, default is `casbin_rules`
+
+For more parameters, please follow [redis-py](https://redis.readthedocs.io/en/stable/connections.html#redis.Redis)
+
 ### Getting Help
 
 - [PyCasbin](https://github.com/casbin/pycasbin)
 
 ### License
 
 This project is licensed under the [Apache 2.0 license](LICENSE).
```

### Comparing `casbin_redis_adapter-1.0.2/setup.py` & `casbin_redis_adapter-1.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         "access control",
         "abac",
         "acl",
         "permission",
     ],
     packages=find_packages(),
     install_requires=install_requires,
-    python_requires=">=3.3",
+    python_requires=">=3.8",
     license="Apache 2.0",
     classifiers=[
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: Apache Software License",
```

### Comparing `casbin_redis_adapter-1.0.2/tests/test_adapter.py` & `casbin_redis_adapter-1.1.0/tests/test_adapter.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     get model path
     """
     dir_path = os.path.split(os.path.realpath(__file__))[0] + "/"
     return os.path.abspath(dir_path + path)
 
 
 def get_enforcer():
-    adapter = Adapter("localhost", 6379)
+    adapter = Adapter("localhost", 6379, encoding="utf-8")
     e = casbin.Enforcer(get_fixture("rbac_model.conf"), adapter)
     model = e.get_model()
 
     model.clear_policy()
     model.add_policy("p", "p", ["alice", "data1", "read"])
     adapter.save_policy(model)
```

