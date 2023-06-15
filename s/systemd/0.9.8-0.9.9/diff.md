# Comparing `tmp/systemd-0.9.8.tar.gz` & `tmp/systemd-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/systemd-0.9.8.tar", last modified: Wed Mar 15 13:18:31 2017, max compression
+gzip compressed data, was "dist/systemd-0.9.9.tar", last modified: Tue Apr 11 21:15:43 2017, max compression
```

## Comparing `systemd-0.9.8.tar` & `systemd-0.9.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 mosquito   (501) staff       (20)        0 2017-03-15 13:18:31.000000 systemd-0.9.8/
--rw-r--r--   0 mosquito   (501) staff       (20)      156 2016-08-29 17:49:38.000000 systemd-0.9.8/MANIFEST.in
--rw-r--r--   0 mosquito   (501) staff       (20)     3420 2017-03-15 13:18:31.000000 systemd-0.9.8/PKG-INFO
--rw-r--r--   0 mosquito   (501) staff       (20)     1451 2016-09-02 08:47:26.000000 systemd-0.9.8/README.rst
--rw-r--r--   0 mosquito   (501) staff       (20)       59 2017-03-15 13:18:31.000000 systemd-0.9.8/setup.cfg
--rw-r--r--   0 mosquito   (501) staff       (20)     2385 2016-11-29 16:57:53.000000 systemd-0.9.8/setup.py
-drwxr-xr-x   0 mosquito   (501) staff       (20)        0 2017-03-15 13:18:31.000000 systemd-0.9.8/systemd/
--rw-r--r--   0 mosquito   (501) staff       (20)      470 2017-03-15 13:18:17.000000 systemd-0.9.8/systemd/__init__.py
--rw-r--r--   0 mosquito   (501) staff       (20)   108809 2017-03-15 13:18:30.000000 systemd-0.9.8/systemd/_daemon.c
--rw-r--r--   0 mosquito   (501) staff       (20)      647 2016-11-29 17:14:22.000000 systemd-0.9.8/systemd/_daemon.pyx
--rw-r--r--   0 mosquito   (501) staff       (20)   180806 2017-03-15 13:18:30.000000 systemd-0.9.8/systemd/_journal.c
--rw-r--r--   0 mosquito   (501) staff       (20)     2046 2016-11-29 17:27:09.000000 systemd-0.9.8/systemd/_journal.pyx
--rw-r--r--   0 mosquito   (501) staff       (20)     2075 2016-11-29 17:21:47.000000 systemd-0.9.8/systemd/daemon.py
--rw-r--r--   0 mosquito   (501) staff       (20)     3948 2017-03-15 13:18:07.000000 systemd-0.9.8/systemd/journal.py
--rw-r--r--   0 mosquito   (501) staff       (20)      109 2016-11-29 17:14:22.000000 systemd-0.9.8/systemd/sd_daemon.pxd
--rw-r--r--   0 mosquito   (501) staff       (20)      333 2016-11-29 17:14:22.000000 systemd-0.9.8/systemd/sd_journal.pxd
-drwxr-xr-x   0 mosquito   (501) staff       (20)        0 2017-03-15 13:18:31.000000 systemd-0.9.8/systemd.egg-info/
--rw-r--r--   0 mosquito   (501) staff       (20)        1 2017-03-15 13:18:31.000000 systemd-0.9.8/systemd.egg-info/dependency_links.txt
--rw-r--r--   0 mosquito   (501) staff       (20)     3420 2017-03-15 13:18:31.000000 systemd-0.9.8/systemd.egg-info/PKG-INFO
--rw-r--r--   0 mosquito   (501) staff       (20)      335 2017-03-15 13:18:31.000000 systemd-0.9.8/systemd.egg-info/SOURCES.txt
--rw-r--r--   0 mosquito   (501) staff       (20)        8 2017-03-15 13:18:31.000000 systemd-0.9.8/systemd.egg-info/top_level.txt
+drwxr-xr-x   0 mosquito   (501) staff       (20)        0 2017-04-11 21:15:43.000000 systemd-0.9.9/
+-rw-r--r--   0 mosquito   (501) staff       (20)      156 2016-08-29 17:49:38.000000 systemd-0.9.9/MANIFEST.in
+-rw-r--r--   0 mosquito   (501) staff       (20)     3462 2017-04-11 21:15:43.000000 systemd-0.9.9/PKG-INFO
+-rw-r--r--   0 mosquito   (501) staff       (20)     1451 2016-09-02 08:47:26.000000 systemd-0.9.9/README.rst
+-rw-r--r--   0 mosquito   (501) staff       (20)       38 2017-04-11 21:15:43.000000 systemd-0.9.9/setup.cfg
+-rw-r--r--   0 mosquito   (501) staff       (20)     2543 2017-04-11 21:12:21.000000 systemd-0.9.9/setup.py
+drwxr-xr-x   0 mosquito   (501) staff       (20)        0 2017-04-11 21:15:43.000000 systemd-0.9.9/systemd/
+-rw-r--r--   0 mosquito   (501) staff       (20)      470 2017-04-11 21:15:23.000000 systemd-0.9.9/systemd/__init__.py
+-rw-r--r--   0 mosquito   (501) staff       (20)   110361 2017-04-11 21:15:42.000000 systemd-0.9.9/systemd/_daemon.c
+-rw-r--r--   0 mosquito   (501) staff       (20)      628 2017-04-11 20:58:38.000000 systemd-0.9.9/systemd/_daemon.pyx
+-rw-r--r--   0 mosquito   (501) staff       (20)   180803 2017-04-11 21:15:43.000000 systemd-0.9.9/systemd/_journal.c
+-rw-r--r--   0 mosquito   (501) staff       (20)     2046 2016-11-29 17:27:09.000000 systemd-0.9.9/systemd/_journal.pyx
+-rw-r--r--   0 mosquito   (501) staff       (20)     2059 2017-04-11 21:12:21.000000 systemd-0.9.9/systemd/daemon.py
+-rw-r--r--   0 mosquito   (501) staff       (20)     4080 2017-04-11 21:14:21.000000 systemd-0.9.9/systemd/journal.py
+-rw-r--r--   0 mosquito   (501) staff       (20)      109 2016-11-29 17:14:22.000000 systemd-0.9.9/systemd/sd_daemon.pxd
+-rw-r--r--   0 mosquito   (501) staff       (20)      333 2016-11-29 17:14:22.000000 systemd-0.9.9/systemd/sd_journal.pxd
+drwxr-xr-x   0 mosquito   (501) staff       (20)        0 2017-04-11 21:15:43.000000 systemd-0.9.9/systemd.egg-info/
+-rw-r--r--   0 mosquito   (501) staff       (20)        1 2017-04-11 21:15:43.000000 systemd-0.9.9/systemd.egg-info/dependency_links.txt
+-rw-r--r--   0 mosquito   (501) staff       (20)     3462 2017-04-11 21:15:43.000000 systemd-0.9.9/systemd.egg-info/PKG-INFO
+-rw-r--r--   0 mosquito   (501) staff       (20)      335 2017-04-11 21:15:43.000000 systemd-0.9.9/systemd.egg-info/SOURCES.txt
+-rw-r--r--   0 mosquito   (501) staff       (20)        8 2017-04-11 21:15:43.000000 systemd-0.9.9/systemd.egg-info/top_level.txt
```

### Comparing `systemd-0.9.8/PKG-INFO` & `systemd-0.9.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: systemd
-Version: 0.9.8
+Version: 0.9.9
 Summary: Python systemd wrapper
 Home-page: http://github.com/mosquito/python-systemd
 Author: Dmitry Orlov <me@mosquito.su>
 Author-email: me@mosquito.su
 License: Apache
 Description: SystemD
         =======
