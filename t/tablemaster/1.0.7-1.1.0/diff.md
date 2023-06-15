# Comparing `tmp/tablemaster-1.0.7.tar.gz` & `tmp/tablemaster-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tablemaster-1.0.7.tar", last modified: Wed May 31 07:35:01 2023, max compression
+gzip compressed data, was "tablemaster-1.1.0.tar", last modified: Thu Jun 15 08:46:37 2023, max compression
```

## Comparing `tablemaster-1.0.7.tar` & `tablemaster-1.1.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 livid      (501) staff       (20)        0 2023-05-31 07:35:01.395635 tablemaster-1.0.7/
--rw-r--r--   0 livid      (501) staff       (20)    11357 2023-03-29 11:23:27.000000 tablemaster-1.0.7/LICENSE
--rw-r--r--   0 livid      (501) staff       (20)      239 2023-05-31 07:35:01.395494 tablemaster-1.0.7/PKG-INFO
--rw-r--r--   0 livid      (501) staff       (20)     1484 2023-05-24 06:49:43.000000 tablemaster-1.0.7/README.md
--rw-r--r--   0 livid      (501) staff       (20)       38 2023-05-31 07:35:01.395673 tablemaster-1.0.7/setup.cfg
--rw-r--r--   0 livid      (501) staff       (20)      521 2023-05-31 07:34:25.000000 tablemaster-1.0.7/setup.py
-drwxr-xr-x   0 livid      (501) staff       (20)        0 2023-05-31 07:35:01.394653 tablemaster-1.0.7/tablemaster/
--rw-r--r--   0 livid      (501) staff       (20)      490 2023-03-31 02:40:15.000000 tablemaster-1.0.7/tablemaster/__init__.py
--rw-r--r--   0 livid      (501) staff       (20)     1009 2023-05-31 07:12:09.000000 tablemaster-1.0.7/tablemaster/gspread.py
--rw-r--r--   0 livid      (501) staff       (20)     3395 2023-04-04 12:32:12.000000 tablemaster-1.0.7/tablemaster/mysql.py
--rw-r--r--   0 livid      (501) staff       (20)      810 2023-03-29 11:23:27.000000 tablemaster-1.0.7/tablemaster/utils.py
-drwxr-xr-x   0 livid      (501) staff       (20)        0 2023-05-31 07:35:01.395328 tablemaster-1.0.7/tablemaster.egg-info/
--rw-r--r--   0 livid      (501) staff       (20)      239 2023-05-31 07:35:01.000000 tablemaster-1.0.7/tablemaster.egg-info/PKG-INFO
--rw-r--r--   0 livid      (501) staff       (20)      289 2023-05-31 07:35:01.000000 tablemaster-1.0.7/tablemaster.egg-info/SOURCES.txt
--rw-r--r--   0 livid      (501) staff       (20)        1 2023-05-31 07:35:01.000000 tablemaster-1.0.7/tablemaster.egg-info/dependency_links.txt
--rw-r--r--   0 livid      (501) staff       (20)       92 2023-05-31 07:35:01.000000 tablemaster-1.0.7/tablemaster.egg-info/requires.txt
--rw-r--r--   0 livid      (501) staff       (20)       12 2023-05-31 07:35:01.000000 tablemaster-1.0.7/tablemaster.egg-info/top_level.txt
+drwxr-xr-x   0 livid      (501) staff       (20)        0 2023-06-15 08:46:37.625527 tablemaster-1.1.0/
+-rw-r--r--   0 livid      (501) staff       (20)    11357 2023-03-29 11:23:27.000000 tablemaster-1.1.0/LICENSE
+-rw-r--r--   0 livid      (501) staff       (20)      239 2023-06-15 08:46:37.625410 tablemaster-1.1.0/PKG-INFO
+-rw-r--r--   0 livid      (501) staff       (20)     1484 2023-05-24 06:49:43.000000 tablemaster-1.1.0/README.md
+-rw-r--r--   0 livid      (501) staff       (20)       38 2023-06-15 08:46:37.625561 tablemaster-1.1.0/setup.cfg
+-rw-r--r--   0 livid      (501) staff       (20)      559 2023-06-15 08:45:44.000000 tablemaster-1.1.0/setup.py
+drwxr-xr-x   0 livid      (501) staff       (20)        0 2023-06-15 08:46:37.624624 tablemaster-1.1.0/tablemaster/
+-rw-r--r--   0 livid      (501) staff       (20)      540 2023-06-15 08:44:02.000000 tablemaster-1.1.0/tablemaster/__init__.py
+-rw-r--r--   0 livid      (501) staff       (20)     1009 2023-05-31 07:12:09.000000 tablemaster-1.1.0/tablemaster/gspread.py
+-rw-r--r--   0 livid      (501) staff       (20)     2342 2023-06-15 08:35:52.000000 tablemaster-1.1.0/tablemaster/local.py
+-rw-r--r--   0 livid      (501) staff       (20)     3523 2023-06-15 07:01:48.000000 tablemaster-1.1.0/tablemaster/mysql.py
+-rw-r--r--   0 livid      (501) staff       (20)      810 2023-03-29 11:23:27.000000 tablemaster-1.1.0/tablemaster/utils.py
+drwxr-xr-x   0 livid      (501) staff       (20)        0 2023-06-15 08:46:37.625276 tablemaster-1.1.0/tablemaster.egg-info/
+-rw-r--r--   0 livid      (501) staff       (20)      239 2023-06-15 08:46:37.000000 tablemaster-1.1.0/tablemaster.egg-info/PKG-INFO
+-rw-r--r--   0 livid      (501) staff       (20)      310 2023-06-15 08:46:37.000000 tablemaster-1.1.0/tablemaster.egg-info/SOURCES.txt
+-rw-r--r--   0 livid      (501) staff       (20)        1 2023-06-15 08:46:37.000000 tablemaster-1.1.0/tablemaster.egg-info/dependency_links.txt
+-rw-r--r--   0 livid      (501) staff       (20)      108 2023-06-15 08:46:37.000000 tablemaster-1.1.0/tablemaster.egg-info/requires.txt
+-rw-r--r--   0 livid      (501) staff       (20)       12 2023-06-15 08:46:37.000000 tablemaster-1.1.0/tablemaster.egg-info/top_level.txt
```

### Comparing `tablemaster-1.0.7/LICENSE` & `tablemaster-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tablemaster-1.0.7/README.md` & `tablemaster-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `tablemaster-1.0.7/setup.py` & `tablemaster-1.1.0/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 from setuptools import setup, find_packages
 
 setup(
     name='tablemaster',
-    version='1.0.7',
+    version='1.1.0',
     packages=find_packages(),
     install_requires=[
         'PyMySQL',
         'SQLAlchemy==1.4.46',
         'pandas',
         'python-dateutil',
         'gspread',
         'tqdm',
         'numpy',
         'mysql-connector-python',
+        'pyyaml',
+        'openpyxl',
     ],
     author='Livid',
     author_email='livid.su@gmail.com',
     description='A Python package makes it easy to manage tables anywhere',
     url='https://github.com/ilivid/tablemaster'
 )
```

