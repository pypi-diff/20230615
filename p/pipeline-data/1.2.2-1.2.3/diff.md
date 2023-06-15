# Comparing `tmp/pipeline-data-1.2.2.tar.gz` & `tmp/pipeline-data-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pipeline-data-1.2.2.tar", last modified: Fri Feb 24 08:40:18 2023, max compression
+gzip compressed data, was "pipeline-data-1.2.3.tar", last modified: Thu Jun 15 03:16:06 2023, max compression
```

## Comparing `pipeline-data-1.2.2.tar` & `pipeline-data-1.2.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-02-24 08:40:18.000000 pipeline-data-1.2.2/
--rw-rw-rw-   0        0        0      204 2023-02-24 08:40:18.000000 pipeline-data-1.2.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-02-24 08:40:18.000000 pipeline-data-1.2.2/pipeline_data/
--rw-rw-rw-   0        0        0      163 2022-10-21 07:17:13.000000 pipeline-data-1.2.2/pipeline_data/__init__.py
--rw-rw-rw-   0        0        0     7894 2022-10-21 07:21:49.000000 pipeline-data-1.2.2/pipeline_data/lock.py
--rw-rw-rw-   0        0        0    28399 2023-02-24 08:33:16.000000 pipeline-data-1.2.2/pipeline_data/pipeline.py
-drwxrwxrwx   0        0        0        0 2023-02-24 08:40:18.000000 pipeline-data-1.2.2/pipeline_data/sqla_decorator/
--rw-rw-rw-   0        0        0      595 2022-09-13 05:51:43.000000 pipeline-data-1.2.2/pipeline_data/sqla_decorator/__init__.py
--rw-rw-rw-   0        0        0    28892 2022-09-13 05:51:43.000000 pipeline-data-1.2.2/pipeline_data/sqla_decorator/engine.py
--rw-rw-rw-   0        0        0    29600 2022-09-13 05:51:43.000000 pipeline-data-1.2.2/pipeline_data/sqla_decorator/manager.py
--rw-rw-rw-   0        0        0     2787 2023-02-24 08:38:10.000000 pipeline-data-1.2.2/pipeline_data/sqla_decorator/models.py
--rw-rw-rw-   0        0        0     4240 2022-09-13 05:51:43.000000 pipeline-data-1.2.2/pipeline_data/sqla_decorator/session_ctx.py
-drwxrwxrwx   0        0        0        0 2023-02-24 08:40:18.000000 pipeline-data-1.2.2/pipeline_data/sqla_decorator/utils/
--rw-rw-rw-   0        0        0      266 2022-10-21 06:22:51.000000 pipeline-data-1.2.2/pipeline_data/sqla_decorator/utils/__init__.py
--rw-rw-rw-   0        0        0    19087 2023-02-24 08:33:16.000000 pipeline-data-1.2.2/pipeline_data/sqla_decorator/utils/db.py
--rw-rw-rw-   0        0        0     4726 2022-09-13 05:51:43.000000 pipeline-data-1.2.2/pipeline_data/sqla_decorator/utils/explain.py
--rw-rw-rw-   0        0        0     1373 2022-09-13 05:51:43.000000 pipeline-data-1.2.2/pipeline_data/sqla_decorator/utils/query_count.py
--rw-rw-rw-   0        0        0     3560 2022-10-21 06:12:05.000000 pipeline-data-1.2.2/pipeline_data/sqla_decorator/utils/tool.py
-drwxrwxrwx   0        0        0        0 2023-02-24 08:40:18.000000 pipeline-data-1.2.2/pipeline_data.egg-info/
--rw-rw-rw-   0        0        0      204 2023-02-24 08:40:18.000000 pipeline-data-1.2.2/pipeline_data.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      696 2023-02-24 08:40:18.000000 pipeline-data-1.2.2/pipeline_data.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-24 08:40:18.000000 pipeline-data-1.2.2/pipeline_data.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       91 2023-02-24 08:40:18.000000 pipeline-data-1.2.2/pipeline_data.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-02-24 08:40:18.000000 pipeline-data-1.2.2/pipeline_data.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-02-24 08:40:18.000000 pipeline-data-1.2.2/setup.cfg
--rw-rw-rw-   0        0        0      514 2023-02-24 08:40:03.000000 pipeline-data-1.2.2/setup.py
+drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-15 03:16:06.261892 pipeline-data-1.2.3/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       97 2023-06-15 03:16:06.260639 pipeline-data-1.2.3/PKG-INFO
+drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-15 03:16:06.046741 pipeline-data-1.2.3/pipeline_data/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      163 2022-10-21 07:17:13.000000 pipeline-data-1.2.3/pipeline_data/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     7894 2022-10-21 07:21:49.000000 pipeline-data-1.2.3/pipeline_data/lock.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    28399 2023-02-24 08:33:16.000000 pipeline-data-1.2.3/pipeline_data/pipeline.py
+drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-15 03:16:06.164801 pipeline-data-1.2.3/pipeline_data/sqla_decorator/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      595 2022-09-13 05:51:43.000000 pipeline-data-1.2.3/pipeline_data/sqla_decorator/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    28892 2022-09-13 05:51:43.000000 pipeline-data-1.2.3/pipeline_data/sqla_decorator/engine.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    29600 2022-09-13 05:51:43.000000 pipeline-data-1.2.3/pipeline_data/sqla_decorator/manager.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2787 2023-02-24 08:38:10.000000 pipeline-data-1.2.3/pipeline_data/sqla_decorator/models.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4240 2022-09-13 05:51:43.000000 pipeline-data-1.2.3/pipeline_data/sqla_decorator/session_ctx.py
+drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-15 03:16:06.246986 pipeline-data-1.2.3/pipeline_data/sqla_decorator/utils/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      266 2022-10-21 06:22:51.000000 pipeline-data-1.2.3/pipeline_data/sqla_decorator/utils/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    19197 2023-06-15 02:54:48.000000 pipeline-data-1.2.3/pipeline_data/sqla_decorator/utils/db.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4726 2022-09-13 05:51:43.000000 pipeline-data-1.2.3/pipeline_data/sqla_decorator/utils/explain.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1373 2022-09-13 05:51:43.000000 pipeline-data-1.2.3/pipeline_data/sqla_decorator/utils/query_count.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3560 2022-10-21 06:12:05.000000 pipeline-data-1.2.3/pipeline_data/sqla_decorator/utils/tool.py
+drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-15 03:16:06.099030 pipeline-data-1.2.3/pipeline_data.egg-info/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       97 2023-06-15 03:16:05.000000 pipeline-data-1.2.3/pipeline_data.egg-info/PKG-INFO
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      696 2023-06-15 03:16:05.000000 pipeline-data-1.2.3/pipeline_data.egg-info/SOURCES.txt
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        1 2023-06-15 03:16:05.000000 pipeline-data-1.2.3/pipeline_data.egg-info/dependency_links.txt
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       90 2023-06-15 03:16:05.000000 pipeline-data-1.2.3/pipeline_data.egg-info/requires.txt
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       14 2023-06-15 03:16:05.000000 pipeline-data-1.2.3/pipeline_data.egg-info/top_level.txt
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       38 2023-06-15 03:16:06.263254 pipeline-data-1.2.3/setup.cfg
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      513 2023-06-15 02:54:48.000000 pipeline-data-1.2.3/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pipeline-data-1.2.2/pipeline_data/lock.py` & `pipeline-data-1.2.3/pipeline_data/lock.py`

 * *Files identical despite different names*

### Comparing `pipeline-data-1.2.2/pipeline_data/pipeline.py` & `pipeline-data-1.2.3/pipeline_data/pipeline.py`

 * *Files identical despite different names*

### Comparing `pipeline-data-1.2.2/pipeline_data/sqla_decorator/__init__.py` & `pipeline-data-1.2.3/pipeline_data/sqla_decorator/__init__.py`

 * *Files identical despite different names*

### Comparing `pipeline-data-1.2.2/pipeline_data/sqla_decorator/engine.py` & `pipeline-data-1.2.3/pipeline_data/sqla_decorator/engine.py`

 * *Files identical despite different names*

### Comparing `pipeline-data-1.2.2/pipeline_data/sqla_decorator/manager.py` & `pipeline-data-1.2.3/pipeline_data/sqla_decorator/manager.py`

 * *Files identical despite different names*

### Comparing `pipeline-data-1.2.2/pipeline_data/sqla_decorator/models.py` & `pipeline-data-1.2.3/pipeline_data/sqla_decorator/models.py`

 * *Files identical despite different names*

### Comparing `pipeline-data-1.2.2/pipeline_data/sqla_decorator/session_ctx.py` & `pipeline-data-1.2.3/pipeline_data/sqla_decorator/session_ctx.py`

 * *Files identical despite different names*

### Comparing `pipeline-data-1.2.2/pipeline_data/sqla_decorator/utils/db.py` & `pipeline-data-1.2.3/pipeline_data/sqla_decorator/utils/db.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,19 +17,20 @@
 
 from sqlalchemy import update, and_, case, select, desc
 from sqlalchemy.orm.session import Session
 
 from ..session_ctx import ctx_session
 
 try:
-    from sqlalchemy.engine.result import ResultProxy, RowProxy
+    from sqlalchemy.engine.result import ResultProxy, RowProxy, ChunkedIteratorResult
 except ImportError:
     # sqlalchemy 1.4以上用法
     from sqlalchemy.engine.cursor import CursorResult as ResultProxy
     from sqlalchemy.engine.row import RowProxy
+    from sqlalchemy.engine.result import ChunkedIteratorResult
 
 from sqlalchemy.ext.compiler import compiles
 
 try:
     from sqlalchemy.ext.declarative.api import DeclarativeMeta
 except ImportError:
     from sqlalchemy.ext.declarative import DeclarativeMeta
@@ -114,15 +115,15 @@
     return keys
 
 
 def sqlalchemy_result_format(results, format_datetime=False):
     if isinstance(type(results), DeclarativeMeta):
         results = [results, ]
 
-    elif isinstance(results, (ResultProxy, Query)):
+    elif isinstance(results, (ResultProxy, Query, ChunkedIteratorResult)):
         if hasattr(results, 'fetchall'):
             results = results.fetchall()
         else:
             results = results.all()
 
     if not results or not isinstance(results, list):
         return results
```

### Comparing `pipeline-data-1.2.2/pipeline_data/sqla_decorator/utils/explain.py` & `pipeline-data-1.2.3/pipeline_data/sqla_decorator/utils/explain.py`

 * *Files identical despite different names*

### Comparing `pipeline-data-1.2.2/pipeline_data/sqla_decorator/utils/query_count.py` & `pipeline-data-1.2.3/pipeline_data/sqla_decorator/utils/query_count.py`

 * *Files identical despite different names*

### Comparing `pipeline-data-1.2.2/pipeline_data/sqla_decorator/utils/tool.py` & `pipeline-data-1.2.3/pipeline_data/sqla_decorator/utils/tool.py`

 * *Files identical despite different names*

### Comparing `pipeline-data-1.2.2/pipeline_data.egg-info/SOURCES.txt` & `pipeline-data-1.2.3/pipeline_data.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pipeline-data-1.2.2/setup.py` & `pipeline-data-1.2.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 # @Time      :2022/10/21 14:26
 # @Author    :huangkewei
 
 import setuptools
 
 setuptools.setup(
     name='pipeline-data',
-    version='1.2.2',
+    version='1.2.3',
     author='zhongbiao',
     description='数据同步',
     packages=setuptools.find_packages(),
     install_requires=[
-        'sqlalchemy==1.3.22',
+        'sqlalchemy~=1.4.0',
         'pottery==3.0.0',
         'werkzeug',
         'regex==2022.7.25',
         'cchardet==2.1.7',
         'pymysql==0.9.3'
     ]
 )
```

