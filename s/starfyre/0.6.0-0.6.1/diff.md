# Comparing `tmp/starfyre-0.6.0.tar.gz` & `tmp/starfyre-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starfyre-0.6.0.tar", max compression
+gzip compressed data, was "starfyre-0.6.1.tar", max compression
```

## Comparing `starfyre-0.6.0.tar` & `starfyre-0.6.1.tar`

### file list

```diff
@@ -1,14 +1,13 @@
--rw-r--r--   0        0        0     2028 2023-02-27 19:03:24.900264 starfyre-0.6.0/README.md
--rw-r--r--   0        0        0      454 2023-04-30 23:22:27.844670 starfyre-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     1099 2023-04-30 23:09:33.032653 starfyre-0.6.0/starfyre/__init__.py
--rw-r--r--   0        0        0     1603 2023-04-30 23:09:53.013426 starfyre-0.6.0/starfyre/__main__.py
--rw-r--r--   0        0        0     4539 2023-04-30 22:55:52.651301 starfyre-0.6.0/starfyre/compiler.py
--rw-r--r--   0        0        0      535 2023-04-30 22:55:52.651503 starfyre-0.6.0/starfyre/component.py
--rw-r--r--   0        0        0     4135 2023-04-30 22:55:52.651684 starfyre-0.6.0/starfyre/dom_methods.py
--rw-r--r--   0        0        0      126 2023-02-21 21:24:47.371882 starfyre-0.6.0/starfyre/global_components.py
--rw-r--r--   0        0        0        0 2023-04-30 23:03:59.576897 starfyre-0.6.0/starfyre/js/__init__.py
--rw-r--r--   0        0        0     1093 2023-04-30 23:00:43.156472 starfyre-0.6.0/starfyre/js/store.js
--rw-r--r--   0        0        0     8837 2023-04-30 22:55:52.651893 starfyre-0.6.0/starfyre/parser.py
--rw-r--r--   0        0        0     3544 2023-04-30 22:55:52.652044 starfyre-0.6.0/starfyre/transpiler.py
--rw-r--r--   0        0        0     2774 1970-01-01 00:00:00.000000 starfyre-0.6.0/setup.py
--rw-r--r--   0        0        0     2566 1970-01-01 00:00:00.000000 starfyre-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     3215 2023-06-15 17:49:37.095611 starfyre-0.6.1/README.md
+-rw-r--r--   0        0        0      454 2023-06-15 17:49:37.095611 starfyre-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     1099 2023-06-15 17:49:37.099611 starfyre-0.6.1/starfyre/__init__.py
+-rw-r--r--   0        0        0     1603 2023-06-15 17:49:37.099611 starfyre-0.6.1/starfyre/__main__.py
+-rw-r--r--   0        0        0     4539 2023-06-15 17:49:37.099611 starfyre-0.6.1/starfyre/compiler.py
+-rw-r--r--   0        0        0      535 2023-06-15 17:49:37.099611 starfyre-0.6.1/starfyre/component.py
+-rw-r--r--   0        0        0     4135 2023-06-15 17:49:37.099611 starfyre-0.6.1/starfyre/dom_methods.py
+-rw-r--r--   0        0        0      126 2023-06-15 17:49:37.099611 starfyre-0.6.1/starfyre/global_components.py
+-rw-r--r--   0        0        0        0 2023-06-15 17:49:37.099611 starfyre-0.6.1/starfyre/js/__init__.py
+-rw-r--r--   0        0        0     1093 2023-06-15 17:49:37.099611 starfyre-0.6.1/starfyre/js/store.js
+-rw-r--r--   0        0        0     8837 2023-06-15 17:49:37.099611 starfyre-0.6.1/starfyre/parser.py
+-rw-r--r--   0        0        0     3544 2023-06-15 17:49:37.099611 starfyre-0.6.1/starfyre/transpiler.py
+-rw-r--r--   0        0        0     3753 1970-01-01 00:00:00.000000 starfyre-0.6.1/PKG-INFO
```

### Comparing `starfyre-0.6.0/starfyre/__init__.py` & `starfyre-0.6.1/starfyre/__init__.py`

 * *Files identical despite different names*

### Comparing `starfyre-0.6.0/starfyre/__main__.py` & `starfyre-0.6.1/starfyre/__main__.py`

 * *Files identical despite different names*

### Comparing `starfyre-0.6.0/starfyre/compiler.py` & `starfyre-0.6.1/starfyre/compiler.py`

 * *Files identical despite different names*

### Comparing `starfyre-0.6.0/starfyre/component.py` & `starfyre-0.6.1/starfyre/component.py`

 * *Files identical despite different names*

### Comparing `starfyre-0.6.0/starfyre/dom_methods.py` & `starfyre-0.6.1/starfyre/dom_methods.py`

 * *Files identical despite different names*

### Comparing `starfyre-0.6.0/starfyre/js/store.js` & `starfyre-0.6.1/starfyre/js/store.js`

 * *Files identical despite different names*

### Comparing `starfyre-0.6.0/starfyre/parser.py` & `starfyre-0.6.1/starfyre/parser.py`

 * *Files identical despite different names*

### Comparing `starfyre-0.6.0/starfyre/transpiler.py` & `starfyre-0.6.1/starfyre/transpiler.py`

 * *Files identical despite different names*

