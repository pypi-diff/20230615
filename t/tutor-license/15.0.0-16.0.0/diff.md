# Comparing `tmp/tutor-license-15.0.0.tar.gz` & `tmp/tutor-license-16.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tutor-license-15.0.0.tar", last modified: Mon Dec 12 20:21:06 2022, max compression
+gzip compressed data, was "tutor-license-16.0.0.tar", last modified: Thu Jun 15 01:20:28 2023, max compression
```

## Comparing `tutor-license-15.0.0.tar` & `tutor-license-16.0.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2022-12-12 20:21:06.000000 tutor-license-15.0.0/
--rw-rw-r--   0 regis     (1000) regis     (1000)     3898 2022-12-12 20:21:06.000000 tutor-license-15.0.0/PKG-INFO
--rw-rw-r--   0 regis     (1000) regis     (1000)     3157 2021-02-04 15:55:53.000000 tutor-license-15.0.0/README.rst
--rw-rw-r--   0 regis     (1000) regis     (1000)       38 2022-12-12 20:21:06.000000 tutor-license-15.0.0/setup.cfg
--rw-rw-r--   0 regis     (1000) regis     (1000)     1887 2022-12-12 20:11:34.000000 tutor-license-15.0.0/setup.py
-drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2022-12-12 20:21:06.000000 tutor-license-15.0.0/tutor_license.egg-info/
--rw-rw-r--   0 regis     (1000) regis     (1000)     3898 2022-12-12 20:21:06.000000 tutor-license-15.0.0/tutor_license.egg-info/PKG-INFO
--rw-rw-r--   0 regis     (1000) regis     (1000)      336 2022-12-12 20:21:06.000000 tutor-license-15.0.0/tutor_license.egg-info/SOURCES.txt
--rw-rw-r--   0 regis     (1000) regis     (1000)        1 2022-12-12 20:21:06.000000 tutor-license-15.0.0/tutor_license.egg-info/dependency_links.txt
--rw-rw-r--   0 regis     (1000) regis     (1000)       48 2022-12-12 20:21:06.000000 tutor-license-15.0.0/tutor_license.egg-info/entry_points.txt
--rw-rw-r--   0 regis     (1000) regis     (1000)       43 2022-12-12 20:21:06.000000 tutor-license-15.0.0/tutor_license.egg-info/requires.txt
--rw-rw-r--   0 regis     (1000) regis     (1000)       13 2022-12-12 20:21:06.000000 tutor-license-15.0.0/tutor_license.egg-info/top_level.txt
-drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2022-12-12 20:21:06.000000 tutor-license-15.0.0/tutorlicense/
--rw-rw-r--   0 regis     (1000) regis     (1000)       23 2022-12-12 18:04:53.000000 tutor-license-15.0.0/tutorlicense/__about__.py
--rw-rw-r--   0 regis     (1000) regis     (1000)        0 2021-02-04 15:55:53.000000 tutor-license-15.0.0/tutorlicense/__init__.py
--rw-rw-r--   0 regis     (1000) regis     (1000)   572280 2022-12-12 20:16:55.000000 tutor-license-15.0.0/tutorlicense/cmd.c
--rw-rw-r--   0 regis     (1000) regis     (1000)      198 2022-06-09 19:45:25.000000 tutor-license-15.0.0/tutorlicense/plugin.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-15 01:20:28.945613 tutor-license-16.0.0/
+-rw-r--r--   0 ci        (1000) ci        (1000)     3899 2023-06-15 01:20:28.945613 tutor-license-16.0.0/PKG-INFO
+-rw-r--r--   0 ci        (1000) ci        (1000)     3158 2023-06-15 01:19:14.000000 tutor-license-16.0.0/README.rst
+-rw-r--r--   0 ci        (1000) ci        (1000)       60 2023-06-15 01:19:14.000000 tutor-license-16.0.0/pyproject.toml
+-rw-r--r--   0 ci        (1000) ci        (1000)       38 2023-06-15 01:20:28.945613 tutor-license-16.0.0/setup.cfg
+-rw-r--r--   0 ci        (1000) ci        (1000)     1888 2023-06-15 01:19:14.000000 tutor-license-16.0.0/setup.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-15 01:20:28.938946 tutor-license-16.0.0/tutor_license.egg-info/
+-rw-r--r--   0 ci        (1000) ci        (1000)     3899 2023-06-15 01:20:28.000000 tutor-license-16.0.0/tutor_license.egg-info/PKG-INFO
+-rw-r--r--   0 ci        (1000) ci        (1000)      351 2023-06-15 01:20:28.000000 tutor-license-16.0.0/tutor_license.egg-info/SOURCES.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)        1 2023-06-15 01:20:28.000000 tutor-license-16.0.0/tutor_license.egg-info/dependency_links.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)       48 2023-06-15 01:20:28.000000 tutor-license-16.0.0/tutor_license.egg-info/entry_points.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)       43 2023-06-15 01:20:28.000000 tutor-license-16.0.0/tutor_license.egg-info/requires.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)       13 2023-06-15 01:20:28.000000 tutor-license-16.0.0/tutor_license.egg-info/top_level.txt
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-15 01:20:28.942279 tutor-license-16.0.0/tutorlicense/
+-rw-r--r--   0 ci        (1000) ci        (1000)      175 2023-06-15 01:19:14.000000 tutor-license-16.0.0/tutorlicense/__about__.py
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-06-15 01:19:14.000000 tutor-license-16.0.0/tutorlicense/__init__.py
+-rw-r--r--   0 ci        (1000) ci        (1000)   581839 2023-06-15 01:19:39.000000 tutor-license-16.0.0/tutorlicense/cmd.c
+-rw-r--r--   0 ci        (1000) ci        (1000)      198 2023-06-15 01:19:14.000000 tutor-license-16.0.0/tutorlicense/plugin.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `tutor-license-15.0.0/PKG-INFO` & `tutor-license-16.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: tutor-license
-Version: 15.0.0
+Version: 16.0.0
 Summary: Tutor license management plugin
 Home-page: https://overhang.io/tutor/
 Author: Overhang.IO
 Author-email: regis@overhang.io
 Project-URL: Homepage, https://overhang.io/tutor/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 
 `Tutor <https://docs.tutor.overhang.io>`__ license management plugin
 ====================================================================
 
 This is a plugin for `Tutor Wizard Edition <https://overhang.io/tutor/>`__ customers. Running this plugin requires a valid license key. A Wizard Edition subscription provides access to exclusive Tutor plugins.
 
@@ -27,15 +27,15 @@
 Installation
 ------------
 
 This plugin requires a working installation of Tutor. To install Tutor, please check the `official installation instructions <https://docs.tutor.overhang.io/install.html>`__.
 
 Then, install and enable the plugin with::
 
-    pip install tutor-license
+    tutor plugins install license
     tutor plugins enable license
 
 Quickstart
 ----------
 
 Obtain a Tutor Wizard Edition license at https://overhang.io/tutor/subscribe. Then, find your license ID and run::
 
@@ -56,15 +56,15 @@
     tutor plugins list
 
 Note that to start using Wizard Edition plugins, you will have to install Tutor from source, and not by downloading the Tutor binary. You will also need to install ``pip`` for Python 3+. To do so, follow the `official instructions <https://pip.pypa.io/en/stable/installing/>`__.
 
 Once a plugin has been installed, you need to enable it to start using it. For instance::
 
     tutor plugins enable monitor
-    tutor local quickstart
+    tutor local launch
 
 How-to guides
 -------------
 
 Storing the Tutor licenses in a different location
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
```

### Comparing `tutor-license-15.0.0/README.rst` & `tutor-license-16.0.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 Installation
 ------------
 
 This plugin requires a working installation of Tutor. To install Tutor, please check the `official installation instructions <https://docs.tutor.overhang.io/install.html>`__.
 
 Then, install and enable the plugin with::
 
-    pip install tutor-license
+    tutor plugins install license
     tutor plugins enable license
 
 Quickstart
 ----------
 
 Obtain a Tutor Wizard Edition license at https://overhang.io/tutor/subscribe. Then, find your license ID and run::
 
@@ -36,15 +36,15 @@
     tutor plugins list
 
 Note that to start using Wizard Edition plugins, you will have to install Tutor from source, and not by downloading the Tutor binary. You will also need to install ``pip`` for Python 3+. To do so, follow the `official instructions <https://pip.pypa.io/en/stable/installing/>`__.
 
 Once a plugin has been installed, you need to enable it to start using it. For instance::
 
     tutor plugins enable monitor
-    tutor local quickstart
+    tutor local launch
 
 How-to guides
 -------------
 
 Storing the Tutor licenses in a different location
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
@@ -76,8 +76,8 @@
 
     tutor license users deactivate --yes \
         --id=$(tutor license users list --name=myinstance --format="{id}")
 
 License
 -------
 
-All rights reserved to SASU NULI NULI.
+All rights reserved to SASU NULI NULI.
```

### Comparing `tutor-license-15.0.0/setup.py` & `tutor-license-16.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,23 +35,23 @@
     },
     author="Overhang.IO",
     author_email="regis@overhang.io",
     description="Tutor license management plugin",
     long_description=readme,
     long_description_content_type="text/x-rst",
     packages=find_packages(exclude=["tests*"]),
-    python_requires=">=3.7",
-    install_requires=["tutor>=15.0.0,<16.0.0", "pycryptodome", "appdirs"],
+    python_requires=">=3.8",
+    install_requires=["tutor>=16.0.0,<17.0.0", "pycryptodome", "appdirs"],
     entry_points={"tutor.plugin.v1": ["license = tutorlicense.plugin"]},
     ext_modules=ext_modules(),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "License :: Other/Proprietary License",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
 )
```

### Comparing `tutor-license-15.0.0/tutor_license.egg-info/PKG-INFO` & `tutor-license-16.0.0/tutor_license.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: tutor-license
-Version: 15.0.0
+Version: 16.0.0
 Summary: Tutor license management plugin
 Home-page: https://overhang.io/tutor/
 Author: Overhang.IO
 Author-email: regis@overhang.io
 Project-URL: Homepage, https://overhang.io/tutor/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 
 `Tutor <https://docs.tutor.overhang.io>`__ license management plugin
 ====================================================================
 
 This is a plugin for `Tutor Wizard Edition <https://overhang.io/tutor/>`__ customers. Running this plugin requires a valid license key. A Wizard Edition subscription provides access to exclusive Tutor plugins.
 
@@ -27,15 +27,15 @@
 Installation
 ------------
 
 This plugin requires a working installation of Tutor. To install Tutor, please check the `official installation instructions <https://docs.tutor.overhang.io/install.html>`__.
 
 Then, install and enable the plugin with::
 
-    pip install tutor-license
+    tutor plugins install license
     tutor plugins enable license
 
 Quickstart
 ----------
 
 Obtain a Tutor Wizard Edition license at https://overhang.io/tutor/subscribe. Then, find your license ID and run::
 
@@ -56,15 +56,15 @@
     tutor plugins list
 
 Note that to start using Wizard Edition plugins, you will have to install Tutor from source, and not by downloading the Tutor binary. You will also need to install ``pip`` for Python 3+. To do so, follow the `official instructions <https://pip.pypa.io/en/stable/installing/>`__.
 
 Once a plugin has been installed, you need to enable it to start using it. For instance::
 
     tutor plugins enable monitor
-    tutor local quickstart
+    tutor local launch
 
 How-to guides
 -------------
 
 Storing the Tutor licenses in a different location
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
```

### Comparing `tutor-license-15.0.0/tutorlicense/cmd.c` & `tutor-license-16.0.0/tutorlicense/cmd.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,32 @@
-/* Generated by Cython 0.29.21 */
+/* Generated by Cython 0.29.35 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "name": "tutorlicense.cmd",
         "sources": [
             "tutorlicense/cmd.pyx"
         ]
     },
     "module_name": "tutorlicense.cmd"
 }
 END: Cython Metadata */
 
+#ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
+#endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_21"
-#define CYTHON_HEX_VERSION 0x001D15F0
+#define CYTHON_ABI "0_29_35"
+#define CYTHON_HEX_VERSION 0x001D23F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -55,14 +57,15 @@
 #ifndef Py_HUGE_VAL
   #define Py_HUGE_VAL HUGE_VAL
 #endif
 #ifdef PYPY_VERSION
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_PYSTON 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
   #define CYTHON_USE_TYPE_SLOTS 0
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #if PY_VERSION_HEX < 0x03050000
     #undef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 0
@@ -83,26 +86,34 @@
   #define CYTHON_ASSUME_SAFE_MACROS 0
   #undef CYTHON_UNPACK_METHODS
   #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
-  #undef CYTHON_PEP489_MULTI_PHASE_INIT
-  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #if PY_VERSION_HEX < 0x03090000
+    #undef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
+  #endif
 #elif defined(PYSTON_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_PYSTON 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #undef CYTHON_USE_ASYNC_SLOTS
   #define CYTHON_USE_ASYNC_SLOTS 0
@@ -132,18 +143,67 @@
   #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
+  #endif
+#elif defined(PY_NOGIL)
+  #define CYTHON_COMPILING_IN_PYPY 0
+  #define CYTHON_COMPILING_IN_PYSTON 0
+  #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_NOGIL 1
+  #ifndef CYTHON_USE_TYPE_SLOTS
+    #define CYTHON_USE_TYPE_SLOTS 1
+  #endif
+  #undef CYTHON_USE_PYTYPE_LOOKUP
+  #define CYTHON_USE_PYTYPE_LOOKUP 0
+  #ifndef CYTHON_USE_ASYNC_SLOTS
+    #define CYTHON_USE_ASYNC_SLOTS 1
+  #endif
+  #undef CYTHON_USE_PYLIST_INTERNALS
+  #define CYTHON_USE_PYLIST_INTERNALS 0
+  #ifndef CYTHON_USE_UNICODE_INTERNALS
+    #define CYTHON_USE_UNICODE_INTERNALS 1
+  #endif
+  #undef CYTHON_USE_UNICODE_WRITER
+  #define CYTHON_USE_UNICODE_WRITER 0
+  #undef CYTHON_USE_PYLONG_INTERNALS
+  #define CYTHON_USE_PYLONG_INTERNALS 0
+  #ifndef CYTHON_AVOID_BORROWED_REFS
+    #define CYTHON_AVOID_BORROWED_REFS 0
+  #endif
+  #ifndef CYTHON_ASSUME_SAFE_MACROS
+    #define CYTHON_ASSUME_SAFE_MACROS 1
+  #endif
+  #ifndef CYTHON_UNPACK_METHODS
+    #define CYTHON_UNPACK_METHODS 1
+  #endif
+  #undef CYTHON_FAST_THREAD_STATE
+  #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_PYCALL
+  #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
+  #ifndef CYTHON_USE_TP_FINALIZE
+    #define CYTHON_USE_TP_FINALIZE 1
+  #endif
+  #undef CYTHON_USE_DICT_VERSIONS
+  #define CYTHON_USE_DICT_VERSIONS 0
+  #undef CYTHON_USE_EXC_INFO_STACK
+  #define CYTHON_USE_EXC_INFO_STACK 0
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_PYSTON 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
+  #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYTYPE_LOOKUP
     #define CYTHON_USE_PYTYPE_LOOKUP 0
   #elif !defined(CYTHON_USE_PYTYPE_LOOKUP)
@@ -155,61 +215,72 @@
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 0
   #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS 1
+    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
-  #if PY_VERSION_HEX < 0x030300F0
+  #if PY_VERSION_HEX < 0x030300F0 || PY_VERSION_HEX >= 0x030B00A2
     #undef CYTHON_USE_UNICODE_WRITER
     #define CYTHON_USE_UNICODE_WRITER 0
   #elif !defined(CYTHON_USE_UNICODE_WRITER)
     #define CYTHON_USE_UNICODE_WRITER 1
   #endif
   #ifndef CYTHON_AVOID_BORROWED_REFS
     #define CYTHON_AVOID_BORROWED_REFS 0
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
-  #ifndef CYTHON_FAST_THREAD_STATE
+  #if PY_VERSION_HEX >= 0x030B00A4
+    #undef CYTHON_FAST_THREAD_STATE
+    #define CYTHON_FAST_THREAD_STATE 0
+  #elif !defined(CYTHON_FAST_THREAD_STATE)
     #define CYTHON_FAST_THREAD_STATE 1
   #endif
   #ifndef CYTHON_FAST_PYCALL
-    #define CYTHON_FAST_PYCALL 1
+    #define CYTHON_FAST_PYCALL (PY_VERSION_HEX < 0x030A0000)
   #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
   #endif
-  #ifndef CYTHON_USE_EXC_INFO_STACK
+  #if PY_VERSION_HEX >= 0x030B00A4
+    #undef CYTHON_USE_EXC_INFO_STACK
+    #define CYTHON_USE_EXC_INFO_STACK 0
+  #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
+  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if CYTHON_USE_PYLONG_INTERNALS
-  #include "longintrepr.h"
+  #if PY_MAJOR_VERSION < 3
+    #include "longintrepr.h"
+  #endif
   #undef SHIFT
   #undef BASE
   #undef MASK
   #ifdef SIZEOF_VOID_P
     enum { __pyx_check_sizeof_voidp = 1 / (int)(SIZEOF_VOID_P == sizeof(void*)) };
   #endif
 #endif
@@ -318,17 +389,76 @@
 #if PY_MAJOR_VERSION < 3
   #define __Pyx_BUILTIN_MODULE_NAME "__builtin__"
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
   #define __Pyx_DefaultClassType PyClass_Type
 #else
   #define __Pyx_BUILTIN_MODULE_NAME "builtins"
-#if PY_VERSION_HEX >= 0x030800A4 && PY_VERSION_HEX < 0x030800B2
-  #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
-          PyCode_New(a, 0, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
+  #define __Pyx_DefaultClassType PyType_Type
+#if PY_VERSION_HEX >= 0x030B00A1
+    static CYTHON_INLINE PyCodeObject* __Pyx_PyCode_New(int a, int k, int l, int s, int f,
+                                                    PyObject *code, PyObject *c, PyObject* n, PyObject *v,
+                                                    PyObject *fv, PyObject *cell, PyObject* fn,
+                                                    PyObject *name, int fline, PyObject *lnos) {
+        PyObject *kwds=NULL, *argcount=NULL, *posonlyargcount=NULL, *kwonlyargcount=NULL;
+        PyObject *nlocals=NULL, *stacksize=NULL, *flags=NULL, *replace=NULL, *call_result=NULL, *empty=NULL;
+        const char *fn_cstr=NULL;
+        const char *name_cstr=NULL;
+        PyCodeObject* co=NULL;
+        PyObject *type, *value, *traceback;
+        PyErr_Fetch(&type, &value, &traceback);
+        if (!(kwds=PyDict_New())) goto end;
+        if (!(argcount=PyLong_FromLong(a))) goto end;
+        if (PyDict_SetItemString(kwds, "co_argcount", argcount) != 0) goto end;
+        if (!(posonlyargcount=PyLong_FromLong(0))) goto end;
+        if (PyDict_SetItemString(kwds, "co_posonlyargcount", posonlyargcount) != 0) goto end;
+        if (!(kwonlyargcount=PyLong_FromLong(k))) goto end;
+        if (PyDict_SetItemString(kwds, "co_kwonlyargcount", kwonlyargcount) != 0) goto end;
+        if (!(nlocals=PyLong_FromLong(l))) goto end;
+        if (PyDict_SetItemString(kwds, "co_nlocals", nlocals) != 0) goto end;
+        if (!(stacksize=PyLong_FromLong(s))) goto end;
+        if (PyDict_SetItemString(kwds, "co_stacksize", stacksize) != 0) goto end;
+        if (!(flags=PyLong_FromLong(f))) goto end;
+        if (PyDict_SetItemString(kwds, "co_flags", flags) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_code", code) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_consts", c) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_names", n) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_varnames", v) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_freevars", fv) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_cellvars", cell) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_linetable", lnos) != 0) goto end;
+        if (!(fn_cstr=PyUnicode_AsUTF8AndSize(fn, NULL))) goto end;
+        if (!(name_cstr=PyUnicode_AsUTF8AndSize(name, NULL))) goto end;
+        if (!(co = PyCode_NewEmpty(fn_cstr, name_cstr, fline))) goto end;
+        if (!(replace = PyObject_GetAttrString((PyObject*)co, "replace"))) goto cleanup_code_too;
+        if (!(empty = PyTuple_New(0))) goto cleanup_code_too; // unfortunately __pyx_empty_tuple isn't available here
+        if (!(call_result = PyObject_Call(replace, empty, kwds))) goto cleanup_code_too;
+        Py_XDECREF((PyObject*)co);
+        co = (PyCodeObject*)call_result;
+        call_result = NULL;
+        if (0) {
+            cleanup_code_too:
+            Py_XDECREF((PyObject*)co);
+            co = NULL;
+        }
+        end:
+        Py_XDECREF(kwds);
+        Py_XDECREF(argcount);
+        Py_XDECREF(posonlyargcount);
+        Py_XDECREF(kwonlyargcount);
+        Py_XDECREF(nlocals);
+        Py_XDECREF(stacksize);
+        Py_XDECREF(replace);
+        Py_XDECREF(call_result);
+        Py_XDECREF(empty);
+        if (type) {
+            PyErr_Restore(type, value, traceback);
+        }
+        return co;
+    }
 #else
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #endif
   #define __Pyx_DefaultClassType PyType_Type
 #endif
 #ifndef Py_TPFLAGS_CHECKTYPES
