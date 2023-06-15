# Comparing `tmp/sentenai-1.6.4.8.tar.gz` & `tmp/sentenai-1.6.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sentenai-1.6.4.8.tar", last modified: Thu May  4 20:28:42 2023, max compression
+gzip compressed data, was "sentenai-1.6.4.9.tar", last modified: Thu Jun  1 19:03:17 2023, max compression
```

## Comparing `sentenai-1.6.4.8.tar` & `sentenai-1.6.4.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 xnomagichash   (501) staff       (20)        0 2023-05-04 20:28:42.000000 sentenai-1.6.4.8/
--rw-r--r--   0 xnomagichash   (501) staff       (20)     1514 2021-12-01 20:18:24.000000 sentenai-1.6.4.8/LICENSE
--rw-r--r--   0 xnomagichash   (501) staff       (20)      670 2023-05-04 20:28:42.000000 sentenai-1.6.4.8/PKG-INFO
--rw-r--r--   0 xnomagichash   (501) staff       (20)      781 2021-12-01 20:18:24.000000 sentenai-1.6.4.8/README.md
-drwxr-xr-x   0 xnomagichash   (501) staff       (20)        0 2023-05-04 20:28:42.000000 sentenai-1.6.4.8/sentenai/
--rw-r--r--   0 xnomagichash   (501) staff       (20)     8918 2023-04-30 01:51:32.000000 sentenai-1.6.4.8/sentenai/__init__.py
--rw-r--r--   0 xnomagichash   (501) staff       (20)     9640 2023-04-29 11:28:45.000000 sentenai-1.6.4.8/sentenai/api.py
-drwxr-xr-x   0 xnomagichash   (501) staff       (20)        0 2023-05-04 20:28:42.000000 sentenai-1.6.4.8/sentenai/stream/
--rw-r--r--   0 xnomagichash   (501) staff       (20)       59 2023-05-04 20:20:46.000000 sentenai-1.6.4.8/sentenai/stream/__init__.py
--rw-r--r--   0 xnomagichash   (501) staff       (20)     5141 2022-03-25 18:39:40.000000 sentenai-1.6.4.8/sentenai/stream/events.py
--rw-r--r--   0 xnomagichash   (501) staff       (20)     2161 2023-02-13 21:49:04.000000 sentenai-1.6.4.8/sentenai/stream/metadata.py
--rw-r--r--   0 xnomagichash   (501) staff       (20)    19900 2023-05-04 20:27:36.000000 sentenai-1.6.4.8/sentenai/stream/streams.py
-drwxr-xr-x   0 xnomagichash   (501) staff       (20)        0 2023-05-04 20:28:42.000000 sentenai-1.6.4.8/sentenai.egg-info/
--rw-r--r--   0 xnomagichash   (501) staff       (20)      670 2023-05-04 20:28:41.000000 sentenai-1.6.4.8/sentenai.egg-info/PKG-INFO
--rw-r--r--   0 xnomagichash   (501) staff       (20)      341 2023-05-04 20:28:42.000000 sentenai-1.6.4.8/sentenai.egg-info/SOURCES.txt
--rw-r--r--   0 xnomagichash   (501) staff       (20)        1 2023-05-04 20:28:41.000000 sentenai-1.6.4.8/sentenai.egg-info/dependency_links.txt
--rw-r--r--   0 xnomagichash   (501) staff       (20)       68 2023-05-04 20:28:42.000000 sentenai-1.6.4.8/sentenai.egg-info/requires.txt
--rw-r--r--   0 xnomagichash   (501) staff       (20)        9 2023-05-04 20:28:42.000000 sentenai-1.6.4.8/sentenai.egg-info/top_level.txt
--rw-r--r--   0 xnomagichash   (501) staff       (20)       79 2023-05-04 20:28:42.000000 sentenai-1.6.4.8/setup.cfg
--rw-r--r--   0 xnomagichash   (501) staff       (20)      980 2023-05-04 20:28:12.000000 sentenai-1.6.4.8/setup.py
+drwxr-xr-x   0 xnomagichash   (501) staff       (20)        0 2023-06-01 19:03:17.402217 sentenai-1.6.4.9/
+-rw-r--r--   0 xnomagichash   (501) staff       (20)     1514 2021-12-01 20:18:24.000000 sentenai-1.6.4.9/LICENSE
+-rw-r--r--   0 xnomagichash   (501) staff       (20)      670 2023-06-01 19:03:17.402298 sentenai-1.6.4.9/PKG-INFO
+-rw-r--r--   0 xnomagichash   (501) staff       (20)      781 2021-12-01 20:18:24.000000 sentenai-1.6.4.9/README.md
+drwxr-xr-x   0 xnomagichash   (501) staff       (20)        0 2023-06-01 19:03:17.399733 sentenai-1.6.4.9/sentenai/
+-rw-r--r--   0 xnomagichash   (501) staff       (20)     8918 2023-04-30 01:51:32.000000 sentenai-1.6.4.9/sentenai/__init__.py
+-rw-r--r--   0 xnomagichash   (501) staff       (20)     9640 2023-04-29 11:28:45.000000 sentenai-1.6.4.9/sentenai/api.py
+drwxr-xr-x   0 xnomagichash   (501) staff       (20)        0 2023-06-01 19:03:17.402049 sentenai-1.6.4.9/sentenai/stream/
+-rw-r--r--   0 xnomagichash   (501) staff       (20)       59 2023-05-04 20:20:46.000000 sentenai-1.6.4.9/sentenai/stream/__init__.py
+-rw-r--r--   0 xnomagichash   (501) staff       (20)     5141 2022-03-25 18:39:40.000000 sentenai-1.6.4.9/sentenai/stream/events.py
+-rw-r--r--   0 xnomagichash   (501) staff       (20)     2161 2023-02-13 21:49:04.000000 sentenai-1.6.4.9/sentenai/stream/metadata.py
+-rw-r--r--   0 xnomagichash   (501) staff       (20)    20085 2023-06-01 19:02:48.000000 sentenai-1.6.4.9/sentenai/stream/streams.py
+drwxr-xr-x   0 xnomagichash   (501) staff       (20)        0 2023-06-01 19:03:17.401039 sentenai-1.6.4.9/sentenai.egg-info/
+-rw-r--r--   0 xnomagichash   (501) staff       (20)      670 2023-06-01 19:03:17.000000 sentenai-1.6.4.9/sentenai.egg-info/PKG-INFO
+-rw-r--r--   0 xnomagichash   (501) staff       (20)      341 2023-06-01 19:03:17.000000 sentenai-1.6.4.9/sentenai.egg-info/SOURCES.txt
+-rw-r--r--   0 xnomagichash   (501) staff       (20)        1 2023-06-01 19:03:17.000000 sentenai-1.6.4.9/sentenai.egg-info/dependency_links.txt
+-rw-r--r--   0 xnomagichash   (501) staff       (20)       68 2023-06-01 19:03:17.000000 sentenai-1.6.4.9/sentenai.egg-info/requires.txt
+-rw-r--r--   0 xnomagichash   (501) staff       (20)        9 2023-06-01 19:03:17.000000 sentenai-1.6.4.9/sentenai.egg-info/top_level.txt
+-rw-r--r--   0 xnomagichash   (501) staff       (20)       79 2023-06-01 19:03:17.402559 sentenai-1.6.4.9/setup.cfg
+-rw-r--r--   0 xnomagichash   (501) staff       (20)      980 2023-06-01 19:03:03.000000 sentenai-1.6.4.9/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `sentenai-1.6.4.8/LICENSE` & `sentenai-1.6.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sentenai-1.6.4.8/PKG-INFO` & `sentenai-1.6.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentenai
-Version: 1.6.4.8
+Version: 1.6.4.9
 Summary: Client library for Sentenai
 Home-page: https://github.com/sentenai/py-sentenai
 Author: Sentenai, Inc.
 Author-email: info@sentenai.com
 License: BSD
 Keywords: sentenai cloud sensor database
 Platform: UNKNOWN
```

