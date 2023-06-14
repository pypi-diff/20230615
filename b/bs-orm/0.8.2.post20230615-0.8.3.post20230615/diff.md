# Comparing `tmp/bs_orm-0.8.2.post20230615.tar.gz` & `tmp/bs_orm-0.8.3.post20230615.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bs_orm-0.8.2.post20230615.tar", last modified: Wed Jun 14 22:23:20 2023, max compression
+gzip compressed data, was "bs_orm-0.8.3.post20230615.tar", last modified: Wed Jun 14 22:30:07 2023, max compression
```

## Comparing `bs_orm-0.8.2.post20230615.tar` & `bs_orm-0.8.3.post20230615.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 22:23:20.251822 bs_orm-0.8.2.post20230615/
--rw-rw-rw-   0        0        0      115 2023-06-14 22:23:20.251822 bs_orm-0.8.2.post20230615/PKG-INFO
--rw-rw-rw-   0        0        0     2557 2023-06-14 21:11:33.000000 bs_orm-0.8.2.post20230615/README.md
-drwxrwxrwx   0        0        0        0 2023-06-14 22:23:20.240278 bs_orm-0.8.2.post20230615/bs_orm/
--rw-rw-rw-   0        0        0     3281 2023-06-14 21:33:52.000000 bs_orm-0.8.2.post20230615/bs_orm/DataTypes.py
--rw-rw-rw-   0        0        0     9281 2023-06-14 22:15:19.000000 bs_orm-0.8.2.post20230615/bs_orm/Requests.py
--rw-rw-rw-   0        0        0        0 2023-06-14 21:11:33.000000 bs_orm-0.8.2.post20230615/bs_orm/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-14 22:23:20.249808 bs_orm-0.8.2.post20230615/bs_orm.egg-info/
--rw-rw-rw-   0        0        0      115 2023-06-14 22:23:20.000000 bs_orm-0.8.2.post20230615/bs_orm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      235 2023-06-14 22:23:20.000000 bs_orm-0.8.2.post20230615/bs_orm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 22:23:20.000000 bs_orm-0.8.2.post20230615/bs_orm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-14 22:23:20.000000 bs_orm-0.8.2.post20230615/bs_orm.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        7 2023-06-14 22:23:20.000000 bs_orm-0.8.2.post20230615/bs_orm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       51 2023-06-14 22:23:20.253816 bs_orm-0.8.2.post20230615/setup.cfg
--rw-rw-rw-   0        0        0      286 2023-06-14 22:23:11.000000 bs_orm-0.8.2.post20230615/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 22:30:07.154329 bs_orm-0.8.3.post20230615/
+-rw-rw-rw-   0        0        0      115 2023-06-14 22:30:07.154329 bs_orm-0.8.3.post20230615/PKG-INFO
+-rw-rw-rw-   0        0        0     2557 2023-06-14 21:11:33.000000 bs_orm-0.8.3.post20230615/README.md
+drwxrwxrwx   0        0        0        0 2023-06-14 22:30:07.144275 bs_orm-0.8.3.post20230615/bs_orm/
+-rw-rw-rw-   0        0        0     3281 2023-06-14 21:33:52.000000 bs_orm-0.8.3.post20230615/bs_orm/DataTypes.py
+-rw-rw-rw-   0        0        0     9283 2023-06-14 22:24:23.000000 bs_orm-0.8.3.post20230615/bs_orm/Requests.py
+-rw-rw-rw-   0        0        0        0 2023-06-14 21:11:33.000000 bs_orm-0.8.3.post20230615/bs_orm/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 22:30:07.152329 bs_orm-0.8.3.post20230615/bs_orm.egg-info/
+-rw-rw-rw-   0        0        0      115 2023-06-14 22:30:07.000000 bs_orm-0.8.3.post20230615/bs_orm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      235 2023-06-14 22:30:07.000000 bs_orm-0.8.3.post20230615/bs_orm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 22:30:07.000000 bs_orm-0.8.3.post20230615/bs_orm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-14 22:30:07.000000 bs_orm-0.8.3.post20230615/bs_orm.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        7 2023-06-14 22:30:07.000000 bs_orm-0.8.3.post20230615/bs_orm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       51 2023-06-14 22:30:07.155329 bs_orm-0.8.3.post20230615/setup.cfg
+-rw-rw-rw-   0        0        0      286 2023-06-14 22:30:01.000000 bs_orm-0.8.3.post20230615/setup.py
```

### Comparing `bs_orm-0.8.2.post20230615/README.md` & `bs_orm-0.8.3.post20230615/README.md`

 * *Files identical despite different names*

### Comparing `bs_orm-0.8.2.post20230615/bs_orm/DataTypes.py` & `bs_orm-0.8.3.post20230615/bs_orm/DataTypes.py`

 * *Files identical despite different names*

### Comparing `bs_orm-0.8.2.post20230615/bs_orm/Requests.py` & `bs_orm-0.8.3.post20230615/bs_orm/Requests.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,15 @@
     except Exception as ex:
         return ['error', ex]
 
 
 def for_default(content, request):
     try:
         if content.default:
-            request += f'DEFAULT {content.default}'
+            request += f'DEFAULT "{content.default}"'
         return ['ok', request]
     except Exception as ex:
         return ['error', ex]
 
 
 def for_check(content, request):
     try:
```