@@ -434,27 +564,35 @@
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1 && CYTHON_USE_UNICODE_INTERNALS
 #define __Pyx_PyDict_GetItemStr(dict, name)  _PyDict_GetItem_KnownHash(dict, name, ((PyASCIIObject *) name)->hash)
 #else
 #define __Pyx_PyDict_GetItemStr(dict, name)  PyDict_GetItem(dict, name)
 #endif
 #if PY_VERSION_HEX > 0x03030000 && defined(PyUnicode_KIND)
   #define CYTHON_PEP393_ENABLED 1
-  #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
-                                              0 : _PyUnicode_Ready((PyObject *)(op)))
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_READY(op)       (0)
+  #else
+    #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
+                                                0 : _PyUnicode_Ready((PyObject *)(op)))
+  #endif
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_LENGTH(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) PyUnicode_READ_CHAR(u, i)
   #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   PyUnicode_MAX_CHAR_VALUE(u)
   #define __Pyx_PyUnicode_KIND(u)         PyUnicode_KIND(u)
   #define __Pyx_PyUnicode_DATA(u)         PyUnicode_DATA(u)
   #define __Pyx_PyUnicode_READ(k, d, i)   PyUnicode_READ(k, d, i)
   #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, ch)
-  #if defined(PyUnicode_IS_READY) && defined(PyUnicode_GET_SIZE)
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
   #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
+    #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
+    #else
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
+    #endif
   #endif
 #else
   #define CYTHON_PEP393_ENABLED 0
   #define PyUnicode_1BYTE_KIND  1
   #define PyUnicode_2BYTE_KIND  2
   #define PyUnicode_4BYTE_KIND  4
   #define __Pyx_PyUnicode_READY(op)       (0)
@@ -550,18 +688,18 @@
   #ifndef PyUnicode_InternFromString
     #define PyUnicode_InternFromString(s) PyUnicode_FromString(s)
   #endif
 #endif
 #if PY_VERSION_HEX < 0x030200A4
   typedef long Py_hash_t;
   #define __Pyx_PyInt_FromHash_t PyInt_FromLong
-  #define __Pyx_PyInt_AsHash_t   PyInt_AsLong
+  #define __Pyx_PyInt_AsHash_t   __Pyx_PyIndex_AsHash_t
 #else
   #define __Pyx_PyInt_FromHash_t PyInt_FromSsize_t
-  #define __Pyx_PyInt_AsHash_t   PyInt_AsSsize_t
+  #define __Pyx_PyInt_AsHash_t   __Pyx_PyIndex_AsSsize_t
 #endif
 #if PY_MAJOR_VERSION >= 3
   #define __Pyx_PyMethod_New(func, self, klass) ((self) ? ((void)(klass), PyMethod_New(func, self)) : __Pyx_NewRef(func))
 #else
   #define __Pyx_PyMethod_New(func, self, klass) PyMethod_New(func, self, klass)
 #endif
 #if CYTHON_USE_ASYNC_SLOTS
@@ -578,16 +716,18 @@
     typedef struct {
         unaryfunc am_await;
         unaryfunc am_aiter;
         unaryfunc am_anext;
     } __Pyx_PyAsyncMethodsStruct;
 #endif
 
-#if defined(WIN32) || defined(MS_WINDOWS)
-  #define _USE_MATH_DEFINES
+#if defined(_WIN32) || defined(WIN32) || defined(MS_WINDOWS)
+  #if !defined(_USE_MATH_DEFINES)
+    #define _USE_MATH_DEFINES
+  #endif
 #endif
 #include <math.h>
 #ifdef NAN
 #define __PYX_NAN() ((float) NAN)
 #else
 static CYTHON_INLINE float __PYX_NAN() {
   float value;
@@ -709,14 +849,15 @@
 static CYTHON_INLINE int __Pyx_PyObject_IsTrue(PyObject*);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrueAndDecref(PyObject*);
 static CYTHON_INLINE PyObject* __Pyx_PyNumber_IntOrLong(PyObject* x);
 #define __Pyx_PySequence_Tuple(obj)\
     (likely(PyTuple_CheckExact(obj)) ? __Pyx_NewRef(obj) : PySequence_Tuple(obj))
 static CYTHON_INLINE Py_ssize_t __Pyx_PyIndex_AsSsize_t(PyObject*);
 static CYTHON_INLINE PyObject * __Pyx_PyInt_FromSize_t(size_t);
+static CYTHON_INLINE Py_hash_t __Pyx_PyIndex_AsHash_t(PyObject*);
 #if CYTHON_ASSUME_SAFE_MACROS
 #define __pyx_PyFloat_AsDouble(x) (PyFloat_CheckExact(x) ? PyFloat_AS_DOUBLE(x) : PyFloat_AsDouble(x))
 #else
 #define __pyx_PyFloat_AsDouble(x) PyFloat_AsDouble(x)
 #endif
 #define __pyx_PyFloat_AsFloat(x) ((float) __pyx_PyFloat_AsDouble(x))
 #if PY_MAJOR_VERSION >= 3
@@ -949,26 +1090,26 @@
 #define __PYX_GET_DICT_VERSION(dict)  (0)
 #define __PYX_UPDATE_DICT_CACHE(dict, value, cache_var, version_var)
 #define __PYX_PY_DICT_LOOKUP_IF_MODIFIED(VAR, DICT, LOOKUP)  (VAR) = (LOOKUP);
 #endif
 
 /* GetModuleGlobalName.proto */
 #if CYTHON_USE_DICT_VERSIONS
-#define __Pyx_GetModuleGlobalName(var, name)  {\
+#define __Pyx_GetModuleGlobalName(var, name)  do {\
     static PY_UINT64_T __pyx_dict_version = 0;\
     static PyObject *__pyx_dict_cached_value = NULL;\
     (var) = (likely(__pyx_dict_version == __PYX_GET_DICT_VERSION(__pyx_d))) ?\
         (likely(__pyx_dict_cached_value) ? __Pyx_NewRef(__pyx_dict_cached_value) : __Pyx_GetBuiltinName(name)) :\
         __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
-#define __Pyx_GetModuleGlobalNameUncached(var, name)  {\
+} while(0)
+#define __Pyx_GetModuleGlobalNameUncached(var, name)  do {\
     PY_UINT64_T __pyx_dict_version;\
     PyObject *__pyx_dict_cached_value;\
     (var) = __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
+} while(0)
 static PyObject *__Pyx__GetModuleGlobalName(PyObject *name, PY_UINT64_T *dict_version, PyObject **dict_cached_value);
 #else
 #define __Pyx_GetModuleGlobalName(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 #define __Pyx_GetModuleGlobalNameUncached(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 static CYTHON_INLINE PyObject *__Pyx__GetModuleGlobalName(PyObject *name);
 #endif
 
@@ -989,21 +1130,29 @@
 #define __Pyx_PyFunction_FastCallDict(func, args, nargs, kwargs) _PyFunction_FastCallDict(func, args, nargs, kwargs)
 #endif
 #define __Pyx_BUILD_ASSERT_EXPR(cond)\
     (sizeof(char [1 - 2*!(cond)]) - 1)
 #ifndef Py_MEMBER_SIZE
 #define Py_MEMBER_SIZE(type, member) sizeof(((type *)0)->member)
 #endif
+#if CYTHON_FAST_PYCALL
   static size_t __pyx_pyframe_localsplus_offset = 0;
   #include "frameobject.h"
+#if PY_VERSION_HEX >= 0x030b00a6
+  #ifndef Py_BUILD_CORE
+    #define Py_BUILD_CORE 1
+  #endif
+  #include "internal/pycore_frame.h"
+#endif
   #define __Pxy_PyFrame_Initialize_Offsets()\
     ((void)__Pyx_BUILD_ASSERT_EXPR(sizeof(PyFrameObject) == offsetof(PyFrameObject, f_localsplus) + Py_MEMBER_SIZE(PyFrameObject, f_localsplus)),\
      (void)(__pyx_pyframe_localsplus_offset = ((size_t)PyFrame_Type.tp_basicsize) - Py_MEMBER_SIZE(PyFrameObject, f_localsplus)))
   #define __Pyx_PyFrame_GetLocalsplus(frame)\
     (assert(__pyx_pyframe_localsplus_offset), (PyObject **)(((char *)(frame)) + __pyx_pyframe_localsplus_offset))
+#endif // CYTHON_FAST_PYCALL
 #endif
 
 /* PyObjectCall.proto */
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw);
 #else
 #define __Pyx_PyObject_Call(func, arg, kw) PyObject_Call(func, arg, kw)
@@ -1399,14 +1548,19 @@
 static PyCodeObject *__pyx_find_code_object(int code_line);
 static void __pyx_insert_code_object(int code_line, PyCodeObject* code_object);
 
 /* AddTraceback.proto */
 static void __Pyx_AddTraceback(const char *funcname, int c_line,
                                int py_line, const char *filename);
 
+/* GCCDiagnostics.proto */
+#if defined(__GNUC__) && (__GNUC__ > 4 || (__GNUC__ == 4 && __GNUC_MINOR__ >= 6))
+#define __Pyx_HAS_GCC_DIAGNOSTIC
+#endif
+
 /* CIntToPy.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value);
 
 /* CIntFromPy.proto */
 static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *);
 
 /* CIntFromPy.proto */
@@ -1485,14 +1639,15 @@
 static const char __pyx_k_json[] = "json";
 static const char __pyx_k_list[] = "list";
 static const char __pyx_k_load[] = "load";
 static const char __pyx_k_main[] = "__main__";
 static const char __pyx_k_name[] = "name";
 static const char __pyx_k_node[] = "node";
 static const char __pyx_k_open[] = "open";
+static const char __pyx_k_palm[] = "palm";
 static const char __pyx_k_path[] = "path";
 static const char __pyx_k_pip3[] = "pip3";
 static const char __pyx_k_read[] = "read";
 static const char __pyx_k_save[] = "save";
 static const char __pyx_k_self[] = "self";
 static const char __pyx_k_test[] = "__test__";
 static const char __pyx_k_user[] = "user";
@@ -1960,14 +2115,15 @@
 static PyObject *__pyx_n_s_obj;
 static PyObject *__pyx_n_u_olive;
 static PyObject *__pyx_n_s_open;
 static PyObject *__pyx_n_s_opener;
 static PyObject *__pyx_n_s_option;
 static PyObject *__pyx_n_s_os;
 static PyObject *__pyx_kp_u_p;
+static PyObject *__pyx_n_u_palm;
 static PyObject *__pyx_n_s_parse;
 static PyObject *__pyx_n_s_pass_context;
 static PyObject *__pyx_n_s_pass_obj;
 static PyObject *__pyx_n_s_path;
 static PyObject *__pyx_n_u_pip;
 static PyObject *__pyx_n_u_pip3;
 static PyObject *__pyx_kp_u_pip3_or_pip_must_be_installed_i;
@@ -4587,55 +4743,56 @@
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_n_u_ironwood);
     __pyx_r = __pyx_n_u_ironwood;
     goto __pyx_L0;
 
   }
 
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 220, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(7); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 220, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (PyDict_SetItem(__pyx_t_3, __pyx_int_10, __pyx_n_u_juniper) < 0) __PYX_ERR(0, 220, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_3, __pyx_int_11, __pyx_n_u_koa) < 0) __PYX_ERR(0, 220, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_3, __pyx_int_12, __pyx_n_u_lilac) < 0) __PYX_ERR(0, 220, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_3, __pyx_int_13, __pyx_n_u_maple) < 0) __PYX_ERR(0, 220, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_3, __pyx_int_14, __pyx_n_u_nutmeg) < 0) __PYX_ERR(0, 220, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_3, __pyx_int_15, __pyx_n_u_olive) < 0) __PYX_ERR(0, 220, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_int_16, __pyx_n_u_palm) < 0) __PYX_ERR(0, 220, __pyx_L1_error)
 
-  __pyx_t_1 = __Pyx_PyDict_GetItemDefault(__pyx_t_3, __pyx_v_major_version, Py_None); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 226, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_GetItemDefault(__pyx_t_3, __pyx_v_major_version, Py_None); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 227, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_release_name = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_v_release_name); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 227, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_v_release_name); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 228, __pyx_L1_error)
   if (__pyx_t_4) {
 
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_v_release_name);
     __pyx_r = __pyx_v_release_name;
     goto __pyx_L0;
 
   }
 
   __Pyx_XDECREF(__pyx_r);
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_fail); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 229, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_fail); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 230, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_2 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_2)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_2);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_2, __pyx_kp_u_You_are_running_an_unknown_relea) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_kp_u_You_are_running_an_unknown_relea);
   __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 229, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 230, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
 
@@ -4685,81 +4842,81 @@
   PyObject *__pyx_t_10 = NULL;
   PyObject *__pyx_t_11 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("load_license", 0);
 
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_os); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 233, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_os); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 234, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_path); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 233, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_path); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 234, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_exists); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 233, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_exists); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 234, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_v_license_path) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v_license_path);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 233, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 234, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 233, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 234, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_5 = ((!__pyx_t_4) != 0);
   if (__pyx_t_5) {
 
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 234, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 235, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_r = __pyx_t_1;
     __pyx_t_1 = 0;
     goto __pyx_L0;
 
   }
 
   /*with:*/ {
-    __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 236, __pyx_L1_error)
+    __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 237, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_v_license_path);
     __Pyx_GIVEREF(__pyx_v_license_path);
     PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_license_path);
-    __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 236, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 237, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_encoding, __pyx_kp_u_utf_8) < 0) __PYX_ERR(0, 236, __pyx_L1_error)
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_open, __pyx_t_1, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 236, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_encoding, __pyx_kp_u_utf_8) < 0) __PYX_ERR(0, 237, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_open, __pyx_t_1, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 237, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_6 = __Pyx_PyObject_LookupSpecial(__pyx_t_3, __pyx_n_s_exit_2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 236, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_LookupSpecial(__pyx_t_3, __pyx_n_s_exit_2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 237, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_1 = __Pyx_PyObject_LookupSpecial(__pyx_t_3, __pyx_n_s_enter); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 236, __pyx_L4_error)
+    __pyx_t_1 = __Pyx_PyObject_LookupSpecial(__pyx_t_3, __pyx_n_s_enter); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 237, __pyx_L4_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_7 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
       __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_1);
       if (likely(__pyx_t_7)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
         __Pyx_INCREF(__pyx_t_7);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_1, function);
       }
     }
     __pyx_t_2 = (__pyx_t_7) ? __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_7) : __Pyx_PyObject_CallNoArg(__pyx_t_1);
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 236, __pyx_L4_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 237, __pyx_L4_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_t_1 = __pyx_t_2;
     __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     /*try:*/ {
       {
@@ -4770,68 +4927,68 @@
         __Pyx_XGOTREF(__pyx_t_9);
         __Pyx_XGOTREF(__pyx_t_10);
         /*try:*/ {
           __pyx_v_f = __pyx_t_1;
           __pyx_t_1 = 0;
 
           __Pyx_XDECREF(__pyx_r);
-          __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_json); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 237, __pyx_L8_error)
+          __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_json); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 238, __pyx_L8_error)
           __Pyx_GOTREF(__pyx_t_3);
-          __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_load); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 237, __pyx_L8_error)
+          __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_load); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 238, __pyx_L8_error)
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
           __pyx_t_3 = NULL;
           if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
             __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
             if (likely(__pyx_t_3)) {
               PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
               __Pyx_INCREF(__pyx_t_3);
               __Pyx_INCREF(function);
               __Pyx_DECREF_SET(__pyx_t_2, function);
             }
           }
           __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_v_f) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v_f);
           __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-          if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 237, __pyx_L8_error)
+          if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 238, __pyx_L8_error)
           __Pyx_GOTREF(__pyx_t_1);
           __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
           __pyx_r = __pyx_t_1;
           __pyx_t_1 = 0;
           goto __pyx_L12_try_return;
 
         }
         __pyx_L8_error:;
         __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
         __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
         __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
         __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
         /*except:*/ {
           __Pyx_AddTraceback("tutorlicense.cmd.load_license", __pyx_clineno, __pyx_lineno, __pyx_filename);
-          if (__Pyx_GetException(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3) < 0) __PYX_ERR(0, 236, __pyx_L10_except_error)
+          if (__Pyx_GetException(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3) < 0) __PYX_ERR(0, 237, __pyx_L10_except_error)
           __Pyx_GOTREF(__pyx_t_1);
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_GOTREF(__pyx_t_3);
-          __pyx_t_7 = PyTuple_Pack(3, __pyx_t_1, __pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 236, __pyx_L10_except_error)
+          __pyx_t_7 = PyTuple_Pack(3, __pyx_t_1, __pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 237, __pyx_L10_except_error)
           __Pyx_GOTREF(__pyx_t_7);
           __pyx_t_11 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_7, NULL);
           __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
           __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-          if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 236, __pyx_L10_except_error)
+          if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 237, __pyx_L10_except_error)
           __Pyx_GOTREF(__pyx_t_11);
           __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_11);
           __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-          if (__pyx_t_5 < 0) __PYX_ERR(0, 236, __pyx_L10_except_error)
+          if (__pyx_t_5 < 0) __PYX_ERR(0, 237, __pyx_L10_except_error)
           __pyx_t_4 = ((!(__pyx_t_5 != 0)) != 0);
           if (__pyx_t_4) {
             __Pyx_GIVEREF(__pyx_t_1);
             __Pyx_GIVEREF(__pyx_t_2);
             __Pyx_XGIVEREF(__pyx_t_3);
             __Pyx_ErrRestoreWithState(__pyx_t_1, __pyx_t_2, __pyx_t_3);
             __pyx_t_1 = 0; __pyx_t_2 = 0; __pyx_t_3 = 0; 
-            __PYX_ERR(0, 236, __pyx_L10_except_error)
+            __PYX_ERR(0, 237, __pyx_L10_except_error)
           }
           __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
           __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
           __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
           goto __pyx_L9_exception_handled;
         }
         __pyx_L10_except_error:;
@@ -4854,27 +5011,27 @@
       }
     }
     /*finally:*/ {
       /*normal exit:*/{
         if (__pyx_t_6) {
           __pyx_t_10 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_tuple__11, NULL);
           __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-          if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 236, __pyx_L1_error)
+          if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 237, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_10);
           __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
         }
         goto __pyx_L7;
       }
       __pyx_L5_return: {
         __pyx_t_10 = __pyx_r;
         __pyx_r = 0;
         if (__pyx_t_6) {
           __pyx_t_9 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_tuple__11, NULL);
           __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-          if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 236, __pyx_L1_error)
+          if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 237, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_9);
           __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
         }
         __pyx_r = __pyx_t_10;
         __pyx_t_10 = 0;
         goto __pyx_L0;
       }
@@ -4937,32 +5094,32 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_license_path)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_licenseid)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("save_license", 1, 2, 2, 1); __PYX_ERR(0, 240, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("save_license", 1, 2, 2, 1); __PYX_ERR(0, 241, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "save_license") < 0)) __PYX_ERR(0, 240, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "save_license") < 0)) __PYX_ERR(0, 241, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
     __pyx_v_license_path = values[0];
     __pyx_v_licenseid = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("save_license", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 240, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("save_license", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 241, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("tutorlicense.cmd.save_license", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_12tutorlicense_3cmd_28save_license(__pyx_self, __pyx_v_license_path, __pyx_v_licenseid);
 
@@ -4992,15 +5149,15 @@
   PyObject *__pyx_t_12 = NULL;
   PyObject *__pyx_t_13 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("save_license", 0);
 
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_make_unverified_request); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 241, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_make_unverified_request); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 242, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   __pyx_t_4 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -5009,208 +5166,208 @@
       __Pyx_DECREF_SET(__pyx_t_2, function);
       __pyx_t_4 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[3] = {__pyx_t_3, __pyx_v_licenseid, __pyx_kp_u_key};
-    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_4, 2+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 241, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_4, 2+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 242, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_GOTREF(__pyx_t_1);
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[3] = {__pyx_t_3, __pyx_v_licenseid, __pyx_kp_u_key};
-    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_4, 2+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 241, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_4, 2+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 242, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_GOTREF(__pyx_t_1);
   } else
   #endif
   {
-    __pyx_t_5 = PyTuple_New(2+__pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 241, __pyx_L1_error)
+    __pyx_t_5 = PyTuple_New(2+__pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 242, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     if (__pyx_t_3) {
       __Pyx_GIVEREF(__pyx_t_3); PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_3); __pyx_t_3 = NULL;
     }
     __Pyx_INCREF(__pyx_v_licenseid);
     __Pyx_GIVEREF(__pyx_v_licenseid);
     PyTuple_SET_ITEM(__pyx_t_5, 0+__pyx_t_4, __pyx_v_licenseid);
     __Pyx_INCREF(__pyx_kp_u_key);
     __Pyx_GIVEREF(__pyx_kp_u_key);
     PyTuple_SET_ITEM(__pyx_t_5, 1+__pyx_t_4, __pyx_kp_u_key);
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_5, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 241, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_5, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 242, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_data = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_load_license); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 242, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_load_license); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 243, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_5 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_5, __pyx_v_license_path) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v_license_path);
   __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 242, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 243, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_license_data = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_license_data, __pyx_n_s_update); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 243, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_license_data, __pyx_n_s_update); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 244, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 243, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 244, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_id, __pyx_v_licenseid) < 0) __PYX_ERR(0, 243, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_PyObject_Dict_GetItem(__pyx_v_data, __pyx_n_u_data); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 243, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_id, __pyx_v_licenseid) < 0) __PYX_ERR(0, 244, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Dict_GetItem(__pyx_v_data, __pyx_n_u_data); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 244, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_6 = __Pyx_PyObject_Dict_GetItem(__pyx_t_3, __pyx_n_u_key_2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 243, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_Dict_GetItem(__pyx_t_3, __pyx_n_u_key_2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 244, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_key_2, __pyx_t_6) < 0) __PYX_ERR(0, 243, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_key_2, __pyx_t_6) < 0) __PYX_ERR(0, 244, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __pyx_t_6 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_6)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_6);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_6, __pyx_t_5) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_5);
   __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 243, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 244, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_os); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 245, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_os); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 246, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_path); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 245, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_path); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 246, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_dirname); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 245, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_dirname); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 246, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_t_5 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_5, __pyx_v_license_path) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v_license_path);
   __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 245, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 246, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_license_directory = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_os); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 246, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_os); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 247, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_path); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 246, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_path); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 247, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_exists); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 246, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_exists); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 247, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_t_5 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_5, __pyx_v_license_directory) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v_license_directory);
   __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 246, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 247, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_7 < 0)) __PYX_ERR(0, 246, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_7 < 0)) __PYX_ERR(0, 247, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_8 = ((!__pyx_t_7) != 0);
   if (__pyx_t_8) {
 
-    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_os); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 247, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_os); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 248, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_makedirs); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 247, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_makedirs); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 248, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_t_2 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
       __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_5);
       if (likely(__pyx_t_2)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
         __Pyx_INCREF(__pyx_t_2);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_5, function);
       }
     }
     __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_2, __pyx_v_license_directory) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_v_license_directory);
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 247, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 248, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   }
 
   /*with:*/ {
-    __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 248, __pyx_L1_error)
+    __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 249, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_v_license_path);
     __Pyx_GIVEREF(__pyx_v_license_path);
     PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_license_path);
     __Pyx_INCREF(__pyx_n_u_w);
     __Pyx_GIVEREF(__pyx_n_u_w);
     PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_n_u_w);