@@ -110,15 +110,16 @@
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Natural Language :: Russian
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Cython
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 2.7
+Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: System
 Classifier: Topic :: System :: Operating System
```

### Comparing `systemd-0.9.8/README.rst` & `systemd-0.9.9/README.rst`

 * *Files identical despite different names*

### Comparing `systemd-0.9.8/setup.py` & `systemd-0.9.9/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,20 @@
 #!/usr/bin/env python
 # encoding: utf-8
+import sys
 import systemd as module
 from setuptools import setup, Extension
 
 
+requires = []
+
+if sys.version_info < (3, 4):
+    requires += ['enum34']
+
+
 try:
     from Cython.Build import cythonize
 
     extensions = cythonize([
         Extension(
             "systemd._daemon",
             ["systemd/_daemon.pyx"],
@@ -66,17 +73,19 @@
         'Intended Audience :: End Users/Desktop',
         'License :: OSI Approved :: Apache Software License',
         'Natural Language :: English',
         'Natural Language :: Russian',
         'Operating System :: POSIX :: Linux',
         'Programming Language :: Cython',
         'Programming Language :: Python',
-        'Programming Language :: Python :: 3 :: Only',
+        'Programming Language :: Python :: 2.7',
+        'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.4',
         'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: Implementation :: CPython',
         'Topic :: Software Development :: Libraries',
         'Topic :: System',
         'Topic :: System :: Operating System',
     ],
-)
+    install_requires=requires,
+)
```

### Comparing `systemd-0.9.8/systemd/_daemon.c` & `systemd-0.9.9/systemd/_daemon.c`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 /* Generated by Cython 0.24.1 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
-        "depends": [], 
+        "depends": [],
         "libraries": [
             "systemd"
         ]
-    }, 
+    },
     "module_name": "systemd._daemon"
 }
 END: Cython Metadata */
 
 #define PY_SSIZE_T_CLEAN
 #include "Python.h"
 #ifndef Py_PYTHON_H
@@ -733,30 +733,30 @@
 static PyObject *__pyx_tuple_;
 static PyObject *__pyx_tuple__2;
 static PyObject *__pyx_codeobj__3;
 
 /* "systemd/_daemon.pyx":4
  * 
  * 
- * def sd_notify(line: str, unset_environment: bool=False) -> int:             # <<<<<<<<<<<<<<
+ * def sd_notify(line, unset_environment=False):             # <<<<<<<<<<<<<<
  *     """ Send notification to systemd daemon
  * 
  */
 
 #line 4 "systemd/_daemon.pyx"
 
 
 #line 4 "systemd/_daemon.pyx"
 /* Python wrapper */
 
 #line 4 "systemd/_daemon.pyx"
 static PyObject *__pyx_pw_7systemd_7_daemon_1sd_notify(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 
 #line 4 "systemd/_daemon.pyx"
-static char __pyx_doc_7systemd_7_daemon_sd_notify[] = " Send notification to systemd daemon\n\n    :type notification: Notification\n    :param notification: Notification instance\n    :param value: str or int value for non constant notifications\n    :returns None\n    ";
+static char __pyx_doc_7systemd_7_daemon_sd_notify[] = " Send notification to systemd daemon\n\n    :type line: str\n    :type: unset_environment: bool\n    :return: int\n    :raises RuntimeError: When c-call returns zero \n    :raises ValueError: Otherwise\n    ";
 static PyMethodDef __pyx_mdef_7systemd_7_daemon_1sd_notify = 
 #line 4 "systemd/_daemon.pyx"
 {"sd_notify", (PyCFunction)__pyx_pw_7systemd_7_daemon_1sd_notify, METH_VARARGS|METH_KEYWORDS, __pyx_doc_7systemd_7_daemon_sd_notify};
 
 #line 4 "systemd/_daemon.pyx"
 static PyObject *__pyx_pw_7systemd_7_daemon_1sd_notify(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_line = 0
@@ -969,312 +969,375 @@
 
 #line 4 "systemd/_daemon.pyx"
   __Pyx_RefNannySetupContext("sd_notify", 0);
 
 #line 4 "systemd/_daemon.pyx"
   __Pyx_INCREF(__pyx_v_line);
 
-  /* "systemd/_daemon.pyx":13
+  /* "systemd/_daemon.pyx":14
  *     """
  * 
  *     line = line.encode()             # <<<<<<<<<<<<<<
  * 
  *     cdef int unset_env
  */
 
-#line 13 "systemd/_daemon.pyx"
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_line, __pyx_n_s_encode); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 13, __pyx_L1_error)
+#line 14 "systemd/_daemon.pyx"
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_line, __pyx_n_s_encode); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 14, __pyx_L1_error)
 
-#line 13 "systemd/_daemon.pyx"
+#line 14 "systemd/_daemon.pyx"
   __Pyx_GOTREF(__pyx_t_2);
 
-#line 13 "systemd/_daemon.pyx"
+#line 14 "systemd/_daemon.pyx"
   __pyx_t_3 = NULL;
 
-#line 13 "systemd/_daemon.pyx"
+#line 14 "systemd/_daemon.pyx"
   if (CYTHON_COMPILING_IN_CPYTHON && likely(PyMethod_Check(__pyx_t_2))) {
 
-#line 13 "systemd/_daemon.pyx"
+#line 14 "systemd/_daemon.pyx"
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
 
-#line 13 "systemd/_daemon.pyx"
+#line 14 "systemd/_daemon.pyx"
     if (likely(__pyx_t_3)) {
 
-#line 13 "systemd/_daemon.pyx"
+#line 14 "systemd/_daemon.pyx"
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
 
-#line 13 "systemd/_daemon.pyx"
+#line 14 "systemd/_daemon.pyx"
       __Pyx_INCREF(__pyx_t_3);
 
-#line 13 "systemd/_daemon.pyx"
+#line 14 "systemd/_daemon.pyx"
       __Pyx_INCREF(function);
 
-#line 13 "systemd/_daemon.pyx"
+#line 14 "systemd/_daemon.pyx"
       __Pyx_DECREF_SET(__pyx_t_2, function);
 
-#line 13 "systemd/_daemon.pyx"
+#line 14 "systemd/_daemon.pyx"
     }
 
-#line 13 "systemd/_daemon.pyx"
+#line 14 "systemd/_daemon.pyx"
   }
 
-#line 13 "systemd/_daemon.pyx"
+#line 14 "systemd/_daemon.pyx"
   if (__pyx_t_3) {
 
-#line 13 "systemd/_daemon.pyx"
-    __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 13, __pyx_L1_error)
+#line 14 "systemd/_daemon.pyx"
+    __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 14, __pyx_L1_error)
 
-#line 13 "systemd/_daemon.pyx"
+#line 14 "systemd/_daemon.pyx"
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-#line 13 "systemd/_daemon.pyx"
+#line 14 "systemd/_daemon.pyx"
   } else {
 
-#line 13 "systemd/_daemon.pyx"
-    __pyx_t_1 = __Pyx_PyObject_CallNoArg(__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 13, __pyx_L1_error)
+#line 14 "systemd/_daemon.pyx"
+    __pyx_t_1 = __Pyx_PyObject_CallNoArg(__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 14, __pyx_L1_error)
 
-#line 13 "systemd/_daemon.pyx"
+#line 14 "systemd/_daemon.pyx"
   }
 
-#line 13 "systemd/_daemon.pyx"
+#line 14 "systemd/_daemon.pyx"
   __Pyx_GOTREF(__pyx_t_1);
 
-#line 13 "systemd/_daemon.pyx"
+#line 14 "systemd/_daemon.pyx"
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-#line 13 "systemd/_daemon.pyx"
+#line 14 "systemd/_daemon.pyx"
   __Pyx_DECREF_SET(__pyx_v_line, __pyx_t_1);
 
-#line 13 "systemd/_daemon.pyx"
+#line 14 "systemd/_daemon.pyx"
   __pyx_t_1 = 0;
 
-  /* "systemd/_daemon.pyx":16
+  /* "systemd/_daemon.pyx":17
  * 
  *     cdef int unset_env
  *     unset_env = 2 if unset_environment else 0             # <<<<<<<<<<<<<<
  * 
- *     result = sd_daemon.sd_notify(unset_env, line)
+ *     result = sd_daemon.sd_notify(unset_env, line.encode())
  */
 
-#line 16 "systemd/_daemon.pyx"
-  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_v_unset_environment); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 16, __pyx_L1_error)
+#line 17 "systemd/_daemon.pyx"
+  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_v_unset_environment); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 17, __pyx_L1_error)
 
-#line 16 "systemd/_daemon.pyx"
+#line 17 "systemd/_daemon.pyx"
   if (__pyx_t_5) {
 
-#line 16 "systemd/_daemon.pyx"
+#line 17 "systemd/_daemon.pyx"
     __pyx_t_4 = 2;
 
-#line 16 "systemd/_daemon.pyx"
+#line 17 "systemd/_daemon.pyx"
   } else {
 
-#line 16 "systemd/_daemon.pyx"
+#line 17 "systemd/_daemon.pyx"
     __pyx_t_4 = 0;
 
-#line 16 "systemd/_daemon.pyx"
+#line 17 "systemd/_daemon.pyx"
   }
 
-#line 16 "systemd/_daemon.pyx"
+#line 17 "systemd/_daemon.pyx"
   __pyx_v_unset_env = __pyx_t_4;
 
-  /* "systemd/_daemon.pyx":18
+  /* "systemd/_daemon.pyx":19
  *     unset_env = 2 if unset_environment else 0
  * 
- *     result = sd_daemon.sd_notify(unset_env, line)             # <<<<<<<<<<<<<<
+ *     result = sd_daemon.sd_notify(unset_env, line.encode())             # <<<<<<<<<<<<<<
  * 
  *     if result > 0:
  */
 
-#line 18 "systemd/_daemon.pyx"
-  __pyx_t_6 = __Pyx_PyObject_AsString(__pyx_v_line); if (unlikely((!__pyx_t_6) && PyErr_Occurred())) __PYX_ERR(0, 18, __pyx_L1_error)
+#line 19 "systemd/_daemon.pyx"
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_line, __pyx_n_s_encode); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 19, __pyx_L1_error)
 
-#line 18 "systemd/_daemon.pyx"
-  __pyx_t_1 = __Pyx_PyInt_From_int(sd_notify(__pyx_v_unset_env, __pyx_t_6)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 18, __pyx_L1_error)
+#line 19 "systemd/_daemon.pyx"
+  __Pyx_GOTREF(__pyx_t_2);
+
+#line 19 "systemd/_daemon.pyx"
+  __pyx_t_3 = NULL;
+
+#line 19 "systemd/_daemon.pyx"
+  if (CYTHON_COMPILING_IN_CPYTHON && likely(PyMethod_Check(__pyx_t_2))) {
+
+#line 19 "systemd/_daemon.pyx"
+    __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
+
+#line 19 "systemd/_daemon.pyx"
+    if (likely(__pyx_t_3)) {
+
+#line 19 "systemd/_daemon.pyx"
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
+
+#line 19 "systemd/_daemon.pyx"
+      __Pyx_INCREF(__pyx_t_3);
+
+#line 19 "systemd/_daemon.pyx"
+      __Pyx_INCREF(function);
+
+#line 19 "systemd/_daemon.pyx"
+      __Pyx_DECREF_SET(__pyx_t_2, function);
+
+#line 19 "systemd/_daemon.pyx"
+    }
+
+#line 19 "systemd/_daemon.pyx"
+  }
+
+#line 19 "systemd/_daemon.pyx"
+  if (__pyx_t_3) {
+
+#line 19 "systemd/_daemon.pyx"
+    __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 19, __pyx_L1_error)
+
+#line 19 "systemd/_daemon.pyx"
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-#line 18 "systemd/_daemon.pyx"
+#line 19 "systemd/_daemon.pyx"
+  } else {
+
+#line 19 "systemd/_daemon.pyx"
+    __pyx_t_1 = __Pyx_PyObject_CallNoArg(__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 19, __pyx_L1_error)
+
+#line 19 "systemd/_daemon.pyx"
+  }
+
+#line 19 "systemd/_daemon.pyx"
   __Pyx_GOTREF(__pyx_t_1);
 
-#line 18 "systemd/_daemon.pyx"
-  __pyx_v_result = __pyx_t_1;
+#line 19 "systemd/_daemon.pyx"
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-#line 18 "systemd/_daemon.pyx"
-  __pyx_t_1 = 0;
+#line 19 "systemd/_daemon.pyx"
+  __pyx_t_6 = __Pyx_PyObject_AsString(__pyx_t_1); if (unlikely((!__pyx_t_6) && PyErr_Occurred())) __PYX_ERR(0, 19, __pyx_L1_error)
+
+#line 19 "systemd/_daemon.pyx"
+  __pyx_t_2 = __Pyx_PyInt_From_int(sd_notify(__pyx_v_unset_env, __pyx_t_6)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 19, __pyx_L1_error)
+
+#line 19 "systemd/_daemon.pyx"
+  __Pyx_GOTREF(__pyx_t_2);
+
+#line 19 "systemd/_daemon.pyx"
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+
+#line 19 "systemd/_daemon.pyx"
+  __pyx_v_result = __pyx_t_2;
 
-  /* "systemd/_daemon.pyx":20
- *     result = sd_daemon.sd_notify(unset_env, line)
+#line 19 "systemd/_daemon.pyx"
+  __pyx_t_2 = 0;
+
+  /* "systemd/_daemon.pyx":21
+ *     result = sd_daemon.sd_notify(unset_env, line.encode())
  * 
  *     if result > 0:             # <<<<<<<<<<<<<<
  *         return result
  *     elif result == 0:
  */
 
-#line 20 "systemd/_daemon.pyx"
-  __pyx_t_1 = PyObject_RichCompare(__pyx_v_result, __pyx_int_0, Py_GT); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 20, __pyx_L1_error)
+#line 21 "systemd/_daemon.pyx"
+  __pyx_t_2 = PyObject_RichCompare(__pyx_v_result, __pyx_int_0, Py_GT); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 21, __pyx_L1_error)
 
-#line 20 "systemd/_daemon.pyx"
-  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 20, __pyx_L1_error)
+#line 21 "systemd/_daemon.pyx"
+  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 21, __pyx_L1_error)
 
-#line 20 "systemd/_daemon.pyx"
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+#line 21 "systemd/_daemon.pyx"
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-#line 20 "systemd/_daemon.pyx"
+#line 21 "systemd/_daemon.pyx"
   if (__pyx_t_5) {
 
-    /* "systemd/_daemon.pyx":21
+    /* "systemd/_daemon.pyx":22
  * 
  *     if result > 0:
  *         return result             # <<<<<<<<<<<<<<
  *     elif result == 0:
  *         raise RuntimeError("Data could not be sent")
  */
 
-#line 21 "systemd/_daemon.pyx"
+#line 22 "systemd/_daemon.pyx"
     __Pyx_XDECREF(__pyx_r);
 
-#line 21 "systemd/_daemon.pyx"
+#line 22 "systemd/_daemon.pyx"
     __Pyx_INCREF(__pyx_v_result);
 
-#line 21 "systemd/_daemon.pyx"
+#line 22 "systemd/_daemon.pyx"
     __pyx_r = __pyx_v_result;
 
-#line 21 "systemd/_daemon.pyx"
+#line 22 "systemd/_daemon.pyx"
     goto __pyx_L0;
 
-    /* "systemd/_daemon.pyx":20
- *     result = sd_daemon.sd_notify(unset_env, line)
+    /* "systemd/_daemon.pyx":21
+ *     result = sd_daemon.sd_notify(unset_env, line.encode())
  * 
  *     if result > 0:             # <<<<<<<<<<<<<<
  *         return result
  *     elif result == 0:
  */
 
-#line 20 "systemd/_daemon.pyx"
+#line 21 "systemd/_daemon.pyx"
   }
 
-  /* "systemd/_daemon.pyx":22
+  /* "systemd/_daemon.pyx":23
  *     if result > 0:
  *         return result
  *     elif result == 0:             # <<<<<<<<<<<<<<
  *         raise RuntimeError("Data could not be sent")
  *     else:
  */
 
-#line 22 "systemd/_daemon.pyx"
-  __pyx_t_1 = __Pyx_PyInt_EqObjC(__pyx_v_result, __pyx_int_0, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 22, __pyx_L1_error)
+#line 23 "systemd/_daemon.pyx"
+  __pyx_t_2 = __Pyx_PyInt_EqObjC(__pyx_v_result, __pyx_int_0, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 23, __pyx_L1_error)
 
-#line 22 "systemd/_daemon.pyx"
-  __Pyx_GOTREF(__pyx_t_1);
+#line 23 "systemd/_daemon.pyx"
+  __Pyx_GOTREF(__pyx_t_2);
 
-#line 22 "systemd/_daemon.pyx"
-  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 22, __pyx_L1_error)
+#line 23 "systemd/_daemon.pyx"
+  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 23, __pyx_L1_error)
 
-#line 22 "systemd/_daemon.pyx"
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+#line 23 "systemd/_daemon.pyx"
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-#line 22 "systemd/_daemon.pyx"
+#line 23 "systemd/_daemon.pyx"
   if (__pyx_t_5) {
 
-    /* "systemd/_daemon.pyx":23
+    /* "systemd/_daemon.pyx":24
  *         return result
  *     elif result == 0:
  *         raise RuntimeError("Data could not be sent")             # <<<<<<<<<<<<<<
  *     else:
  *         raise ValueError("Notification error #%d" % result, result)
  */
 
-#line 23 "systemd/_daemon.pyx"
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_RuntimeError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 23, __pyx_L1_error)
+#line 24 "systemd/_daemon.pyx"
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_RuntimeError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 24, __pyx_L1_error)
 
-#line 23 "systemd/_daemon.pyx"
-    __Pyx_GOTREF(__pyx_t_1);
+#line 24 "systemd/_daemon.pyx"
+    __Pyx_GOTREF(__pyx_t_2);
 
-#line 23 "systemd/_daemon.pyx"
-    __Pyx_Raise(__pyx_t_1, 0, 0, 0);
+#line 24 "systemd/_daemon.pyx"
+    __Pyx_Raise(__pyx_t_2, 0, 0, 0);
 
-#line 23 "systemd/_daemon.pyx"
-    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+#line 24 "systemd/_daemon.pyx"
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-#line 23 "systemd/_daemon.pyx"
-    __PYX_ERR(0, 23, __pyx_L1_error)
+#line 24 "systemd/_daemon.pyx"
+    __PYX_ERR(0, 24, __pyx_L1_error)
 
-    /* "systemd/_daemon.pyx":22
+    /* "systemd/_daemon.pyx":23
  *     if result > 0:
  *         return result
  *     elif result == 0:             # <<<<<<<<<<<<<<
  *         raise RuntimeError("Data could not be sent")
  *     else:
  */
 
-#line 22 "systemd/_daemon.pyx"
+#line 23 "systemd/_daemon.pyx"
   }
 
-  /* "systemd/_daemon.pyx":25
+  /* "systemd/_daemon.pyx":26
  *         raise RuntimeError("Data could not be sent")
  *     else:
  *         raise ValueError("Notification error #%d" % result, result)             # <<<<<<<<<<<<<<
  */
 
-#line 25 "systemd/_daemon.pyx"
+#line 26 "systemd/_daemon.pyx"
   /*else*/ {
 
-#line 25 "systemd/_daemon.pyx"
-    __pyx_t_1 = __Pyx_PyString_Format(__pyx_kp_s_Notification_error_d, __pyx_v_result); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 25, __pyx_L1_error)
+#line 26 "systemd/_daemon.pyx"
+    __pyx_t_2 = __Pyx_PyString_Format(__pyx_kp_s_Notification_error_d, __pyx_v_result); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 26, __pyx_L1_error)
 
-#line 25 "systemd/_daemon.pyx"
-    __Pyx_GOTREF(__pyx_t_1);
+#line 26 "systemd/_daemon.pyx"
+    __Pyx_GOTREF(__pyx_t_2);
 
-#line 25 "systemd/_daemon.pyx"
-    __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 25, __pyx_L1_error)
+#line 26 "systemd/_daemon.pyx"
+    __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 26, __pyx_L1_error)
 
-#line 25 "systemd/_daemon.pyx"
-    __Pyx_GOTREF(__pyx_t_2);
+#line 26 "systemd/_daemon.pyx"
+    __Pyx_GOTREF(__pyx_t_1);
 
-#line 25 "systemd/_daemon.pyx"
-    __Pyx_GIVEREF(__pyx_t_1);
+#line 26 "systemd/_daemon.pyx"
+    __Pyx_GIVEREF(__pyx_t_2);
 
-#line 25 "systemd/_daemon.pyx"
-    PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_1);
+#line 26 "systemd/_daemon.pyx"
+    PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_2);
 
-#line 25 "systemd/_daemon.pyx"
+#line 26 "systemd/_daemon.pyx"
     __Pyx_INCREF(__pyx_v_result);
 
-#line 25 "systemd/_daemon.pyx"
+#line 26 "systemd/_daemon.pyx"
     __Pyx_GIVEREF(__pyx_v_result);
 
-#line 25 "systemd/_daemon.pyx"
-    PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_v_result);
+#line 26 "systemd/_daemon.pyx"
+    PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_v_result);
 
-#line 25 "systemd/_daemon.pyx"
-    __pyx_t_1 = 0;
+#line 26 "systemd/_daemon.pyx"
+    __pyx_t_2 = 0;
 
-#line 25 "systemd/_daemon.pyx"
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_t_2, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 25, __pyx_L1_error)
+#line 26 "systemd/_daemon.pyx"
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_t_1, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 26, __pyx_L1_error)
 
-#line 25 "systemd/_daemon.pyx"
-    __Pyx_GOTREF(__pyx_t_1);
+#line 26 "systemd/_daemon.pyx"
+    __Pyx_GOTREF(__pyx_t_2);
 
-#line 25 "systemd/_daemon.pyx"
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+#line 26 "systemd/_daemon.pyx"
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-#line 25 "systemd/_daemon.pyx"
-    __Pyx_Raise(__pyx_t_1, 0, 0, 0);
+#line 26 "systemd/_daemon.pyx"
+    __Pyx_Raise(__pyx_t_2, 0, 0, 0);
 
-#line 25 "systemd/_daemon.pyx"
-    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+#line 26 "systemd/_daemon.pyx"
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-#line 25 "systemd/_daemon.pyx"
-    __PYX_ERR(0, 25, __pyx_L1_error)
+#line 26 "systemd/_daemon.pyx"
+    __PYX_ERR(0, 26, __pyx_L1_error)
 
-#line 25 "systemd/_daemon.pyx"
+#line 26 "systemd/_daemon.pyx"
   }
 
   /* "systemd/_daemon.pyx":4
  * 
  * 
- * def sd_notify(line: str, unset_environment: bool=False) -> int:             # <<<<<<<<<<<<<<
+ * def sd_notify(line, unset_environment=False):             # <<<<<<<<<<<<<<
  *     """ Send notification to systemd daemon
  * 
  */
 
 #line 4 "systemd/_daemon.pyx"
 
 
@@ -1400,46 +1463,46 @@
   {&__pyx_n_s_systemd__daemon, __pyx_k_systemd__daemon, sizeof(__pyx_k_systemd__daemon), 0, 0, 1, 1},
   {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
   {&__pyx_n_s_unset_env, __pyx_k_unset_env, sizeof(__pyx_k_unset_env), 0, 0, 1, 1},
   {&__pyx_n_s_unset_environment, __pyx_k_unset_environment, sizeof(__pyx_k_unset_environment), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static int __Pyx_InitCachedBuiltins(void) {
-  __pyx_builtin_RuntimeError = __Pyx_GetBuiltinName(__pyx_n_s_RuntimeError); if (!__pyx_builtin_RuntimeError) __PYX_ERR(0, 23, __pyx_L1_error)
-  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 25, __pyx_L1_error)
+  __pyx_builtin_RuntimeError = __Pyx_GetBuiltinName(__pyx_n_s_RuntimeError); if (!__pyx_builtin_RuntimeError) __PYX_ERR(0, 24, __pyx_L1_error)
+  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 26, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "systemd/_daemon.pyx":23
+  /* "systemd/_daemon.pyx":24
  *         return result
  *     elif result == 0:
  *         raise RuntimeError("Data could not be sent")             # <<<<<<<<<<<<<<
  *     else:
  *         raise ValueError("Notification error #%d" % result, result)
  */
 
-#line 23 "systemd/_daemon.pyx"
-  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_s_Data_could_not_be_sent); if (unlikely(!__pyx_tuple_)) __PYX_ERR(0, 23, __pyx_L1_error)
+#line 24 "systemd/_daemon.pyx"
+  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_s_Data_could_not_be_sent); if (unlikely(!__pyx_tuple_)) __PYX_ERR(0, 24, __pyx_L1_error)
 
-#line 23 "systemd/_daemon.pyx"
+#line 24 "systemd/_daemon.pyx"
   __Pyx_GOTREF(__pyx_tuple_);
 
-#line 23 "systemd/_daemon.pyx"
+#line 24 "systemd/_daemon.pyx"
   __Pyx_GIVEREF(__pyx_tuple_);
 
   /* "systemd/_daemon.pyx":4
  * 
  * 
- * def sd_notify(line: str, unset_environment: bool=False) -> int:             # <<<<<<<<<<<<<<
+ * def sd_notify(line, unset_environment=False):             # <<<<<<<<<<<<<<
  *     """ Send notification to systemd daemon
  * 
  */
 
 #line 4 "systemd/_daemon.pyx"
   __pyx_tuple__2 = PyTuple_Pack(4, __pyx_n_s_line, __pyx_n_s_unset_environment, __pyx_n_s_unset_env, __pyx_n_s_result); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 4, __pyx_L1_error)
 
@@ -1569,15 +1632,15 @@
   #if defined(__Pyx_Generator_USED) || defined(__Pyx_Coroutine_USED)
   if (__Pyx_patch_abc() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
 
   /* "systemd/_daemon.pyx":4
  * 
  * 
- * def sd_notify(line: str, unset_environment: bool=False) -> int:             # <<<<<<<<<<<<<<
+ * def sd_notify(line, unset_environment=False):             # <<<<<<<<<<<<<<
  *     """ Send notification to systemd daemon
  * 
  */
 
 #line 4 "systemd/_daemon.pyx"
   __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_7systemd_7_daemon_1sd_notify, NULL, __pyx_n_s_systemd__daemon); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 4, __pyx_L1_error)
```

