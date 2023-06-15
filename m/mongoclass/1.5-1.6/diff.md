# Comparing `tmp/mongoclass-1.5.tar.gz` & `tmp/mongoclass-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongoclass-1.5.tar", last modified: Wed Apr 26 02:21:11 2023, max compression
+gzip compressed data, was "mongoclass-1.6.tar", last modified: Thu Jun 15 01:13:17 2023, max compression
```

## Comparing `mongoclass-1.5.tar` & `mongoclass-1.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-26 02:21:11.818704 mongoclass-1.5/
--rw-rw-rw-   0        0        0     1093 2022-10-28 01:48:28.000000 mongoclass-1.5/LICENSE
--rw-rw-rw-   0        0        0     3408 2023-04-26 02:21:11.818704 mongoclass-1.5/PKG-INFO
--rw-rw-rw-   0        0        0     2973 2022-10-28 01:48:28.000000 mongoclass-1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-26 02:21:11.786704 mongoclass-1.5/mongoclass/
--rw-rw-rw-   0        0        0       58 2022-10-28 01:48:28.000000 mongoclass-1.5/mongoclass/__init__.py
--rw-rw-rw-   0        0        0     5420 2023-04-18 14:44:13.000000 mongoclass-1.5/mongoclass/cache.py
--rw-rw-rw-   0        0        0    25925 2023-04-26 02:19:59.000000 mongoclass-1.5/mongoclass/client.py
--rw-rw-rw-   0        0        0     2015 2022-10-28 01:48:58.000000 mongoclass-1.5/mongoclass/cursor.py
-drwxrwxrwx   0        0        0        0 2023-04-26 02:21:11.816709 mongoclass-1.5/mongoclass.egg-info/
--rw-rw-rw-   0        0        0     3408 2023-04-26 02:21:11.000000 mongoclass-1.5/mongoclass.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      290 2023-04-26 02:21:11.000000 mongoclass-1.5/mongoclass.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-26 02:21:11.000000 mongoclass-1.5/mongoclass.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-04-26 02:21:11.000000 mongoclass-1.5/mongoclass.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-26 02:21:11.000000 mongoclass-1.5/mongoclass.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-04-26 02:21:11.820703 mongoclass-1.5/setup.cfg
--rw-rw-rw-   0        0        0      769 2023-04-26 02:20:39.000000 mongoclass-1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 01:13:17.657285 mongoclass-1.6/
+-rw-rw-rw-   0        0        0     1093 2022-10-28 01:48:28.000000 mongoclass-1.6/LICENSE
+-rw-rw-rw-   0        0        0     3408 2023-06-15 01:13:17.657285 mongoclass-1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2973 2022-10-28 01:48:28.000000 mongoclass-1.6/README.md
+drwxrwxrwx   0        0        0        0 2023-06-15 01:13:17.623428 mongoclass-1.6/mongoclass/
+-rw-rw-rw-   0        0        0       58 2022-10-28 01:48:28.000000 mongoclass-1.6/mongoclass/__init__.py
+-rw-rw-rw-   0        0        0     5420 2023-04-18 14:44:13.000000 mongoclass-1.6/mongoclass/cache.py
+-rw-rw-rw-   0        0        0    25999 2023-06-14 12:15:49.000000 mongoclass-1.6/mongoclass/client.py
+-rw-rw-rw-   0        0        0     2015 2022-10-28 01:48:58.000000 mongoclass-1.6/mongoclass/cursor.py
+drwxrwxrwx   0        0        0        0 2023-06-15 01:13:17.655408 mongoclass-1.6/mongoclass.egg-info/
+-rw-rw-rw-   0        0        0     3408 2023-06-15 01:13:17.000000 mongoclass-1.6/mongoclass.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      290 2023-06-15 01:13:17.000000 mongoclass-1.6/mongoclass.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 01:13:17.000000 mongoclass-1.6/mongoclass.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-06-15 01:13:17.000000 mongoclass-1.6/mongoclass.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-15 01:13:17.000000 mongoclass-1.6/mongoclass.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-15 01:13:17.659285 mongoclass-1.6/setup.cfg
+-rw-rw-rw-   0        0        0      769 2023-06-15 01:12:49.000000 mongoclass-1.6/setup.py
```

### Comparing `mongoclass-1.5/LICENSE` & `mongoclass-1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mongoclass-1.5/PKG-INFO` & `mongoclass-1.6/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: mongoclass
-Version: 1.5
-Summary: A basic ORM like interface for mongodb in python that uses dataclasses.
-Home-page: https://github.com/bossauh/mongoclass
-Download-URL: https://github.com/bossauh/mongoclass/archive/refs/tags/v_15.tar.gz
-Author: Philippe Mathew
-Author-email: philmattdev@gmail.com
-License: MIT
-Keywords: pymongo,orm
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Mongoclass
 A basic ORM like interface for mongodb in python that uses dataclasses.
 
 ## Installation
 To get started, install mongoclass using pip like so.
 ```bash
 pip install -U mongoclass
```