-    __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 248, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 249, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_encoding, __pyx_kp_u_utf_8) < 0) __PYX_ERR(0, 248, __pyx_L1_error)
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_open, __pyx_t_1, __pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 248, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_encoding, __pyx_kp_u_utf_8) < 0) __PYX_ERR(0, 249, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_open, __pyx_t_1, __pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 249, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __pyx_t_9 = __Pyx_PyObject_LookupSpecial(__pyx_t_2, __pyx_n_s_exit_2); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 248, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyObject_LookupSpecial(__pyx_t_2, __pyx_n_s_exit_2); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 249, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
-    __pyx_t_1 = __Pyx_PyObject_LookupSpecial(__pyx_t_2, __pyx_n_s_enter); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 248, __pyx_L4_error)
+    __pyx_t_1 = __Pyx_PyObject_LookupSpecial(__pyx_t_2, __pyx_n_s_enter); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 249, __pyx_L4_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_6 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
       __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_1);
       if (likely(__pyx_t_6)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
         __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_1, function);
       }
     }
     __pyx_t_5 = (__pyx_t_6) ? __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_6) : __Pyx_PyObject_CallNoArg(__pyx_t_1);
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 248, __pyx_L4_error)
+    if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 249, __pyx_L4_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_t_1 = __pyx_t_5;
     __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     /*try:*/ {
       {
@@ -5220,17 +5377,17 @@
         __Pyx_XGOTREF(__pyx_t_10);
         __Pyx_XGOTREF(__pyx_t_11);
         __Pyx_XGOTREF(__pyx_t_12);
         /*try:*/ {
           __pyx_v_f = __pyx_t_1;
           __pyx_t_1 = 0;
 
-          __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_json); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 249, __pyx_L8_error)
+          __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_json); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 250, __pyx_L8_error)
           __Pyx_GOTREF(__pyx_t_2);
-          __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_dump); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 249, __pyx_L8_error)
+          __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_dump); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 250, __pyx_L8_error)
           __Pyx_GOTREF(__pyx_t_5);
           __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
           __pyx_t_2 = NULL;
           __pyx_t_4 = 0;
           if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
             __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_5);
             if (likely(__pyx_t_2)) {
@@ -5240,40 +5397,40 @@
               __Pyx_DECREF_SET(__pyx_t_5, function);
               __pyx_t_4 = 1;
             }
           }
           #if CYTHON_FAST_PYCALL
           if (PyFunction_Check(__pyx_t_5)) {
             PyObject *__pyx_temp[3] = {__pyx_t_2, __pyx_v_license_data, __pyx_v_f};
-            __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_4, 2+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 249, __pyx_L8_error)
+            __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_4, 2+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 250, __pyx_L8_error)
             __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
             __Pyx_GOTREF(__pyx_t_1);
           } else
           #endif
           #if CYTHON_FAST_PYCCALL
           if (__Pyx_PyFastCFunction_Check(__pyx_t_5)) {
             PyObject *__pyx_temp[3] = {__pyx_t_2, __pyx_v_license_data, __pyx_v_f};
-            __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_4, 2+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 249, __pyx_L8_error)
+            __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_4, 2+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 250, __pyx_L8_error)
             __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
             __Pyx_GOTREF(__pyx_t_1);
           } else
           #endif
           {
-            __pyx_t_6 = PyTuple_New(2+__pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 249, __pyx_L8_error)
+            __pyx_t_6 = PyTuple_New(2+__pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 250, __pyx_L8_error)
             __Pyx_GOTREF(__pyx_t_6);
             if (__pyx_t_2) {
               __Pyx_GIVEREF(__pyx_t_2); PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_2); __pyx_t_2 = NULL;
             }
             __Pyx_INCREF(__pyx_v_license_data);
             __Pyx_GIVEREF(__pyx_v_license_data);
             PyTuple_SET_ITEM(__pyx_t_6, 0+__pyx_t_4, __pyx_v_license_data);
             __Pyx_INCREF(__pyx_v_f);
             __Pyx_GIVEREF(__pyx_v_f);
             PyTuple_SET_ITEM(__pyx_t_6, 1+__pyx_t_4, __pyx_v_f);
-            __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_6, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 249, __pyx_L8_error)
+            __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_6, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 250, __pyx_L8_error)
             __Pyx_GOTREF(__pyx_t_1);
             __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
           }
           __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
           __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
         }
@@ -5285,36 +5442,36 @@
         __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
         __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
         __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
         __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
         __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
         /*except:*/ {
           __Pyx_AddTraceback("tutorlicense.cmd.save_license", __pyx_clineno, __pyx_lineno, __pyx_filename);
-          if (__Pyx_GetException(&__pyx_t_1, &__pyx_t_5, &__pyx_t_6) < 0) __PYX_ERR(0, 248, __pyx_L10_except_error)
+          if (__Pyx_GetException(&__pyx_t_1, &__pyx_t_5, &__pyx_t_6) < 0) __PYX_ERR(0, 249, __pyx_L10_except_error)
           __Pyx_GOTREF(__pyx_t_1);
           __Pyx_GOTREF(__pyx_t_5);
           __Pyx_GOTREF(__pyx_t_6);
-          __pyx_t_2 = PyTuple_Pack(3, __pyx_t_1, __pyx_t_5, __pyx_t_6); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 248, __pyx_L10_except_error)
+          __pyx_t_2 = PyTuple_Pack(3, __pyx_t_1, __pyx_t_5, __pyx_t_6); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 249, __pyx_L10_except_error)
           __Pyx_GOTREF(__pyx_t_2);
           __pyx_t_13 = __Pyx_PyObject_Call(__pyx_t_9, __pyx_t_2, NULL);
           __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
           __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-          if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 248, __pyx_L10_except_error)
+          if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 249, __pyx_L10_except_error)
           __Pyx_GOTREF(__pyx_t_13);
           __pyx_t_8 = __Pyx_PyObject_IsTrue(__pyx_t_13);
           __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
-          if (__pyx_t_8 < 0) __PYX_ERR(0, 248, __pyx_L10_except_error)
+          if (__pyx_t_8 < 0) __PYX_ERR(0, 249, __pyx_L10_except_error)
           __pyx_t_7 = ((!(__pyx_t_8 != 0)) != 0);
           if (__pyx_t_7) {
             __Pyx_GIVEREF(__pyx_t_1);
             __Pyx_GIVEREF(__pyx_t_5);
             __Pyx_XGIVEREF(__pyx_t_6);
             __Pyx_ErrRestoreWithState(__pyx_t_1, __pyx_t_5, __pyx_t_6);
             __pyx_t_1 = 0; __pyx_t_5 = 0; __pyx_t_6 = 0; 
-            __PYX_ERR(0, 248, __pyx_L10_except_error)
+            __PYX_ERR(0, 249, __pyx_L10_except_error)
           }
           __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
           __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
           __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
           goto __pyx_L9_exception_handled;
         }
         __pyx_L10_except_error:;
@@ -5332,15 +5489,15 @@
       }
     }
     /*finally:*/ {
       /*normal exit:*/{
         if (__pyx_t_9) {
           __pyx_t_12 = __Pyx_PyObject_Call(__pyx_t_9, __pyx_tuple__11, NULL);
           __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-          if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 248, __pyx_L1_error)
+          if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 249, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_12);
           __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
         }
         goto __pyx_L7;
       }
       __pyx_L7:;
     }
@@ -5416,15 +5573,15 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_license_path)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_endpoint)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("make_request", 0, 2, 4, 1); __PYX_ERR(0, 253, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("make_request", 0, 2, 4, 1); __PYX_ERR(0, 254, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_data);
           if (value) { values[2] = value; kw_args--; }
         }
@@ -5432,15 +5589,15 @@
         case  3:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_method);
           if (value) { values[3] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "make_request") < 0)) __PYX_ERR(0, 253, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "make_request") < 0)) __PYX_ERR(0, 254, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
         CYTHON_FALLTHROUGH;
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
@@ -5453,15 +5610,15 @@
     __pyx_v_license_path = values[0];
     __pyx_v_endpoint = values[1];
     __pyx_v_data = values[2];
     __pyx_v_method = values[3];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("make_request", 0, 2, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 253, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("make_request", 0, 2, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 254, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("tutorlicense.cmd.make_request", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_12tutorlicense_3cmd_30make_request(__pyx_self, __pyx_v_license_path, __pyx_v_endpoint, __pyx_v_data, __pyx_v_method);
 
@@ -5497,114 +5654,114 @@
   PyObject *__pyx_t_12 = NULL;
   int __pyx_t_13;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("make_request", 0);
 
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_load_license); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 255, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_load_license); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 256, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_v_license_path) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v_license_path);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 255, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 256, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_license_data = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_license_data, __pyx_n_s_get); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 258, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_license_data, __pyx_n_s_get); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 259, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_n_u_id) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_n_u_id);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 258, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 259, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 258, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 259, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_5 = ((!__pyx_t_4) != 0);
   if (__pyx_t_5) {
 
-    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_fail); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 259, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_fail); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 260, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_3 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_3)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
         __Pyx_INCREF(__pyx_t_3);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_2, function);
       }
     }
     __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_kp_u_Undefined_license_ID_You_should) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_kp_u_Undefined_license_ID_You_should);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 259, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 260, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   }
 
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_license_data, __pyx_n_s_get); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 266, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_license_data, __pyx_n_s_get); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 267, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_n_u_key_2) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_n_u_key_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 266, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 267, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 266, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 267, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_4 = ((!__pyx_t_5) != 0);
   if (__pyx_t_4) {
 
-    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_fail); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 267, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_fail); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 268, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_3 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_3)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
         __Pyx_INCREF(__pyx_t_3);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_2, function);
       }
     }
     __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_kp_u_Undefined_license_key_You_should) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_kp_u_Undefined_license_key_You_should);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 267, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 268, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   }
 
   {
@@ -5612,169 +5769,169 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_6, &__pyx_t_7, &__pyx_t_8);
     __Pyx_XGOTREF(__pyx_t_6);
     __Pyx_XGOTREF(__pyx_t_7);
     __Pyx_XGOTREF(__pyx_t_8);
     /*try:*/ {
 
-      __pyx_t_2 = __Pyx_PyObject_Dict_GetItem(__pyx_v_license_data, __pyx_n_u_key_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 274, __pyx_L5_error)
+      __pyx_t_2 = __Pyx_PyObject_Dict_GetItem(__pyx_v_license_data, __pyx_n_u_key_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 275, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_split); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 274, __pyx_L5_error)
+      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_split); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 275, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __pyx_t_2 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
         __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
         if (likely(__pyx_t_2)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
           __Pyx_INCREF(__pyx_t_2);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_3, function);
         }
       }
       __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_2, __pyx_kp_u__9) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_kp_u__9);
       __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 274, __pyx_L5_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 275, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       if ((likely(PyTuple_CheckExact(__pyx_t_1))) || (PyList_CheckExact(__pyx_t_1))) {
         PyObject* sequence = __pyx_t_1;
         Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
         if (unlikely(size != 2)) {
           if (size > 2) __Pyx_RaiseTooManyValuesError(2);
           else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-          __PYX_ERR(0, 274, __pyx_L5_error)
+          __PYX_ERR(0, 275, __pyx_L5_error)
         }
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
         if (likely(PyTuple_CheckExact(sequence))) {
           __pyx_t_3 = PyTuple_GET_ITEM(sequence, 0); 
           __pyx_t_2 = PyTuple_GET_ITEM(sequence, 1); 
         } else {
           __pyx_t_3 = PyList_GET_ITEM(sequence, 0); 
           __pyx_t_2 = PyList_GET_ITEM(sequence, 1); 
         }
         __Pyx_INCREF(__pyx_t_3);
         __Pyx_INCREF(__pyx_t_2);
         #else
-        __pyx_t_3 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 274, __pyx_L5_error)
+        __pyx_t_3 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 275, __pyx_L5_error)
         __Pyx_GOTREF(__pyx_t_3);
-        __pyx_t_2 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 274, __pyx_L5_error)
+        __pyx_t_2 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 275, __pyx_L5_error)
         __Pyx_GOTREF(__pyx_t_2);
         #endif
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       } else {
         Py_ssize_t index = -1;
-        __pyx_t_9 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 274, __pyx_L5_error)
+        __pyx_t_9 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 275, __pyx_L5_error)
         __Pyx_GOTREF(__pyx_t_9);
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         __pyx_t_10 = Py_TYPE(__pyx_t_9)->tp_iternext;
         index = 0; __pyx_t_3 = __pyx_t_10(__pyx_t_9); if (unlikely(!__pyx_t_3)) goto __pyx_L11_unpacking_failed;
         __Pyx_GOTREF(__pyx_t_3);
         index = 1; __pyx_t_2 = __pyx_t_10(__pyx_t_9); if (unlikely(!__pyx_t_2)) goto __pyx_L11_unpacking_failed;
         __Pyx_GOTREF(__pyx_t_2);
-        if (__Pyx_IternextUnpackEndCheck(__pyx_t_10(__pyx_t_9), 2) < 0) __PYX_ERR(0, 274, __pyx_L5_error)
+        if (__Pyx_IternextUnpackEndCheck(__pyx_t_10(__pyx_t_9), 2) < 0) __PYX_ERR(0, 275, __pyx_L5_error)
         __pyx_t_10 = NULL;
         __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
         goto __pyx_L12_unpacking_done;
         __pyx_L11_unpacking_failed:;
         __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
         __pyx_t_10 = NULL;
         if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
-        __PYX_ERR(0, 274, __pyx_L5_error)
+        __PYX_ERR(0, 275, __pyx_L5_error)
         __pyx_L12_unpacking_done:;
       }
       __pyx_v_encoded_key = __pyx_t_3;
       __pyx_t_3 = 0;
       __pyx_v_encoded_signature = __pyx_t_2;
       __pyx_t_2 = 0;
 
-      __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_base64); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 275, __pyx_L5_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_base64); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 276, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_urlsafe_b64decode); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 275, __pyx_L5_error)
+      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_urlsafe_b64decode); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 276, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __pyx_t_2 = NULL;
       if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
         __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
         if (likely(__pyx_t_2)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
           __Pyx_INCREF(__pyx_t_2);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_3, function);
         }
       }
       __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_2, __pyx_v_encoded_key) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_v_encoded_key);
       __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 275, __pyx_L5_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 276, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __pyx_v_key = __pyx_t_1;
       __pyx_t_1 = 0;
 
-      __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_base64); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 276, __pyx_L5_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_base64); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 277, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_urlsafe_b64decode); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 276, __pyx_L5_error)
+      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_urlsafe_b64decode); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 277, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __pyx_t_3 = NULL;
       if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
         __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
         if (likely(__pyx_t_3)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
           __Pyx_INCREF(__pyx_t_3);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_2, function);
         }
       }
       __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_v_encoded_signature) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v_encoded_signature);
       __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 276, __pyx_L5_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 277, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __pyx_v_signature = __pyx_t_1;
       __pyx_t_1 = 0;
 
-      __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_json); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 277, __pyx_L5_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_json); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 278, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_loads); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 277, __pyx_L5_error)
+      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_loads); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 278, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __pyx_t_2 = NULL;
       if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
         __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
         if (likely(__pyx_t_2)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
           __Pyx_INCREF(__pyx_t_2);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_3, function);
         }
       }
       __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_2, __pyx_v_key) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_v_key);
       __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 277, __pyx_L5_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 278, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __pyx_t_3 = __Pyx_PyObject_Dict_GetItem(__pyx_t_1, __pyx_n_u_product); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 277, __pyx_L5_error)
+      __pyx_t_3 = __Pyx_PyObject_Dict_GetItem(__pyx_t_1, __pyx_n_u_product); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 278, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      __pyx_t_5 = (__Pyx_PyUnicode_Equals(__pyx_t_3, __pyx_n_u_tutorlts, Py_NE)); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 277, __pyx_L5_error)
+      __pyx_t_5 = (__Pyx_PyUnicode_Equals(__pyx_t_3, __pyx_n_u_tutorlts, Py_NE)); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 278, __pyx_L5_error)
       if (__pyx_t_5) {
       } else {
         __pyx_t_4 = __pyx_t_5;
         goto __pyx_L14_bool_binop_done;
       }
-      __pyx_t_5 = (__Pyx_PyUnicode_Equals(__pyx_t_3, __pyx_n_u_tutorwizardedition, Py_NE)); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 277, __pyx_L5_error)
+      __pyx_t_5 = (__Pyx_PyUnicode_Equals(__pyx_t_3, __pyx_n_u_tutorwizardedition, Py_NE)); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 278, __pyx_L5_error)
       __pyx_t_4 = __pyx_t_5;
       __pyx_L14_bool_binop_done:;
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __pyx_t_5 = (__pyx_t_4 != 0);
       if (unlikely(__pyx_t_5)) {
 
         __Pyx_Raise(__pyx_builtin_ValueError, 0, 0, 0);
-        __PYX_ERR(0, 278, __pyx_L5_error)
+        __PYX_ERR(0, 279, __pyx_L5_error)
 
       }
 
     }
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
@@ -5782,51 +5939,51 @@
     __pyx_L5_error:;
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
 
     __Pyx_ErrFetch(&__pyx_t_3, &__pyx_t_1, &__pyx_t_2);
-    __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_binascii); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 279, __pyx_L7_except_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_binascii); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 280, __pyx_L7_except_error)
     __Pyx_GOTREF(__pyx_t_9);
-    __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_t_9, __pyx_n_s_Error); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 279, __pyx_L7_except_error)
+    __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_t_9, __pyx_n_s_Error); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 280, __pyx_L7_except_error)
     __Pyx_GOTREF(__pyx_t_11);
     __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-    __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_json); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 279, __pyx_L7_except_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_json); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 280, __pyx_L7_except_error)
     __Pyx_GOTREF(__pyx_t_9);
-    __pyx_t_12 = __Pyx_PyObject_GetAttrStr(__pyx_t_9, __pyx_n_s_JSONDecodeError); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 279, __pyx_L7_except_error)
+    __pyx_t_12 = __Pyx_PyObject_GetAttrStr(__pyx_t_9, __pyx_n_s_JSONDecodeError); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 280, __pyx_L7_except_error)
     __Pyx_GOTREF(__pyx_t_12);
     __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
     __pyx_t_13 = __Pyx_PyErr_GivenExceptionMatches(__pyx_t_3, __pyx_builtin_AttributeError) || __Pyx_PyErr_GivenExceptionMatches(__pyx_t_3, __pyx_t_11) || __Pyx_PyErr_GivenExceptionMatches(__pyx_t_3, __pyx_t_12) || __Pyx_PyErr_GivenExceptionMatches(__pyx_t_3, __pyx_builtin_KeyError) || __Pyx_PyErr_GivenExceptionMatches(__pyx_t_3, __pyx_builtin_ValueError);
     __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
     __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
     __Pyx_ErrRestore(__pyx_t_3, __pyx_t_1, __pyx_t_2);
     __pyx_t_3 = 0; __pyx_t_1 = 0; __pyx_t_2 = 0;
     if (__pyx_t_13) {
       __Pyx_AddTraceback("tutorlicense.cmd.make_request", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_2, &__pyx_t_1, &__pyx_t_3) < 0) __PYX_ERR(0, 279, __pyx_L7_except_error)
+      if (__Pyx_GetException(&__pyx_t_2, &__pyx_t_1, &__pyx_t_3) < 0) __PYX_ERR(0, 280, __pyx_L7_except_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_GOTREF(__pyx_t_3);
 
-      __Pyx_GetModuleGlobalName(__pyx_t_11, __pyx_n_s_fail); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 280, __pyx_L7_except_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_11, __pyx_n_s_fail); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 281, __pyx_L7_except_error)
       __Pyx_GOTREF(__pyx_t_11);
       __pyx_t_9 = NULL;
       if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_11))) {
         __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_11);
         if (likely(__pyx_t_9)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_11);
           __Pyx_INCREF(__pyx_t_9);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_11, function);
         }
       }
       __pyx_t_12 = (__pyx_t_9) ? __Pyx_PyObject_Call2Args(__pyx_t_11, __pyx_t_9, __pyx_kp_u_Invalid_license_key_The_license) : __Pyx_PyObject_CallOneArg(__pyx_t_11, __pyx_kp_u_Invalid_license_key_The_license);
       __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
