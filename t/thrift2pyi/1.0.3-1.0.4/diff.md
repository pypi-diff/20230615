# Comparing `tmp/thrift2pyi-1.0.3.tar.gz` & `tmp/thrift2pyi-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/yanweizhi/repos/nhywieza/thrift2pyi/dist/tmpfz3ddfbj/thrift2pyi-1.0.3.tar", last modified: Wed Mar  3 09:32:53 2021, max compression
+gzip compressed data, was "thrift2pyi-1.0.4.tar", last modified: Thu Jun 15 09:04:45 2023, max compression
```

## Comparing `thrift2pyi-1.0.3.tar` & `thrift2pyi-1.0.4.tar`

### file list

```diff
@@ -1,28 +1,22 @@
-drwxr-xr-x   0 yanweizhi   (502) staff       (20)        0 2021-03-03 09:32:53.343560 thrift2pyi-1.0.3/
--rw-r--r--   0 yanweizhi   (502) staff       (20)       18 2019-11-20 09:22:51.000000 thrift2pyi-1.0.3/MANIFEST.in
--rw-r--r--   0 yanweizhi   (502) staff       (20)     5389 2021-03-03 09:32:53.342758 thrift2pyi-1.0.3/PKG-INFO
--rw-r--r--   0 yanweizhi   (502) staff       (20)     3427 2020-10-09 08:06:21.000000 thrift2pyi-1.0.3/README.md
-drwxr-xr-x   0 yanweizhi   (502) staff       (20)        0 2021-03-03 09:32:53.330458 thrift2pyi-1.0.3/gen-py/
--rw-r--r--   0 yanweizhi   (502) staff       (20)        0 2019-11-20 09:22:51.000000 thrift2pyi-1.0.3/gen-py/__init__.py
-drwxr-xr-x   0 yanweizhi   (502) staff       (20)        0 2021-03-03 09:32:53.333026 thrift2pyi-1.0.3/gen-py/example/
--rw-r--r--   0 yanweizhi   (502) staff       (20)    20054 2019-11-20 09:22:51.000000 thrift2pyi-1.0.3/gen-py/example/ExampleService.py
--rw-r--r--   0 yanweizhi   (502) staff       (20)       52 2019-11-20 09:22:51.000000 thrift2pyi-1.0.3/gen-py/example/__init__.py
--rw-r--r--   0 yanweizhi   (502) staff       (20)      380 2019-11-20 09:22:51.000000 thrift2pyi-1.0.3/gen-py/example/constants.py
--rw-r--r--   0 yanweizhi   (502) staff       (20)    22132 2019-11-20 09:22:51.000000 thrift2pyi-1.0.3/gen-py/example/ttypes.py
--rw-r--r--   0 yanweizhi   (502) staff       (20)       38 2021-03-03 09:32:53.343745 thrift2pyi-1.0.3/setup.cfg
--rw-r--r--   0 yanweizhi   (502) staff       (20)     1998 2019-11-20 09:27:16.000000 thrift2pyi-1.0.3/setup.py
-drwxr-xr-x   0 yanweizhi   (502) staff       (20)        0 2021-03-03 09:32:53.338255 thrift2pyi-1.0.3/thrift2pyi/
--rw-r--r--   0 yanweizhi   (502) staff       (20)      264 2019-11-20 09:27:16.000000 thrift2pyi-1.0.3/thrift2pyi/__init__.py
--rw-r--r--   0 yanweizhi   (502) staff       (20)      239 2019-11-20 09:22:51.000000 thrift2pyi-1.0.3/thrift2pyi/__main__.py
--rw-r--r--   0 yanweizhi   (502) staff       (20)       63 2021-03-03 09:27:33.000000 thrift2pyi-1.0.3/thrift2pyi/__version__.py
--rw-r--r--   0 yanweizhi   (502) staff       (20)    10228 2021-03-03 09:13:33.000000 thrift2pyi-1.0.3/thrift2pyi/convert.py
--rw-r--r--   0 yanweizhi   (502) staff       (20)      215 2020-10-09 08:06:21.000000 thrift2pyi-1.0.3/thrift2pyi/exceptions.py
--rw-r--r--   0 yanweizhi   (502) staff       (20)      593 2020-02-26 12:08:49.000000 thrift2pyi-1.0.3/thrift2pyi/main.py
--rw-r--r--   0 yanweizhi   (502) staff       (20)     3080 2021-03-03 09:13:48.000000 thrift2pyi-1.0.3/thrift2pyi/peg.py
-drwxr-xr-x   0 yanweizhi   (502) staff       (20)        0 2021-03-03 09:32:53.341562 thrift2pyi-1.0.3/thrift2pyi.egg-info/
--rw-r--r--   0 yanweizhi   (502) staff       (20)     5389 2021-03-03 09:32:53.000000 thrift2pyi-1.0.3/thrift2pyi.egg-info/PKG-INFO
--rw-r--r--   0 yanweizhi   (502) staff       (20)      524 2021-03-03 09:32:53.000000 thrift2pyi-1.0.3/thrift2pyi.egg-info/SOURCES.txt
--rw-r--r--   0 yanweizhi   (502) staff       (20)        1 2021-03-03 09:32:53.000000 thrift2pyi-1.0.3/thrift2pyi.egg-info/dependency_links.txt
--rw-r--r--   0 yanweizhi   (502) staff       (20)       53 2021-03-03 09:32:53.000000 thrift2pyi-1.0.3/thrift2pyi.egg-info/entry_points.txt
--rw-r--r--   0 yanweizhi   (502) staff       (20)      232 2021-03-03 09:32:53.000000 thrift2pyi-1.0.3/thrift2pyi.egg-info/requires.txt
--rw-r--r--   0 yanweizhi   (502) staff       (20)       18 2021-03-03 09:32:53.000000 thrift2pyi-1.0.3/thrift2pyi.egg-info/top_level.txt
+drwxr-xr-x   0 bytedance   (502) staff       (20)        0 2023-06-15 09:04:45.172662 thrift2pyi-1.0.4/
+-rw-r--r--   0 bytedance   (502) staff       (20)     1056 2023-06-15 06:01:06.000000 thrift2pyi-1.0.4/LICENSE
+-rw-r--r--   0 bytedance   (502) staff       (20)       18 2023-06-15 06:01:06.000000 thrift2pyi-1.0.4/MANIFEST.in
+-rw-r--r--   0 bytedance   (502) staff       (20)     3968 2023-06-15 09:04:45.172052 thrift2pyi-1.0.4/PKG-INFO
+-rw-r--r--   0 bytedance   (502) staff       (20)     3427 2023-06-15 06:01:06.000000 thrift2pyi-1.0.4/README.md
+-rw-r--r--   0 bytedance   (502) staff       (20)       38 2023-06-15 09:04:45.172846 thrift2pyi-1.0.4/setup.cfg
+-rw-r--r--   0 bytedance   (502) staff       (20)     1998 2023-06-15 06:01:06.000000 thrift2pyi-1.0.4/setup.py
+drwxr-xr-x   0 bytedance   (502) staff       (20)        0 2023-06-15 09:04:45.166404 thrift2pyi-1.0.4/thrift2pyi/
+-rw-r--r--   0 bytedance   (502) staff       (20)      264 2023-06-15 06:01:06.000000 thrift2pyi-1.0.4/thrift2pyi/__init__.py
+-rw-r--r--   0 bytedance   (502) staff       (20)      239 2023-06-15 06:01:06.000000 thrift2pyi-1.0.4/thrift2pyi/__main__.py
+-rw-r--r--   0 bytedance   (502) staff       (20)       63 2023-06-15 06:05:30.000000 thrift2pyi-1.0.4/thrift2pyi/__version__.py
+-rw-r--r--   0 bytedance   (502) staff       (20)    10306 2023-06-15 06:10:28.000000 thrift2pyi-1.0.4/thrift2pyi/convert.py
+-rw-r--r--   0 bytedance   (502) staff       (20)      215 2023-06-15 06:01:06.000000 thrift2pyi-1.0.4/thrift2pyi/exceptions.py
+-rw-r--r--   0 bytedance   (502) staff       (20)      593 2023-06-15 06:01:06.000000 thrift2pyi-1.0.4/thrift2pyi/main.py
+-rw-r--r--   0 bytedance   (502) staff       (20)     3080 2023-06-15 06:01:06.000000 thrift2pyi-1.0.4/thrift2pyi/peg.py
+drwxr-xr-x   0 bytedance   (502) staff       (20)        0 2023-06-15 09:04:45.171248 thrift2pyi-1.0.4/thrift2pyi.egg-info/
+-rw-r--r--   0 bytedance   (502) staff       (20)     3968 2023-06-15 09:04:45.000000 thrift2pyi-1.0.4/thrift2pyi.egg-info/PKG-INFO
+-rw-r--r--   0 bytedance   (502) staff       (20)      400 2023-06-15 09:04:45.000000 thrift2pyi-1.0.4/thrift2pyi.egg-info/SOURCES.txt
+-rw-r--r--   0 bytedance   (502) staff       (20)        1 2023-06-15 09:04:45.000000 thrift2pyi-1.0.4/thrift2pyi.egg-info/dependency_links.txt
+-rw-r--r--   0 bytedance   (502) staff       (20)       52 2023-06-15 09:04:45.000000 thrift2pyi-1.0.4/thrift2pyi.egg-info/entry_points.txt
+-rw-r--r--   0 bytedance   (502) staff       (20)      232 2023-06-15 09:04:45.000000 thrift2pyi-1.0.4/thrift2pyi.egg-info/requires.txt
+-rw-r--r--   0 bytedance   (502) staff       (20)       11 2023-06-15 09:04:45.000000 thrift2pyi-1.0.4/thrift2pyi.egg-info/top_level.txt
```

### Comparing `thrift2pyi-1.0.3/README.md` & `thrift2pyi-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `thrift2pyi-1.0.3/setup.py` & `thrift2pyi-1.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `thrift2pyi-1.0.3/thrift2pyi/convert.py` & `thrift2pyi-1.0.4/thrift2pyi/convert.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,14 +77,16 @@
                 return "List[%s]" % self._get_type(nest)
             elif thrift_type == TType.MAP:
                 self._imports["typing"].add("Dict")
                 return "Dict[%s,%s]" % (self._get_type(nest[0]), self._get_type(nest[1]))
             elif thrift_type == TType.SET:
                 self._imports["typing"].add("Set")
                 return "Set[%s]" % self._get_type(nest)
+            elif thrift_type in [TType.BINARY]:
+                return "bytes"
             elif thrift_type == TType.I32:
                 return u(nest.__name__)
             else:
                 raise Thrift2pyiException("do not type support %s" % thrift_type)
 
     def _spec2type(self, spec):
         if len(spec) == 3:
@@ -289,8 +291,8 @@
         shutil.copyfile(self.filename, filename)
 
         with open("%s.pyi" % filename.replace(".thrift", "_thrift"), "w") as f:
             f.write(o)
 
 
 if __name__ == "__main__":
-    Thrift2pyi("../tests/example.thrift", prefix="", out="").output()
+    Thrift2pyi("./tests/example.thrift", prefix="", out="").output()
```

### Comparing `thrift2pyi-1.0.3/thrift2pyi/main.py` & `thrift2pyi-1.0.4/thrift2pyi/main.py`

 * *Files identical despite different names*

### Comparing `thrift2pyi-1.0.3/thrift2pyi/peg.py` & `thrift2pyi-1.0.4/thrift2pyi/peg.py`

 * *Files identical despite different names*

