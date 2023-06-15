# Comparing `tmp/caniform-0.0.7.tar.gz` & `tmp/caniform-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caniform-0.0.7.tar", last modified: Thu Jun 15 20:50:27 2023, max compression
+gzip compressed data, was "caniform-0.0.8.tar", last modified: Thu Jun 15 20:54:46 2023, max compression
```

## Comparing `caniform-0.0.7.tar` & `caniform-0.0.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 dev        (501) staff       (20)        0 2023-06-15 20:50:27.338935 caniform-0.0.7/
--rw-r--r--   0 dev        (501) staff       (20)     1112 2022-06-02 18:33:45.000000 caniform-0.0.7/LICENSE
--rw-r--r--   0 dev        (501) staff       (20)      610 2023-06-15 20:50:27.339066 caniform-0.0.7/PKG-INFO
--rw-r--r--   0 dev        (501) staff       (20)       93 2022-06-02 18:36:10.000000 caniform-0.0.7/README.md
--rw-r--r--   0 dev        (501) staff       (20)      151 2022-06-07 15:32:34.000000 caniform-0.0.7/pyproject.toml
--rw-r--r--   0 dev        (501) staff       (20)      642 2023-06-15 20:50:27.339711 caniform-0.0.7/setup.cfg
-drwxr-xr-x   0 dev        (501) staff       (20)        0 2023-06-15 20:50:27.334339 caniform-0.0.7/src/
-drwxr-xr-x   0 dev        (501) staff       (20)        0 2023-06-15 20:50:27.337444 caniform-0.0.7/src/caniform/
--rw-r--r--   0 dev        (501) staff       (20)     9306 2023-06-15 20:48:14.000000 caniform-0.0.7/src/caniform/Extend.py
--rw-r--r--   0 dev        (501) staff       (20)        0 2022-06-02 18:32:13.000000 caniform-0.0.7/src/caniform/__init__.py
-drwxr-xr-x   0 dev        (501) staff       (20)        0 2023-06-15 20:50:27.338691 caniform-0.0.7/src/caniform.egg-info/
--rw-r--r--   0 dev        (501) staff       (20)      610 2023-06-15 20:50:27.000000 caniform-0.0.7/src/caniform.egg-info/PKG-INFO
--rw-r--r--   0 dev        (501) staff       (20)      234 2023-06-15 20:50:27.000000 caniform-0.0.7/src/caniform.egg-info/SOURCES.txt
--rw-r--r--   0 dev        (501) staff       (20)        1 2023-06-15 20:50:27.000000 caniform-0.0.7/src/caniform.egg-info/dependency_links.txt
--rw-r--r--   0 dev        (501) staff       (20)        9 2023-06-15 20:50:27.000000 caniform-0.0.7/src/caniform.egg-info/top_level.txt
+drwxr-xr-x   0 dev        (501) staff       (20)        0 2023-06-15 20:54:46.010411 caniform-0.0.8/
+-rw-r--r--   0 dev        (501) staff       (20)     1112 2022-06-02 18:33:45.000000 caniform-0.0.8/LICENSE
+-rw-r--r--   0 dev        (501) staff       (20)      610 2023-06-15 20:54:46.010517 caniform-0.0.8/PKG-INFO
+-rw-r--r--   0 dev        (501) staff       (20)       93 2022-06-02 18:36:10.000000 caniform-0.0.8/README.md
+-rw-r--r--   0 dev        (501) staff       (20)      151 2022-06-07 15:32:34.000000 caniform-0.0.8/pyproject.toml
+-rw-r--r--   0 dev        (501) staff       (20)      642 2023-06-15 20:54:46.011236 caniform-0.0.8/setup.cfg
+drwxr-xr-x   0 dev        (501) staff       (20)        0 2023-06-15 20:54:46.006433 caniform-0.0.8/src/
+drwxr-xr-x   0 dev        (501) staff       (20)        0 2023-06-15 20:54:46.008717 caniform-0.0.8/src/caniform/
+-rw-r--r--   0 dev        (501) staff       (20)     9305 2023-06-15 20:53:47.000000 caniform-0.0.8/src/caniform/Extend.py
+-rw-r--r--   0 dev        (501) staff       (20)        0 2022-06-02 18:32:13.000000 caniform-0.0.8/src/caniform/__init__.py
+drwxr-xr-x   0 dev        (501) staff       (20)        0 2023-06-15 20:54:46.010191 caniform-0.0.8/src/caniform.egg-info/
+-rw-r--r--   0 dev        (501) staff       (20)      610 2023-06-15 20:54:45.000000 caniform-0.0.8/src/caniform.egg-info/PKG-INFO
+-rw-r--r--   0 dev        (501) staff       (20)      234 2023-06-15 20:54:46.000000 caniform-0.0.8/src/caniform.egg-info/SOURCES.txt
+-rw-r--r--   0 dev        (501) staff       (20)        1 2023-06-15 20:54:45.000000 caniform-0.0.8/src/caniform.egg-info/dependency_links.txt
+-rw-r--r--   0 dev        (501) staff       (20)        9 2023-06-15 20:54:45.000000 caniform-0.0.8/src/caniform.egg-info/top_level.txt
```

### Comparing `caniform-0.0.7/LICENSE` & `caniform-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `caniform-0.0.7/PKG-INFO` & `caniform-0.0.8/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caniform
-Version: 0.0.7
+Version: 0.0.8
 Summary: A package that extends the functionality of Pandas.
 Home-page: https://gitlab.com/tomathon/caniform/
 Author: tomathon
 Author-email: tomathon.dev@pm.me
 Project-URL: Bug Tracker, https://gitlab.com/tomathon/caniform/-/issues/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `caniform-0.0.7/setup.cfg` & `caniform-0.0.8/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = caniform
-version = 0.0.7
+version = 0.0.8
 author = tomathon
 author_email = tomathon.dev@pm.me
 description = A package that extends the functionality of Pandas.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://gitlab.com/tomathon/caniform/
 project_urls =
```

### Comparing `caniform-0.0.7/src/caniform/Extend.py` & `caniform-0.0.8/src/caniform/Extend.py`

 * *Files 1% similar despite different names*

```diff
@@ -244,15 +244,15 @@
         processes = []
         with ThreadPoolExecutor(max_workers = n_max_workers) as executor:
             for pdl in payload_dict_list:
                 processes.append(executor.submit(self.__post_request, _payload_dict = pdl, _url = endpoint, _headers = headers))
 
 
     def split_row(self, split_column, split_by):
-        df = self.__obj
+        df = self._obj
         tmp = df[df[split_column].str.contains(split_by)]
         ret = df.drop(tmp.index)
         tmp = tmp.reset_index(drop = True)
         for r in range(tmp.shape[0]):
             tmp.at[r, split_column] = tmp.at[r, split_column].split(split_by)
         tmp = tmp.explode(split_column)
         return pd.concat([ret, tmp]).reset_index(drop = True)
```

### Comparing `caniform-0.0.7/src/caniform.egg-info/PKG-INFO` & `caniform-0.0.8/src/caniform.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caniform
-Version: 0.0.7
+Version: 0.0.8
 Summary: A package that extends the functionality of Pandas.
 Home-page: https://gitlab.com/tomathon/caniform/
 Author: tomathon
 Author-email: tomathon.dev@pm.me
 Project-URL: Bug Tracker, https://gitlab.com/tomathon/caniform/-/issues/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