-      if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 280, __pyx_L7_except_error)
+      if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 281, __pyx_L7_except_error)
       __Pyx_GOTREF(__pyx_t_12);
       __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
       __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
       __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
       __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
       goto __pyx_L6_exception_handled;
@@ -5843,79 +6000,79 @@
     __Pyx_XGIVEREF(__pyx_t_6);
     __Pyx_XGIVEREF(__pyx_t_7);
     __Pyx_XGIVEREF(__pyx_t_8);
     __Pyx_ExceptionReset(__pyx_t_6, __pyx_t_7, __pyx_t_8);
     __pyx_L10_try_end:;
   }
 
-  __pyx_t_3 = PyList_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 283, __pyx_L1_error)
+  __pyx_t_3 = PyList_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 284, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_INCREF(__pyx_n_s_SHA256);
   __Pyx_GIVEREF(__pyx_n_s_SHA256);
   PyList_SET_ITEM(__pyx_t_3, 0, __pyx_n_s_SHA256);
-  __pyx_t_1 = __Pyx_Import(__pyx_n_s_Crypto_Hash, __pyx_t_3, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 283, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_Import(__pyx_n_s_Crypto_Hash, __pyx_t_3, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 284, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_ImportFrom(__pyx_t_1, __pyx_n_s_SHA256); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 283, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_ImportFrom(__pyx_t_1, __pyx_n_s_SHA256); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 284, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_INCREF(__pyx_t_3);
   __pyx_v_SHA256 = __pyx_t_3;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 284, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 285, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_n_s_RSA);
   __Pyx_GIVEREF(__pyx_n_s_RSA);
   PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_RSA);
-  __pyx_t_3 = __Pyx_Import(__pyx_n_s_Crypto_PublicKey, __pyx_t_1, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 284, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_Import(__pyx_n_s_Crypto_PublicKey, __pyx_t_1, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 285, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_3, __pyx_n_s_RSA); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 284, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_3, __pyx_n_s_RSA); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 285, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_t_1);
   __pyx_v_RSA = __pyx_t_1;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  __pyx_t_3 = PyList_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 285, __pyx_L1_error)
+  __pyx_t_3 = PyList_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 286, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_INCREF(__pyx_n_s_PKCS1_v1_5);
   __Pyx_GIVEREF(__pyx_n_s_PKCS1_v1_5);
   PyList_SET_ITEM(__pyx_t_3, 0, __pyx_n_s_PKCS1_v1_5);
-  __pyx_t_1 = __Pyx_Import(__pyx_n_s_Crypto_Signature, __pyx_t_3, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 285, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_Import(__pyx_n_s_Crypto_Signature, __pyx_t_3, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 286, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_ImportFrom(__pyx_t_1, __pyx_n_s_PKCS1_v1_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 285, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_ImportFrom(__pyx_t_1, __pyx_n_s_PKCS1_v1_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 286, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_INCREF(__pyx_t_3);
   __pyx_v_Signer = __pyx_t_3;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_Signer, __pyx_n_s_new); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 287, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_Signer, __pyx_n_s_new); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 288, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_12 = __Pyx_PyObject_GetAttrStr(__pyx_v_RSA, __pyx_n_s_import_key); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 287, __pyx_L1_error)
+  __pyx_t_12 = __Pyx_PyObject_GetAttrStr(__pyx_v_RSA, __pyx_n_s_import_key); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 288, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_12);
-  __Pyx_GetModuleGlobalName(__pyx_t_11, __pyx_n_s_PUBLIC_KEY); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 287, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_11, __pyx_n_s_PUBLIC_KEY); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 288, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_11);
   __pyx_t_9 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_12))) {
     __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_12);
     if (likely(__pyx_t_9)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_12);
       __Pyx_INCREF(__pyx_t_9);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_12, function);
     }
   }
   __pyx_t_2 = (__pyx_t_9) ? __Pyx_PyObject_Call2Args(__pyx_t_12, __pyx_t_9, __pyx_t_11) : __Pyx_PyObject_CallOneArg(__pyx_t_12, __pyx_t_11);
   __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
   __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 287, __pyx_L1_error)
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 288, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
   __pyx_t_12 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_12 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_12)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
@@ -5923,36 +6080,36 @@
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_1 = (__pyx_t_12) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_12, __pyx_t_2) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_2);
   __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 287, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 288, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_cipher = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_SHA256, __pyx_n_s_new); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 288, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_SHA256, __pyx_n_s_new); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 289, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 288, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 289, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (unlikely(!__pyx_v_key)) { __Pyx_RaiseUnboundLocalError("key"); __PYX_ERR(0, 288, __pyx_L1_error) }
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_data, __pyx_v_key) < 0) __PYX_ERR(0, 288, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_empty_tuple, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 288, __pyx_L1_error)
+  if (unlikely(!__pyx_v_key)) { __Pyx_RaiseUnboundLocalError("key"); __PYX_ERR(0, 289, __pyx_L1_error) }
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_data, __pyx_v_key) < 0) __PYX_ERR(0, 289, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_empty_tuple, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 289, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_digest = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_cipher, __pyx_n_s_verify); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 289, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_cipher, __pyx_n_s_verify); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 290, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (unlikely(!__pyx_v_signature)) { __Pyx_RaiseUnboundLocalError("signature"); __PYX_ERR(0, 289, __pyx_L1_error) }
+  if (unlikely(!__pyx_v_signature)) { __Pyx_RaiseUnboundLocalError("signature"); __PYX_ERR(0, 290, __pyx_L1_error) }
   __pyx_t_1 = NULL;
   __pyx_t_13 = 0;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_1)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_1);
@@ -5960,92 +6117,92 @@
       __Pyx_DECREF_SET(__pyx_t_3, function);
       __pyx_t_13 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_3)) {
     PyObject *__pyx_temp[3] = {__pyx_t_1, __pyx_v_digest, __pyx_v_signature};
-    __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_13, 2+__pyx_t_13); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 289, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_13, 2+__pyx_t_13); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 290, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_GOTREF(__pyx_t_2);
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_3)) {
     PyObject *__pyx_temp[3] = {__pyx_t_1, __pyx_v_digest, __pyx_v_signature};
-    __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_13, 2+__pyx_t_13); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 289, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_13, 2+__pyx_t_13); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 290, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_GOTREF(__pyx_t_2);
   } else
   #endif
   {
-    __pyx_t_12 = PyTuple_New(2+__pyx_t_13); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 289, __pyx_L1_error)
+    __pyx_t_12 = PyTuple_New(2+__pyx_t_13); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 290, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_12);
     if (__pyx_t_1) {
       __Pyx_GIVEREF(__pyx_t_1); PyTuple_SET_ITEM(__pyx_t_12, 0, __pyx_t_1); __pyx_t_1 = NULL;
     }
     __Pyx_INCREF(__pyx_v_digest);
     __Pyx_GIVEREF(__pyx_v_digest);
     PyTuple_SET_ITEM(__pyx_t_12, 0+__pyx_t_13, __pyx_v_digest);
     __Pyx_INCREF(__pyx_v_signature);
     __Pyx_GIVEREF(__pyx_v_signature);
     PyTuple_SET_ITEM(__pyx_t_12, 1+__pyx_t_13, __pyx_v_signature);
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_12, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 289, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_12, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 290, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
   }
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 289, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 290, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_4 = ((!__pyx_t_5) != 0);
   if (__pyx_t_4) {
 
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_fail); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 290, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_fail); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 291, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_12 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_12 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_12)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
         __Pyx_INCREF(__pyx_t_12);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_3, function);
       }
     }
     __pyx_t_2 = (__pyx_t_12) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_12, __pyx_kp_u_Your_license_key_is_invalid_Plea) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_kp_u_Your_license_key_is_invalid_Plea);
     __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 290, __pyx_L1_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 291, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   }
 
   __Pyx_XDECREF(__pyx_r);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_make_unverified_request); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 297, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_make_unverified_request); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 298, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
 
-  __pyx_t_3 = __Pyx_PyObject_Dict_GetItem(__pyx_v_license_data, __pyx_n_u_id); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 298, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Dict_GetItem(__pyx_v_license_data, __pyx_n_u_id); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 299, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
 
-  __pyx_t_12 = PyTuple_New(2); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 297, __pyx_L1_error)
+  __pyx_t_12 = PyTuple_New(2); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 298, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_12);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_12, 0, __pyx_t_3);
   __Pyx_INCREF(__pyx_v_endpoint);
   __Pyx_GIVEREF(__pyx_v_endpoint);
   PyTuple_SET_ITEM(__pyx_t_12, 1, __pyx_v_endpoint);
   __pyx_t_3 = 0;
 
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 298, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 299, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_data, __pyx_v_data) < 0) __PYX_ERR(0, 298, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_method, __pyx_v_method) < 0) __PYX_ERR(0, 298, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_data, __pyx_v_data) < 0) __PYX_ERR(0, 299, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_method, __pyx_v_method) < 0) __PYX_ERR(0, 299, __pyx_L1_error)
 
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_12, __pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 297, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_12, __pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 298, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
@@ -6117,15 +6274,15 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_license_id)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_endpoint)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("make_unverified_request", 0, 2, 4, 1); __PYX_ERR(0, 302, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("make_unverified_request", 0, 2, 4, 1); __PYX_ERR(0, 303, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_data);
           if (value) { values[2] = value; kw_args--; }
         }
@@ -6133,15 +6290,15 @@
         case  3:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_method);
           if (value) { values[3] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "make_unverified_request") < 0)) __PYX_ERR(0, 302, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "make_unverified_request") < 0)) __PYX_ERR(0, 303, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
         CYTHON_FALLTHROUGH;
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
@@ -6154,15 +6311,15 @@
     __pyx_v_license_id = values[0];
     __pyx_v_endpoint = values[1];
     __pyx_v_data = values[2];
     __pyx_v_method = values[3];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("make_unverified_request", 0, 2, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 302, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("make_unverified_request", 0, 2, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 303, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("tutorlicense.cmd.make_unverified_request", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_12tutorlicense_3cmd_32make_unverified_request(__pyx_self, __pyx_v_license_id, __pyx_v_endpoint, __pyx_v_data, __pyx_v_method);
 
@@ -6196,85 +6353,85 @@
   PyObject *__pyx_t_3 = NULL;
   int __pyx_t_4;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("getnode", 0);
 
-  __pyx_t_1 = __Pyx_Import(__pyx_n_s_uuid, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 323, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_Import(__pyx_n_s_uuid, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 324, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_uuid = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_uuid, __pyx_n_s_getnode); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 325, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_uuid, __pyx_n_s_getnode); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 326, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 325, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 326, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_node = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_uuid, __pyx_n_s_getnode); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 326, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_uuid, __pyx_n_s_getnode); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 327, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 326, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 327, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = PyObject_RichCompare(__pyx_v_node, __pyx_t_1, Py_NE); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 326, __pyx_L1_error)
+  __pyx_t_2 = PyObject_RichCompare(__pyx_v_node, __pyx_t_1, Py_NE); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 327, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 326, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 327, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (__pyx_t_4) {
 
-    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_fail); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 328, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_fail); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 329, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_3 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
       __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_1);
       if (likely(__pyx_t_3)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
         __Pyx_INCREF(__pyx_t_3);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_1, function);
       }
     }
     __pyx_t_2 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_3, __pyx_kp_u_Unable_to_read_a_consistent_fing) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_kp_u_Unable_to_read_a_consistent_fing);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 328, __pyx_L1_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 329, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   }
 
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyUnicode_Type)), __pyx_v_node); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 332, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyUnicode_Type)), __pyx_v_node); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 333, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
 
   /* function exit code */
@@ -6329,85 +6486,85 @@
   PyObject *__pyx_t_6 = NULL;
   PyObject *(*__pyx_t_7)(PyObject *);
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("encrypt", 0);
 
-  __pyx_t_1 = PyList_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 336, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 337, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_n_s_AES);
   __Pyx_GIVEREF(__pyx_n_s_AES);
   PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_AES);
   __Pyx_INCREF(__pyx_n_s_PKCS1_OAEP);
   __Pyx_GIVEREF(__pyx_n_s_PKCS1_OAEP);
   PyList_SET_ITEM(__pyx_t_1, 1, __pyx_n_s_PKCS1_OAEP);
-  __pyx_t_2 = __Pyx_Import(__pyx_n_s_Crypto_Cipher, __pyx_t_1, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 336, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_Import(__pyx_n_s_Crypto_Cipher, __pyx_t_1, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 337, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_AES); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 336, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_AES); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 337, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_t_1);
   __pyx_v_AES = __pyx_t_1;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_PKCS1_OAEP); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 336, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_PKCS1_OAEP); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 337, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_t_1);
   __pyx_v_PKCS1_OAEP = __pyx_t_1;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 337, __pyx_L1_error)
+  __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 338, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_n_s_RSA);
   __Pyx_GIVEREF(__pyx_n_s_RSA);
   PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_RSA);
-  __pyx_t_1 = __Pyx_Import(__pyx_n_s_Crypto_PublicKey, __pyx_t_2, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 337, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_Import(__pyx_n_s_Crypto_PublicKey, __pyx_t_2, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 338, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_1, __pyx_n_s_RSA); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 337, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_1, __pyx_n_s_RSA); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 338, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_t_2);
   __pyx_v_RSA = __pyx_t_2;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 338, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 339, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_n_s_get_random_bytes);
   __Pyx_GIVEREF(__pyx_n_s_get_random_bytes);
   PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_get_random_bytes);
-  __pyx_t_2 = __Pyx_Import(__pyx_n_s_Crypto_Random, __pyx_t_1, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 338, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_Import(__pyx_n_s_Crypto_Random, __pyx_t_1, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 339, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_get_random_bytes); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 338, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_get_random_bytes); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 339, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_t_1);
   __pyx_v_get_random_bytes = __pyx_t_1;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_RSA, __pyx_n_s_import_key); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 340, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_RSA, __pyx_n_s_import_key); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 341, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_PUBLIC_KEY); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 340, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_PUBLIC_KEY); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 341, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_4 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_1);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
       __Pyx_INCREF(__pyx_t_4);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_1, function);
     }
   }
   __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_4, __pyx_t_3) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 340, __pyx_L1_error)
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 341, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_recipient_key = __pyx_t_2;
   __pyx_t_2 = 0;
 
   __Pyx_INCREF(__pyx_v_get_random_bytes);
   __pyx_t_1 = __pyx_v_get_random_bytes; __pyx_t_3 = NULL;
@@ -6418,63 +6575,63 @@
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_1, function);
     }
   }
   __pyx_t_2 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_3, __pyx_int_16) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_int_16);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 341, __pyx_L1_error)
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 342, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_session_key = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_PKCS1_OAEP, __pyx_n_s_new); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 344, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_PKCS1_OAEP, __pyx_n_s_new); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 345, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_1);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_1, function);
     }
   }
   __pyx_t_2 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_3, __pyx_v_recipient_key) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_v_recipient_key);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 344, __pyx_L1_error)
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 345, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_cipher_rsa = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_cipher_rsa, __pyx_n_s_encrypt); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 345, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_cipher_rsa, __pyx_n_s_encrypt); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 346, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_1);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_1, function);
     }
   }
   __pyx_t_2 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_3, __pyx_v_session_key) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_v_session_key);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 345, __pyx_L1_error)
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 346, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_enc_session_key = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_AES, __pyx_n_s_new); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 348, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_AES, __pyx_n_s_new); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 349, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_AES, __pyx_n_s_MODE_EAX); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 348, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_AES, __pyx_n_s_MODE_EAX); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 349, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_4 = NULL;
   __pyx_t_5 = 0;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_1);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
@@ -6483,127 +6640,127 @@
       __Pyx_DECREF_SET(__pyx_t_1, function);
       __pyx_t_5 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_1)) {
     PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_v_session_key, __pyx_t_3};
-    __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 348, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 349, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_1)) {
     PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_v_session_key, __pyx_t_3};
-    __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 348, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 349, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   } else
   #endif
   {
-    __pyx_t_6 = PyTuple_New(2+__pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 348, __pyx_L1_error)
+    __pyx_t_6 = PyTuple_New(2+__pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 349, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     if (__pyx_t_4) {
       __Pyx_GIVEREF(__pyx_t_4); PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_4); __pyx_t_4 = NULL;
     }
     __Pyx_INCREF(__pyx_v_session_key);
     __Pyx_GIVEREF(__pyx_v_session_key);
     PyTuple_SET_ITEM(__pyx_t_6, 0+__pyx_t_5, __pyx_v_session_key);
     __Pyx_GIVEREF(__pyx_t_3);
     PyTuple_SET_ITEM(__pyx_t_6, 1+__pyx_t_5, __pyx_t_3);
     __pyx_t_3 = 0;
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_6, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 348, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_6, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 349, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_cipher_aes = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_cipher_aes, __pyx_n_s_encrypt_and_digest); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 349, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_cipher_aes, __pyx_n_s_encrypt_and_digest); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 350, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_6 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
     __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_1);
     if (likely(__pyx_t_6)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
       __Pyx_INCREF(__pyx_t_6);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_1, function);
     }
   }
   __pyx_t_2 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_6, __pyx_v_message) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_v_message);
   __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 349, __pyx_L1_error)
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 350, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if ((likely(PyTuple_CheckExact(__pyx_t_2))) || (PyList_CheckExact(__pyx_t_2))) {
     PyObject* sequence = __pyx_t_2;
     Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
     if (unlikely(size != 2)) {
       if (size > 2) __Pyx_RaiseTooManyValuesError(2);
       else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-      __PYX_ERR(0, 349, __pyx_L1_error)
+      __PYX_ERR(0, 350, __pyx_L1_error)
     }
     #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
     if (likely(PyTuple_CheckExact(sequence))) {
       __pyx_t_1 = PyTuple_GET_ITEM(sequence, 0); 
       __pyx_t_6 = PyTuple_GET_ITEM(sequence, 1); 
     } else {
       __pyx_t_1 = PyList_GET_ITEM(sequence, 0); 
       __pyx_t_6 = PyList_GET_ITEM(sequence, 1); 
     }
     __Pyx_INCREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_t_6);
     #else
-    __pyx_t_1 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 349, __pyx_L1_error)
+    __pyx_t_1 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 350, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_6 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 349, __pyx_L1_error)
+    __pyx_t_6 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 350, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     #endif
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   } else {
     Py_ssize_t index = -1;
-    __pyx_t_3 = PyObject_GetIter(__pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 349, __pyx_L1_error)
+    __pyx_t_3 = PyObject_GetIter(__pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 350, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_t_7 = Py_TYPE(__pyx_t_3)->tp_iternext;
     index = 0; __pyx_t_1 = __pyx_t_7(__pyx_t_3); if (unlikely(!__pyx_t_1)) goto __pyx_L3_unpacking_failed;
     __Pyx_GOTREF(__pyx_t_1);
     index = 1; __pyx_t_6 = __pyx_t_7(__pyx_t_3); if (unlikely(!__pyx_t_6)) goto __pyx_L3_unpacking_failed;
     __Pyx_GOTREF(__pyx_t_6);
-    if (__Pyx_IternextUnpackEndCheck(__pyx_t_7(__pyx_t_3), 2) < 0) __PYX_ERR(0, 349, __pyx_L1_error)
+    if (__Pyx_IternextUnpackEndCheck(__pyx_t_7(__pyx_t_3), 2) < 0) __PYX_ERR(0, 350, __pyx_L1_error)
     __pyx_t_7 = NULL;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L4_unpacking_done;
     __pyx_L3_unpacking_failed:;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_t_7 = NULL;
     if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
-    __PYX_ERR(0, 349, __pyx_L1_error)
+    __PYX_ERR(0, 350, __pyx_L1_error)
     __pyx_L4_unpacking_done:;
   }
   __pyx_v_ciphertext = __pyx_t_1;
   __pyx_t_1 = 0;
   __pyx_v_tag = __pyx_t_6;
   __pyx_t_6 = 0;
 
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_cipher_aes, __pyx_n_s_nonce); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 351, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_cipher_aes, __pyx_n_s_nonce); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 352, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_6 = PyNumber_Add(__pyx_v_enc_session_key, __pyx_t_2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 351, __pyx_L1_error)
+  __pyx_t_6 = PyNumber_Add(__pyx_v_enc_session_key, __pyx_t_2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 352, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = PyNumber_Add(__pyx_t_6, __pyx_v_tag); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 351, __pyx_L1_error)
+  __pyx_t_2 = PyNumber_Add(__pyx_t_6, __pyx_v_tag); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 352, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = PyNumber_Add(__pyx_t_2, __pyx_v_ciphertext); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 351, __pyx_L1_error)
+  __pyx_t_6 = PyNumber_Add(__pyx_t_2, __pyx_v_ciphertext); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 352, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_6;
   __pyx_t_6 = 0;
   goto __pyx_L0;
 
 
@@ -6677,34 +6834,34 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      __pyx_t_4 = __Pyx_Import(__pyx_n_s_uuid, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 305, __pyx_L3_error)
+      __pyx_t_4 = __Pyx_Import(__pyx_n_s_uuid, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 306, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_4);
       __pyx_v_uuid = __pyx_t_4;
       __pyx_t_4 = 0;
 