### Comparing `tablemaster-1.0.7/tablemaster/gspread.py` & `tablemaster-1.1.0/tablemaster/gspread.py`

 * *Files identical despite different names*

### Comparing `tablemaster-1.0.7/tablemaster/mysql.py` & `tablemaster-1.1.0/tablemaster/mysql.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,30 +16,34 @@
     try:
         cf_port = configs.port
     except:
         cf_port = 3306
     print(f'try to connect to {configs.name}...')
     conn = mysql.connector.connect(user=configs.user, password=configs.password, \
                                    host=configs.host, database=configs.database, port=cf_port)
-    cursor = conn.cursor()
     print('reading...')
     df = pd.read_sql(sql, conn)
+    conn.commit()
+    conn.close()
     return df
 
 
 def opt(sql, configs):
     try:
         cf_port = configs.port
     except:
         cf_port = 3306
     print(f'try to connect to {configs.name}...')
     conn = mysql.connector.connect(user=configs.user, password=configs.password, \
                                    host=configs.host, database=configs.database, port=cf_port)
     cursor = conn.cursor()
     cursor.execute(sql)
+    conn.commit()
+    cursor.close()
+    conn.close()
 
 
 class Manage_table:
     def __init__(self, table, configs):
         try:
             self.port = configs.port
         except:
@@ -92,8 +96,11 @@
         cursor = conn.cursor()
         del_query = f"delete from {self.table} where {clause} "
         print(del_query)
         try:
             cursor.execute(del_query)
             print(f'records of table that {clause} are deleted!')
         except:
-            print('del error!')
+            print('del error!')
+        conn.commit()
+        cursor.close()
+        conn.close()
```

### Comparing `tablemaster-1.0.7/tablemaster/utils.py` & `tablemaster-1.1.0/tablemaster/utils.py`

 * *Files identical despite different names*