### Comparing `systemd-0.9.8/systemd/_journal.c` & `systemd-0.9.9/systemd/_journal.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 /* Generated by Cython 0.24.1 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
-        "depends": [], 
+        "depends": [],
         "extra_compile_args": [
             "-DSYSLOG_NAMES=1"
-        ], 
+        ],
         "libraries": [
             "systemd"
         ]
-    }, 
+    },
     "module_name": "systemd._journal"
 }
 END: Cython Metadata */
 
 #define PY_SSIZE_T_CLEAN
 #include "Python.h"
 #ifndef Py_PYTHON_H
```

### Comparing `systemd-0.9.8/systemd/_journal.pyx` & `systemd-0.9.9/systemd/_journal.pyx`

 * *Files identical despite different names*

### Comparing `systemd-0.9.8/systemd/daemon.py` & `systemd-0.9.9/systemd/daemon.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,19 +21,20 @@
     MAINPID = NotificationValue(name='MAINPID', constant=None, type=int)
     WATCHDOG = NotificationValue(name='WATCHDOG', constant=1, type=int)
     FDSTORE = NotificationValue(name='FDSTORE', constant=1, type=int)
     FDNAME = NotificationValue(name='FDNAME', constant=None, type=int)
     WATCHDOG_USEC = NotificationValue(name='WATCHDOG_USEC', constant=None, type=int)
 
 