### Comparing `mongoclass-1.5/README.md` & `mongoclass-1.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: mongoclass
+Version: 1.6
+Summary: A basic ORM like interface for mongodb in python that uses dataclasses.
+Home-page: https://github.com/bossauh/mongoclass
+Download-URL: https://github.com/bossauh/mongoclass/archive/refs/tags/v_16.tar.gz
+Author: Philippe Mathew
+Author-email: philmattdev@gmail.com
+License: MIT
+Keywords: pymongo,orm
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Mongoclass
 A basic ORM like interface for mongodb in python that uses dataclasses.
 
 ## Installation
 To get started, install mongoclass using pip like so.
 ```bash
 pip install -U mongoclass
```

### Comparing `mongoclass-1.5/mongoclass/cache.py` & `mongoclass-1.6/mongoclass/cache.py`

 * *Files identical despite different names*

### Comparing `mongoclass-1.5/mongoclass/client.py` & `mongoclass-1.6/mongoclass/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -384,28 +384,30 @@
                         database: Optional[
                             Union[
                                 str,
                                 pymongo.database.Database,
                                 mongita.database.Database,
                             ]
                         ] = None,
+                        pre_call: Optional[Callable] = None,
                         page: int,
                         size: int,
                         **kwargs,
                     ) -> Cursor:
                         skip = (page - 1) * size
 
-                        results = (
-                            self.find_classes(
-                                collection_name, *args, database, **kwargs
-                            )
-                            .skip(skip)
-                            .limit(size)
+                        cursor = self.find_classes(
+                            collection_name, *args, database, **kwargs
                         )
 
+                        if pre_call:
+                            cursor = pre_call(cursor)
+
+                        results = cursor.skip(skip).limit(size)
+
                         return results
 
                     @staticmethod
                     def find_classes(
                         *args,
                         database: Optional[
                             Union[
```

### Comparing `mongoclass-1.5/mongoclass/cursor.py` & `mongoclass-1.6/mongoclass/cursor.py`

 * *Files identical despite different names*

### Comparing `mongoclass-1.5/mongoclass.egg-info/PKG-INFO` & `mongoclass-1.6/mongoclass.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: mongoclass
-Version: 1.5
+Version: 1.6
 Summary: A basic ORM like interface for mongodb in python that uses dataclasses.
 Home-page: https://github.com/bossauh/mongoclass
-Download-URL: https://github.com/bossauh/mongoclass/archive/refs/tags/v_15.tar.gz
+Download-URL: https://github.com/bossauh/mongoclass/archive/refs/tags/v_16.tar.gz
 Author: Philippe Mathew
 Author-email: philmattdev@gmail.com
 License: MIT
 Keywords: pymongo,orm
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `mongoclass-1.5/setup.py` & `mongoclass-1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 
 install_requires = ["dnspython==2.2.1", "mongita==1.1.1"]
 long_description = (Path(__file__).parent / "README.md").read_text()
 
 setup(
     name="mongoclass",
     packages=["mongoclass"],
-    version="1.5",
+    version="1.6",
     license="MIT",
     description="A basic ORM like interface for mongodb in python that uses dataclasses.",
     author="Philippe Mathew",
     author_email="philmattdev@gmail.com",
     url="https://github.com/bossauh/mongoclass",
-    download_url="https://github.com/bossauh/mongoclass/archive/refs/tags/v_15.tar.gz",
+    download_url="https://github.com/bossauh/mongoclass/archive/refs/tags/v_16.tar.gz",
     keywords=["pymongo", "orm"],
     install_requires=install_requires,
     long_description=long_description,
     long_description_content_type="text/markdown",
 )
```

