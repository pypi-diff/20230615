# Comparing `tmp/leocli-3.4.2.tar.gz` & `tmp/leocli-3.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "leocli-3.4.2.tar", max compression
+gzip compressed data, was "leocli-3.4.3.tar", max compression
```

## Comparing `leocli-3.4.2.tar` & `leocli-3.4.3.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0      265 2020-06-27 16:29:17.968091 leocli-3.4.2/leocli/__init__.py
--rw-r--r--   0        0        0     3195 2022-07-30 18:52:24.042936 leocli-3.4.2/leocli/cache.py
--rw-r--r--   0        0        0     2939 2022-07-30 18:05:19.634248 leocli-3.4.2/leocli/conf.py
--rw-r--r--   0        0        0     1036 2022-07-30 18:36:49.671999 leocli-3.4.2/leocli/consts.py
--rwxr-xr-x   0        0        0     9205 2022-07-30 18:37:03.103844 leocli-3.4.2/leocli/leo.py
--rw-r--r--   0        0        0      724 2023-04-27 07:06:54.166769 leocli-3.4.2/pyproject.toml
--rw-r--r--   0        0        0      848 1970-01-01 00:00:00.000000 leocli-3.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1291 2023-06-15 07:39:25.215909 leocli-3.4.3/README.md
+-rw-r--r--   0        0        0      265 2020-06-27 16:29:17.968091 leocli-3.4.3/leocli/__init__.py
+-rw-r--r--   0        0        0     3195 2022-07-30 18:52:24.042936 leocli-3.4.3/leocli/cache.py
+-rw-r--r--   0        0        0     2939 2022-07-30 18:05:19.634248 leocli-3.4.3/leocli/conf.py
+-rw-r--r--   0        0        0     1036 2022-07-30 18:36:49.671999 leocli-3.4.3/leocli/consts.py
+-rwxr-xr-x   0        0        0     9205 2022-07-30 18:37:03.103844 leocli-3.4.3/leocli/leo.py
+-rw-r--r--   0        0        0      768 2023-06-15 07:42:03.823369 leocli-3.4.3/pyproject.toml
+-rw-r--r--   0        0        0     2216 1970-01-01 00:00:00.000000 leocli-3.4.3/PKG-INFO
```

### Comparing `leocli-3.4.2/leocli/cache.py` & `leocli-3.4.3/leocli/cache.py`

 * *Files identical despite different names*

### Comparing `leocli-3.4.2/leocli/conf.py` & `leocli-3.4.3/leocli/conf.py`

 * *Files identical despite different names*

### Comparing `leocli-3.4.2/leocli/consts.py` & `leocli-3.4.3/leocli/consts.py`

 * *Files identical despite different names*

### Comparing `leocli-3.4.2/leocli/leo.py` & `leocli-3.4.3/leocli/leo.py`

 * *Files identical despite different names*