-def notify(notification: Notification, value: int=None, unset_environment: bool=False):
+def notify(notification, value=None, unset_environment=False):
     """ Send notification to systemd daemon
 
     :type notification: Notification
-    :param notification: Notification instance
+    :type value: int
+    :type unset_environment: bool 
     :param value: str or int value for non constant notifications
     :returns None
     """
 
     if not isinstance(notification, Notification):
         raise TypeError("state must be an instance of Notigication")
```

### Comparing `systemd-0.9.8/systemd/journal.py` & `systemd-0.9.9/systemd/journal.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,16 +48,19 @@
     LOCAL3 = 19
     LOCAL4 = 20
     LOCAL5 = 21
     LOCAL6 = 22
     LOCAL7 = 23
 
 
-def write(message: str, priority: Priority=Priority.INFO):
-    """ Write message into systemd journal """
+def write(message, priority=Priority.INFO):
+    """ Write message into systemd journal 
+    :type priority: Priority
+    :type message: str
+    """
 
     priority = int(Priority(int(priority)))
 
     send(priority=priority, message=message)
 
 
 class JournaldLogHandler(logging.Handler):
@@ -70,20 +73,28 @@
         logging.INFO: Priority.INFO.value,
         logging.DEBUG: Priority.DEBUG.value,
         logging.NOTSET: Priority.NONE.value,
     }
 
     __slots__ = '__facility',
 
-    def __init__(self, facility: Facility=Facility.DAEMON):
+    def __init__(self, facility=Facility.DAEMON):
+        """
+
+        :type facility: Facility
+        """
         logging.Handler.__init__(self)
         self.__facility = Facility(int(facility))
 
     @staticmethod
-    def _to_microsecond(ts: float):
+    def _to_microsecond(ts):
+        """
+
+        :type ts: float
+        """
         return int(ts * 1000 * 1000)
 
     def emit(self, record):
         message = str(record.getMessage())
 
         tb_message = ''
         if record.exc_info:
```

### Comparing `systemd-0.9.8/systemd.egg-info/PKG-INFO` & `systemd-0.9.9/systemd.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: systemd
-Version: 0.9.8
+Version: 0.9.9
 Summary: Python systemd wrapper
 Home-page: http://github.com/mosquito/python-systemd
 Author: Dmitry Orlov <me@mosquito.su>
 Author-email: me@mosquito.su
 License: Apache
 Description: SystemD
         =======
@@ -110,15 +110,16 @@
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Natural Language :: Russian
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Cython
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 2.7
+Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: System
 Classifier: Topic :: System :: Operating System
```

