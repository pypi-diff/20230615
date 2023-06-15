# Comparing `tmp/bs_admin_utils-1.1.0.tar.gz` & `tmp/bs_admin_utils-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bs_admin_utils-1.1.0.tar", last modified: Wed Jun 14 11:58:26 2023, max compression
+gzip compressed data, was "bs_admin_utils-1.1.1.tar", last modified: Thu Jun 15 04:03:56 2023, max compression
```

## Comparing `bs_admin_utils-1.1.0.tar` & `bs_admin_utils-1.1.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)        0 2023-06-14 11:58:26.420617 bs_admin_utils-1.1.0/
--rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)     1067 2023-04-07 03:25:03.000000 bs_admin_utils-1.1.0/LICENSE
--rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)       35 2023-04-07 04:04:08.000000 bs_admin_utils-1.1.0/MANIFEST.in
--rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)      260 2023-06-14 11:58:26.420617 bs_admin_utils-1.1.0/PKG-INFO
--rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)      206 2023-04-07 03:35:29.000000 bs_admin_utils-1.1.0/README.md
-drwxrwxr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)        0 2023-06-14 11:58:26.416617 bs_admin_utils-1.1.0/bs_admin_utils/
--rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)       13 2023-04-07 03:39:05.000000 bs_admin_utils-1.1.0/bs_admin_utils/__init__.py
--rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)     4394 2023-06-14 11:57:54.000000 bs_admin_utils-1.1.0/bs_admin_utils/api.py
--rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)      490 2023-04-07 04:11:32.000000 bs_admin_utils-1.1.0/bs_admin_utils/decorators.py
--rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)     1034 2023-04-07 03:48:50.000000 bs_admin_utils-1.1.0/bs_admin_utils/model.py
-drwxrwxr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)        0 2023-06-14 11:58:26.420617 bs_admin_utils-1.1.0/bs_admin_utils/static/
--rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)   367112 2023-04-07 03:52:07.000000 bs_admin_utils-1.1.0/bs_admin_utils/static/arial.ttf
--rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)     6248 2023-06-14 10:45:34.000000 bs_admin_utils-1.1.0/bs_admin_utils/static/nstc.ttf
--rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)     2439 2023-06-14 10:58:06.000000 bs_admin_utils-1.1.0/bs_admin_utils/vercode.py
--rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)     2868 2023-04-07 04:10:45.000000 bs_admin_utils-1.1.0/bs_admin_utils/websocket.py
-drwxrwxr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)        0 2023-06-14 11:58:26.416617 bs_admin_utils-1.1.0/bs_admin_utils.egg-info/
--rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)      260 2023-06-14 11:58:26.000000 bs_admin_utils-1.1.0/bs_admin_utils.egg-info/PKG-INFO
--rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)      479 2023-06-14 11:58:26.000000 bs_admin_utils-1.1.0/bs_admin_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)        1 2023-06-14 11:58:26.000000 bs_admin_utils-1.1.0/bs_admin_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)       44 2023-06-14 11:58:26.000000 bs_admin_utils-1.1.0/bs_admin_utils.egg-info/requires.txt
--rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)       15 2023-06-14 11:58:26.000000 bs_admin_utils-1.1.0/bs_admin_utils.egg-info/top_level.txt
--rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)        1 2023-06-14 11:58:26.000000 bs_admin_utils-1.1.0/bs_admin_utils.egg-info/zip-safe
--rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)       38 2023-06-14 11:58:26.420617 bs_admin_utils-1.1.0/setup.cfg
--rwxr-xr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)      620 2023-06-14 11:55:31.000000 bs_admin_utils-1.1.0/setup.py
+drwxrwxr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)        0 2023-06-15 04:03:56.375122 bs_admin_utils-1.1.1/
+-rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)     1067 2023-04-07 03:25:03.000000 bs_admin_utils-1.1.1/LICENSE
+-rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)       35 2023-04-07 04:04:08.000000 bs_admin_utils-1.1.1/MANIFEST.in
+-rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)      260 2023-06-15 04:03:56.375122 bs_admin_utils-1.1.1/PKG-INFO
+-rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)      206 2023-04-07 03:35:29.000000 bs_admin_utils-1.1.1/README.md
+drwxrwxr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)        0 2023-06-15 04:03:56.371122 bs_admin_utils-1.1.1/bs_admin_utils/
+-rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)       13 2023-04-07 03:39:05.000000 bs_admin_utils-1.1.1/bs_admin_utils/__init__.py
+-rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)     4220 2023-06-15 04:01:20.000000 bs_admin_utils-1.1.1/bs_admin_utils/api.py
+-rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)      490 2023-04-07 04:11:32.000000 bs_admin_utils-1.1.1/bs_admin_utils/decorators.py
+-rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)     1034 2023-04-07 03:48:50.000000 bs_admin_utils-1.1.1/bs_admin_utils/model.py
+drwxrwxr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)        0 2023-06-15 04:03:56.375122 bs_admin_utils-1.1.1/bs_admin_utils/static/
+-rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)   367112 2023-04-07 03:52:07.000000 bs_admin_utils-1.1.1/bs_admin_utils/static/arial.ttf
+-rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)     6248 2023-06-14 10:45:34.000000 bs_admin_utils-1.1.1/bs_admin_utils/static/nstc.ttf
+-rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)     2439 2023-06-14 10:58:06.000000 bs_admin_utils-1.1.1/bs_admin_utils/vercode.py
+-rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)     2868 2023-04-07 04:10:45.000000 bs_admin_utils-1.1.1/bs_admin_utils/websocket.py
+drwxrwxr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)        0 2023-06-15 04:03:56.375122 bs_admin_utils-1.1.1/bs_admin_utils.egg-info/
+-rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)      260 2023-06-15 04:03:56.000000 bs_admin_utils-1.1.1/bs_admin_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)      479 2023-06-15 04:03:56.000000 bs_admin_utils-1.1.1/bs_admin_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)        1 2023-06-15 04:03:56.000000 bs_admin_utils-1.1.1/bs_admin_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)       44 2023-06-15 04:03:56.000000 bs_admin_utils-1.1.1/bs_admin_utils.egg-info/requires.txt
+-rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)       15 2023-06-15 04:03:56.000000 bs_admin_utils-1.1.1/bs_admin_utils.egg-info/top_level.txt
+-rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)        1 2023-06-15 04:03:56.000000 bs_admin_utils-1.1.1/bs_admin_utils.egg-info/zip-safe
+-rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)       38 2023-06-15 04:03:56.375122 bs_admin_utils-1.1.1/setup.cfg
+-rwxr-xr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)      620 2023-06-15 04:01:44.000000 bs_admin_utils-1.1.1/setup.py
```

### Comparing `bs_admin_utils-1.1.0/LICENSE` & `bs_admin_utils-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bs_admin_utils-1.1.0/bs_admin_utils/api.py` & `bs_admin_utils-1.1.1/bs_admin_utils/api.py`

 * *Files 5% similar despite different names*

```diff
@@ -68,33 +68,24 @@
 
     async def delete(self, id: str):
         if model := await self.model.from_id(id):
             await model.delete()
             return self.success
         return self.not_found()
 