-      __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_uuid, __pyx_n_s_UUID); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 307, __pyx_L3_error)
+      __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_uuid, __pyx_n_s_UUID); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 308, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_5);
       __pyx_t_6 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
         __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_5);
         if (likely(__pyx_t_6)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
           __Pyx_INCREF(__pyx_t_6);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_5, function);
         }
       }
       __pyx_t_4 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_6, __pyx_v_license_id) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_v_license_id);
       __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-      if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 307, __pyx_L3_error)
+      if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 308, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
@@ -6714,34 +6871,34 @@
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
 
     __pyx_t_7 = __Pyx_PyErr_ExceptionMatches(__pyx_builtin_ValueError);
     if (__pyx_t_7) {
       __Pyx_AddTraceback("tutorlicense.cmd.make_unverified_request", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_4, &__pyx_t_5, &__pyx_t_6) < 0) __PYX_ERR(0, 308, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_4, &__pyx_t_5, &__pyx_t_6) < 0) __PYX_ERR(0, 309, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
 
-      __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_fail); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 309, __pyx_L5_except_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_fail); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 310, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_9);
       __pyx_t_10 = NULL;
       if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_9))) {
         __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_9);
         if (likely(__pyx_t_10)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_9);
           __Pyx_INCREF(__pyx_t_10);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_9, function);
         }
       }
       __pyx_t_8 = (__pyx_t_10) ? __Pyx_PyObject_Call2Args(__pyx_t_9, __pyx_t_10, __pyx_kp_u_Incorrect_license_ID_format_Your) : __Pyx_PyObject_CallOneArg(__pyx_t_9, __pyx_kp_u_Incorrect_license_ID_format_Your);
       __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
-      if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 309, __pyx_L5_except_error)
+      if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 310, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
       goto __pyx_L4_exception_handled;
@@ -6758,201 +6915,201 @@
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     __pyx_L8_try_end:;
   }
 
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_os); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 314, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_os); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 315, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_environ); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 314, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_environ); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 315, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_get); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 314, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_get); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 315, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 314, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 315, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __pyx_v_url = __pyx_t_5;
   __pyx_t_5 = 0;
 
-  __pyx_t_5 = PyNumber_InPlaceAdd(__pyx_v_url, __pyx_kp_u_tutor_lts_api_v1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 315, __pyx_L1_error)
+  __pyx_t_5 = PyNumber_InPlaceAdd(__pyx_v_url, __pyx_kp_u_tutor_lts_api_v1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 316, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF_SET(__pyx_v_url, __pyx_t_5);
   __pyx_t_5 = 0;
 
-  __pyx_t_5 = PyNumber_Add(__pyx_kp_u_license, __pyx_v_license_id); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 316, __pyx_L1_error)
+  __pyx_t_5 = PyNumber_Add(__pyx_kp_u_license, __pyx_v_license_id); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 317, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_6 = PyNumber_InPlaceAdd(__pyx_v_url, __pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 316, __pyx_L1_error)
+  __pyx_t_6 = PyNumber_InPlaceAdd(__pyx_v_url, __pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 317, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF_SET(__pyx_v_url, __pyx_t_6);
   __pyx_t_6 = 0;
 
-  __pyx_t_6 = PyNumber_InPlaceAdd(__pyx_v_url, __pyx_v_endpoint); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 317, __pyx_L1_error)
+  __pyx_t_6 = PyNumber_InPlaceAdd(__pyx_v_url, __pyx_v_endpoint); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 318, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF_SET(__pyx_v_url, __pyx_t_6);
   __pyx_t_6 = 0;
 
-  __pyx_t_11 = __Pyx_PyObject_IsTrue(__pyx_v_data); if (unlikely(__pyx_t_11 < 0)) __PYX_ERR(0, 318, __pyx_L1_error)
+  __pyx_t_11 = __Pyx_PyObject_IsTrue(__pyx_v_data); if (unlikely(__pyx_t_11 < 0)) __PYX_ERR(0, 319, __pyx_L1_error)
   if (__pyx_t_11) {
-    __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_json); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 318, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_json); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 319, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
-    __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_dumps); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 318, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_dumps); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 319, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     __pyx_t_8 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_9))) {
       __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_9);
       if (likely(__pyx_t_8)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_9);
         __Pyx_INCREF(__pyx_t_8);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_9, function);
       }
     }
     __pyx_t_4 = (__pyx_t_8) ? __Pyx_PyObject_Call2Args(__pyx_t_9, __pyx_t_8, __pyx_v_data) : __Pyx_PyObject_CallOneArg(__pyx_t_9, __pyx_v_data);
     __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
-    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 318, __pyx_L1_error)
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 319, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-    __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_encode); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 318, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_encode); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 319, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_4 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_9))) {
       __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_9);
       if (likely(__pyx_t_4)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_9);
         __Pyx_INCREF(__pyx_t_4);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_9, function);
       }
     }
     __pyx_t_5 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_9, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_9);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 318, __pyx_L1_error)
+    if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 319, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
     __pyx_t_6 = __pyx_t_5;
     __pyx_t_5 = 0;
   } else {
     __Pyx_INCREF(Py_None);
     __pyx_t_6 = Py_None;
   }
   __Pyx_DECREF_SET(__pyx_v_data, __pyx_t_6);
   __pyx_t_6 = 0;
 
-  __pyx_t_6 = __Pyx_CyFunction_New(&__pyx_mdef_12tutorlicense_3cmd_23make_unverified_request_1getnode, 0, __pyx_n_s_make_unverified_request_locals_g, NULL, __pyx_n_s_tutorlicense_cmd, __pyx_d, ((PyObject *)__pyx_codeobj__13)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 320, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_CyFunction_New(&__pyx_mdef_12tutorlicense_3cmd_23make_unverified_request_1getnode, 0, __pyx_n_s_make_unverified_request_locals_g, NULL, __pyx_n_s_tutorlicense_cmd, __pyx_d, ((PyObject *)__pyx_codeobj__13)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 321, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __pyx_v_getnode = __pyx_t_6;
   __pyx_t_6 = 0;
 
-  __pyx_t_6 = __Pyx_CyFunction_New(&__pyx_mdef_12tutorlicense_3cmd_23make_unverified_request_3encrypt, 0, __pyx_n_s_make_unverified_request_locals_e, NULL, __pyx_n_s_tutorlicense_cmd, __pyx_d, ((PyObject *)__pyx_codeobj__15)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 334, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_CyFunction_New(&__pyx_mdef_12tutorlicense_3cmd_23make_unverified_request_3encrypt, 0, __pyx_n_s_make_unverified_request_locals_e, NULL, __pyx_n_s_tutorlicense_cmd, __pyx_d, ((PyObject *)__pyx_codeobj__15)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 335, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __pyx_v_encrypt = __pyx_t_6;
   __pyx_t_6 = 0;
 
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_json); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 353, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_json); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 354, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_dumps); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 353, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_dumps); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 354, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 353, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 354, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_9 = __pyx_pf_12tutorlicense_3cmd_23make_unverified_request_getnode(__pyx_v_getnode); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 353, __pyx_L1_error)
+  __pyx_t_9 = __pyx_pf_12tutorlicense_3cmd_23make_unverified_request_getnode(__pyx_v_getnode); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 354, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
-  if (PyDict_SetItem(__pyx_t_6, __pyx_n_u_node, __pyx_t_9) < 0) __PYX_ERR(0, 353, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_6, __pyx_n_u_node, __pyx_t_9) < 0) __PYX_ERR(0, 354, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-  __pyx_t_9 = PyTuple_New(1); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 353, __pyx_L1_error)
+  __pyx_t_9 = PyTuple_New(1); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 354, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
   __Pyx_GIVEREF(__pyx_t_6);
   PyTuple_SET_ITEM(__pyx_t_9, 0, __pyx_t_6);
   __pyx_t_6 = 0;
-  __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 353, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 354, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_sort_keys, Py_True) < 0) __PYX_ERR(0, 353, __pyx_L1_error)
-  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_9, __pyx_t_6); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 353, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_sort_keys, Py_True) < 0) __PYX_ERR(0, 354, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_9, __pyx_t_6); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 354, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __pyx_v_fingerprint = __pyx_t_4;
   __pyx_t_4 = 0;
 
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_fingerprint, __pyx_n_s_encode); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 354, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_fingerprint, __pyx_n_s_encode); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 355, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __pyx_t_9 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_6))) {
     __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_6);
     if (likely(__pyx_t_9)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
       __Pyx_INCREF(__pyx_t_9);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_6, function);
     }
   }
   __pyx_t_4 = (__pyx_t_9) ? __Pyx_PyObject_CallOneArg(__pyx_t_6, __pyx_t_9) : __Pyx_PyObject_CallNoArg(__pyx_t_6);
   __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
-  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 354, __pyx_L1_error)
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 355, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = __pyx_pf_12tutorlicense_3cmd_23make_unverified_request_2encrypt(__pyx_v_encrypt, __pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 354, __pyx_L1_error)
+  __pyx_t_6 = __pyx_pf_12tutorlicense_3cmd_23make_unverified_request_2encrypt(__pyx_v_encrypt, __pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 355, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF_SET(__pyx_v_fingerprint, __pyx_t_6);
   __pyx_t_6 = 0;
 
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_base64); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 355, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_base64); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 356, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_urlsafe_b64encode); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 355, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_urlsafe_b64encode); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 356, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_t_4 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_9))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_9);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_9);
       __Pyx_INCREF(__pyx_t_4);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_9, function);
     }
   }
   __pyx_t_6 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_9, __pyx_t_4, __pyx_v_fingerprint) : __Pyx_PyObject_CallOneArg(__pyx_t_9, __pyx_v_fingerprint);
   __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 355, __pyx_L1_error)
+  if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 356, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
   __Pyx_DECREF_SET(__pyx_v_fingerprint, __pyx_t_6);
   __pyx_t_6 = 0;
 
-  __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_urllib); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 358, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_urllib); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 359, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_9, __pyx_n_s_request); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 358, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_9, __pyx_n_s_request); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 359, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-  __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_build_opener); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 358, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_build_opener); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 359, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_HTTPErrorHandler); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 358, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_HTTPErrorHandler); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 359, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __pyx_t_8 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
     __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_5);
     if (likely(__pyx_t_8)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
       __Pyx_INCREF(__pyx_t_8);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_5, function);
     }
   }
   __pyx_t_4 = (__pyx_t_8) ? __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_t_8) : __Pyx_PyObject_CallNoArg(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
-  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 358, __pyx_L1_error)
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 359, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_t_5 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_9))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_9);
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_9);
@@ -6960,127 +7117,127 @@
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_9, function);
     }
   }
   __pyx_t_6 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_9, __pyx_t_5, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_9, __pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 358, __pyx_L1_error)
+  if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 359, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
   __pyx_v_opener = __pyx_t_6;
   __pyx_t_6 = 0;
 
-  __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_urllib); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 359, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_urllib); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 360, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_9, __pyx_n_s_request); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 359, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_9, __pyx_n_s_request); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 360, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-  __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_install_opener); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 359, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_install_opener); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 360, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_t_4 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_9))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_9);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_9);
       __Pyx_INCREF(__pyx_t_4);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_9, function);
     }
   }
   __pyx_t_6 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_9, __pyx_t_4, __pyx_v_opener) : __Pyx_PyObject_CallOneArg(__pyx_t_9, __pyx_v_opener);
   __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 359, __pyx_L1_error)
+  if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 360, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_urllib); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 361, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_urllib); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 362, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_request); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 361, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_request); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 362, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_9, __pyx_n_s_Request); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 361, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_9, __pyx_n_s_Request); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 362, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
 
-  __pyx_t_9 = PyTuple_New(1); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 361, __pyx_L1_error)
+  __pyx_t_9 = PyTuple_New(1); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 362, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
   __Pyx_INCREF(__pyx_v_url);
   __Pyx_GIVEREF(__pyx_v_url);
   PyTuple_SET_ITEM(__pyx_t_9, 0, __pyx_v_url);
 
-  __pyx_t_4 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 363, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 364, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_data, __pyx_v_data) < 0) __PYX_ERR(0, 363, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_data, __pyx_v_data) < 0) __PYX_ERR(0, 364, __pyx_L1_error)
 
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_method, __pyx_v_method) < 0) __PYX_ERR(0, 363, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_method, __pyx_v_method) < 0) __PYX_ERR(0, 364, __pyx_L1_error)
 
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 366, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 367, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_kp_u_X_TUTOR_LTS_FINGERPRINT, __pyx_v_fingerprint) < 0) __PYX_ERR(0, 366, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_kp_u_X_TUTOR_LTS_FINGERPRINT, __pyx_v_fingerprint) < 0) __PYX_ERR(0, 367, __pyx_L1_error)
 
-  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_version); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 367, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_version); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 368, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_kp_u_X_TUTOR_LTS_VERSION, __pyx_t_8) < 0) __PYX_ERR(0, 366, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_kp_u_X_TUTOR_LTS_VERSION, __pyx_t_8) < 0) __PYX_ERR(0, 367, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  if (PyDict_SetItem(__pyx_t_5, __pyx_kp_u_Content_Type, __pyx_kp_u_application_json) < 0) __PYX_ERR(0, 366, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_headers, __pyx_t_5) < 0) __PYX_ERR(0, 363, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_kp_u_Content_Type, __pyx_kp_u_application_json) < 0) __PYX_ERR(0, 367, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_headers, __pyx_t_5) < 0) __PYX_ERR(0, 364, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_9, __pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 361, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_9, __pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 362, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_v_request = __pyx_t_5;
   __pyx_t_5 = 0;
 
   /*with:*/ {
-    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_urllib); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 371, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_urllib); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 372, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_request); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 371, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_request); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 372, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_9, __pyx_n_s_urlopen); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 371, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_9, __pyx_n_s_urlopen); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 372, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
     __pyx_t_9 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
       __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_4);
       if (likely(__pyx_t_9)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
         __Pyx_INCREF(__pyx_t_9);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_4, function);
       }
     }
     __pyx_t_5 = (__pyx_t_9) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_9, __pyx_v_request) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_v_request);
     __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
-    if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 371, __pyx_L1_error)
+    if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 372, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_3 = __Pyx_PyObject_LookupSpecial(__pyx_t_5, __pyx_n_s_exit_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 371, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_LookupSpecial(__pyx_t_5, __pyx_n_s_exit_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 372, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_9 = __Pyx_PyObject_LookupSpecial(__pyx_t_5, __pyx_n_s_enter); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 371, __pyx_L11_error)
+    __pyx_t_9 = __Pyx_PyObject_LookupSpecial(__pyx_t_5, __pyx_n_s_enter); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 372, __pyx_L11_error)
     __Pyx_GOTREF(__pyx_t_9);
     __pyx_t_6 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_9))) {
       __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_9);
       if (likely(__pyx_t_6)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_9);
         __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_9, function);
       }
     }
     __pyx_t_4 = (__pyx_t_6) ? __Pyx_PyObject_CallOneArg(__pyx_t_9, __pyx_t_6) : __Pyx_PyObject_CallNoArg(__pyx_t_9);
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 371, __pyx_L11_error)
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 372, __pyx_L11_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
     __pyx_t_9 = __pyx_t_4;
     __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     /*try:*/ {
       {
@@ -7090,20 +7247,20 @@
         __Pyx_XGOTREF(__pyx_t_2);
         __Pyx_XGOTREF(__pyx_t_1);
         __Pyx_XGOTREF(__pyx_t_12);
         /*try:*/ {
           __pyx_v_fp = __pyx_t_9;
           __pyx_t_9 = 0;
 
-          __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_fp, __pyx_n_s_status); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 372, __pyx_L15_error)
+          __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_fp, __pyx_n_s_status); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 373, __pyx_L15_error)
           __Pyx_GOTREF(__pyx_t_9);
-          __pyx_t_5 = __Pyx_PyInt_EqObjC(__pyx_t_9, __pyx_int_204, 0xCC, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 372, __pyx_L15_error)
+          __pyx_t_5 = __Pyx_PyInt_EqObjC(__pyx_t_9, __pyx_int_204, 0xCC, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 373, __pyx_L15_error)
           __Pyx_GOTREF(__pyx_t_5);
           __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-          __pyx_t_11 = __Pyx_PyObject_IsTrue(__pyx_t_5); if (unlikely(__pyx_t_11 < 0)) __PYX_ERR(0, 372, __pyx_L15_error)
+          __pyx_t_11 = __Pyx_PyObject_IsTrue(__pyx_t_5); if (unlikely(__pyx_t_11 < 0)) __PYX_ERR(0, 373, __pyx_L15_error)
           __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
           if (__pyx_t_11) {
 
             __Pyx_XDECREF(__pyx_r);
             __pyx_r = Py_None; __Pyx_INCREF(Py_None);
             goto __pyx_L19_try_return;
 
@@ -7114,52 +7271,52 @@
             __Pyx_PyThreadState_assign
             __Pyx_ExceptionSave(&__pyx_t_13, &__pyx_t_14, &__pyx_t_15);
             __Pyx_XGOTREF(__pyx_t_13);
             __Pyx_XGOTREF(__pyx_t_14);
             __Pyx_XGOTREF(__pyx_t_15);
             /*try:*/ {
 
-              __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_json); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 375, __pyx_L22_error)
+              __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_json); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 376, __pyx_L22_error)
               __Pyx_GOTREF(__pyx_t_9);
-              __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_9, __pyx_n_s_loads); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 375, __pyx_L22_error)
+              __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_9, __pyx_n_s_loads); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 376, __pyx_L22_error)
               __Pyx_GOTREF(__pyx_t_4);
               __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-              __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_v_fp, __pyx_n_s_read); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 375, __pyx_L22_error)
+              __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_v_fp, __pyx_n_s_read); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 376, __pyx_L22_error)
               __Pyx_GOTREF(__pyx_t_8);
               __pyx_t_10 = NULL;
               if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_8))) {
                 __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_8);
                 if (likely(__pyx_t_10)) {
                   PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_8);
                   __Pyx_INCREF(__pyx_t_10);
                   __Pyx_INCREF(function);
                   __Pyx_DECREF_SET(__pyx_t_8, function);
                 }
               }
               __pyx_t_6 = (__pyx_t_10) ? __Pyx_PyObject_CallOneArg(__pyx_t_8, __pyx_t_10) : __Pyx_PyObject_CallNoArg(__pyx_t_8);
               __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
-              if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 375, __pyx_L22_error)
+              if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 376, __pyx_L22_error)
               __Pyx_GOTREF(__pyx_t_6);
               __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-              __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_decode); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 375, __pyx_L22_error)
+              __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_decode); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 376, __pyx_L22_error)
               __Pyx_GOTREF(__pyx_t_8);
               __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
               __pyx_t_6 = NULL;
               if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_8))) {
                 __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_8);
                 if (likely(__pyx_t_6)) {
                   PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_8);
                   __Pyx_INCREF(__pyx_t_6);
                   __Pyx_INCREF(function);
                   __Pyx_DECREF_SET(__pyx_t_8, function);
                 }
               }
               __pyx_t_9 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_8, __pyx_t_6, __pyx_kp_u_utf_8) : __Pyx_PyObject_CallOneArg(__pyx_t_8, __pyx_kp_u_utf_8);
               __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-              if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 375, __pyx_L22_error)
+              if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 376, __pyx_L22_error)
               __Pyx_GOTREF(__pyx_t_9);
               __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
               __pyx_t_8 = NULL;
               if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
                 __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_4);
                 if (likely(__pyx_t_8)) {
                   PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
@@ -7167,15 +7324,15 @@
                   __Pyx_INCREF(function);
                   __Pyx_DECREF_SET(__pyx_t_4, function);
                 }
               }
               __pyx_t_5 = (__pyx_t_8) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_8, __pyx_t_9) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_9);
               __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
               __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-              if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 375, __pyx_L22_error)
+              if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 376, __pyx_L22_error)
               __Pyx_GOTREF(__pyx_t_5);
               __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
               __Pyx_DECREF_SET(__pyx_v_data, __pyx_t_5);
               __pyx_t_5 = 0;
 
             }
             __Pyx_XDECREF(__pyx_t_13); __pyx_t_13 = 0;
@@ -7187,56 +7344,56 @@
             __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
             __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
             __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
             __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
             __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
 
             __Pyx_ErrFetch(&__pyx_t_5, &__pyx_t_4, &__pyx_t_9);
-            __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_json); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 376, __pyx_L24_except_error)
+            __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_json); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 377, __pyx_L24_except_error)
             __Pyx_GOTREF(__pyx_t_8);
-            __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_JSONDecodeError); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 376, __pyx_L24_except_error)
+            __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_JSONDecodeError); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 377, __pyx_L24_except_error)
             __Pyx_GOTREF(__pyx_t_6);
             __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
             __pyx_t_7 = __Pyx_PyErr_GivenExceptionMatches(__pyx_t_5, __pyx_t_6);
             __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
             __Pyx_ErrRestore(__pyx_t_5, __pyx_t_4, __pyx_t_9);
             __pyx_t_5 = 0; __pyx_t_4 = 0; __pyx_t_9 = 0;
             if (__pyx_t_7) {
               __Pyx_AddTraceback("tutorlicense.cmd.make_unverified_request", __pyx_clineno, __pyx_lineno, __pyx_filename);
-              if (__Pyx_GetException(&__pyx_t_9, &__pyx_t_4, &__pyx_t_5) < 0) __PYX_ERR(0, 376, __pyx_L24_except_error)
+              if (__Pyx_GetException(&__pyx_t_9, &__pyx_t_4, &__pyx_t_5) < 0) __PYX_ERR(0, 377, __pyx_L24_except_error)
               __Pyx_GOTREF(__pyx_t_9);
               __Pyx_GOTREF(__pyx_t_4);
               __Pyx_GOTREF(__pyx_t_5);
 
-              __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_fp, __pyx_n_s_status); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 377, __pyx_L24_except_error)
+              __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_fp, __pyx_n_s_status); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 378, __pyx_L24_except_error)
               __Pyx_GOTREF(__pyx_t_6);
