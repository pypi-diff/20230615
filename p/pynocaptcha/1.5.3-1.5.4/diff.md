# Comparing `tmp/pynocaptcha-1.5.3.tar.gz` & `tmp/pynocaptcha-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pynocaptcha-1.5.3.tar", last modified: Wed Jun 14 09:34:50 2023, max compression
+gzip compressed data, was "dist/pynocaptcha-1.5.4.tar", last modified: Thu Jun 15 08:58:20 2023, max compression
```

## Comparing `pynocaptcha-1.5.3.tar` & `pynocaptcha-1.5.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 esbiya     (501) staff       (20)        0 2023-06-14 09:34:50.000000 pynocaptcha-1.5.3/
--rw-r--r--   0 esbiya     (501) staff       (20)      566 2023-06-14 09:34:50.000000 pynocaptcha-1.5.3/PKG-INFO
-drwxr-xr-x   0 esbiya     (501) staff       (20)        0 2023-06-14 09:34:50.000000 pynocaptcha-1.5.3/pynocaptcha/
--rw-r--r--   0 esbiya     (501) staff       (20)      630 2023-06-14 09:34:47.000000 pynocaptcha-1.5.3/pynocaptcha/__init__.py
-drwxr-xr-x   0 esbiya     (501) staff       (20)        0 2023-06-14 09:34:50.000000 pynocaptcha-1.5.3/pynocaptcha/crackers/
--rw-r--r--   0 esbiya     (501) staff       (20)     1006 2023-06-14 09:31:37.000000 pynocaptcha-1.5.3/pynocaptcha/crackers/akamai.py
--rw-r--r--   0 esbiya     (501) staff       (20)     4715 2023-06-06 02:54:14.000000 pynocaptcha-1.5.3/pynocaptcha/crackers/base.py
--rw-r--r--   0 esbiya     (501) staff       (20)     5186 2023-04-23 09:01:32.000000 pynocaptcha-1.5.3/pynocaptcha/crackers/cloudflare.py
--rw-r--r--   0 esbiya     (501) staff       (20)     1339 2023-04-05 02:45:58.000000 pynocaptcha-1.5.3/pynocaptcha/crackers/hcaptcha.py
--rw-r--r--   0 esbiya     (501) staff       (20)   222114 2023-06-13 04:02:11.000000 pynocaptcha-1.5.3/pynocaptcha/crackers/incapsula.py
--rw-r--r--   0 esbiya     (501) staff       (20)     2449 2023-04-23 08:59:52.000000 pynocaptcha-1.5.3/pynocaptcha/crackers/recaptcha.py
--rw-r--r--   0 esbiya     (501) staff       (20)      890 2023-06-14 09:32:19.000000 pynocaptcha-1.5.3/pynocaptcha/crackers/tls.py
--rw-r--r--   0 esbiya     (501) staff       (20)      846 2023-06-14 09:33:44.000000 pynocaptcha-1.5.3/setup.py
+drwxr-xr-x   0 esbiya     (501) staff       (20)        0 2023-06-15 08:58:20.000000 pynocaptcha-1.5.4/
+-rw-r--r--   0 esbiya     (501) staff       (20)      566 2023-06-15 08:58:20.000000 pynocaptcha-1.5.4/PKG-INFO
+drwxr-xr-x   0 esbiya     (501) staff       (20)        0 2023-06-15 08:58:20.000000 pynocaptcha-1.5.4/pynocaptcha/
+-rw-r--r--   0 esbiya     (501) staff       (20)      630 2023-06-14 09:34:47.000000 pynocaptcha-1.5.4/pynocaptcha/__init__.py
+drwxr-xr-x   0 esbiya     (501) staff       (20)        0 2023-06-15 08:58:20.000000 pynocaptcha-1.5.4/pynocaptcha/crackers/
+-rw-r--r--   0 esbiya     (501) staff       (20)     1006 2023-06-14 09:31:37.000000 pynocaptcha-1.5.4/pynocaptcha/crackers/akamai.py
+-rw-r--r--   0 esbiya     (501) staff       (20)     4785 2023-06-15 08:58:13.000000 pynocaptcha-1.5.4/pynocaptcha/crackers/base.py
+-rw-r--r--   0 esbiya     (501) staff       (20)     5186 2023-04-23 09:01:32.000000 pynocaptcha-1.5.4/pynocaptcha/crackers/cloudflare.py
+-rw-r--r--   0 esbiya     (501) staff       (20)     1339 2023-04-05 02:45:58.000000 pynocaptcha-1.5.4/pynocaptcha/crackers/hcaptcha.py
+-rw-r--r--   0 esbiya     (501) staff       (20)   222114 2023-06-13 04:02:11.000000 pynocaptcha-1.5.4/pynocaptcha/crackers/incapsula.py
+-rw-r--r--   0 esbiya     (501) staff       (20)     2449 2023-04-23 08:59:52.000000 pynocaptcha-1.5.4/pynocaptcha/crackers/recaptcha.py
+-rw-r--r--   0 esbiya     (501) staff       (20)     1639 2023-06-15 08:25:19.000000 pynocaptcha-1.5.4/pynocaptcha/crackers/tls.py
+-rw-r--r--   0 esbiya     (501) staff       (20)      846 2023-06-15 08:18:05.000000 pynocaptcha-1.5.4/setup.py
```

### Comparing `pynocaptcha-1.5.3/PKG-INFO` & `pynocaptcha-1.5.4/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pynocaptcha
-Version: 1.5.3
+Version: 1.5.4
 Summary: nocaptcha.io api
 Home-page: UNKNOWN
 Author: UNKNOWN
 Author-email: UNKNOWN
 License: MIT
 Description: nocaptcha.io python api
 Keywords: nocaptcha