### Comparing `sentenai-1.6.4.8/README.md` & `sentenai-1.6.4.9/README.md`

 * *Files identical despite different names*

### Comparing `sentenai-1.6.4.8/sentenai/__init__.py` & `sentenai-1.6.4.9/sentenai/__init__.py`

 * *Files identical despite different names*

### Comparing `sentenai-1.6.4.8/sentenai/api.py` & `sentenai-1.6.4.9/sentenai/api.py`

 * *Files identical despite different names*

### Comparing `sentenai-1.6.4.8/sentenai/stream/events.py` & `sentenai-1.6.4.9/sentenai/stream/events.py`

 * *Files identical despite different names*

### Comparing `sentenai-1.6.4.8/sentenai/stream/metadata.py` & `sentenai-1.6.4.9/sentenai/stream/metadata.py`

 * *Files identical despite different names*

### Comparing `sentenai-1.6.4.8/sentenai/stream/streams.py` & `sentenai-1.6.4.9/sentenai/stream/streams.py`

 * *Files 2% similar despite different names*

```diff
@@ -173,49 +173,60 @@
                 nid = self._put('paths', *path).json()['node']
                 self._put('nodes', nid, 'types', 'event')
                 cmap = {'start': nid}
                 tmap = {'start': 'event'}
                 dmap = {'start': []}
                 df = content
             df = df.sort_values(by='start', ignore_index=True)
-            for cname in df.columns:
-                if cname in ('start', 'end'):
-                    continue
+
+
+
+            def add(cname):
                 if isinstance(content, list):
                     nid = self._put('paths', *path).json()['node']
                 else:
                     nid = self._put('paths', *path, cname).json()['node']
                 if df[cname].dtype == np.dtype('float32'):
-                    tmap[cname] = 'float'
+                    tm = 'float'
                 elif df[cname].dtype == np.dtype('float64'):
-                    tmap[cname] = 'float'
+                    tm = 'float'
                 elif df[cname].dtype == np.dtype('int32'):
-                    tmap[cname] = 'int'
+                    tm = 'int'
                 elif df[cname].dtype == np.dtype('int64'):
-                    tmap[cname] = 'int'
+                    tm = 'int'
                 elif df[cname].dtype == bool:
-                    tmap[cname] = 'bool'
+                    tm = 'bool'
                 elif df[cname].dtype == np.dtype('datetime64[ns]'):
-                    tmap[cname] = 'datetime'
+                    tm = 'datetime'
                 elif df[cname].dtype == np.dtype('timedelta64[ns]'):
-                    tmap[cname] = 'timedelta'
+                    tm = 'timedelta'
                 elif type(df[cname][0]) == date:
-                    tmap[cname] = 'date'
+                    tm = 'date'
                 elif type(df[cname][0]) == time:
-                    tmap[cname] = 'time'
+                    tm = 'time'
                 elif type(df[cname][0]) == Point and df[cname][0].has_z:
-                    tmap[cname] = 'point3'
+                    tm = 'point3'
                 elif type(df[cname][0]) == Point:
-                    tmap[cname] = 'point'
+                    tm = 'point'
                 else:
-                    tmap[cname] = 'text'
+                    tm = 'text'
+
+                self._put('nodes', nid, 'types', tm)
+                #cmap[cname] = nid
+                #dmap[cname] = []
+                #tmap[cname] = tm
+                return (cname, nid, tm)
+
+            with ThreadPoolExecutor(max_workers=8) as pool:
+                res = pool.map(add, [x for x in df.columns if x not in ['start', 'end']])
+                for cname, nid, tm in res:
+                    cmap[cname] = nid
+                    dmap[cname] = []
+                    tmap[cname] = tm
 
-                self._put('nodes', nid, 'types', tmap[cname])
-                cmap[cname] = nid
-                dmap[cname] = []
 
             origin = self.origin
             res = []
             q = Queue()
             Thread(target=worker, args=(q, workers, len(df) * (len(df.columns) - 1), self._parent.interactive)).start()
 
             for i, row in df.iterrows():
```

### Comparing `sentenai-1.6.4.8/sentenai.egg-info/PKG-INFO` & `sentenai-1.6.4.9/sentenai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentenai
-Version: 1.6.4.8
+Version: 1.6.4.9
 Summary: Client library for Sentenai
 Home-page: https://github.com/sentenai/py-sentenai
 Author: Sentenai, Inc.
 Author-email: info@sentenai.com
 License: BSD
 Keywords: sentenai cloud sensor database
 Platform: UNKNOWN
```

### Comparing `sentenai-1.6.4.8/setup.py` & `sentenai-1.6.4.9/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='sentenai',
-    version='1.6.4.8',
+    version='1.6.4.9',
     description='Client library for Sentenai',
     long_description="",
     url='https://github.com/sentenai/py-sentenai',
 
     author='Sentenai, Inc.',
     author_email='info@sentenai.com',
```