-              __pyx_t_8 = __Pyx_PyObject_FormatSimple(__pyx_t_6, __pyx_empty_unicode); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 377, __pyx_L24_except_error)
+              __pyx_t_8 = __Pyx_PyObject_FormatSimple(__pyx_t_6, __pyx_empty_unicode); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 378, __pyx_L24_except_error)
               __Pyx_GOTREF(__pyx_t_8);
               __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-              __pyx_t_6 = __Pyx_PyUnicode_Concat(__pyx_kp_u_ERROR_Could_not_parse_upstream_s, __pyx_t_8); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 377, __pyx_L24_except_error)
+              __pyx_t_6 = __Pyx_PyUnicode_Concat(__pyx_kp_u_ERROR_Could_not_parse_upstream_s, __pyx_t_8); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 378, __pyx_L24_except_error)
               __Pyx_GOTREF(__pyx_t_6);
               __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
               __pyx_v_message = ((PyObject*)__pyx_t_6);
               __pyx_t_6 = 0;
 
-              __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_fail); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 378, __pyx_L24_except_error)
+              __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_fail); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 379, __pyx_L24_except_error)
               __Pyx_GOTREF(__pyx_t_8);
               __pyx_t_10 = NULL;
               if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_8))) {
                 __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_8);
                 if (likely(__pyx_t_10)) {
                   PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_8);
                   __Pyx_INCREF(__pyx_t_10);
                   __Pyx_INCREF(function);
                   __Pyx_DECREF_SET(__pyx_t_8, function);
                 }
               }
               __pyx_t_6 = (__pyx_t_10) ? __Pyx_PyObject_Call2Args(__pyx_t_8, __pyx_t_10, __pyx_v_message) : __Pyx_PyObject_CallOneArg(__pyx_t_8, __pyx_v_message);
               __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
-              if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 378, __pyx_L24_except_error)
+              if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 379, __pyx_L24_except_error)
               __Pyx_GOTREF(__pyx_t_6);
               __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
               __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
               __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
               __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
               __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
               goto __pyx_L23_exception_handled;
@@ -7267,36 +7424,36 @@
         __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
         __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
         __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
         __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
         __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
         /*except:*/ {
           __Pyx_AddTraceback("tutorlicense.cmd.make_unverified_request", __pyx_clineno, __pyx_lineno, __pyx_filename);
-          if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_4, &__pyx_t_9) < 0) __PYX_ERR(0, 371, __pyx_L17_except_error)
+          if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_4, &__pyx_t_9) < 0) __PYX_ERR(0, 372, __pyx_L17_except_error)
           __Pyx_GOTREF(__pyx_t_5);
           __Pyx_GOTREF(__pyx_t_4);
           __Pyx_GOTREF(__pyx_t_9);
-          __pyx_t_6 = PyTuple_Pack(3, __pyx_t_5, __pyx_t_4, __pyx_t_9); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 371, __pyx_L17_except_error)
+          __pyx_t_6 = PyTuple_Pack(3, __pyx_t_5, __pyx_t_4, __pyx_t_9); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 372, __pyx_L17_except_error)
           __Pyx_GOTREF(__pyx_t_6);
           __pyx_t_15 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_6, NULL);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
           __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-          if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 371, __pyx_L17_except_error)
+          if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 372, __pyx_L17_except_error)
           __Pyx_GOTREF(__pyx_t_15);
           __pyx_t_11 = __Pyx_PyObject_IsTrue(__pyx_t_15);
           __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
-          if (__pyx_t_11 < 0) __PYX_ERR(0, 371, __pyx_L17_except_error)
+          if (__pyx_t_11 < 0) __PYX_ERR(0, 372, __pyx_L17_except_error)
           __pyx_t_16 = ((!(__pyx_t_11 != 0)) != 0);
           if (__pyx_t_16) {
             __Pyx_GIVEREF(__pyx_t_5);
             __Pyx_GIVEREF(__pyx_t_4);
             __Pyx_XGIVEREF(__pyx_t_9);
             __Pyx_ErrRestoreWithState(__pyx_t_5, __pyx_t_4, __pyx_t_9);
             __pyx_t_5 = 0; __pyx_t_4 = 0; __pyx_t_9 = 0; 
-            __PYX_ERR(0, 371, __pyx_L17_except_error)
+            __PYX_ERR(0, 372, __pyx_L17_except_error)
           }
           __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
           __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
           __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
           goto __pyx_L16_exception_handled;
         }
         __pyx_L17_except_error:;
@@ -7320,27 +7477,27 @@
       }
     }
     /*finally:*/ {
       /*normal exit:*/{
         if (__pyx_t_3) {
           __pyx_t_12 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_tuple__11, NULL);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-          if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 371, __pyx_L1_error)
+          if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 372, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_12);
           __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
         }
         goto __pyx_L14;
       }
       __pyx_L12_return: {
         __pyx_t_12 = __pyx_r;
         __pyx_r = 0;
         if (__pyx_t_3) {
           __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_tuple__11, NULL);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-          if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 371, __pyx_L1_error)
+          if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 372, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_1);
           __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         }
         __pyx_r = __pyx_t_12;
         __pyx_t_12 = 0;
         goto __pyx_L0;
       }
@@ -7349,114 +7506,114 @@
     goto __pyx_L33;
     __pyx_L11_error:;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L1_error;
     __pyx_L33:;
   }
 
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_data, __pyx_n_s_get); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 380, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_data, __pyx_n_s_get); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 381, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_5 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
       __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_4, function);
     }
   }
   __pyx_t_9 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, __pyx_n_u_errors) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_n_u_errors);
   __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 380, __pyx_L1_error)
+  if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 381, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_16 = __Pyx_PyObject_IsTrue(__pyx_t_9); if (unlikely(__pyx_t_16 < 0)) __PYX_ERR(0, 380, __pyx_L1_error)
+  __pyx_t_16 = __Pyx_PyObject_IsTrue(__pyx_t_9); if (unlikely(__pyx_t_16 < 0)) __PYX_ERR(0, 381, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
   if (__pyx_t_16) {
 
-    __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_fail); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 381, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_fail); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 382, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
     { /* enter inner scope */
-      __pyx_t_4 = PyList_New(0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 381, __pyx_L37_error)
+      __pyx_t_4 = PyList_New(0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 382, __pyx_L37_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_5 = __Pyx_PyObject_Dict_GetItem(__pyx_v_data, __pyx_n_u_errors); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 381, __pyx_L37_error)
+      __pyx_t_5 = __Pyx_PyObject_Dict_GetItem(__pyx_v_data, __pyx_n_u_errors); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 382, __pyx_L37_error)
       __Pyx_GOTREF(__pyx_t_5);
       if (likely(PyList_CheckExact(__pyx_t_5)) || PyTuple_CheckExact(__pyx_t_5)) {
         __pyx_t_6 = __pyx_t_5; __Pyx_INCREF(__pyx_t_6); __pyx_t_17 = 0;
         __pyx_t_18 = NULL;
       } else {
-        __pyx_t_17 = -1; __pyx_t_6 = PyObject_GetIter(__pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 381, __pyx_L37_error)
+        __pyx_t_17 = -1; __pyx_t_6 = PyObject_GetIter(__pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 382, __pyx_L37_error)
         __Pyx_GOTREF(__pyx_t_6);
-        __pyx_t_18 = Py_TYPE(__pyx_t_6)->tp_iternext; if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 381, __pyx_L37_error)
+        __pyx_t_18 = Py_TYPE(__pyx_t_6)->tp_iternext; if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 382, __pyx_L37_error)
       }
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       for (;;) {
         if (likely(!__pyx_t_18)) {
           if (likely(PyList_CheckExact(__pyx_t_6))) {
             if (__pyx_t_17 >= PyList_GET_SIZE(__pyx_t_6)) break;
             #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-            __pyx_t_5 = PyList_GET_ITEM(__pyx_t_6, __pyx_t_17); __Pyx_INCREF(__pyx_t_5); __pyx_t_17++; if (unlikely(0 < 0)) __PYX_ERR(0, 381, __pyx_L37_error)
+            __pyx_t_5 = PyList_GET_ITEM(__pyx_t_6, __pyx_t_17); __Pyx_INCREF(__pyx_t_5); __pyx_t_17++; if (unlikely(0 < 0)) __PYX_ERR(0, 382, __pyx_L37_error)
             #else
-            __pyx_t_5 = PySequence_ITEM(__pyx_t_6, __pyx_t_17); __pyx_t_17++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 381, __pyx_L37_error)
+            __pyx_t_5 = PySequence_ITEM(__pyx_t_6, __pyx_t_17); __pyx_t_17++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 382, __pyx_L37_error)
             __Pyx_GOTREF(__pyx_t_5);
             #endif
           } else {
             if (__pyx_t_17 >= PyTuple_GET_SIZE(__pyx_t_6)) break;
             #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-            __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_6, __pyx_t_17); __Pyx_INCREF(__pyx_t_5); __pyx_t_17++; if (unlikely(0 < 0)) __PYX_ERR(0, 381, __pyx_L37_error)
+            __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_6, __pyx_t_17); __Pyx_INCREF(__pyx_t_5); __pyx_t_17++; if (unlikely(0 < 0)) __PYX_ERR(0, 382, __pyx_L37_error)
             #else
-            __pyx_t_5 = PySequence_ITEM(__pyx_t_6, __pyx_t_17); __pyx_t_17++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 381, __pyx_L37_error)
+            __pyx_t_5 = PySequence_ITEM(__pyx_t_6, __pyx_t_17); __pyx_t_17++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 382, __pyx_L37_error)
             __Pyx_GOTREF(__pyx_t_5);
             #endif
           }
         } else {
           __pyx_t_5 = __pyx_t_18(__pyx_t_6);
           if (unlikely(!__pyx_t_5)) {
             PyObject* exc_type = PyErr_Occurred();
             if (exc_type) {
               if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-              else __PYX_ERR(0, 381, __pyx_L37_error)
+              else __PYX_ERR(0, 382, __pyx_L37_error)
             }
             break;
           }
           __Pyx_GOTREF(__pyx_t_5);
         }
         __Pyx_XDECREF_SET(__pyx_7genexpr__pyx_v_error, __pyx_t_5);
         __pyx_t_5 = 0;
-        __pyx_t_5 = __Pyx_PyObject_Dict_GetItem(__pyx_7genexpr__pyx_v_error, __pyx_n_u_message); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 381, __pyx_L37_error)
+        __pyx_t_5 = __Pyx_PyObject_Dict_GetItem(__pyx_7genexpr__pyx_v_error, __pyx_n_u_message); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 382, __pyx_L37_error)
         __Pyx_GOTREF(__pyx_t_5);
-        __pyx_t_8 = PyNumber_Add(__pyx_kp_u_ERROR, __pyx_t_5); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 381, __pyx_L37_error)
+        __pyx_t_8 = PyNumber_Add(__pyx_kp_u_ERROR, __pyx_t_5); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 382, __pyx_L37_error)
         __Pyx_GOTREF(__pyx_t_8);
         __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-        if (unlikely(__Pyx_ListComp_Append(__pyx_t_4, (PyObject*)__pyx_t_8))) __PYX_ERR(0, 381, __pyx_L37_error)
+        if (unlikely(__Pyx_ListComp_Append(__pyx_t_4, (PyObject*)__pyx_t_8))) __PYX_ERR(0, 382, __pyx_L37_error)
         __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       }
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       __Pyx_XDECREF(__pyx_7genexpr__pyx_v_error); __pyx_7genexpr__pyx_v_error = 0;
       goto __pyx_L40_exit_scope;
       __pyx_L37_error:;
       __Pyx_XDECREF(__pyx_7genexpr__pyx_v_error); __pyx_7genexpr__pyx_v_error = 0;
       goto __pyx_L1_error;
       __pyx_L40_exit_scope:;
     } /* exit inner scope */
-    __pyx_t_6 = PySequence_Tuple(__pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 381, __pyx_L1_error)
+    __pyx_t_6 = PySequence_Tuple(__pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 382, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_9, __pyx_t_6, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 381, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_9, __pyx_t_6, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 382, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
   }
 
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_data, __pyx_n_s_get); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 383, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_data, __pyx_n_s_get); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 384, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_9 = PyList_New(0); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 383, __pyx_L1_error)
+  __pyx_t_9 = PyList_New(0); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 384, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
   __pyx_t_8 = NULL;
   __pyx_t_7 = 0;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_6))) {
     __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_6);
     if (likely(__pyx_t_8)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
@@ -7465,107 +7622,107 @@
       __Pyx_DECREF_SET(__pyx_t_6, function);
       __pyx_t_7 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_6)) {
     PyObject *__pyx_temp[3] = {__pyx_t_8, __pyx_n_u_warnings, __pyx_t_9};
-    __pyx_t_4 = __Pyx_PyFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 383, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 384, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_6)) {
     PyObject *__pyx_temp[3] = {__pyx_t_8, __pyx_n_u_warnings, __pyx_t_9};
-    __pyx_t_4 = __Pyx_PyCFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 383, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyCFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 384, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
   } else
   #endif
   {
-    __pyx_t_5 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 383, __pyx_L1_error)
+    __pyx_t_5 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 384, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     if (__pyx_t_8) {
       __Pyx_GIVEREF(__pyx_t_8); PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_8); __pyx_t_8 = NULL;
     }
     __Pyx_INCREF(__pyx_n_u_warnings);
     __Pyx_GIVEREF(__pyx_n_u_warnings);
     PyTuple_SET_ITEM(__pyx_t_5, 0+__pyx_t_7, __pyx_n_u_warnings);
     __Pyx_GIVEREF(__pyx_t_9);
     PyTuple_SET_ITEM(__pyx_t_5, 1+__pyx_t_7, __pyx_t_9);
     __pyx_t_9 = 0;
-    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_5, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 383, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_5, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 384, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   }
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   if (likely(PyList_CheckExact(__pyx_t_4)) || PyTuple_CheckExact(__pyx_t_4)) {
     __pyx_t_6 = __pyx_t_4; __Pyx_INCREF(__pyx_t_6); __pyx_t_17 = 0;
     __pyx_t_18 = NULL;
   } else {
-    __pyx_t_17 = -1; __pyx_t_6 = PyObject_GetIter(__pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 383, __pyx_L1_error)
+    __pyx_t_17 = -1; __pyx_t_6 = PyObject_GetIter(__pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 384, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_18 = Py_TYPE(__pyx_t_6)->tp_iternext; if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 383, __pyx_L1_error)
+    __pyx_t_18 = Py_TYPE(__pyx_t_6)->tp_iternext; if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 384, __pyx_L1_error)
   }
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   for (;;) {
     if (likely(!__pyx_t_18)) {
       if (likely(PyList_CheckExact(__pyx_t_6))) {
         if (__pyx_t_17 >= PyList_GET_SIZE(__pyx_t_6)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_4 = PyList_GET_ITEM(__pyx_t_6, __pyx_t_17); __Pyx_INCREF(__pyx_t_4); __pyx_t_17++; if (unlikely(0 < 0)) __PYX_ERR(0, 383, __pyx_L1_error)
+        __pyx_t_4 = PyList_GET_ITEM(__pyx_t_6, __pyx_t_17); __Pyx_INCREF(__pyx_t_4); __pyx_t_17++; if (unlikely(0 < 0)) __PYX_ERR(0, 384, __pyx_L1_error)
         #else
-        __pyx_t_4 = PySequence_ITEM(__pyx_t_6, __pyx_t_17); __pyx_t_17++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 383, __pyx_L1_error)
+        __pyx_t_4 = PySequence_ITEM(__pyx_t_6, __pyx_t_17); __pyx_t_17++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 384, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         #endif
       } else {
         if (__pyx_t_17 >= PyTuple_GET_SIZE(__pyx_t_6)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_4 = PyTuple_GET_ITEM(__pyx_t_6, __pyx_t_17); __Pyx_INCREF(__pyx_t_4); __pyx_t_17++; if (unlikely(0 < 0)) __PYX_ERR(0, 383, __pyx_L1_error)
+        __pyx_t_4 = PyTuple_GET_ITEM(__pyx_t_6, __pyx_t_17); __Pyx_INCREF(__pyx_t_4); __pyx_t_17++; if (unlikely(0 < 0)) __PYX_ERR(0, 384, __pyx_L1_error)
         #else
-        __pyx_t_4 = PySequence_ITEM(__pyx_t_6, __pyx_t_17); __pyx_t_17++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 383, __pyx_L1_error)
+        __pyx_t_4 = PySequence_ITEM(__pyx_t_6, __pyx_t_17); __pyx_t_17++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 384, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         #endif
       }
     } else {
       __pyx_t_4 = __pyx_t_18(__pyx_t_6);
       if (unlikely(!__pyx_t_4)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(0, 383, __pyx_L1_error)
+          else __PYX_ERR(0, 384, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_4);
     }
     __Pyx_XDECREF_SET(__pyx_v_warning, __pyx_t_4);
     __pyx_t_4 = 0;
 
-    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_log_warning); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 384, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_log_warning); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 385, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_9 = __Pyx_PyObject_Dict_GetItem(__pyx_v_warning, __pyx_n_u_message); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 384, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyObject_Dict_GetItem(__pyx_v_warning, __pyx_n_u_message); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 385, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
     __pyx_t_8 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
       __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_5);
       if (likely(__pyx_t_8)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
         __Pyx_INCREF(__pyx_t_8);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_5, function);
       }
     }
     __pyx_t_4 = (__pyx_t_8) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_8, __pyx_t_9) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_t_9);
     __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
     __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 384, __pyx_L1_error)
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 385, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
   }
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
@@ -7647,43 +7804,43 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_self)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_req)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("http_error_default", 1, 6, 6, 1); __PYX_ERR(0, 390, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("http_error_default", 1, 6, 6, 1); __PYX_ERR(0, 391, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_fp)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("http_error_default", 1, 6, 6, 2); __PYX_ERR(0, 390, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("http_error_default", 1, 6, 6, 2); __PYX_ERR(0, 391, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_code)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("http_error_default", 1, 6, 6, 3); __PYX_ERR(0, 390, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("http_error_default", 1, 6, 6, 3); __PYX_ERR(0, 391, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  4:
         if (likely((values[4] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_errmsg)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("http_error_default", 1, 6, 6, 4); __PYX_ERR(0, 390, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("http_error_default", 1, 6, 6, 4); __PYX_ERR(0, 391, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  5:
         if (likely((values[5] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_hdrs)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("http_error_default", 1, 6, 6, 5); __PYX_ERR(0, 390, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("http_error_default", 1, 6, 6, 5); __PYX_ERR(0, 391, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "http_error_default") < 0)) __PYX_ERR(0, 390, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "http_error_default") < 0)) __PYX_ERR(0, 391, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 6) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
@@ -7696,15 +7853,15 @@
     __pyx_v_fp = values[2];
     __pyx_v_code = values[3];
     __pyx_v__errmsg = values[4];
     __pyx_v_hdrs = values[5];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("http_error_default", 1, 6, 6, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 390, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("http_error_default", 1, 6, 6, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 391, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("tutorlicense.cmd.HTTPErrorHandler.http_error_default", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_12tutorlicense_3cmd_16HTTPErrorHandler_http_error_default(__pyx_self, __pyx_v_self, __pyx_v_req, __pyx_v_fp, __pyx_v_code, __pyx_v__errmsg, __pyx_v_hdrs);
 
@@ -7724,23 +7881,23 @@
   PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("http_error_default", 0);
 
   __Pyx_XDECREF(__pyx_r);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_urllib); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 391, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_urllib); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 392, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_request); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 391, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_request); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 392, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_addinfourl); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 391, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_addinfourl); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 392, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_req, __pyx_n_s_full_url); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 391, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_req, __pyx_n_s_full_url); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 392, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_4 = NULL;
   __pyx_t_5 = 0;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -7749,31 +7906,31 @@
       __Pyx_DECREF_SET(__pyx_t_2, function);
       __pyx_t_5 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[5] = {__pyx_t_4, __pyx_v_fp, __pyx_v_hdrs, __pyx_t_3, __pyx_v_code};
-    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_5, 4+__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 391, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_5, 4+__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 392, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[5] = {__pyx_t_4, __pyx_v_fp, __pyx_v_hdrs, __pyx_t_3, __pyx_v_code};
-    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_5, 4+__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 391, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_5, 4+__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 392, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   } else
   #endif
   {
-    __pyx_t_6 = PyTuple_New(4+__pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 391, __pyx_L1_error)
+    __pyx_t_6 = PyTuple_New(4+__pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 392, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     if (__pyx_t_4) {
       __Pyx_GIVEREF(__pyx_t_4); PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_4); __pyx_t_4 = NULL;
     }
     __Pyx_INCREF(__pyx_v_fp);
     __Pyx_GIVEREF(__pyx_v_fp);
     PyTuple_SET_ITEM(__pyx_t_6, 0+__pyx_t_5, __pyx_v_fp);
@@ -7782,15 +7939,15 @@
     PyTuple_SET_ITEM(__pyx_t_6, 1+__pyx_t_5, __pyx_v_hdrs);
     __Pyx_GIVEREF(__pyx_t_3);
     PyTuple_SET_ITEM(__pyx_t_6, 2+__pyx_t_5, __pyx_t_3);
     __Pyx_INCREF(__pyx_v_code);
     __Pyx_GIVEREF(__pyx_v_code);
     PyTuple_SET_ITEM(__pyx_t_6, 3+__pyx_t_5, __pyx_v_code);
     __pyx_t_3 = 0;
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_6, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 391, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_6, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 392, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
@@ -8086,14 +8243,15 @@
   {&__pyx_n_s_obj, __pyx_k_obj, sizeof(__pyx_k_obj), 0, 0, 1, 1},
   {&__pyx_n_u_olive, __pyx_k_olive, sizeof(__pyx_k_olive), 0, 1, 0, 1},
   {&__pyx_n_s_open, __pyx_k_open, sizeof(__pyx_k_open), 0, 0, 1, 1},
   {&__pyx_n_s_opener, __pyx_k_opener, sizeof(__pyx_k_opener), 0, 0, 1, 1},
   {&__pyx_n_s_option, __pyx_k_option, sizeof(__pyx_k_option), 0, 0, 1, 1},
   {&__pyx_n_s_os, __pyx_k_os, sizeof(__pyx_k_os), 0, 0, 1, 1},
   {&__pyx_kp_u_p, __pyx_k_p, sizeof(__pyx_k_p), 0, 1, 0, 0},
+  {&__pyx_n_u_palm, __pyx_k_palm, sizeof(__pyx_k_palm), 0, 1, 0, 1},
   {&__pyx_n_s_parse, __pyx_k_parse, sizeof(__pyx_k_parse), 0, 0, 1, 1},
   {&__pyx_n_s_pass_context, __pyx_k_pass_context, sizeof(__pyx_k_pass_context), 0, 0, 1, 1},
   {&__pyx_n_s_pass_obj, __pyx_k_pass_obj, sizeof(__pyx_k_pass_obj), 0, 0, 1, 1},
   {&__pyx_n_s_path, __pyx_k_path, sizeof(__pyx_k_path), 0, 0, 1, 1},
   {&__pyx_n_u_pip, __pyx_k_pip, sizeof(__pyx_k_pip), 0, 1, 0, 1},
   {&__pyx_n_u_pip3, __pyx_k_pip3, sizeof(__pyx_k_pip3), 0, 1, 0, 1},
   {&__pyx_kp_u_pip3_or_pip_must_be_installed_i, __pyx_k_pip3_or_pip_must_be_installed_i, sizeof(__pyx_k_pip3_or_pip_must_be_installed_i), 0, 1, 0, 0},
@@ -8171,18 +8329,18 @@
   {&__pyx_n_u_yellow, __pyx_k_yellow, sizeof(__pyx_k_yellow), 0, 1, 0, 1},
   {&__pyx_n_s_yes, __pyx_k_yes, sizeof(__pyx_k_yes), 0, 0, 1, 1},
   {&__pyx_kp_u_yes_2, __pyx_k_yes_2, sizeof(__pyx_k_yes_2), 0, 1, 0, 0},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
   __pyx_builtin_print = __Pyx_GetBuiltinName(__pyx_n_s_print); if (!__pyx_builtin_print) __PYX_ERR(0, 54, __pyx_L1_error)
-  __pyx_builtin_open = __Pyx_GetBuiltinName(__pyx_n_s_open); if (!__pyx_builtin_open) __PYX_ERR(0, 236, __pyx_L1_error)
-  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 278, __pyx_L1_error)
-  __pyx_builtin_AttributeError = __Pyx_GetBuiltinName(__pyx_n_s_AttributeError); if (!__pyx_builtin_AttributeError) __PYX_ERR(0, 279, __pyx_L1_error)
-  __pyx_builtin_KeyError = __Pyx_GetBuiltinName(__pyx_n_s_KeyError); if (!__pyx_builtin_KeyError) __PYX_ERR(0, 279, __pyx_L1_error)
+  __pyx_builtin_open = __Pyx_GetBuiltinName(__pyx_n_s_open); if (!__pyx_builtin_open) __PYX_ERR(0, 237, __pyx_L1_error)
+  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 279, __pyx_L1_error)
+  __pyx_builtin_AttributeError = __Pyx_GetBuiltinName(__pyx_n_s_AttributeError); if (!__pyx_builtin_AttributeError) __PYX_ERR(0, 280, __pyx_L1_error)
+  __pyx_builtin_KeyError = __Pyx_GetBuiltinName(__pyx_n_s_KeyError); if (!__pyx_builtin_KeyError) __PYX_ERR(0, 280, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
@@ -8196,27 +8354,27 @@
   __Pyx_GOTREF(__pyx_tuple__5);
   __Pyx_GIVEREF(__pyx_tuple__5);
 
   __pyx_tuple__10 = PyTuple_Pack(1, __pyx_kp_u__9); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(0, 216, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__10);
   __Pyx_GIVEREF(__pyx_tuple__10);
 
-  __pyx_tuple__11 = PyTuple_Pack(3, Py_None, Py_None, Py_None); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(0, 236, __pyx_L1_error)
+  __pyx_tuple__11 = PyTuple_Pack(3, Py_None, Py_None, Py_None); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(0, 237, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__11);
   __Pyx_GIVEREF(__pyx_tuple__11);
 
-  __pyx_tuple__12 = PyTuple_Pack(2, __pyx_n_s_uuid, __pyx_n_s_node); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(0, 320, __pyx_L1_error)
+  __pyx_tuple__12 = PyTuple_Pack(2, __pyx_n_s_uuid, __pyx_n_s_node); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(0, 321, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__12);
   __Pyx_GIVEREF(__pyx_tuple__12);
-  __pyx_codeobj__13 = (PyObject*)__Pyx_PyCode_New(0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__12, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_tutorlicense_cmd_pyx, __pyx_n_s_getnode, 320, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__13)) __PYX_ERR(0, 320, __pyx_L1_error)
+  __pyx_codeobj__13 = (PyObject*)__Pyx_PyCode_New(0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__12, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_tutorlicense_cmd_pyx, __pyx_n_s_getnode, 321, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__13)) __PYX_ERR(0, 321, __pyx_L1_error)
 
