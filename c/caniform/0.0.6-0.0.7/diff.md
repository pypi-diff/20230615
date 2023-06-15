# Comparing `tmp/caniform-0.0.6.tar.gz` & `tmp/caniform-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caniform-0.0.6.tar", last modified: Thu May  4 17:26:47 2023, max compression
+gzip compressed data, was "caniform-0.0.7.tar", last modified: Thu Jun 15 20:50:27 2023, max compression
```

## Comparing `caniform-0.0.6.tar` & `caniform-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 dev        (501) staff       (20)        0 2023-05-04 17:26:47.717943 caniform-0.0.6/
--rw-r--r--   0 dev        (501) staff       (20)     1112 2022-06-02 18:33:45.000000 caniform-0.0.6/LICENSE
--rw-r--r--   0 dev        (501) staff       (20)      610 2023-05-04 17:26:47.718110 caniform-0.0.6/PKG-INFO
--rw-r--r--   0 dev        (501) staff       (20)       93 2022-06-02 18:36:10.000000 caniform-0.0.6/README.md
--rw-r--r--   0 dev        (501) staff       (20)      151 2022-06-07 15:32:34.000000 caniform-0.0.6/pyproject.toml
--rw-r--r--   0 dev        (501) staff       (20)      642 2023-05-04 17:26:47.718906 caniform-0.0.6/setup.cfg
-drwxr-xr-x   0 dev        (501) staff       (20)        0 2023-05-04 17:26:47.706837 caniform-0.0.6/src/
-drwxr-xr-x   0 dev        (501) staff       (20)        0 2023-05-04 17:26:47.715801 caniform-0.0.6/src/caniform/
--rw-r--r--   0 dev        (501) staff       (20)     8879 2023-05-04 17:16:03.000000 caniform-0.0.6/src/caniform/Extend.py
--rw-r--r--   0 dev        (501) staff       (20)        0 2022-06-02 18:32:13.000000 caniform-0.0.6/src/caniform/__init__.py
-drwxr-xr-x   0 dev        (501) staff       (20)        0 2023-05-04 17:26:47.717573 caniform-0.0.6/src/caniform.egg-info/
--rw-r--r--   0 dev        (501) staff       (20)      610 2023-05-04 17:26:47.000000 caniform-0.0.6/src/caniform.egg-info/PKG-INFO
--rw-r--r--   0 dev        (501) staff       (20)      234 2023-05-04 17:26:47.000000 caniform-0.0.6/src/caniform.egg-info/SOURCES.txt
--rw-r--r--   0 dev        (501) staff       (20)        1 2023-05-04 17:26:47.000000 caniform-0.0.6/src/caniform.egg-info/dependency_links.txt
--rw-r--r--   0 dev        (501) staff       (20)        9 2023-05-04 17:26:47.000000 caniform-0.0.6/src/caniform.egg-info/top_level.txt
+drwxr-xr-x   0 dev        (501) staff       (20)        0 2023-06-15 20:50:27.338935 caniform-0.0.7/
+-rw-r--r--   0 dev        (501) staff       (20)     1112 2022-06-02 18:33:45.000000 caniform-0.0.7/LICENSE
+-rw-r--r--   0 dev        (501) staff       (20)      610 2023-06-15 20:50:27.339066 caniform-0.0.7/PKG-INFO
+-rw-r--r--   0 dev        (501) staff       (20)       93 2022-06-02 18:36:10.000000 caniform-0.0.7/README.md
+-rw-r--r--   0 dev        (501) staff       (20)      151 2022-06-07 15:32:34.000000 caniform-0.0.7/pyproject.toml
+-rw-r--r--   0 dev        (501) staff       (20)      642 2023-06-15 20:50:27.339711 caniform-0.0.7/setup.cfg
+drwxr-xr-x   0 dev        (501) staff       (20)        0 2023-06-15 20:50:27.334339 caniform-0.0.7/src/
+drwxr-xr-x   0 dev        (501) staff       (20)        0 2023-06-15 20:50:27.337444 caniform-0.0.7/src/caniform/
+-rw-r--r--   0 dev        (501) staff       (20)     9306 2023-06-15 20:48:14.000000 caniform-0.0.7/src/caniform/Extend.py
+-rw-r--r--   0 dev        (501) staff       (20)        0 2022-06-02 18:32:13.000000 caniform-0.0.7/src/caniform/__init__.py
+drwxr-xr-x   0 dev        (501) staff       (20)        0 2023-06-15 20:50:27.338691 caniform-0.0.7/src/caniform.egg-info/
+-rw-r--r--   0 dev        (501) staff       (20)      610 2023-06-15 20:50:27.000000 caniform-0.0.7/src/caniform.egg-info/PKG-INFO
+-rw-r--r--   0 dev        (501) staff       (20)      234 2023-06-15 20:50:27.000000 caniform-0.0.7/src/caniform.egg-info/SOURCES.txt
+-rw-r--r--   0 dev        (501) staff       (20)        1 2023-06-15 20:50:27.000000 caniform-0.0.7/src/caniform.egg-info/dependency_links.txt
+-rw-r--r--   0 dev        (501) staff       (20)        9 2023-06-15 20:50:27.000000 caniform-0.0.7/src/caniform.egg-info/top_level.txt
```

### Comparing `caniform-0.0.6/LICENSE` & `caniform-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `caniform-0.0.6/PKG-INFO` & `caniform-0.0.7/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caniform
-Version: 0.0.6
+Version: 0.0.7
 Summary: A package that extends the functionality of Pandas.
 Home-page: https://gitlab.com/tomathon/caniform/
 Author: tomathon
 Author-email: tomathon.dev@pm.me
 Project-URL: Bug Tracker, https://gitlab.com/tomathon/caniform/-/issues/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `caniform-0.0.6/setup.cfg` & `caniform-0.0.7/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = caniform
-version = 0.0.6
+version = 0.0.7
 author = tomathon
 author_email = tomathon.dev@pm.me
 description = A package that extends the functionality of Pandas.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://gitlab.com/tomathon/caniform/
 project_urls =
```

### Comparing `caniform-0.0.6/src/caniform/Extend.py` & `caniform-0.0.7/src/caniform/Extend.py`

 * *Files 3% similar despite different names*

```diff
@@ -241,7 +241,18 @@
         df = self._obj
         headers = {"Accept-Charset": "UTF-8"} if headers is None else headers
         payload_dict_list = self.__make_dict_list(df)
         processes = []
         with ThreadPoolExecutor(max_workers = n_max_workers) as executor:
             for pdl in payload_dict_list:
                 processes.append(executor.submit(self.__post_request, _payload_dict = pdl, _url = endpoint, _headers = headers))
+
+
+    def split_row(self, split_column, split_by):
+        df = self.__obj
+        tmp = df[df[split_column].str.contains(split_by)]
+        ret = df.drop(tmp.index)
+        tmp = tmp.reset_index(drop = True)
+        for r in range(tmp.shape[0]):
+            tmp.at[r, split_column] = tmp.at[r, split_column].split(split_by)
+        tmp = tmp.explode(split_column)
+        return pd.concat([ret, tmp]).reset_index(drop = True)
```

### Comparing `caniform-0.0.6/src/caniform.egg-info/PKG-INFO` & `caniform-0.0.7/src/caniform.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caniform
-Version: 0.0.6
+Version: 0.0.7
 Summary: A package that extends the functionality of Pandas.
 Home-page: https://gitlab.com/tomathon/caniform/
 Author: tomathon
 Author-email: tomathon.dev@pm.me
 Project-URL: Bug Tracker, https://gitlab.com/tomathon/caniform/-/issues/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