```

### Comparing `pynocaptcha-1.5.3/pynocaptcha/__init__.py` & `pynocaptcha-1.5.4/pynocaptcha/__init__.py`

 * *Files identical despite different names*

### Comparing `pynocaptcha-1.5.3/pynocaptcha/crackers/akamai.py` & `pynocaptcha-1.5.4/pynocaptcha/crackers/akamai.py`

 * *Files identical despite different names*

### Comparing `pynocaptcha-1.5.3/pynocaptcha/crackers/base.py` & `pynocaptcha-1.5.4/pynocaptcha/crackers/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -67,20 +67,22 @@
         self.wanda_args = {
             "internal": internal
         }
         for k in self.must_check_params:
             _v = kwargs.get(k)
             if not hasattr(self, k) or getattr(self, k) is None:
                 setattr(self, k, _v)
-            self.wanda_args.update({ k: _v })
+            if _v is not None:
+                self.wanda_args.update({ k: _v })
         for k, v in self.option_params.items():
             _v = kwargs.get(k, v)
             if not hasattr(self, k) or getattr(self, k) is None:
                 setattr(self, k, _v)
-            self.wanda_args.update({ k: _v })
+            if _v is not None:
+                self.wanda_args.update({ k: _v })
         
         for k in self.delete_params:
             if k in self.wanda_args:
                 del self.wanda_args[k]
 
         if any(getattr(self, k) is None for k in self.must_check_params):
            raise AttributeError("缺少参数, 请检查")
```

### Comparing `pynocaptcha-1.5.3/pynocaptcha/crackers/cloudflare.py` & `pynocaptcha-1.5.4/pynocaptcha/crackers/cloudflare.py`

 * *Files identical despite different names*

### Comparing `pynocaptcha-1.5.3/pynocaptcha/crackers/hcaptcha.py` & `pynocaptcha-1.5.4/pynocaptcha/crackers/hcaptcha.py`

 * *Files identical despite different names*

### Comparing `pynocaptcha-1.5.3/pynocaptcha/crackers/incapsula.py` & `pynocaptcha-1.5.4/pynocaptcha/crackers/incapsula.py`

 * *Files identical despite different names*

### Comparing `pynocaptcha-1.5.3/pynocaptcha/crackers/recaptcha.py` & `pynocaptcha-1.5.4/pynocaptcha/crackers/recaptcha.py`

 * *Files identical despite different names*

### Comparing `pynocaptcha-1.5.3/setup.py` & `pynocaptcha-1.5.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 
 from distutils.core import setup
 
 
 setup(
     name='pynocaptcha',
-    version='1.5.3',
+    version='1.5.4',
     description='nocaptcha.io api',
     long_description='nocaptcha.io python api',
     install_requires=["pyhttpx", "loguru"],
     license='MIT',
     packages=["pynocaptcha/crackers", "pynocaptcha"],
     package_dir={'pynocaptcha': 'pynocaptcha'},
     platforms=["all"],
```