-    async def get_list(
-        self,
-        rq: Request,
-        fetch_links: bool = True,
-        with_children: bool = True,
-        find_many: Optional[FindMany] = None
-    ):
+    async def get_list(self, rq: Request, fetch_links: bool = True, with_children: bool = True):
         skip, limit = get_data_range(rq)
-        kwargs = {
-            'fetch_links': fetch_links,
-            'limit': limit,
-            'skip': skip
-        }
+        models = self.model.find(
+            fetch_links=fetch_links,
+            limit=limit,
+            skip=skip,
+            with_children=with_children
+        )
 
-        if find_many is None:
-            kwargs['with_children'] = with_children
-
-        models = (find_many or self.model).find(**kwargs)
-        return await self.models_to_data(await models.count(), models)
+        return await self.models_to_data(await self.model.count(), models)
 
     async def save(self, data: dict, id: str = ''):
         await self.model.update_or_create(id, **data)
         return self.success
 
     # Response
```

### Comparing `bs_admin_utils-1.1.0/bs_admin_utils/model.py` & `bs_admin_utils-1.1.1/bs_admin_utils/model.py`

 * *Files identical despite different names*

### Comparing `bs_admin_utils-1.1.0/bs_admin_utils/static/arial.ttf` & `bs_admin_utils-1.1.1/bs_admin_utils/static/arial.ttf`

 * *Files identical despite different names*

### Comparing `bs_admin_utils-1.1.0/bs_admin_utils/static/nstc.ttf` & `bs_admin_utils-1.1.1/bs_admin_utils/static/nstc.ttf`

 * *Files identical despite different names*

### Comparing `bs_admin_utils-1.1.0/bs_admin_utils/vercode.py` & `bs_admin_utils-1.1.1/bs_admin_utils/vercode.py`

 * *Files identical despite different names*

### Comparing `bs_admin_utils-1.1.0/bs_admin_utils/websocket.py` & `bs_admin_utils-1.1.1/bs_admin_utils/websocket.py`

 * *Files identical despite different names*

### Comparing `bs_admin_utils-1.1.0/setup.py` & `bs_admin_utils-1.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     ],
     packages=find_packages(),
     package_data={
         'bs_admin_utils': ['*.ttf']
     },
     include_package_data=True,
     zip_safe=True,
-    version='1.1.0',
+    version='1.1.1',
     description='Blacksheep admin backend utils classes and function.',
     author='kiki-kanri',
     author_email='a470666@gmail.com',
     keywords=[],
     install_requires=[
         'beanie',
         'blacksheep',
```

