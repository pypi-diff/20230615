# Comparing `tmp/jobmanager-0.1.0.tar.gz` & `tmp/jobmanager-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/jobmanager-0.1.0.tar", last modified: Tue Jan  6 17:12:21 2015, max compression
+gzip compressed data, was "jobmanager-0.4.0.tar", max compression
```

## Comparing `jobmanager-0.1.0.tar` & `jobmanager-0.4.0.tar`

### file list

```diff
@@ -1,37 +1,10 @@
-drwxr-xr-x   0 cima      (1037) users      (200)        0 2015-01-06 17:12:21.000000 jobmanager-0.1.0/
-drwxr-xr-x   0 cima      (1037) users      (200)        0 2015-01-06 17:12:21.000000 jobmanager-0.1.0/doc/
--rw-r--r--   0 cima      (1037) users      (200)    38998 2015-01-06 16:42:43.000000 jobmanager-0.1.0/doc/server_client_communication.pdf
-drwxr-xr-x   0 cima      (1037) users      (200)        0 2015-01-06 17:12:21.000000 jobmanager-0.1.0/test/
--rw-r--r--   0 cima      (1037) users      (200)    16705 2015-01-06 16:42:43.000000 jobmanager-0.1.0/test/test_jobmanager.py
--rw-r--r--   0 cima      (1037) users      (200)    13915 2015-01-06 16:42:43.000000 jobmanager-0.1.0/test/test_progress.py
--rw-r--r--   0 cima      (1037) users      (200)      903 2015-01-06 16:51:27.000000 jobmanager-0.1.0/test/test_persistentData.py
--rw-r--r--   0 cima      (1037) users      (200)     5751 2015-01-06 16:51:27.000000 jobmanager-0.1.0/test/test_clients.py
--rw-r--r--   0 cima      (1037) users      (200)      469 2015-01-06 16:42:43.000000 jobmanager-0.1.0/README.md
--rw-r--r--   0 cima      (1037) users      (200)      673 2015-01-06 17:12:21.000000 jobmanager-0.1.0/PKG-INFO
-drwxr-xr-x   0 cima      (1037) users      (200)        0 2015-01-06 17:12:21.000000 jobmanager-0.1.0/jobmanager.egg-info/
--rw-r--r--   0 cima      (1037) users      (200)      673 2015-01-06 17:12:20.000000 jobmanager-0.1.0/jobmanager.egg-info/PKG-INFO
--rw-r--r--   0 cima      (1037) users      (200)        1 2015-01-06 17:12:20.000000 jobmanager-0.1.0/jobmanager.egg-info/dependency_links.txt
--rw-r--r--   0 cima      (1037) users      (200)      748 2015-01-06 17:12:21.000000 jobmanager-0.1.0/jobmanager.egg-info/SOURCES.txt
--rw-r--r--   0 cima      (1037) users      (200)       11 2015-01-06 17:12:20.000000 jobmanager-0.1.0/jobmanager.egg-info/top_level.txt
--rw-r--r--   0 cima      (1037) users      (200)       24 2015-01-06 17:12:20.000000 jobmanager-0.1.0/jobmanager.egg-info/requires.txt
--rw-r--r--   0 cima      (1037) users      (200)       59 2015-01-06 17:12:21.000000 jobmanager-0.1.0/setup.cfg
--rw-r--r--   0 cima      (1037) users      (200)       85 2015-01-06 16:42:43.000000 jobmanager-0.1.0/MANIFEST.in
--rw-r--r--   0 cima      (1037) users      (200)     1422 2015-01-06 17:12:07.000000 jobmanager-0.1.0/setup.py
-drwxr-xr-x   0 cima      (1037) users      (200)        0 2015-01-06 17:12:21.000000 jobmanager-0.1.0/examples/
--rw-r--r--   0 cima      (1037) users      (200)     1781 2015-01-06 16:42:43.000000 jobmanager-0.1.0/examples/simple_example.py
--rw-r--r--   0 cima      (1037) users      (200)     3197 2015-01-06 16:42:43.000000 jobmanager-0.1.0/examples/wrapper_example.py
-drwxr-xr-x   0 cima      (1037) users      (200)        0 2015-01-06 17:12:21.000000 jobmanager-0.1.0/examples/advanced/
--rw-r--r--   0 cima      (1037) users      (200)      186 2015-01-06 16:42:43.000000 jobmanager-0.1.0/examples/advanced/server.py
--rw-r--r--   0 cima      (1037) users      (200)     1001 2015-01-06 16:42:43.000000 jobmanager-0.1.0/examples/advanced/calculations.py
--rw-r--r--   0 cima      (1037) users      (200)      154 2015-01-06 16:42:43.000000 jobmanager-0.1.0/examples/advanced/client.py
--rw-r--r--   0 cima      (1037) users      (200)     4744 2015-01-06 16:42:43.000000 jobmanager-0.1.0/examples/advanced/my_jobmanager_classes.py
-drwxr-xr-x   0 cima      (1037) users      (200)        0 2015-01-06 17:12:21.000000 jobmanager-0.1.0/jobmanager/
--rw-r--r--   0 cima      (1037) users      (200)      137 2015-01-06 16:42:43.000000 jobmanager-0.1.0/jobmanager/jm_version.py
--rw-r--r--   0 cima      (1037) users      (200)     6144 2015-01-06 16:42:43.000000 jobmanager-0.1.0/jobmanager/decorators.py
--rw-r--r--   0 cima      (1037) users      (200)    39406 2015-01-06 16:42:43.000000 jobmanager-0.1.0/jobmanager/progress.py
--rw-r--r--   0 cima      (1037) users      (200)     3039 2015-01-06 16:51:27.000000 jobmanager-0.1.0/jobmanager/persistentData.py
--rw-r--r--   0 cima      (1037) users      (200)     3419 2015-01-06 16:51:27.000000 jobmanager-0.1.0/jobmanager/servers.py
--rw-r--r--   0 cima      (1037) users      (200)     5560 2015-01-06 16:51:27.000000 jobmanager-0.1.0/jobmanager/clients.py
--rw-r--r--   0 cima      (1037) users      (200)    48405 2015-01-06 16:51:27.000000 jobmanager-0.1.0/jobmanager/jobmanager.py
--rw-r--r--   0 cima      (1037) users      (200)      419 2015-01-06 16:42:43.000000 jobmanager-0.1.0/jobmanager/__init__.py
--rw-r--r--   0 cima      (1037) users      (200)     3602 2015-01-06 16:51:27.000000 jobmanager-0.1.0/jobmanager/ode_wrapper.py
+-rw-r--r--   0        0        0     1083 2016-09-27 20:39:36.170516 jobmanager-0.4.0/LICENSE
+-rw-r--r--   0        0        0     1359 2023-06-15 21:46:17.941745 jobmanager-0.4.0/README.md
+-rw-r--r--   0        0        0      851 2016-09-29 18:55:19.118543 jobmanager-0.4.0/jobmanager/__init__.py
+-rw-r--r--   0        0        0     6633 2023-06-15 21:32:12.814108 jobmanager-0.4.0/jobmanager/clients.py
+-rw-r--r--   0        0        0    99780 2023-06-15 21:34:26.912639 jobmanager-0.4.0/jobmanager/jobmanager.py
+-rw-r--r--   0        0        0    10228 2023-06-15 21:36:19.606765 jobmanager-0.4.0/jobmanager/ode_wrapper.py
+-rw-r--r--   0        0        0     2049 2023-06-15 21:34:26.916639 jobmanager-0.4.0/jobmanager/servers.py
+-rw-r--r--   0        0        0     3357 2021-11-01 21:25:44.466676 jobmanager-0.4.0/jobmanager/signalDelay.py
+-rw-r--r--   0        0        0      928 2023-06-15 21:44:57.464301 jobmanager-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     2455 1970-01-01 00:00:00.000000 jobmanager-0.4.0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `jobmanager-0.1.0/jobmanager/clients.py` & `jobmanager-0.4.0/jobmanager/clients.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,78 +1,94 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
 """
 The clients module
 
 This module provides special subclasses of the JobManager_Client
 """
 
-import os
-import sys
-import traceback
-
 from .jobmanager import JobManager_Client
 from . import ode_wrapper
 
 
 def merge_arg_and_const_arg(arg, const_arg):
     """
-        prepares data from arg and const_arg such that they can be passed
-        to the general integration routine
-        
-        arg and const_arg are both assumed to be dictionaries
-        
-        the merge process must not alter arg nor const_arg
-        in order to be used in the jobmanager context
-        
-        returns the arguments passed to the function
-        defining the derivative such that
-        args_dgl = arg['args'] + const_arg['args']
-        where as arg['args'] and const_arg['args'] have been assumed to be tuples
-        
-        e.g. 
-            arg['args'] = (2, 'low')
-            const_arg['args'] = (15, np.pi)
-        f will be called with
-        f(t, x, 2, 'low', 15, np.pi)
-        
-        returns further the combined dictionary
-        arg + const_arg with the keyword 'args' removed 
-    """
+    prepares data from arg and const_arg such that they can be passed
+    to the general integration routine
+    
+    arg and const_arg are both assumed to be dictionaries
+    
+    the merge process must not alter arg nor const_arg
+    in order to be used in the jobmanager context
+    
+    returns the arguments passed to the function
+    defining the derivative such that
+    args_dgl = arg['args'] + const_arg['args']
+    where as arg['args'] and const_arg['args'] have been assumed to be tuples
+    
+    e.g. 
+        arg['args'] = (2, 'low')
+        const_arg['args'] = (15, np.pi)
+    f will be called with
+    f(t, x, 2, 'low', 15, np.pi)
+    
+    returns further the combined dictionary
+    arg + const_arg with the keyword 'args' removed
+    
+    For any duplicate keys the value will be the value
+    from the 'arg' dictionary. 
+    """
+    
+    # allows arg to be a namedtuple (or any other object that
+    # can be converted to a dict)
+    # the purpose is that dicts are not allowed as keys for
+    # the persistent data structure, where as namedtupled are
+    # and therefore arg as a neamedtuple may be used to identify
+    # the result of this calculation in the database
+    if hasattr(arg, '_asdict'):
+        arg = arg._asdict()
+        
+    # same for const_arg, as a reason of consistency
+    if hasattr(const_arg, '_asdict'):
+        const_arg = const_arg._asdict() 
     
     # extract the args keyword from arg and const_arg
     args_dgl = tuple()
     if 'args' in arg:
         args_dgl += arg['args']
     if 'args' in const_arg:
         args_dgl += const_arg['args']
 
     kwargs = {}
-    kwargs.update(arg)
     kwargs.update(const_arg)
+    kwargs.update(arg)
     # remove args as they have been constructed explicitly
-    kwargs.pop('args')
+    if 'args' in kwargs:
+        del kwargs['args']
+        
+    # remove id, when it comes from the persistentDataServer 
+    if 'id' in kwargs:
+        del kwargs['id']
     
     return args_dgl, kwargs
 
 
 class Integration_Client_CPLX(JobManager_Client):
     """
         A JobManager_Client subclass to integrate a set of complex valued ODE.
         
-        'arg' as well as 'const_arg' which are passed from the JobManager_Server
-        to the JobManager_Client's function 'func' must be hashable dictionaries
-        (see for example jobmanager.HashDict). The updated dictionary kwargs
-         
-            kwargs = {}
-            kwargs.update(const_arg)
-            kwargs.update(arg)
+        'arg' and 'const_arg' are understood as keyword arguments in oder to
+        call ode_wrapper.integrate_cplx. They are passed to merge_arg_and_const_arg
+        in order to separate the kwargs needed by ode_wrapper.integrate_cplx
+        from the args (as tupled) passed to the function calculating derivative of the DGL.
+        This tuple of parameters itself is passed as a special argument to
+        ode_wrapper.integrate_cplx namely 'args'.
         
-        will hold the keyword arguments passed to ode_wrapper.integrate_cplx.
-        This implies that the keys of kwargs MUST include
+        If 'arg' or 'const_arg' provide the attribute '_asdict' it will be called
+        in order to construct dictionaries and use them for further processing.
+        
+        The following keys MUST be provided by 'arg' or 'const_arg'
             
             t0            : initial time
             t1            : final time
             N             : number of time steps for the solution x(t)
                             t = linspace(t0, t1, N)
             f             : function holding the derivatives 
             args          : additional positional arguments passed to f(t, x, *args)
@@ -90,27 +106,25 @@
                                        that 'zvode'. Consider using Integration_Client_REAL
                                        in the first place.  
                                        
         optional keys are:
             verbose        : default 0
             integrator related arguments (see the scipy doc ODE)
             
-        As the key 'args' itself has a tuple as value, it's composition used
-        instead of a simple update. So 
-        
-            kwargs['args'] = arg['args'] + const_arg['args']
-            
+        The key 'args' itself (should be tuple) will be merged as
+        kwargs['args'] = arg['args'] + const_arg['args']  
         which means that the call signature of f has to be
-        f(t, x, arg_1, arg_2, ... const_arg_1, const_arg_2, ...) 
+        f(t, x, arg_1, arg_2, ... const_arg_1, const_arg_2, ...). 
     """
     def __init__(self, **kwargs):
         super(Integration_Client_CPLX, self).__init__(**kwargs)
         
     @staticmethod
     def func(arg, const_arg, c, m):
+        # named tupled to dict conversion moved to merge_arg_and_const_arg
         args_dgl, kwargs = merge_arg_and_const_arg(arg, const_arg)
         m.value = kwargs['N']
        
         # t0, t1, N, f, args, x0, integrator, verbose, c, **kwargs
         return ode_wrapper.integrate_cplx(c=c, args=args_dgl, **kwargs)
     
     
@@ -124,25 +138,31 @@
         performance issue and 'zvode' is obviously not supported. 
     """
     def __init__(self, **kwargs):
         super(Integration_Client_REAL, self).__init__(**kwargs)
         
     @staticmethod
     def func(arg, const_arg, c, m):
+        # named tupled to dict conversion moved to merge_arg_and_const_arg
         args_dgl, kwargs = merge_arg_and_const_arg(arg, const_arg)
         m.value = kwargs['N']
         
         # t0, t1, N, f, args, x0, integrator, verbose, c, **kwargs
         return ode_wrapper.integrate_real(c=c, args=args_dgl, **kwargs)
     
     
     
 class FunctionCall_Client(JobManager_Client):
     @staticmethod
     def func(arg, const_arg, c, m):
+        if hasattr(arg, '_asdict'):
+            arg = arg._asdict()
+        if hasattr(const_arg, '_asdict'):
+            const_arg = const_arg._asdict()     
+        
         f = const_arg['f']
         f_kwargs = {}
         f_kwargs.update(arg)
         f_kwargs.update(const_arg)
         f_kwargs.pop('f')
         f_kwargs['__c'] = c
         f_kwargs['__m'] = m
```

