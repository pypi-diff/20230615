# Comparing `tmp/cythonconst-1.0.0.tar.gz` & `tmp/cythonconst-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cythonconst-1.0.0.tar", last modified: Mon Jun 12 17:06:20 2023, max compression
+gzip compressed data, was "cythonconst-1.1.0.tar", last modified: Thu Jun 15 09:42:15 2023, max compression
```

## Comparing `cythonconst-1.0.0.tar` & `cythonconst-1.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 lysnikolaou   (501) staff       (20)        0 2023-06-12 17:06:20.993799 cythonconst-1.0.0/
--rw-r--r--   0 lysnikolaou   (501) staff       (20)      127 2023-06-12 17:06:20.993607 cythonconst-1.0.0/PKG-INFO
-drwxr-xr-x   0 lysnikolaou   (501) staff       (20)        0 2023-06-12 17:06:20.992412 cythonconst-1.0.0/cythonconst/
--rw-r--r--   0 lysnikolaou   (501) staff       (20)       81 2023-06-12 17:06:03.000000 cythonconst-1.0.0/cythonconst/__init__.py
--rw-r--r--   0 lysnikolaou   (501) staff       (20)   113625 2023-06-12 17:06:20.000000 cythonconst-1.0.0/cythonconst/plus.c
--rw-r--r--   0 lysnikolaou   (501) staff       (20)       76 2023-06-12 17:06:13.000000 cythonconst-1.0.0/cythonconst/plus.pyx
-drwxr-xr-x   0 lysnikolaou   (501) staff       (20)        0 2023-06-12 17:06:20.993201 cythonconst-1.0.0/cythonconst.egg-info/
--rw-r--r--   0 lysnikolaou   (501) staff       (20)      127 2023-06-12 17:06:20.000000 cythonconst-1.0.0/cythonconst.egg-info/PKG-INFO
--rw-r--r--   0 lysnikolaou   (501) staff       (20)      295 2023-06-12 17:06:20.000000 cythonconst-1.0.0/cythonconst.egg-info/SOURCES.txt
--rw-r--r--   0 lysnikolaou   (501) staff       (20)        1 2023-06-12 17:06:20.000000 cythonconst-1.0.0/cythonconst.egg-info/dependency_links.txt
--rw-r--r--   0 lysnikolaou   (501) staff       (20)        1 2023-06-12 17:06:20.000000 cythonconst-1.0.0/cythonconst.egg-info/not-zip-safe
--rw-r--r--   0 lysnikolaou   (501) staff       (20)       15 2023-06-12 17:06:20.000000 cythonconst-1.0.0/cythonconst.egg-info/requires.txt
--rw-r--r--   0 lysnikolaou   (501) staff       (20)       12 2023-06-12 17:06:20.000000 cythonconst-1.0.0/cythonconst.egg-info/top_level.txt
--rw-r--r--   0 lysnikolaou   (501) staff       (20)      281 2023-06-12 17:05:11.000000 cythonconst-1.0.0/pyproject.toml
--rw-r--r--   0 lysnikolaou   (501) staff       (20)       38 2023-06-12 17:06:20.993854 cythonconst-1.0.0/setup.cfg
--rw-r--r--   0 lysnikolaou   (501) staff       (20)      342 2023-06-12 17:05:31.000000 cythonconst-1.0.0/setup.py
+drwxr-xr-x   0 lysnikolaou   (501) staff       (20)        0 2023-06-15 09:42:15.106091 cythonconst-1.1.0/
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)      127 2023-06-15 09:42:15.105933 cythonconst-1.1.0/PKG-INFO
+drwxr-xr-x   0 lysnikolaou   (501) staff       (20)        0 2023-06-15 09:42:15.104588 cythonconst-1.1.0/cythonconst/
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)       81 2023-06-12 17:17:33.000000 cythonconst-1.1.0/cythonconst/__init__.py
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)   113597 2023-06-15 09:42:14.000000 cythonconst-1.1.0/cythonconst/plus.c
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)       76 2023-06-12 17:17:33.000000 cythonconst-1.1.0/cythonconst/plus.pyx
+drwxr-xr-x   0 lysnikolaou   (501) staff       (20)        0 2023-06-15 09:42:15.105692 cythonconst-1.1.0/cythonconst.egg-info/
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)      127 2023-06-15 09:42:15.000000 cythonconst-1.1.0/cythonconst.egg-info/PKG-INFO
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)      295 2023-06-15 09:42:15.000000 cythonconst-1.1.0/cythonconst.egg-info/SOURCES.txt
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)        1 2023-06-15 09:42:15.000000 cythonconst-1.1.0/cythonconst.egg-info/dependency_links.txt
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)        1 2023-06-12 17:06:20.000000 cythonconst-1.1.0/cythonconst.egg-info/not-zip-safe
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)       15 2023-06-15 09:42:15.000000 cythonconst-1.1.0/cythonconst.egg-info/requires.txt
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)       12 2023-06-15 09:42:15.000000 cythonconst-1.1.0/cythonconst.egg-info/top_level.txt
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)      397 2023-06-15 09:42:10.000000 cythonconst-1.1.0/pyproject.toml
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)       38 2023-06-15 09:42:15.106143 cythonconst-1.1.0/setup.cfg
+-rw-r--r--   0 lysnikolaou   (501) staff       (20)      342 2023-06-12 17:17:33.000000 cythonconst-1.1.0/setup.py
```

### Comparing `cythonconst-1.0.0/cythonconst/plus.c` & `cythonconst-1.1.0/cythonconst/plus.c`

 * *Files 0% similar despite different names*

```diff
@@ -1164,15 +1164,15 @@
 static int __Pyx_ImportFunction_0_29_35(PyObject *module, const char *funcname, void (**f)(void), const char *sig);
 
 /* InitStrings.proto */
 static int __Pyx_InitStrings(__Pyx_StringTabEntry *t);
 
 
 /* Module declarations from 'libcythonconst.lsum' */
-static PyObject *(*__pyx_f_14libcythonconst_4lsum_lsum)(int const , int const ); /*proto*/
+static PyObject *(*__pyx_f_14libcythonconst_4lsum_lsum)(int, int); /*proto*/
 
 /* Module declarations from 'cythonconst.plus' */
 #define __Pyx_MODULE_NAME "cythonconst.plus"
 extern int __pyx_module_is_main_cythonconst__plus;
 int __pyx_module_is_main_cythonconst__plus = 0;
 
 /* Implementation of 'cythonconst.plus' */
@@ -1409,15 +1409,15 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_function_import_code", 0);
   /*--- Function import code ---*/
   __pyx_t_1 = PyImport_ImportModule("libcythonconst.lsum"); if (!__pyx_t_1) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (__Pyx_ImportFunction_0_29_35(__pyx_t_1, "lsum", (void (**)(void))&__pyx_f_14libcythonconst_4lsum_lsum, "PyObject *(int const , int const )") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_0_29_35(__pyx_t_1, "lsum", (void (**)(void))&__pyx_f_14libcythonconst_4lsum_lsum, "PyObject *(int, int)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
```