-  __pyx_tuple__14 = PyTuple_Pack(12, __pyx_n_s_message, __pyx_n_s_AES, __pyx_n_s_PKCS1_OAEP, __pyx_n_s_RSA, __pyx_n_s_get_random_bytes, __pyx_n_s_recipient_key, __pyx_n_s_session_key, __pyx_n_s_cipher_rsa, __pyx_n_s_enc_session_key, __pyx_n_s_cipher_aes, __pyx_n_s_ciphertext, __pyx_n_s_tag); if (unlikely(!__pyx_tuple__14)) __PYX_ERR(0, 334, __pyx_L1_error)
+  __pyx_tuple__14 = PyTuple_Pack(12, __pyx_n_s_message, __pyx_n_s_AES, __pyx_n_s_PKCS1_OAEP, __pyx_n_s_RSA, __pyx_n_s_get_random_bytes, __pyx_n_s_recipient_key, __pyx_n_s_session_key, __pyx_n_s_cipher_rsa, __pyx_n_s_enc_session_key, __pyx_n_s_cipher_aes, __pyx_n_s_ciphertext, __pyx_n_s_tag); if (unlikely(!__pyx_tuple__14)) __PYX_ERR(0, 335, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__14);
   __Pyx_GIVEREF(__pyx_tuple__14);
-  __pyx_codeobj__15 = (PyObject*)__Pyx_PyCode_New(1, 0, 12, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__14, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_tutorlicense_cmd_pyx, __pyx_n_s_encrypt, 334, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__15)) __PYX_ERR(0, 334, __pyx_L1_error)
+  __pyx_codeobj__15 = (PyObject*)__Pyx_PyCode_New(1, 0, 12, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__14, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_tutorlicense_cmd_pyx, __pyx_n_s_encrypt, 335, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__15)) __PYX_ERR(0, 335, __pyx_L1_error)
 
   __pyx_tuple__16 = PyTuple_Pack(1, __pyx_n_u_tutorlicense); if (unlikely(!__pyx_tuple__16)) __PYX_ERR(0, 28, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__16);
   __Pyx_GIVEREF(__pyx_tuple__16);
 
   __pyx_tuple__17 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_license_path); if (unlikely(!__pyx_tuple__17)) __PYX_ERR(0, 33, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__17);
@@ -8333,48 +8491,48 @@
   __pyx_codeobj__54 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__53, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_tutorlicense_cmd_pyx, __pyx_n_s_log_error, 208, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__54)) __PYX_ERR(0, 208, __pyx_L1_error)
 
   __pyx_tuple__55 = PyTuple_Pack(2, __pyx_n_s_major_version, __pyx_n_s_release_name); if (unlikely(!__pyx_tuple__55)) __PYX_ERR(0, 212, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__55);
   __Pyx_GIVEREF(__pyx_tuple__55);
   __pyx_codeobj__56 = (PyObject*)__Pyx_PyCode_New(0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__55, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_tutorlicense_cmd_pyx, __pyx_n_s_current_release_name, 212, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__56)) __PYX_ERR(0, 212, __pyx_L1_error)
 
-  __pyx_tuple__57 = PyTuple_Pack(2, __pyx_n_s_license_path, __pyx_n_s_f_2); if (unlikely(!__pyx_tuple__57)) __PYX_ERR(0, 232, __pyx_L1_error)
+  __pyx_tuple__57 = PyTuple_Pack(2, __pyx_n_s_license_path, __pyx_n_s_f_2); if (unlikely(!__pyx_tuple__57)) __PYX_ERR(0, 233, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__57);
   __Pyx_GIVEREF(__pyx_tuple__57);
-  __pyx_codeobj__58 = (PyObject*)__Pyx_PyCode_New(1, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__57, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_tutorlicense_cmd_pyx, __pyx_n_s_load_license, 232, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__58)) __PYX_ERR(0, 232, __pyx_L1_error)
+  __pyx_codeobj__58 = (PyObject*)__Pyx_PyCode_New(1, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__57, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_tutorlicense_cmd_pyx, __pyx_n_s_load_license, 233, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__58)) __PYX_ERR(0, 233, __pyx_L1_error)
 
-  __pyx_tuple__59 = PyTuple_Pack(6, __pyx_n_s_license_path, __pyx_n_s_licenseid, __pyx_n_s_data, __pyx_n_s_license_data, __pyx_n_s_license_directory, __pyx_n_s_f_2); if (unlikely(!__pyx_tuple__59)) __PYX_ERR(0, 240, __pyx_L1_error)
+  __pyx_tuple__59 = PyTuple_Pack(6, __pyx_n_s_license_path, __pyx_n_s_licenseid, __pyx_n_s_data, __pyx_n_s_license_data, __pyx_n_s_license_directory, __pyx_n_s_f_2); if (unlikely(!__pyx_tuple__59)) __PYX_ERR(0, 241, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__59);
   __Pyx_GIVEREF(__pyx_tuple__59);
-  __pyx_codeobj__60 = (PyObject*)__Pyx_PyCode_New(2, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__59, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_tutorlicense_cmd_pyx, __pyx_n_s_save_license, 240, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__60)) __PYX_ERR(0, 240, __pyx_L1_error)
+  __pyx_codeobj__60 = (PyObject*)__Pyx_PyCode_New(2, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__59, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_tutorlicense_cmd_pyx, __pyx_n_s_save_license, 241, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__60)) __PYX_ERR(0, 241, __pyx_L1_error)
 
-  __pyx_tuple__61 = PyTuple_Pack(14, __pyx_n_s_license_path, __pyx_n_s_endpoint, __pyx_n_s_data, __pyx_n_s_method, __pyx_n_s_license_data, __pyx_n_s_encoded_key, __pyx_n_s_encoded_signature, __pyx_n_s_key_2, __pyx_n_s_signature, __pyx_n_s_SHA256, __pyx_n_s_RSA, __pyx_n_s_Signer, __pyx_n_s_cipher, __pyx_n_s_digest); if (unlikely(!__pyx_tuple__61)) __PYX_ERR(0, 253, __pyx_L1_error)
+  __pyx_tuple__61 = PyTuple_Pack(14, __pyx_n_s_license_path, __pyx_n_s_endpoint, __pyx_n_s_data, __pyx_n_s_method, __pyx_n_s_license_data, __pyx_n_s_encoded_key, __pyx_n_s_encoded_signature, __pyx_n_s_key_2, __pyx_n_s_signature, __pyx_n_s_SHA256, __pyx_n_s_RSA, __pyx_n_s_Signer, __pyx_n_s_cipher, __pyx_n_s_digest); if (unlikely(!__pyx_tuple__61)) __PYX_ERR(0, 254, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__61);
   __Pyx_GIVEREF(__pyx_tuple__61);
-  __pyx_codeobj__62 = (PyObject*)__Pyx_PyCode_New(4, 0, 14, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__61, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_tutorlicense_cmd_pyx, __pyx_n_s_make_request, 253, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__62)) __PYX_ERR(0, 253, __pyx_L1_error)
+  __pyx_codeobj__62 = (PyObject*)__Pyx_PyCode_New(4, 0, 14, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__61, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_tutorlicense_cmd_pyx, __pyx_n_s_make_request, 254, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__62)) __PYX_ERR(0, 254, __pyx_L1_error)
 
-  __pyx_tuple__63 = PyTuple_Pack(17, __pyx_n_s_license_id, __pyx_n_s_endpoint, __pyx_n_s_data, __pyx_n_s_method, __pyx_n_s_uuid, __pyx_n_s_url, __pyx_n_s_getnode, __pyx_n_s_getnode, __pyx_n_s_encrypt, __pyx_n_s_encrypt, __pyx_n_s_fingerprint, __pyx_n_s_opener, __pyx_n_s_request, __pyx_n_s_fp, __pyx_n_s_message, __pyx_n_s_warning, __pyx_n_s_error); if (unlikely(!__pyx_tuple__63)) __PYX_ERR(0, 302, __pyx_L1_error)
+  __pyx_tuple__63 = PyTuple_Pack(17, __pyx_n_s_license_id, __pyx_n_s_endpoint, __pyx_n_s_data, __pyx_n_s_method, __pyx_n_s_uuid, __pyx_n_s_url, __pyx_n_s_getnode, __pyx_n_s_getnode, __pyx_n_s_encrypt, __pyx_n_s_encrypt, __pyx_n_s_fingerprint, __pyx_n_s_opener, __pyx_n_s_request, __pyx_n_s_fp, __pyx_n_s_message, __pyx_n_s_warning, __pyx_n_s_error); if (unlikely(!__pyx_tuple__63)) __PYX_ERR(0, 303, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__63);
   __Pyx_GIVEREF(__pyx_tuple__63);
-  __pyx_codeobj__64 = (PyObject*)__Pyx_PyCode_New(4, 0, 17, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__63, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_tutorlicense_cmd_pyx, __pyx_n_s_make_unverified_request, 302, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__64)) __PYX_ERR(0, 302, __pyx_L1_error)
+  __pyx_codeobj__64 = (PyObject*)__Pyx_PyCode_New(4, 0, 17, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__63, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_tutorlicense_cmd_pyx, __pyx_n_s_make_unverified_request, 303, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__64)) __PYX_ERR(0, 303, __pyx_L1_error)
 
-  __pyx_tuple__65 = PyTuple_Pack(6, __pyx_n_s_self, __pyx_n_s_req, __pyx_n_s_fp, __pyx_n_s_code, __pyx_n_s_errmsg, __pyx_n_s_hdrs); if (unlikely(!__pyx_tuple__65)) __PYX_ERR(0, 390, __pyx_L1_error)
+  __pyx_tuple__65 = PyTuple_Pack(6, __pyx_n_s_self, __pyx_n_s_req, __pyx_n_s_fp, __pyx_n_s_code, __pyx_n_s_errmsg, __pyx_n_s_hdrs); if (unlikely(!__pyx_tuple__65)) __PYX_ERR(0, 391, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__65);
   __Pyx_GIVEREF(__pyx_tuple__65);
-  __pyx_codeobj__66 = (PyObject*)__Pyx_PyCode_New(6, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__65, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_tutorlicense_cmd_pyx, __pyx_n_s_http_error_default, 390, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__66)) __PYX_ERR(0, 390, __pyx_L1_error)
+  __pyx_codeobj__66 = (PyObject*)__Pyx_PyCode_New(6, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__65, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_tutorlicense_cmd_pyx, __pyx_n_s_http_error_default, 391, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__66)) __PYX_ERR(0, 391, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
   __pyx_umethod_PyDict_Type_get.type = (PyObject*)&PyDict_Type;
-  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_1 = PyInt_FromLong(1); if (unlikely(!__pyx_int_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_9 = PyInt_FromLong(9); if (unlikely(!__pyx_int_9)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_10 = PyInt_FromLong(10); if (unlikely(!__pyx_int_10)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_11 = PyInt_FromLong(11); if (unlikely(!__pyx_int_11)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_12 = PyInt_FromLong(12); if (unlikely(!__pyx_int_12)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_13 = PyInt_FromLong(13); if (unlikely(!__pyx_int_13)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_14 = PyInt_FromLong(14); if (unlikely(!__pyx_int_14)) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -8599,19 +8757,17 @@
   if (__pyx_AsyncGen_init() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   #ifdef __Pyx_StopAsyncIteration_USED
   if (__pyx_StopAsyncIteration_init() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   /*--- Library function declarations ---*/
   /*--- Threads initialization code ---*/
-  #if defined(__PYX_FORCE_INIT_THREADS) && __PYX_FORCE_INIT_THREADS
-  #ifdef WITH_THREAD /* Python build with threading support? */
+  #if defined(WITH_THREAD) && PY_VERSION_HEX < 0x030700F0 && defined(__PYX_FORCE_INIT_THREADS) && __PYX_FORCE_INIT_THREADS
   PyEval_InitThreads();
   #endif
-  #endif
   /*--- Module creation code ---*/
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   __pyx_m = __pyx_pyinit_module;
   Py_INCREF(__pyx_m);
   #else
   #if PY_MAJOR_VERSION < 3
   __pyx_m = Py_InitModule4("cmd", __pyx_methods, 0, 0, PYTHON_API_VERSION); Py_XINCREF(__pyx_m);
@@ -8622,15 +8778,15 @@
   #endif
   __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_d);
   __pyx_b = PyImport_AddModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_b);
   __pyx_cython_runtime = PyImport_AddModule((char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_cython_runtime);
-  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Initialize various global constants etc. ---*/
   if (__Pyx_InitGlobals() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #if PY_MAJOR_VERSION < 3 && (__PYX_DEFAULT_STRING_ENCODING_IS_ASCII || __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT)
   if (__Pyx_init_sys_getdefaultencoding_params() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   if (__pyx_module_is_main_tutorlicense__cmd) {
     if (PyObject_SetAttr(__pyx_m, __pyx_n_s_name_2, __pyx_n_s_main) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -9352,60 +9508,60 @@
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
   __pyx_t_7 = PyCFunction_NewEx(&__pyx_mdef_12tutorlicense_3cmd_25current_release_name, NULL, __pyx_n_s_tutorlicense_cmd); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 212, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_current_release_name, __pyx_t_7) < 0) __PYX_ERR(0, 212, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  __pyx_t_7 = PyCFunction_NewEx(&__pyx_mdef_12tutorlicense_3cmd_27load_license, NULL, __pyx_n_s_tutorlicense_cmd); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 232, __pyx_L1_error)
+  __pyx_t_7 = PyCFunction_NewEx(&__pyx_mdef_12tutorlicense_3cmd_27load_license, NULL, __pyx_n_s_tutorlicense_cmd); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 233, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_load_license, __pyx_t_7) < 0) __PYX_ERR(0, 232, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_load_license, __pyx_t_7) < 0) __PYX_ERR(0, 233, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  __pyx_t_7 = PyCFunction_NewEx(&__pyx_mdef_12tutorlicense_3cmd_29save_license, NULL, __pyx_n_s_tutorlicense_cmd); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 240, __pyx_L1_error)
+  __pyx_t_7 = PyCFunction_NewEx(&__pyx_mdef_12tutorlicense_3cmd_29save_license, NULL, __pyx_n_s_tutorlicense_cmd); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 241, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_save_license, __pyx_t_7) < 0) __PYX_ERR(0, 240, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_save_license, __pyx_t_7) < 0) __PYX_ERR(0, 241, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  __pyx_t_7 = PyCFunction_NewEx(&__pyx_mdef_12tutorlicense_3cmd_31make_request, NULL, __pyx_n_s_tutorlicense_cmd); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 253, __pyx_L1_error)
+  __pyx_t_7 = PyCFunction_NewEx(&__pyx_mdef_12tutorlicense_3cmd_31make_request, NULL, __pyx_n_s_tutorlicense_cmd); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 254, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_make_request, __pyx_t_7) < 0) __PYX_ERR(0, 253, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_make_request, __pyx_t_7) < 0) __PYX_ERR(0, 254, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  __pyx_t_7 = PyCFunction_NewEx(&__pyx_mdef_12tutorlicense_3cmd_33make_unverified_request, NULL, __pyx_n_s_tutorlicense_cmd); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 302, __pyx_L1_error)
+  __pyx_t_7 = PyCFunction_NewEx(&__pyx_mdef_12tutorlicense_3cmd_33make_unverified_request, NULL, __pyx_n_s_tutorlicense_cmd); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 303, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_make_unverified_request, __pyx_t_7) < 0) __PYX_ERR(0, 302, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_make_unverified_request, __pyx_t_7) < 0) __PYX_ERR(0, 303, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_urllib); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 388, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_urllib); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 389, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_request); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 388, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_request); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 389, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_HTTPDefaultErrorHandler); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 388, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_HTTPDefaultErrorHandler); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 389, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 388, __pyx_L1_error)
+  __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 389, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_GIVEREF(__pyx_t_7);
   PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_7);
   __pyx_t_7 = 0;
-  __pyx_t_7 = __Pyx_CalculateMetaclass(NULL, __pyx_t_5); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 388, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_CalculateMetaclass(NULL, __pyx_t_5); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 389, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_3 = __Pyx_Py3MetaclassPrepare(__pyx_t_7, __pyx_t_5, __pyx_n_s_HTTPErrorHandler, __pyx_n_s_HTTPErrorHandler, (PyObject *) NULL, __pyx_n_s_tutorlicense_cmd, (PyObject *) NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 388, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_Py3MetaclassPrepare(__pyx_t_7, __pyx_t_5, __pyx_n_s_HTTPErrorHandler, __pyx_n_s_HTTPErrorHandler, (PyObject *) NULL, __pyx_n_s_tutorlicense_cmd, (PyObject *) NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 389, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
 
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_12tutorlicense_3cmd_16HTTPErrorHandler_1http_error_default, 0, __pyx_n_s_HTTPErrorHandler_http_error_defa, NULL, __pyx_n_s_tutorlicense_cmd, __pyx_d, ((PyObject *)__pyx_codeobj__66)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 390, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_12tutorlicense_3cmd_16HTTPErrorHandler_1http_error_default, 0, __pyx_n_s_HTTPErrorHandler_http_error_defa, NULL, __pyx_n_s_tutorlicense_cmd, __pyx_d, ((PyObject *)__pyx_codeobj__66)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 391, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_http_error_default, __pyx_t_2) < 0) __PYX_ERR(0, 390, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_http_error_default, __pyx_t_2) < 0) __PYX_ERR(0, 391, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  __pyx_t_2 = __Pyx_Py3ClassCreate(__pyx_t_7, __pyx_n_s_HTTPErrorHandler, __pyx_t_5, __pyx_t_3, NULL, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 388, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_Py3ClassCreate(__pyx_t_7, __pyx_n_s_HTTPErrorHandler, __pyx_t_5, __pyx_t_3, NULL, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 389, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_HTTPErrorHandler, __pyx_t_2) < 0) __PYX_ERR(0, 388, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_HTTPErrorHandler, __pyx_t_2) < 0) __PYX_ERR(0, 389, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   __pyx_t_5 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
@@ -9848,15 +10004,15 @@
 #endif
 #endif
 
 /* PyObjectCall */
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw) {
     PyObject *result;
-    ternaryfunc call = func->ob_type->tp_call;
+    ternaryfunc call = Py_TYPE(func)->tp_call;
     if (unlikely(!call))
         return PyObject_Call(func, arg, kw);
     if (unlikely(Py_EnterRecursiveCall((char*)" while calling a Python object")))
         return NULL;
     result = (*call)(func, arg, kw);
     Py_LeaveRecursiveCall();
     if (unlikely(!result) && unlikely(!PyErr_Occurred())) {
@@ -9935,15 +10091,15 @@
         return __Pyx_PyFunction_FastCall(func, &arg, 1);
     }
 #endif
     if (likely(PyCFunction_Check(func))) {
         if (likely(PyCFunction_GET_FLAGS(func) & METH_O)) {
             return __Pyx_PyObject_CallMethO(func, arg);
 #if CYTHON_FAST_PYCCALL
-        } else if (PyCFunction_GET_FLAGS(func) & METH_FASTCALL) {
+        } else if (__Pyx_PyFastCFunction_Check(func)) {
             return __Pyx_PyCFunction_FastCall(func, &arg, 1);
 #endif
         }
     }
     return __Pyx__PyObject_CallOneArg(func, arg);
 }
 #else
@@ -10023,15 +10179,15 @@
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func) {
 #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(func)) {
         return __Pyx_PyFunction_FastCall(func, NULL, 0);
     }
 #endif
-#ifdef __Pyx_CyFunction_USED
+#if defined(__Pyx_CyFunction_USED) && defined(NDEBUG)
     if (likely(PyCFunction_Check(func) || __Pyx_CyFunction_Check(func)))
 #else
     if (likely(PyCFunction_Check(func)))
 #endif
     {
         if (likely(PyCFunction_GET_FLAGS(func) & METH_NOARGS)) {
             return __Pyx_PyObject_CallMethO(func, NULL);
@@ -10281,19 +10437,19 @@
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_CallUnboundCMethod1(__Pyx_CachedCFunction* cfunc, PyObject* self, PyObject* arg) {
     if (likely(cfunc->func)) {
         int flag = cfunc->flag;
         if (flag == METH_O) {
             return (*(cfunc->func))(self, arg);
         } else if (PY_VERSION_HEX >= 0x030600B1 && flag == METH_FASTCALL) {
-            if (PY_VERSION_HEX >= 0x030700A0) {
+            #if PY_VERSION_HEX >= 0x030700A0
                 return (*(__Pyx_PyCFunctionFast)(void*)(PyCFunction)cfunc->func)(self, &arg, 1);
-            } else {
+            #else
                 return (*(__Pyx_PyCFunctionFastWithKeywords)(void*)(PyCFunction)cfunc->func)(self, &arg, 1, NULL);
-            }
+            #endif
         } else if (PY_VERSION_HEX >= 0x030700A0 && flag == (METH_FASTCALL | METH_KEYWORDS)) {
             return (*(__Pyx_PyCFunctionFastWithKeywords)(void*)(PyCFunction)cfunc->func)(self, &arg, 1, NULL);
         }
     }
     return __Pyx__CallUnboundCMethod1(cfunc, self, arg);
 }
 #endif
@@ -10619,18 +10775,16 @@
 
 /* UnpackItemEndCheck */
 static int __Pyx_IternextUnpackEndCheck(PyObject *retval, Py_ssize_t expected) {
     if (unlikely(retval)) {
         Py_DECREF(retval);
         __Pyx_RaiseTooManyValuesError(expected);
         return -1;
-    } else {
-        return __Pyx_IterFinish();
     }
-    return 0;
+    return __Pyx_IterFinish();
 }
 
 /* BytesEquals */
 static CYTHON_INLINE int __Pyx_PyBytes_Equals(PyObject* s1, PyObject* s2, int equals) {
 #if CYTHON_COMPILING_IN_PYPY
     return PyObject_RichCompareBool(s1, s2, equals);
 #else
@@ -10645,15 +10799,15 @@
         ps2 = PyBytes_AS_STRING(s2);
         if (ps1[0] != ps2[0]) {
             return (equals == Py_NE);
         } else if (length == 1) {
             return (equals == Py_EQ);
         } else {
             int result;
-#if CYTHON_USE_UNICODE_INTERNALS
+#if CYTHON_USE_UNICODE_INTERNALS && (PY_VERSION_HEX < 0x030B0000)
             Py_hash_t hash1, hash2;
             hash1 = ((PyBytesObject*)s1)->ob_shash;
             hash2 = ((PyBytesObject*)s2)->ob_shash;
             if (hash1 != hash2 && hash1 != -1 && hash2 != -1) {
                 return (equals == Py_NE);
             }
 #endif
@@ -10911,28 +11065,28 @@
                             "BaseException");
             goto bad;
         }
         PyException_SetCause(value, fixed_cause);
     }
     PyErr_SetObject(type, value);
     if (tb) {
-#if CYTHON_COMPILING_IN_PYPY
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
-#else
+#if CYTHON_FAST_THREAD_STATE
         PyThreadState *tstate = __Pyx_PyThreadState_Current;
         PyObject* tmp_tb = tstate->curexc_traceback;
         if (tb != tmp_tb) {
             Py_INCREF(tb);
             tstate->curexc_traceback = tb;
             Py_XDECREF(tmp_tb);
         }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
 #endif
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
@@ -11409,15 +11563,16 @@
     {(char *) "__module__", T_OBJECT, offsetof(PyCFunctionObject, m_module), PY_WRITE_RESTRICTED, 0},
     {0, 0, 0,  0, 0}
 };
 static PyObject *
 __Pyx_CyFunction_reduce(__pyx_CyFunctionObject *m, CYTHON_UNUSED PyObject *args)
 {
 #if PY_MAJOR_VERSION >= 3
-    return PyUnicode_FromString(m->func.m_ml->ml_name);
+    Py_INCREF(m->func_qualname);
+    return m->func_qualname;
 #else
     return PyString_FromString(m->func.m_ml->ml_name);
 #endif
 }
 static PyMethodDef __pyx_CyFunction_methods[] = {
     {"__reduce__", (PyCFunction)__Pyx_CyFunction_reduce, METH_VARARGS, 0},
     {0, 0, 0, 0}
@@ -11612,14 +11767,22 @@
         argc = PyTuple_GET_SIZE(args);
         new_args = PyTuple_GetSlice(args, 1, argc);
         if (unlikely(!new_args))
             return NULL;
         self = PyTuple_GetItem(args, 0);
         if (unlikely(!self)) {
             Py_DECREF(new_args);
+#if PY_MAJOR_VERSION > 2
+            PyErr_Format(PyExc_TypeError,
+                         "unbound method %.200S() needs an argument",
+                         cyfunc->func_qualname);
+#else
+            PyErr_SetString(PyExc_TypeError,
+                            "unbound method needs an argument");
+#endif
             return NULL;
         }
         result = __Pyx_CyFunction_CallMethod(func, self, new_args, kw);
         Py_DECREF(new_args);
     } else {
         result = __Pyx_CyFunction_Call(func, args, kw);
     }
@@ -11680,20 +11843,26 @@
     0,
     0,
     0,
     0,
 #if PY_VERSION_HEX >= 0x030400a1
     0,
 #endif
-#if PY_VERSION_HEX >= 0x030800b1
+#if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
     0,
 #endif
 #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
     0,
 #endif
+#if PY_VERSION_HEX >= 0x030C0000
+    0,
+#endif
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+    0,
+#endif
 };
 static int __pyx_CyFunction_init(void) {
     __pyx_CyFunctionType = __Pyx_FetchCommonType(&__pyx_CyFunctionType_type);
     if (unlikely(__pyx_CyFunctionType == NULL)) {
         return -1;
     }
     return 0;
@@ -11908,15 +12077,15 @@
     }
     Py_XDECREF(owned_metaclass);
     return result;
 }
 
 /* CLineInTraceback */
 #ifndef CYTHON_CLINE_IN_TRACEBACK
-static int __Pyx_CLineForTraceback(CYTHON_NCP_UNUSED PyThreadState *tstate, int c_line) {
+static int __Pyx_CLineForTraceback(CYTHON_UNUSED PyThreadState *tstate, int c_line) {
     PyObject *use_cline;
     PyObject *ptype, *pvalue, *ptraceback;
 #if CYTHON_COMPILING_IN_CPYTHON
     PyObject **cython_runtime_dict;
 #endif
     if (unlikely(!__pyx_cython_runtime)) {
         return c_line;
@@ -11938,15 +12107,15 @@
       } else {
         PyErr_Clear();
         use_cline = NULL;
       }
     }
     if (!use_cline) {
         c_line = 0;
-        PyObject_SetAttr(__pyx_cython_runtime, __pyx_n_s_cline_in_traceback, Py_False);
+        (void) PyObject_SetAttr(__pyx_cython_runtime, __pyx_n_s_cline_in_traceback, Py_False);
     }
     else if (use_cline == Py_False || (use_cline != Py_True && PyObject_Not(use_cline) != 0)) {
         c_line = 0;
     }
     __Pyx_ErrRestoreInState(tstate, ptype, pvalue, ptraceback);
     return c_line;
 }
@@ -12032,41 +12201,48 @@
     Py_INCREF(code_object);
 }
 
 /* AddTraceback */
 #include "compile.h"
 #include "frameobject.h"
 #include "traceback.h"
+#if PY_VERSION_HEX >= 0x030b00a6
+  #ifndef Py_BUILD_CORE
+    #define Py_BUILD_CORE 1
+  #endif
+  #include "internal/pycore_frame.h"
+#endif
 static PyCodeObject* __Pyx_CreateCodeObjectForTraceback(
             const char *funcname, int c_line,
             int py_line, const char *filename) {
-    PyCodeObject *py_code = 0;
-    PyObject *py_srcfile = 0;
-    PyObject *py_funcname = 0;
+    PyCodeObject *py_code = NULL;
+    PyObject *py_funcname = NULL;
     #if PY_MAJOR_VERSION < 3
+    PyObject *py_srcfile = NULL;
     py_srcfile = PyString_FromString(filename);
-    #else
-    py_srcfile = PyUnicode_FromString(filename);
-    #endif
     if (!py_srcfile) goto bad;
+    #endif
     if (c_line) {
         #if PY_MAJOR_VERSION < 3
         py_funcname = PyString_FromFormat( "%s (%s:%d)", funcname, __pyx_cfilenm, c_line);
+        if (!py_funcname) goto bad;
         #else
         py_funcname = PyUnicode_FromFormat( "%s (%s:%d)", funcname, __pyx_cfilenm, c_line);
+        if (!py_funcname) goto bad;
+        funcname = PyUnicode_AsUTF8(py_funcname);
+        if (!funcname) goto bad;
         #endif
     }
     else {
         #if PY_MAJOR_VERSION < 3
         py_funcname = PyString_FromString(funcname);
-        #else
-        py_funcname = PyUnicode_FromString(funcname);
+        if (!py_funcname) goto bad;
         #endif
     }
-    if (!py_funcname) goto bad;
+    #if PY_MAJOR_VERSION < 3
     py_code = __Pyx_PyCode_New(
         0,
         0,
         0,
         0,
         0,
         __pyx_empty_bytes, /*PyObject *code,*/
@@ -12077,34 +12253,49 @@
         __pyx_empty_tuple, /*PyObject *cellvars,*/
         py_srcfile,   /*PyObject *filename,*/
         py_funcname,  /*PyObject *name,*/
         py_line,
         __pyx_empty_bytes  /*PyObject *lnotab*/
     );
     Py_DECREF(py_srcfile);
-    Py_DECREF(py_funcname);
+    #else
+    py_code = PyCode_NewEmpty(filename, funcname, py_line);
+    #endif
+    Py_XDECREF(py_funcname);  // XDECREF since it's only set on Py3 if cline
     return py_code;
 bad:
-    Py_XDECREF(py_srcfile);
     Py_XDECREF(py_funcname);
+    #if PY_MAJOR_VERSION < 3
+    Py_XDECREF(py_srcfile);
+    #endif
     return NULL;
 }
 static void __Pyx_AddTraceback(const char *funcname, int c_line,
                                int py_line, const char *filename) {
     PyCodeObject *py_code = 0;
     PyFrameObject *py_frame = 0;
     PyThreadState *tstate = __Pyx_PyThreadState_Current;
+    PyObject *ptype, *pvalue, *ptraceback;
     if (c_line) {
         c_line = __Pyx_CLineForTraceback(tstate, c_line);
     }
     py_code = __pyx_find_code_object(c_line ? -c_line : py_line);
     if (!py_code) {
+        __Pyx_ErrFetchInState(tstate, &ptype, &pvalue, &ptraceback);
         py_code = __Pyx_CreateCodeObjectForTraceback(
             funcname, c_line, py_line, filename);
-        if (!py_code) goto bad;
+        if (!py_code) {
+            /* If the code object creation fails, then we should clear the
+               fetched exception references and propagate the new exception */
+            Py_XDECREF(ptype);
+            Py_XDECREF(pvalue);
+            Py_XDECREF(ptraceback);
+            goto bad;
+        }
+        __Pyx_ErrRestoreInState(tstate, ptype, pvalue, ptraceback);
         __pyx_insert_code_object(c_line ? -c_line : py_line, py_code);
     }
     py_frame = PyFrame_New(
         tstate,            /*PyThreadState *tstate,*/
         py_code,           /*PyCodeObject *code,*/
         __pyx_d,    /*PyObject *globals,*/
         0                  /*PyObject *locals*/
@@ -12115,15 +12306,22 @@
 bad:
     Py_XDECREF(py_code);
     Py_XDECREF(py_frame);
 }
 
 /* CIntToPy */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value) {
-    const long neg_one = (long) ((long) 0 - (long) 1), const_zero = (long) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic push
+#pragma GCC diagnostic ignored "-Wconversion"
+#endif
+    const long neg_one = (long) -1, const_zero = (long) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic pop
+#endif
     const int is_unsigned = neg_one > const_zero;
     if (is_unsigned) {
         if (sizeof(long) < sizeof(long)) {
             return PyInt_FromLong((long) value);
         } else if (sizeof(long) <= sizeof(unsigned long)) {
             return PyLong_FromUnsignedLong((unsigned long) value);
 #ifdef HAVE_LONG_LONG
@@ -12168,15 +12366,22 @@
             }\
         }\
         return (target_type) value;\
     }
 
 /* CIntFromPy */
 static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *x) {
-    const long neg_one = (long) ((long) 0 - (long) 1), const_zero = (long) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic push
+#pragma GCC diagnostic ignored "-Wconversion"
+#endif
+    const long neg_one = (long) -1, const_zero = (long) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic pop
+#endif
     const int is_unsigned = neg_one > const_zero;
 #if PY_MAJOR_VERSION < 3
     if (likely(PyInt_Check(x))) {
         if (sizeof(long) < sizeof(long)) {
             __PYX_VERIFY_RETURN_INT(long, long, PyInt_AS_LONG(x))
         } else {
             long val = PyInt_AS_LONG(x);
@@ -12219,15 +12424,15 @@
                         } else if (8 * sizeof(long) >= 4 * PyLong_SHIFT) {
                             return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -12357,15 +12562,22 @@
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to long");
     return (long) -1;
 }
 
 /* CIntFromPy */
 static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *x) {
-    const int neg_one = (int) ((int) 0 - (int) 1), const_zero = (int) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic push
+#pragma GCC diagnostic ignored "-Wconversion"
+#endif
+    const int neg_one = (int) -1, const_zero = (int) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic pop
+#endif
     const int is_unsigned = neg_one > const_zero;
 #if PY_MAJOR_VERSION < 3
     if (likely(PyInt_Check(x))) {
         if (sizeof(int) < sizeof(long)) {
             __PYX_VERIFY_RETURN_INT(int, long, PyInt_AS_LONG(x))
         } else {
             long val = PyInt_AS_LONG(x);
@@ -12408,15 +12620,15 @@
                         } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
                             return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -12546,19 +12758,41 @@
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to int");
     return (int) -1;
 }
 
 /* CheckBinaryVersion */
 static int __Pyx_check_binary_version(void) {
-    char ctversion[4], rtversion[4];
-    PyOS_snprintf(ctversion, 4, "%d.%d", PY_MAJOR_VERSION, PY_MINOR_VERSION);
-    PyOS_snprintf(rtversion, 4, "%s", Py_GetVersion());
-    if (ctversion[0] != rtversion[0] || ctversion[2] != rtversion[2]) {
+    char ctversion[5];
+    int same=1, i, found_dot;
+    const char* rt_from_call = Py_GetVersion();
+    PyOS_snprintf(ctversion, 5, "%d.%d", PY_MAJOR_VERSION, PY_MINOR_VERSION);
+    found_dot = 0;
+    for (i = 0; i < 4; i++) {
+        if (!ctversion[i]) {
+            same = (rt_from_call[i] < '0' || rt_from_call[i] > '9');
+            break;
+        }
+        if (rt_from_call[i] != ctversion[i]) {
+            same = 0;
+            break;
+        }
+    }
+    if (!same) {
+        char rtversion[5] = {'\0'};
         char message[200];
+        for (i=0; i<4; ++i) {
+            if (rt_from_call[i] == '.') {
+                if (found_dot) break;
+                found_dot = 1;
+            } else if (rt_from_call[i] < '0' || rt_from_call[i] > '9') {
+                break;
+            }
+            rtversion[i] = rt_from_call[i];
+        }
         PyOS_snprintf(message, sizeof(message),
                       "compiletime version %s of module '%.100s' "
                       "does not match runtime version %s",
                       ctversion, __Pyx_MODULE_NAME, rtversion);
         return PyErr_WarnEx(NULL, message, 1);
     }
     return 0;
@@ -12808,14 +13042,31 @@
   }
   x = PyNumber_Index(b);
   if (!x) return -1;
   ival = PyInt_AsSsize_t(x);
   Py_DECREF(x);
   return ival;
 }
+static CYTHON_INLINE Py_hash_t __Pyx_PyIndex_AsHash_t(PyObject* o) {
+  if (sizeof(Py_hash_t) == sizeof(Py_ssize_t)) {
+    return (Py_hash_t) __Pyx_PyIndex_AsSsize_t(o);
+#if PY_MAJOR_VERSION < 3
+  } else if (likely(PyInt_CheckExact(o))) {
+    return PyInt_AS_LONG(o);
+#endif
+  } else {
+    Py_ssize_t ival;
+    PyObject *x;
+    x = PyNumber_Index(o);
+    if (!x) return -1;
+    ival = PyInt_AsLong(x);
+    Py_DECREF(x);
+    return ival;
+  }
+}
 static CYTHON_INLINE PyObject * __Pyx_PyBool_FromLong(long b) {
   return b ? __Pyx_NewRef(Py_True) : __Pyx_NewRef(Py_False);
 }
 static CYTHON_INLINE PyObject * __Pyx_PyInt_FromSize_t(size_t ival) {
     return PyInt_FromSize_t(ival);
 }
```

