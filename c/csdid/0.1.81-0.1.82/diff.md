# Comparing `tmp/csdid-0.1.81.tar.gz` & `tmp/csdid-0.1.82.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csdid-0.1.81.tar", last modified: Thu Jun 15 20:53:20 2023, max compression
+gzip compressed data, was "csdid-0.1.82.tar", last modified: Thu Jun 15 21:22:36 2023, max compression
```

## Comparing `csdid-0.1.81.tar` & `csdid-0.1.82.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 20:53:20.762987 csdid-0.1.81/
--rw-rw-rw-   0        0        0     1126 2023-06-15 19:08:39.000000 csdid-0.1.81/LICENSE
--rw-rw-rw-   0        0        0      534 2023-06-15 20:53:20.762987 csdid-0.1.81/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-15 20:53:20.738982 csdid-0.1.81/csdid/
--rw-rw-rw-   0        0        0        0 2023-06-15 19:08:39.000000 csdid-0.1.81/csdid/__init__.py
--rw-rw-rw-   0        0        0       20 2023-06-15 20:53:14.000000 csdid-0.1.81/csdid/_version.py
-drwxrwxrwx   0        0        0        0 2023-06-15 20:53:20.756986 csdid-0.1.81/csdid/aggte_fnc/
--rw-rw-rw-   0        0        0        0 2023-06-15 19:08:39.000000 csdid-0.1.81/csdid/aggte_fnc/__init__.py
--rw-rw-rw-   0        0        0     4712 2023-06-15 19:08:39.000000 csdid-0.1.81/csdid/aggte_fnc/aggte.py
--rw-rw-rw-   0        0        0    22816 2023-06-15 19:08:39.000000 csdid-0.1.81/csdid/aggte_fnc/compute_aggte.py
--rw-rw-rw-   0        0        0     7182 2023-06-15 19:08:39.000000 csdid-0.1.81/csdid/aggte_fnc/utils.py
--rw-rw-rw-   0        0        0     6269 2023-06-15 19:08:39.000000 csdid-0.1.81/csdid/att_gt.py
-drwxrwxrwx   0        0        0        0 2023-06-15 20:53:20.758986 csdid-0.1.81/csdid/attgt_fnc/
--rw-rw-rw-   0        0        0        0 2023-06-15 19:08:39.000000 csdid-0.1.81/csdid/attgt_fnc/__init__.py
--rw-rw-rw-   0        0        0     5837 2023-06-15 19:08:39.000000 csdid-0.1.81/csdid/attgt_fnc/compute_att_gt.py
--rw-rw-rw-   0        0        0     5389 2023-06-15 19:08:39.000000 csdid-0.1.81/csdid/attgt_fnc/preprocess_did.py
-drwxrwxrwx   0        0        0        0 2023-06-15 20:53:20.759986 csdid-0.1.81/csdid/plots/
--rw-rw-rw-   0        0        0        0 2023-06-15 19:08:39.000000 csdid-0.1.81/csdid/plots/__init__.py
--rw-rw-rw-   0        0        0     4016 2023-06-15 19:08:39.000000 csdid-0.1.81/csdid/plots/gplot.py
-drwxrwxrwx   0        0        0        0 2023-06-15 20:53:20.761987 csdid-0.1.81/csdid/utils/
--rw-rw-rw-   0        0        0        0 2023-06-15 19:08:39.000000 csdid-0.1.81/csdid/utils/__init__.py
--rw-rw-rw-   0        0        0     1574 2023-06-15 19:08:39.000000 csdid-0.1.81/csdid/utils/bmisc.py
--rw-rw-rw-   0        0        0     4280 2023-06-15 19:08:39.000000 csdid-0.1.81/csdid/utils/mboot.py
-drwxrwxrwx   0        0        0        0 2023-06-15 20:53:20.754985 csdid-0.1.81/csdid.egg-info/
--rw-rw-rw-   0        0        0      534 2023-06-15 20:53:20.000000 csdid-0.1.81/csdid.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      530 2023-06-15 20:53:20.000000 csdid-0.1.81/csdid.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 20:53:20.000000 csdid-0.1.81/csdid.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-06-15 20:53:20.000000 csdid-0.1.81/csdid.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-15 20:53:20.000000 csdid-0.1.81/csdid.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-15 20:53:20.762987 csdid-0.1.81/setup.cfg
--rw-rw-rw-   0        0        0     1008 2023-06-15 20:52:55.000000 csdid-0.1.81/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:22:36.373232 csdid-0.1.82/
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-06-15 21:21:55.000000 csdid-0.1.82/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-15 21:22:36.373232 csdid-0.1.82/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:22:36.373232 csdid-0.1.82/csdid/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 21:21:55.000000 csdid-0.1.82/csdid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-15 21:21:55.000000 csdid-0.1.82/csdid/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:22:36.373232 csdid-0.1.82/csdid/aggte_fnc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 21:21:55.000000 csdid-0.1.82/csdid/aggte_fnc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4599 2023-06-15 21:21:55.000000 csdid-0.1.82/csdid/aggte_fnc/aggte.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22322 2023-06-15 21:21:55.000000 csdid-0.1.82/csdid/aggte_fnc/compute_aggte.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6987 2023-06-15 21:21:55.000000 csdid-0.1.82/csdid/aggte_fnc/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6051 2023-06-15 21:21:55.000000 csdid-0.1.82/csdid/att_gt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:22:36.373232 csdid-0.1.82/csdid/attgt_fnc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 21:21:55.000000 csdid-0.1.82/csdid/attgt_fnc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5643 2023-06-15 21:21:55.000000 csdid-0.1.82/csdid/attgt_fnc/compute_att_gt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-06-15 21:21:55.000000 csdid-0.1.82/csdid/attgt_fnc/preprocess_did.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:22:36.373232 csdid-0.1.82/csdid/plots/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 21:21:55.000000 csdid-0.1.82/csdid/plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-06-15 21:21:55.000000 csdid-0.1.82/csdid/plots/gplot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:22:36.373232 csdid-0.1.82/csdid/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 21:21:55.000000 csdid-0.1.82/csdid/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-06-15 21:21:55.000000 csdid-0.1.82/csdid/utils/bmisc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4168 2023-06-15 21:21:55.000000 csdid-0.1.82/csdid/utils/mboot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:22:36.373232 csdid-0.1.82/csdid.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-15 21:22:35.000000 csdid-0.1.82/csdid.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-15 21:22:36.000000 csdid-0.1.82/csdid.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 21:22:35.000000 csdid-0.1.82/csdid.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-15 21:22:35.000000 csdid-0.1.82/csdid.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-15 21:22:35.000000 csdid-0.1.82/csdid.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 21:22:36.373232 csdid-0.1.82/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-06-15 21:21:55.000000 csdid-0.1.82/setup.py
```

### Comparing `csdid-0.1.81/LICENSE` & `csdid-0.1.82/LICENSE`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 Alexander Quispe, Jhon Flores and Rodrigo Grijalba
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+MIT License
+
+Copyright (c) 2023 Alexander Quispe, Jhon Flores and Rodrigo Grijalba
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

### Comparing `csdid-0.1.81/csdid/aggte_fnc/aggte.py` & `csdid-0.1.82/csdid/aggte_fnc/aggte.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,113 +1,113 @@
-#' @title Aggregate Group-Time Average Treatment Effects
-#'
-#' @description A function to take group-time average treatment effects
-#'  and aggregate them into a smaller number of parameters.  There are
-#'  several possible aggregations including "simple", "dynamic", "group",
-#'  and "calendar."
-#'
-#' @param MP an MP object (i.e., the results of the [att_gt()] method)
-#' @param type Which type of aggregated treatment effect parameter to compute.
-#'   One option is "simple" (this just computes a weighted average of all
-#'   group-time average treatment effects with weights proportional to group
-#'   size).  Other options are "dynamic" (this computes average effects across
-#'   different lengths of exposure to the treatment and is similar to an
-#'   "event study"; here the overall effect averages the effect of the
-#'   treatment across all positive lengths of exposure); "group" (this
-#'   is the default option and
-#'   computes average treatment effects across different groups; here
-#'   the overall effect averages the effect across different groups); and
-#'   "calendar" (this computes average treatment effects across different
-#'   time periods; here the overall effect averages the effect across each
-#'   time period).
-#' @param balance_e If set (and if one computes dynamic effects), it balances
-#'  the sample with respect to event time.  For example, if `balance.e=2`,
-#'  `aggte` will drop groups that are not exposed to treatment for
-#'  at least three periods. (the initial period when `e=0` as well as the
-#'  next two periods when `e=1` and the `e=2`).  This ensures that
-#'  the composition of groups does not change when event time changes.
-#' @param min_e For event studies, this is the smallest event time to compute
-#'  dynamic effects for.  By default, `min_e = -Inf` so that effects at
-#'  all lengths of exposure are computed.
-#' @param max_e For event studies, this is the largest event time to compute
-#'  dynamic effects for.  By default, `max_e = Inf` so that effects at
-#'  all lengths of exposure are computed.
-#' @param na.rm Logical value if we are to remove missing Values from analyses. Defaults is FALSE.
-#' @param bstrap Boolean for whether or not to compute standard errors using
-#'  the multiplier bootstrap.  If standard errors are clustered, then one
-#'  must set `bstrap=TRUE`. Default is value set in the MP object.  If bstrap is `FALSE`, then analytical
-#'  standard errors are reported.
-#' @param biters The number of bootstrap iterations to use.  The default is the value set in the MP object,
-#'  and this is only applicable if `bstrap=TRUE`.
-#'
-#' @param cband Boolean for whether or not to compute a uniform confidence
-#'  band that covers all of the group-time average treatment effects
-#'  with fixed probability `1-alp`.  In order to compute uniform confidence
-#'  bands, `bstrap` must also be set to `TRUE`.  The default is
-#'  the value set in the MP object
-#' @param alp the significance level, default is value set in the MP object.
-#' @param clustervars A vector of variables to cluster on.  At most, there
-#'  can be two variables (otherwise will throw an error) and one of these
-#'  must be the same as idname which allows for clustering at the individual
-#'  level. Default is the variables set in the MP object
-
-#'
-#' @return An [`AGGTEobj`] object that holds the results from the
-#'  aggregation
-#'
-#' @section Examples:
-#'
-#
-#' Initial ATT(g,t) estimates from [att_gt()]
-#'
-#'
-#' You can aggregate the ATT(g,t) in many ways.
-#'
-#' **Overall ATT:**
-#' aggte(out, type = "simple")
-#' ```
-#'
-#' **Dynamic ATT (Event-Study):**
-#' aggte(out, type = "dynamic")
-#' ```
-#'
-#' **ATT for each group:**
-#' aggte(out, type = "group")
-#' ```
-#'
-#' **ATT for each calendar year:**
-#' aggte(out, type = "calendar")
-#' ```
-#'
-#'
-#'
-from csdid.aggte_fnc.compute_aggte import compute_aggte
-import inspect
-
-def aggte(MP, 
-          typec="group", 
-          balance_e=None, 
-          min_e=float('-inf'), 
-          max_e=float('inf'), 
-          na_rm=False,
-          bstrap=None, 
-          biters=None, 
-          cband=None, 
-          alp=None, 
-          clustervars=None):
-    call = inspect.currentframe().f_back.f_locals.copy()
-
-    return compute_aggte(MP=MP, 
-                  typec=typec, 
-                  balance_e=balance_e, 
-                  min_e=min_e, 
-                  max_e=max_e, 
-                  na_rm=na_rm,
-                  bstrap=bstrap, 
-                  biters=biters, 
-                  cband=cband, 
-                  alp=alp, 
-                  clustervars=clustervars, 
-                  call=call)
-
- 
-
+#' @title Aggregate Group-Time Average Treatment Effects
+#'
+#' @description A function to take group-time average treatment effects
+#'  and aggregate them into a smaller number of parameters.  There are
+#'  several possible aggregations including "simple", "dynamic", "group",
+#'  and "calendar."
+#'
+#' @param MP an MP object (i.e., the results of the [att_gt()] method)
+#' @param type Which type of aggregated treatment effect parameter to compute.
+#'   One option is "simple" (this just computes a weighted average of all
+#'   group-time average treatment effects with weights proportional to group
+#'   size).  Other options are "dynamic" (this computes average effects across
+#'   different lengths of exposure to the treatment and is similar to an
+#'   "event study"; here the overall effect averages the effect of the
+#'   treatment across all positive lengths of exposure); "group" (this
+#'   is the default option and
+#'   computes average treatment effects across different groups; here
+#'   the overall effect averages the effect across different groups); and
+#'   "calendar" (this computes average treatment effects across different
+#'   time periods; here the overall effect averages the effect across each
+#'   time period).
+#' @param balance_e If set (and if one computes dynamic effects), it balances
+#'  the sample with respect to event time.  For example, if `balance.e=2`,
+#'  `aggte` will drop groups that are not exposed to treatment for
+#'  at least three periods. (the initial period when `e=0` as well as the
+#'  next two periods when `e=1` and the `e=2`).  This ensures that
+#'  the composition of groups does not change when event time changes.
+#' @param min_e For event studies, this is the smallest event time to compute
+#'  dynamic effects for.  By default, `min_e = -Inf` so that effects at
+#'  all lengths of exposure are computed.
+#' @param max_e For event studies, this is the largest event time to compute
+#'  dynamic effects for.  By default, `max_e = Inf` so that effects at
+#'  all lengths of exposure are computed.
+#' @param na.rm Logical value if we are to remove missing Values from analyses. Defaults is FALSE.
+#' @param bstrap Boolean for whether or not to compute standard errors using
+#'  the multiplier bootstrap.  If standard errors are clustered, then one
+#'  must set `bstrap=TRUE`. Default is value set in the MP object.  If bstrap is `FALSE`, then analytical
+#'  standard errors are reported.
+#' @param biters The number of bootstrap iterations to use.  The default is the value set in the MP object,
+#'  and this is only applicable if `bstrap=TRUE`.
+#'
+#' @param cband Boolean for whether or not to compute a uniform confidence
+#'  band that covers all of the group-time average treatment effects
+#'  with fixed probability `1-alp`.  In order to compute uniform confidence
+#'  bands, `bstrap` must also be set to `TRUE`.  The default is
+#'  the value set in the MP object
+#' @param alp the significance level, default is value set in the MP object.
+#' @param clustervars A vector of variables to cluster on.  At most, there
+#'  can be two variables (otherwise will throw an error) and one of these
+#'  must be the same as idname which allows for clustering at the individual
+#'  level. Default is the variables set in the MP object
+
+#'
+#' @return An [`AGGTEobj`] object that holds the results from the
+#'  aggregation
+#'
+#' @section Examples:
+#'
+#
+#' Initial ATT(g,t) estimates from [att_gt()]
+#'
+#'
+#' You can aggregate the ATT(g,t) in many ways.
+#'
+#' **Overall ATT:**
+#' aggte(out, type = "simple")
+#' ```
+#'
+#' **Dynamic ATT (Event-Study):**
+#' aggte(out, type = "dynamic")
+#' ```
+#'
+#' **ATT for each group:**
+#' aggte(out, type = "group")
+#' ```
+#'
+#' **ATT for each calendar year:**
+#' aggte(out, type = "calendar")
+#' ```
+#'
+#'
+#'
+from csdid.aggte_fnc.compute_aggte import compute_aggte
+import inspect
+
+def aggte(MP, 
+          typec="group", 
+          balance_e=None, 
+          min_e=float('-inf'), 
+          max_e=float('inf'), 
+          na_rm=False,
+          bstrap=None, 
+          biters=None, 
+          cband=None, 
+          alp=None, 
+          clustervars=None):
+    call = inspect.currentframe().f_back.f_locals.copy()
+
+    return compute_aggte(MP=MP, 
+                  typec=typec, 
+                  balance_e=balance_e, 
+                  min_e=min_e, 
+                  max_e=max_e, 
+                  na_rm=na_rm,
+                  bstrap=bstrap, 
+                  biters=biters, 
+                  cband=cband, 
+                  alp=alp, 
+                  clustervars=clustervars, 
+                  call=call)
+
+ 
+
```

### Comparing `csdid-0.1.81/csdid/aggte_fnc/compute_aggte.py` & `csdid-0.1.82/csdid/aggte_fnc/compute_aggte.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,494 +1,494 @@
-import pickle
-import pandas as pd
-import numpy as np
-from scipy.stats import norm
-
-
-from csdid.aggte_fnc.utils import get_agg_inf_func, get_se, wif, AGGTEobj
-from csdid.utils.mboot import mboot
-import warnings
-
-def compute_aggte(MP,
-                      typec         = "group",
-                      balance_e     = None,
-                      min_e         = float('-inf'),
-                      max_e         = float('inf'),
-                      na_rm         = False,
-                      bstrap        = None,
-                      biters        = None,
-                      cband         = None,
-                      alp           = None,
-                      clustervars   = None,
-                      call          = None):
-  
-# =============================================================================
-# unpack MP object
-# =============================================================================
-    group       = np.array( MP['group'] )
-    t           = np.array( MP['t']     )
-    att         = np.array( MP['att'] )
-    dp          = MP['DIDparams']
-    tlist       = np.array( dp['tlist'] )
-    glist       = np.array( dp['glist'] )
-    data        = pd.DataFrame( dp['data'] )    
-    inffunc     = MP['inffunc']['inffunc']
-    n           = MP['n']
-    gname       = dp['gname']
-    tname       = dp['tname']
-    idname      = dp['idname']
-    # typec       = MP['type']  
-    panel       = dp['panel']    
-
-
-    
-    if clustervars is None:
-        clustervars = dp['clustervars']
-    if bstrap is None:
-        bstrap = dp['bstrap']
-    if biters is None:
-        biters = dp['biters']
-    if alp is None:
-        alp = dp['alp']
-    if cband is None:
-        cband = dp['cband']
-
-
-
-    # Overwrite MP objects (to compute bootstrap)
-    MP['DIDparams']['clustervars'] = clustervars
-    MP['DIDparams']['bstrap'] = bstrap
-    MP['DIDparams']['biters'] = biters
-    MP['DIDparams']['alp'] = alp
-    MP['DIDparams']['cband'] = cband
-    
-# =============================================================================
-#  Treat data
-# =============================================================================
-
-    if typec not in ["simple", "dynamic", "group", "calendar"]:
-        raise ValueError("`typec` must be one of ['simple', 'dynamic', 'group', 'calendar']")
-    # Removing missing values    
-    if na_rm:
-        notna = ~np.isnan(att)
-        group = group[notna]
-        t = t[notna]
-        att = att[notna]
-        inffunc = inffunc[:, notna]
-        glist = np.sort(np.unique(group))
-    
-        if typec == "group":
-            gnotna = []
-            for g in glist:
-                indices = np.where((group == g) & (g <= t))
-                is_not_na = np.any(~np.isnan(att[indices]))
-                gnotna.append(is_not_na)
-            
-            gnotna = np.array(gnotna)
-            glist = glist[gnotna]
-            not_all_na = np.isin(group, glist)
-            group = group[not_all_na]
-            t = t[not_all_na]
-            att = att[not_all_na]
-            inffunc = inffunc[:, not_all_na]
-            glist = np.sort(np.unique(group))
-
-    
-    if (not na_rm) and np.any(np.isnan(att)):
-        raise ValueError("Missing values at att_gt found. If you want to remove these, set `na_rm = True`.")
-
-    if panel:
-        dta = data[data[tname] == tlist[0]]
-    else:
-        dta = data.groupby(idname).mean().reset_index()
-        dta = dta.iloc[:, 1:]
-
-# =============================================================================
-#  Treat data 2
-# =============================================================================
-
-    
-    originalt = t
-    originalgroup = group
-    originalglist = glist
-    originaltlist = tlist
-    # In case g's are not part of tlist
-    originalgtlist = np.sort(np.unique(np.concatenate((originaltlist, originalglist))))
-    uniquet = list(range(1, len(originalgtlist) + 1))
-    
-    # Function to switch from "new" t values to original t values
-    def t2orig(t):
-        return originalgtlist[uniquet.index(t) if t in uniquet else -1]
-    
-    # Function to switch between "original" t values and new t values
-    def orig2t(orig):
-        new_t = [uniquet[i] for i in range(len(originalgtlist)) if originalgtlist[i] == orig]
-        out = new_t[0] if new_t else None
-        return out
-    
-    t     = [orig2t(orig) for orig in originalt]
-    group = [orig2t(orig) for orig in originalgroup]
-    glist = [orig2t(orig) for orig in originalglist]
-    tlist = np.asarray(list(set(t)))
-    maxT  = max(t)
-        
-    # Set the weights
-    weights_ind = dta['.w']
-    
-    # We can work in overall probabilities because conditioning will cancel out
-    # since it shows up in numerator and denominator
-    pg = np.array([np.mean(weights_ind * (dta[gname] == g)) for g in originalglist])
-    
-    # Length of this is equal to the number of groups
-    pgg = pg
-
-    # Same but length is equal to the number of ATT(g,t)
-    pg = [pg[glist.index(g)] for g in group]  
-    
-    # Which group time average treatment effects are post-treatment
-    keepers = [i for i in range(len(group)) if group[i] <= t[i] <= (group[i] + max_e)] ### added second condition to allow for limit on longest period included in att
-    
-    # n x 1 vector of group variable
-    G = [orig2t(g) for g in dta[gname]]
-
-# =============================================================================
-#  simple
-# =============================================================================
-
-
-    if typec == "simple":
-        # Simple ATT
-        # Averages all post-treatment ATT(g,t) with weights given by group size
-        pg = np.array(pg)
-        simple_att = np.sum(att[keepers] * pg[keepers]) / np.sum(pg[keepers])
-        if np.isnan(simple_att):
-            simple_att = None
-    
-        # Get the part of the influence function coming from estimated weights
-        simple_wif = wif(keepers, pg, weights_ind, G, group)
-    
-        # Get the overall influence function
-        simple_if = get_agg_inf_func(att = att , 
-                                     inffunc = inffunc , 
-                                     whichones = keepers ,
-                                     weights_agg = np.array(pg)[keepers]/np.sum(np.array(pg)[keepers]) , 
-                                     wif = simple_wif )[:, None]
-    
-        # Get standard errors from the overall influence function
-        simple_se = get_se(simple_if, dp)
-        
-        if simple_se is not None:
-            if simple_se <= np.sqrt(np.finfo(float).eps) * 10:
-                simple_se = None
-                
-        AGGTEobj_print = AGGTEobj(overall_att=simple_att, 
-                                  overall_se=simple_se, 
-                                  typec=typec,
-                                  inf_function={'simple_att': simple_if}, 
-                                  call=call, DIDparams=dp)
-        
-        return AGGTEobj_print
-
-
-# =============================================================================
-#  GRoup
-# =============================================================================
-
-    if typec == "group":
-        group = np.array(group)
-        t = np.array(t) 
-        pg = np.array(pg) 
-        selective_att_g = [np.mean(att[( group== g) & (t >= g) & (t <= (group + max_e))]) for g in glist]
-        selective_att_g = np.asarray(selective_att_g)
-        selective_att_g[np.isnan(selective_att_g)] = None
-    
-        selective_se_inner = [None] * len(glist)
-        for i, g in enumerate(glist):
-            whichg = np.where(np.logical_and.reduce((group == g, g <= t, t <= (group + max_e))))[0]
-            weightsg =  pg[whichg] / np.sum(pg[whichg])
-            inf_func_g = get_agg_inf_func(att = att , 
-                                            inffunc = inffunc , 
-                                            whichones = whichg ,
-                                            weights_agg = weightsg , 
-                                            wif = None)[:, None]
-            se_g = get_se(inf_func_g, dp)
-            selective_se_inner[i] = {'inf_func': inf_func_g, 'se': se_g}
-            
-        # recover standard errors separately by group   
-        selective_se_g = np.asarray([item['se'] for item in selective_se_inner]).T
-        
-        selective_se_g[selective_se_g <= np.sqrt(np.finfo(float).eps) * 10] = None
-        
-        selective_inf_func_g = np.column_stack([elem["inf_func"] for elem in selective_se_inner])
-  
-        # use multiplier bootstrap (across groups) to get critical value
-        # for constructing uniform confidence bands   
-        selective_crit_val = norm.ppf(1 - alp/2)
-        
-        if dp['cband']:
-            if not dp['bstrap']:
-                print("Used bootstrap procedure to compute simultaneous confidence band")
-        
-            selective_crit_val = mboot(selective_inf_func_g, dp)['crit_val']
-        
-            if np.isnan(selective_crit_val) or np.isinf(selective_crit_val):
-                print("Simultaneous critical value is NA. This probably happened because we cannot compute t-statistic (std errors are NA). We then report pointwise conf. intervals.")
-                selective_crit_val = norm.ppf(1 - alp/2)
-                dp['cband'] = False
-        
-            if selective_crit_val < norm.ppf(1 - alp/2):
-                print("Simultaneous conf. band is somehow smaller than pointwise one using normal approximation. Since this is unusual, we are reporting pointwise confidence intervals")
-                selective_crit_val = norm.ppf(1 - alp/2)
-                dp['cband'] = False
-        
-            if selective_crit_val >= 7:
-                print("Simultaneous critical value is arguably 'too large' to be reliable. This usually happens when the number of observations per group is small and/or there is not much variation in outcomes.")
-  
-        # get overall att under selective treatment timing
-        # (here use pgg instead of pg because we can just look at each group)            
-        selective_att = np.sum(selective_att_g * pgg) / np.sum(pgg)
-        
-        # account for having to estimate pgg in the influence function    
-        selective_wif = wif(keepers = np.arange(1, len(glist)+1)-1, 
-                            pg  = pgg, 
-                            weights_ind = weights_ind, 
-                            G = G, 
-                            group = group)
-        
-        # get overall influence function   
-        selective_inf_func = get_agg_inf_func(att = selective_att_g, 
-                                              inffunc = selective_inf_func_g,
-                                              whichones = np.arange(1, len(glist)+1)-1, 
-                                              weights_agg = pgg/np.sum(pgg),
-                                              wif = selective_wif)[:, None]    
-        
-        # get overall standard error        
-        selective_se = get_se(selective_inf_func, dp)
-        if not np.isnan(selective_se):
-            if selective_se <= np.sqrt(np.finfo(float).eps) * 10:
-                selective_se = None
-    
-        AGGTEobj_print = AGGTEobj(overall_att = selective_att, 
-                            overall_se = selective_se, 
-                            typec = typec,
-                            egt = originalglist,
-                            att_egt = selective_att_g,
-                            se_egt = selective_se_g,
-                            crit_val_egt = selective_crit_val,
-                            inf_function = {'selective_inf_func_g': selective_inf_func_g, 
-                                            'selective_inf_func': selective_inf_func},
-                            call = call, 
-                            DIDparams = dp)
-
-        return AGGTEobj_print
-
-
-# =============================================================================
-#  Dynamic
-# =============================================================================
-
-    if typec == "dynamic":
-        # event times
-        # this looks at all available event times
-        # note: event times can be negative here.
-        # note: event time = 0 corresponds to "on impact"
-        eseq = np.unique(np.array(originalt) - np.array(originalgroup) ) # Subtract corresponding elements and convert to NumPy array
-        eseq = np.sort(eseq)  # Sort the unique values in ascending order
-    
-        # if the user specifies balance_e, then we are going to
-        # drop some event times and some groups; if not, we just
-        # keep everything (that is what this variable is for)
-        originalt = np.array(originalt)
-        originalgroup = np.array(originalgroup)
-        pg = np.array(pg)
-        include_balanced_gt = np.repeat(True, len(originalgroup))
-
-        if balance_e is not None:
-            include_balanced_gt = (t2orig(maxT) - originalgroup >= balance_e)        
-            eseq = np.unique(originalt[include_balanced_gt] - originalgroup[include_balanced_gt])
-            eseq = np.sort(eseq)      
-            eseq = eseq[(eseq <= balance_e) & (eseq >= balance_e - t2orig(maxT) + t2orig(1))]
-        eseq = eseq[(eseq >= min_e) & (eseq <= max_e)]
-
-        dynamic_att_e = []
-        for e in eseq:
-            whiche = np.where((originalt - originalgroup == e) & include_balanced_gt)
-            atte = att[whiche]
-            pge = pg[whiche] / np.sum(pg[whiche])
-            dynamic_att_e.append(np.sum(atte * pge))
-        
-        dynamic_se_inner = []
-        for e in eseq:
-            whiche = np.where((originalt - originalgroup == e) & (include_balanced_gt) )[0]
-            pge = pg[whiche] / sum(pg[whiche])
-            wif_e = wif(whiche, 
-                        pg, 
-                        weights_ind, 
-                        G, 
-                        group)
-            inf_func_e = get_agg_inf_func(att         = att, 
-                                          inffunc     = inffunc, 
-                                          whichones   = whiche, 
-                                          weights_agg = pge, 
-                                          wif         = wif_e)[:, None]
-            se_e = get_se(inf_func_e, dp)
-            dynamic_se_inner.append({'inf_func': inf_func_e, 'se': se_e})
-
-        dynamic_se_e = np.array([item['se'] for item in dynamic_se_inner]).T
-        
-        dynamic_se_e[dynamic_se_e <= np.sqrt(np.finfo(float).eps) * 10] = np.nan
-        
-        dynamic_inf_func_e = np.column_stack([item['inf_func'] for item in dynamic_se_inner])
-                
-        dynamic_crit_val = norm.ppf(1 - alp/2)
-        if dp['cband']:
-            if not dp['bstrap']:
-                print('Used bootstrap procedure to compute simultaneous confidence band')
-            dynamic_crit_val = mboot(dynamic_inf_func_e, dp)['crit_val']
-        
-            if np.isnan(dynamic_crit_val) or np.isinf(dynamic_crit_val):
-                print('Simultaneous critical value is NA. This probably happened because we cannot compute t-statistic (std errors are NA). We then report pointwise conf. intervals.')
-                dynamic_crit_val = norm.ppf(1 - alp/2)
-                dp['cband'] = False
-        
-            if dynamic_crit_val < norm.ppf(1 - alp/2):
-                print('Simultaneous conf. band is somehow smaller than pointwise one using normal approximation. Since this is unusual, we are reporting pointwise confidence intervals')
-                dynamic_crit_val = norm.ppf(1 - alp/2)
-                dp['cband'] = False
-        
-            if dynamic_crit_val >= 7:
-                print("Simultaneous critical value is arguably 'too large' to be reliable. This usually happens when the number of observations per group is small and/or there is not much variation in outcomes.")
-
-            epos = eseq >= 0
-            dynamic_att = np.mean(np.array(dynamic_att_e)[epos])
-            dynamic_inf_func = get_agg_inf_func(att         = np.array(dynamic_att_e)[epos],
-                                                inffunc     = np.array(dynamic_inf_func_e[:, epos]),
-                                                whichones   = np.arange(1, np.sum(epos)+1)-1,
-                                                weights_agg = np.repeat(1 / np.sum(epos), np.sum(epos)),
-                                                wif=None)[:, None]
-            
-            dynamic_se = get_se(dynamic_inf_func, dp)
-            if not np.isnan(dynamic_se):
-                if dynamic_se <= np.sqrt(np.finfo(float).eps) * 10:
-                    dynamic_se = np.nan
-
-        AGGTEobj_print = AGGTEobj(overall_att=dynamic_att,
-                                overall_se=dynamic_se,
-                                typec=typec,
-                                egt=eseq,
-                                att_egt=dynamic_att_e,
-                                se_egt=dynamic_se_e,
-                                crit_val_egt=dynamic_crit_val,
-                                inf_function={'dynamic_inf_func_e': dynamic_inf_func_e,
-                                              'dynamic_inf_func': dynamic_inf_func},
-                                call=call,
-                                min_e=min_e,
-                                max_e=max_e,
-                                balance_e=balance_e,
-                                DIDparams=dp)
-            
-        return AGGTEobj_print
-
-
-
-# =============================================================================
-#  Calendar
-# =============================================================================
-
- # np.array(group)
-    if typec == "calendar":
-        minG = min(group)
-        calendar_tlist = tlist[tlist >= minG]
-        pg = np.array(pg)
-        calendar_att_t = []
-        group = np.array(group)
-        t = np.array(t)
-        for t1 in calendar_tlist:
-            whicht = np.where((t == t1) & (group <= t))[0]
-            attt = att[whicht]
-            pgt = pg[whicht] / np.sum(pg[whicht])
-            calendar_att_t.append(np.sum(pgt * attt))
-            
-        # get standard errors and influence functions
-        # for each time specific att
-        calendar_se_inner = []
-        for t1 in calendar_tlist:
-            which_t = np.where((t == t1) & (group <= t))[0]
-            pgt = pg[which_t] / np.sum(pg[which_t])
-            wif_t = wif(keepers=which_t, 
-                        pg=pg, 
-                        weights_ind=weights_ind, 
-                        G=G, 
-                        group=group)
-            inf_func_t = get_agg_inf_func(att=att, 
-                                            inffunc=inffunc, 
-                                            whichones=which_t, 
-                                            weights_agg=pgt, 
-                                            wif=wif_t)[:, None]
-            se_t = get_se(inf_func_t, dp)
-            calendar_se_inner.append({"inf_func": inf_func_t, "se": se_t})
-    
-    
-    
-        # recover standard errors separately by time
-        calendar_se_t = np.array([se["se"] for se in calendar_se_inner]).T
-        calendar_se_t[calendar_se_t <= np.sqrt(np.finfo(float).eps) * 10] = np.nan
-        
-        # recover influence function separately by time
-        calendar_inf_func_t = np.column_stack([se["inf_func"] for se in calendar_se_inner])
-    
-        # use multiplier boostrap (across groups) to get critical value
-        # for constructing uniform confidence bands
-        calendar_crit_val = norm.ppf(1 - alp/2)
-        
-        if dp['cband']:
-            if not dp['bstrap']:
-                warnings.warn('Used bootstrap procedure to compute simultaneous confidence band')
-        
-            # mboot function is not provided, please define it separately
-            calendar_crit_val = mboot(calendar_inf_func_t, dp)['crit_val']
-        
-            if np.isnan(calendar_crit_val) or np.isinf(calendar_crit_val):
-                warnings.warn('Simultaneous critical value is NA. This probably happened because we cannot compute t-statistic (std errors are NA). We then report pointwise conf. intervals.')
-                calendar_crit_val = norm.ppf(1 - alp/2)
-                dp['cband'] = False
-        
-            if calendar_crit_val < norm.ppf(1 - alp/2):
-                warnings.warn('Simultaneous conf. band is somehow smaller than pointwise one using normal approximation. Since this is unusual, we are reporting pointwise confidence intervals.')
-                calendar_crit_val = norm.ppf(1 - alp/2)
-                dp['cband'] = False
-        
-            if calendar_crit_val >= 7:
-                warnings.warn("Simultaneous critical value is arguably 'too large' to be reliable. This usually happens when the number of observations per group is small and/or there is not much variation in outcomes.")
-    
-    
-        # get overall att under calendar time effects
-        # this is just average over all time periods
-        calendar_att = np.mean(calendar_att_t)
-        
-        # get overall influence function
-        calendar_inf_func = get_agg_inf_func(att=calendar_att_t,
-                                             inffunc=calendar_inf_func_t,
-                                             whichones=range(len(calendar_tlist)),
-                                             weights_agg=np.repeat(1/len(calendar_tlist), len(calendar_tlist)),
-                                             wif=None)[:, None]
-        calendar_inf_func = np.array(calendar_inf_func)
-        
-        # get overall standard error
-        calendar_se = get_se(calendar_inf_func, dp)
-        if not np.isnan(calendar_se):
-            if calendar_se <= np.sqrt(np.finfo(float).eps) * 10:
-                calendar_se = np.nan
-        
-        AGGTEobj_print = AGGTEobj(overall_att=calendar_att,
-                                overall_se=calendar_se,
-                                typec=typec,
-                                egt=list(map(t2orig, calendar_tlist)),
-                                att_egt=calendar_att_t,
-                                se_egt=calendar_se_t,
-                                crit_val_egt=calendar_crit_val,
-                                inf_function={"calendar_inf_func_t": calendar_inf_func_t,
-                                              "calendar_inf_func": calendar_inf_func},
-                                call=call,
-                                DIDparams=dp)
-    
-        return AGGTEobj_print
+import pickle
+import pandas as pd
+import numpy as np
+from scipy.stats import norm
+
+
+from csdid.aggte_fnc.utils import get_agg_inf_func, get_se, wif, AGGTEobj
+from csdid.utils.mboot import mboot
+import warnings
+
+def compute_aggte(MP,
+                      typec         = "group",
+                      balance_e     = None,
+                      min_e         = float('-inf'),
+                      max_e         = float('inf'),
+                      na_rm         = False,
+                      bstrap        = None,
+                      biters        = None,
+                      cband         = None,
+                      alp           = None,
+                      clustervars   = None,
+                      call          = None):
+  
+# =============================================================================
+# unpack MP object
+# =============================================================================
+    group       = np.array( MP['group'] )
+    t           = np.array( MP['t']     )
+    att         = np.array( MP['att'] )
+    dp          = MP['DIDparams']
+    tlist       = np.array( dp['tlist'] )
+    glist       = np.array( dp['glist'] )
+    data        = pd.DataFrame( dp['data'] )    
+    inffunc     = MP['inffunc']['inffunc']
+    n           = MP['n']
+    gname       = dp['gname']
+    tname       = dp['tname']
+    idname      = dp['idname']
+    # typec       = MP['type']  
+    panel       = dp['panel']    
+
+
+    
+    if clustervars is None:
+        clustervars = dp['clustervars']
+    if bstrap is None:
+        bstrap = dp['bstrap']
+    if biters is None:
+        biters = dp['biters']
+    if alp is None:
+        alp = dp['alp']
+    if cband is None:
+        cband = dp['cband']
+
+
+
+    # Overwrite MP objects (to compute bootstrap)
+    MP['DIDparams']['clustervars'] = clustervars
+    MP['DIDparams']['bstrap'] = bstrap
+    MP['DIDparams']['biters'] = biters
+    MP['DIDparams']['alp'] = alp
+    MP['DIDparams']['cband'] = cband
+    
+# =============================================================================
+#  Treat data
+# =============================================================================
+
+    if typec not in ["simple", "dynamic", "group", "calendar"]:
+        raise ValueError("`typec` must be one of ['simple', 'dynamic', 'group', 'calendar']")
+    # Removing missing values    
+    if na_rm:
+        notna = ~np.isnan(att)
+        group = group[notna]
+        t = t[notna]
+        att = att[notna]
+        inffunc = inffunc[:, notna]
+        glist = np.sort(np.unique(group))
+    
+        if typec == "group":
+            gnotna = []
+            for g in glist:
+                indices = np.where((group == g) & (g <= t))
+                is_not_na = np.any(~np.isnan(att[indices]))
+                gnotna.append(is_not_na)
+            
+            gnotna = np.array(gnotna)
+            glist = glist[gnotna]
+            not_all_na = np.isin(group, glist)
+            group = group[not_all_na]
+            t = t[not_all_na]
+            att = att[not_all_na]
+            inffunc = inffunc[:, not_all_na]
+            glist = np.sort(np.unique(group))
+
+    
+    if (not na_rm) and np.any(np.isnan(att)):
+        raise ValueError("Missing values at att_gt found. If you want to remove these, set `na_rm = True`.")
+
+    if panel:
+        dta = data[data[tname] == tlist[0]]
+    else:
+        dta = data.groupby(idname).mean().reset_index()
+        dta = dta.iloc[:, 1:]
+
+# =============================================================================
+#  Treat data 2
+# =============================================================================
+
+    
+    originalt = t
+    originalgroup = group
+    originalglist = glist
+    originaltlist = tlist
+    # In case g's are not part of tlist
+    originalgtlist = np.sort(np.unique(np.concatenate((originaltlist, originalglist))))
+    uniquet = list(range(1, len(originalgtlist) + 1))
+    
+    # Function to switch from "new" t values to original t values
+    def t2orig(t):
+        return originalgtlist[uniquet.index(t) if t in uniquet else -1]
+    
+    # Function to switch between "original" t values and new t values
+    def orig2t(orig):
+        new_t = [uniquet[i] for i in range(len(originalgtlist)) if originalgtlist[i] == orig]
+        out = new_t[0] if new_t else None
+        return out
+    
+    t     = [orig2t(orig) for orig in originalt]
+    group = [orig2t(orig) for orig in originalgroup]
+    glist = [orig2t(orig) for orig in originalglist]
+    tlist = np.asarray(list(set(t)))
+    maxT  = max(t)
+        
+    # Set the weights
+    weights_ind = dta['.w']
+    
+    # We can work in overall probabilities because conditioning will cancel out
+    # since it shows up in numerator and denominator
+    pg = np.array([np.mean(weights_ind * (dta[gname] == g)) for g in originalglist])
+    
+    # Length of this is equal to the number of groups
+    pgg = pg
+
+    # Same but length is equal to the number of ATT(g,t)
+    pg = [pg[glist.index(g)] for g in group]  
+    
+    # Which group time average treatment effects are post-treatment
+    keepers = [i for i in range(len(group)) if group[i] <= t[i] <= (group[i] + max_e)] ### added second condition to allow for limit on longest period included in att
+    
+    # n x 1 vector of group variable
+    G = [orig2t(g) for g in dta[gname]]
+
+# =============================================================================
+#  simple
+# =============================================================================
+
+
+    if typec == "simple":
+        # Simple ATT
+        # Averages all post-treatment ATT(g,t) with weights given by group size
+        pg = np.array(pg)
+        simple_att = np.sum(att[keepers] * pg[keepers]) / np.sum(pg[keepers])
+        if np.isnan(simple_att):
+            simple_att = None
+    
+        # Get the part of the influence function coming from estimated weights
+        simple_wif = wif(keepers, pg, weights_ind, G, group)
+    
+        # Get the overall influence function
+        simple_if = get_agg_inf_func(att = att , 
+                                     inffunc = inffunc , 
+                                     whichones = keepers ,
+                                     weights_agg = np.array(pg)[keepers]/np.sum(np.array(pg)[keepers]) , 
+                                     wif = simple_wif )[:, None]
+    
+        # Get standard errors from the overall influence function
+        simple_se = get_se(simple_if, dp)
+        
+        if simple_se is not None:
+            if simple_se <= np.sqrt(np.finfo(float).eps) * 10:
+                simple_se = None
+                
+        AGGTEobj_print = AGGTEobj(overall_att=simple_att, 
+                                  overall_se=simple_se, 
+                                  typec=typec,
+                                  inf_function={'simple_att': simple_if}, 
+                                  call=call, DIDparams=dp)
+        
+        return AGGTEobj_print
+
+
+# =============================================================================
+#  GRoup
+# =============================================================================
+
+    if typec == "group":
+        group = np.array(group)
+        t = np.array(t) 
+        pg = np.array(pg) 
+        selective_att_g = [np.mean(att[( group== g) & (t >= g) & (t <= (group + max_e))]) for g in glist]
+        selective_att_g = np.asarray(selective_att_g)
+        selective_att_g[np.isnan(selective_att_g)] = None
+    
+        selective_se_inner = [None] * len(glist)
+        for i, g in enumerate(glist):
+            whichg = np.where(np.logical_and.reduce((group == g, g <= t, t <= (group + max_e))))[0]
+            weightsg =  pg[whichg] / np.sum(pg[whichg])
+            inf_func_g = get_agg_inf_func(att = att , 
+                                            inffunc = inffunc , 
+                                            whichones = whichg ,
+                                            weights_agg = weightsg , 
+                                            wif = None)[:, None]
+            se_g = get_se(inf_func_g, dp)
+            selective_se_inner[i] = {'inf_func': inf_func_g, 'se': se_g}
+            
+        # recover standard errors separately by group   
+        selective_se_g = np.asarray([item['se'] for item in selective_se_inner]).T
+        
+        selective_se_g[selective_se_g <= np.sqrt(np.finfo(float).eps) * 10] = None
+        
+        selective_inf_func_g = np.column_stack([elem["inf_func"] for elem in selective_se_inner])
+  
+        # use multiplier bootstrap (across groups) to get critical value
+        # for constructing uniform confidence bands   
+        selective_crit_val = norm.ppf(1 - alp/2)
+        
+        if dp['cband']:
+            if not dp['bstrap']:
+                print("Used bootstrap procedure to compute simultaneous confidence band")
+        
+            selective_crit_val = mboot(selective_inf_func_g, dp)['crit_val']
+        
+            if np.isnan(selective_crit_val) or np.isinf(selective_crit_val):
+                print("Simultaneous critical value is NA. This probably happened because we cannot compute t-statistic (std errors are NA). We then report pointwise conf. intervals.")
+                selective_crit_val = norm.ppf(1 - alp/2)
+                dp['cband'] = False
+        
+            if selective_crit_val < norm.ppf(1 - alp/2):
+                print("Simultaneous conf. band is somehow smaller than pointwise one using normal approximation. Since this is unusual, we are reporting pointwise confidence intervals")
+                selective_crit_val = norm.ppf(1 - alp/2)
+                dp['cband'] = False
+        
+            if selective_crit_val >= 7:
+                print("Simultaneous critical value is arguably 'too large' to be reliable. This usually happens when the number of observations per group is small and/or there is not much variation in outcomes.")
+  
+        # get overall att under selective treatment timing
+        # (here use pgg instead of pg because we can just look at each group)            
+        selective_att = np.sum(selective_att_g * pgg) / np.sum(pgg)
+        
+        # account for having to estimate pgg in the influence function    
+        selective_wif = wif(keepers = np.arange(1, len(glist)+1)-1, 
+                            pg  = pgg, 
+                            weights_ind = weights_ind, 
+                            G = G, 
+                            group = group)
+        
+        # get overall influence function   
+        selective_inf_func = get_agg_inf_func(att = selective_att_g, 
+                                              inffunc = selective_inf_func_g,
+                                              whichones = np.arange(1, len(glist)+1)-1, 
+                                              weights_agg = pgg/np.sum(pgg),
+                                              wif = selective_wif)[:, None]    
+        
+        # get overall standard error        
+        selective_se = get_se(selective_inf_func, dp)
+        if not np.isnan(selective_se):
+            if selective_se <= np.sqrt(np.finfo(float).eps) * 10:
+                selective_se = None
+    
+        AGGTEobj_print = AGGTEobj(overall_att = selective_att, 
+                            overall_se = selective_se, 
+                            typec = typec,
+                            egt = originalglist,
+                            att_egt = selective_att_g,
+                            se_egt = selective_se_g,
+                            crit_val_egt = selective_crit_val,
+                            inf_function = {'selective_inf_func_g': selective_inf_func_g, 
+                                            'selective_inf_func': selective_inf_func},
+                            call = call, 
+                            DIDparams = dp)
+
+        return AGGTEobj_print
+
+
+# =============================================================================
+#  Dynamic
+# =============================================================================
+
+    if typec == "dynamic":
+        # event times
+        # this looks at all available event times
+        # note: event times can be negative here.
+        # note: event time = 0 corresponds to "on impact"
+        eseq = np.unique(np.array(originalt) - np.array(originalgroup) ) # Subtract corresponding elements and convert to NumPy array
+        eseq = np.sort(eseq)  # Sort the unique values in ascending order
+    
+        # if the user specifies balance_e, then we are going to
+        # drop some event times and some groups; if not, we just
+        # keep everything (that is what this variable is for)
+        originalt = np.array(originalt)
+        originalgroup = np.array(originalgroup)
+        pg = np.array(pg)
+        include_balanced_gt = np.repeat(True, len(originalgroup))
+
+        if balance_e is not None:
+            include_balanced_gt = (t2orig(maxT) - originalgroup >= balance_e)        
+            eseq = np.unique(originalt[include_balanced_gt] - originalgroup[include_balanced_gt])
+            eseq = np.sort(eseq)      
+            eseq = eseq[(eseq <= balance_e) & (eseq >= balance_e - t2orig(maxT) + t2orig(1))]
+        eseq = eseq[(eseq >= min_e) & (eseq <= max_e)]
+
+        dynamic_att_e = []
+        for e in eseq:
+            whiche = np.where((originalt - originalgroup == e) & include_balanced_gt)
+            atte = att[whiche]
+            pge = pg[whiche] / np.sum(pg[whiche])
+            dynamic_att_e.append(np.sum(atte * pge))
+        
+        dynamic_se_inner = []
+        for e in eseq:
+            whiche = np.where((originalt - originalgroup == e) & (include_balanced_gt) )[0]
+            pge = pg[whiche] / sum(pg[whiche])
+            wif_e = wif(whiche, 
+                        pg, 
+                        weights_ind, 
+                        G, 
+                        group)
+            inf_func_e = get_agg_inf_func(att         = att, 
+                                          inffunc     = inffunc, 
+                                          whichones   = whiche, 
+                                          weights_agg = pge, 
+                                          wif         = wif_e)[:, None]
+            se_e = get_se(inf_func_e, dp)
+            dynamic_se_inner.append({'inf_func': inf_func_e, 'se': se_e})
+
+        dynamic_se_e = np.array([item['se'] for item in dynamic_se_inner]).T
+        
+        dynamic_se_e[dynamic_se_e <= np.sqrt(np.finfo(float).eps) * 10] = np.nan
+        
+        dynamic_inf_func_e = np.column_stack([item['inf_func'] for item in dynamic_se_inner])
+                
+        dynamic_crit_val = norm.ppf(1 - alp/2)
+        if dp['cband']:
+            if not dp['bstrap']:
+                print('Used bootstrap procedure to compute simultaneous confidence band')
+            dynamic_crit_val = mboot(dynamic_inf_func_e, dp)['crit_val']
+        
+            if np.isnan(dynamic_crit_val) or np.isinf(dynamic_crit_val):
+                print('Simultaneous critical value is NA. This probably happened because we cannot compute t-statistic (std errors are NA). We then report pointwise conf. intervals.')
+                dynamic_crit_val = norm.ppf(1 - alp/2)
+                dp['cband'] = False
+        
+            if dynamic_crit_val < norm.ppf(1 - alp/2):
+                print('Simultaneous conf. band is somehow smaller than pointwise one using normal approximation. Since this is unusual, we are reporting pointwise confidence intervals')
+                dynamic_crit_val = norm.ppf(1 - alp/2)
+                dp['cband'] = False
+        
+            if dynamic_crit_val >= 7:
+                print("Simultaneous critical value is arguably 'too large' to be reliable. This usually happens when the number of observations per group is small and/or there is not much variation in outcomes.")
+
+            epos = eseq >= 0
+            dynamic_att = np.mean(np.array(dynamic_att_e)[epos])
+            dynamic_inf_func = get_agg_inf_func(att         = np.array(dynamic_att_e)[epos],
+                                                inffunc     = np.array(dynamic_inf_func_e[:, epos]),
+                                                whichones   = np.arange(1, np.sum(epos)+1)-1,
+                                                weights_agg = np.repeat(1 / np.sum(epos), np.sum(epos)),
+                                                wif=None)[:, None]
+            
+            dynamic_se = get_se(dynamic_inf_func, dp)
+            if not np.isnan(dynamic_se):
+                if dynamic_se <= np.sqrt(np.finfo(float).eps) * 10:
+                    dynamic_se = np.nan
+
+        AGGTEobj_print = AGGTEobj(overall_att=dynamic_att,
+                                overall_se=dynamic_se,
+                                typec=typec,
+                                egt=eseq,
+                                att_egt=dynamic_att_e,
+                                se_egt=dynamic_se_e,
+                                crit_val_egt=dynamic_crit_val,
+                                inf_function={'dynamic_inf_func_e': dynamic_inf_func_e,
+                                              'dynamic_inf_func': dynamic_inf_func},
+                                call=call,
+                                min_e=min_e,
+                                max_e=max_e,
+                                balance_e=balance_e,
+                                DIDparams=dp)
+            
+        return AGGTEobj_print
+
+
+
+# =============================================================================
+#  Calendar
+# =============================================================================
+
+ # np.array(group)
+    if typec == "calendar":
+        minG = min(group)
+        calendar_tlist = tlist[tlist >= minG]
+        pg = np.array(pg)
+        calendar_att_t = []
+        group = np.array(group)
+        t = np.array(t)
+        for t1 in calendar_tlist:
+            whicht = np.where((t == t1) & (group <= t))[0]
+            attt = att[whicht]
+            pgt = pg[whicht] / np.sum(pg[whicht])
+            calendar_att_t.append(np.sum(pgt * attt))
+            
+        # get standard errors and influence functions
+        # for each time specific att
+        calendar_se_inner = []
+        for t1 in calendar_tlist:
+            which_t = np.where((t == t1) & (group <= t))[0]
+            pgt = pg[which_t] / np.sum(pg[which_t])
+            wif_t = wif(keepers=which_t, 
+                        pg=pg, 
+                        weights_ind=weights_ind, 
+                        G=G, 
+                        group=group)
+            inf_func_t = get_agg_inf_func(att=att, 
+                                            inffunc=inffunc, 
+                                            whichones=which_t, 
+                                            weights_agg=pgt, 
+                                            wif=wif_t)[:, None]
+            se_t = get_se(inf_func_t, dp)
+            calendar_se_inner.append({"inf_func": inf_func_t, "se": se_t})
+    
+    
+    
+        # recover standard errors separately by time
+        calendar_se_t = np.array([se["se"] for se in calendar_se_inner]).T
+        calendar_se_t[calendar_se_t <= np.sqrt(np.finfo(float).eps) * 10] = np.nan
+        
+        # recover influence function separately by time
+        calendar_inf_func_t = np.column_stack([se["inf_func"] for se in calendar_se_inner])
+    
+        # use multiplier boostrap (across groups) to get critical value
+        # for constructing uniform confidence bands
+        calendar_crit_val = norm.ppf(1 - alp/2)
+        
+        if dp['cband']:
+            if not dp['bstrap']:
+                warnings.warn('Used bootstrap procedure to compute simultaneous confidence band')
+        
+            # mboot function is not provided, please define it separately
+            calendar_crit_val = mboot(calendar_inf_func_t, dp)['crit_val']
+        
+            if np.isnan(calendar_crit_val) or np.isinf(calendar_crit_val):
+                warnings.warn('Simultaneous critical value is NA. This probably happened because we cannot compute t-statistic (std errors are NA). We then report pointwise conf. intervals.')
+                calendar_crit_val = norm.ppf(1 - alp/2)
+                dp['cband'] = False
+        
+            if calendar_crit_val < norm.ppf(1 - alp/2):
+                warnings.warn('Simultaneous conf. band is somehow smaller than pointwise one using normal approximation. Since this is unusual, we are reporting pointwise confidence intervals.')
+                calendar_crit_val = norm.ppf(1 - alp/2)
+                dp['cband'] = False
+        
+            if calendar_crit_val >= 7:
+                warnings.warn("Simultaneous critical value is arguably 'too large' to be reliable. This usually happens when the number of observations per group is small and/or there is not much variation in outcomes.")
+    
+    
+        # get overall att under calendar time effects
+        # this is just average over all time periods
+        calendar_att = np.mean(calendar_att_t)
+        
+        # get overall influence function
+        calendar_inf_func = get_agg_inf_func(att=calendar_att_t,
+                                             inffunc=calendar_inf_func_t,
+                                             whichones=range(len(calendar_tlist)),
+                                             weights_agg=np.repeat(1/len(calendar_tlist), len(calendar_tlist)),
+                                             wif=None)[:, None]
+        calendar_inf_func = np.array(calendar_inf_func)
+        
+        # get overall standard error
+        calendar_se = get_se(calendar_inf_func, dp)
+        if not np.isnan(calendar_se):
+            if calendar_se <= np.sqrt(np.finfo(float).eps) * 10:
+                calendar_se = np.nan
+        
+        AGGTEobj_print = AGGTEobj(overall_att=calendar_att,
+                                overall_se=calendar_se,
+                                typec=typec,
+                                egt=list(map(t2orig, calendar_tlist)),
+                                att_egt=calendar_att_t,
+                                se_egt=calendar_se_t,
+                                crit_val_egt=calendar_crit_val,
+                                inf_function={"calendar_inf_func_t": calendar_inf_func_t,
+                                              "calendar_inf_func": calendar_inf_func},
+                                call=call,
+                                DIDparams=dp)
+    
+        return AGGTEobj_print
```

### Comparing `csdid-0.1.81/csdid/att_gt.py` & `csdid-0.1.82/csdid/att_gt.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,218 +1,218 @@
-# from aggte import AGGte
-from csdid.aggte_fnc.aggte import aggte as agg_te
-
-from csdid.attgt_fnc.preprocess_did import pre_process_did
-from csdid.attgt_fnc.compute_att_gt import compute_att_gt
-
-from csdid.utils.mboot import mboot
-
-from csdid.plots.gplot import gplot, splot
-
-
-from plotnine import ggplot, facet_wrap
-
-
-import numpy as np, pandas as pd
-
-# class ATTgt(AGGte):
-class ATTgt:
-  def __init__(self, yname, tname, idname, gname, data, control_group = ['nevertreated', 'notyertreated'], 
-  xformla: str = None, panel = True, allow_unbalanced_panel = True, 
-  clustervar = None, weights_name = None, anticipation = 0, 
-  cband = False, biters = 1000, alp = 0.05
-  ):
-    dp = pre_process_did(
-      yname=yname, tname = tname, idname=idname, gname = gname,
-      data = data, control_group=control_group, anticipation=anticipation,
-      xformla=xformla, panel=panel, allow_unbalanced_panel=allow_unbalanced_panel, cband=cband, clustervar=None, weights_name=None
-    )
-
-    dp['biters'] = biters
-    dp['alp'] = alp
-    dp['true_repeated_cross_sections'] = dp['true_rep_cross_section']
-    dp['cband'] = cband
-    self.dp = dp
-
-  def fit(self, est_method = 'dr', base_period = 'varying', bstrap = True):
-    # print(self.dp)
-    dp = self.dp
-    result, inffunc = compute_att_gt(dp)
-    att = result['att']
-    if bstrap:
-      ref_se = mboot(inffunc.T, dp)
-      crit_val, se = ref_se['crit_val'], ref_se['se']
-      V = ref_se['V']
-    
-    ############# aggte input
-    group = result['group']
-    att = result['att']
-    tt = result['year']
-    inf_fnc = {'inffunc': inffunc.T}
-
-    dp['bstrap'] = bstrap
-    dp['est_method'] = est_method
-    dp['base_period'] = base_period
-    self.dp = dp
-    n = dp['n']
-
-    mp = {
-      'group': group, 'att': att, 't': tt,
-      'DIDparams': dp, 'inffunc': inf_fnc, 
-      'n': n
-    }
-    self.MP = mp
-
-
-    cband_lower = att - crit_val * se
-    cband_upper = att + crit_val * se
-    sig = (cband_upper < 0) | (cband_lower > 0)
-    sig[np.isnan(sig)] = False
-    sig_text = np.where(sig, "*", "")
-
-    result.update(
-      {
-        'se': se, 'l_se': cband_lower,
-        'c': crit_val,
-        'u_se': cband_upper, 'sig': sig_text
-       })
-    
-    self.results = result
-
-    rst = result
-    did_object = {
-      'group': mp['group'],
-      't': mp['t'],
-      'att': rst['att'],
-      'se': rst['se'],
-      'c': rst['c'],
-    }
-    self.did_object = did_object
-    return self
-  def summ_attgt(self, n = 4):
-    result = self.results
-    att_gt = pd.DataFrame(result)
-    att_gt = att_gt.drop('c', axis=1)
-    name_attgt_df = ['Group', 'Time', 'ATT(g, t)', 'Post', "Std. Error", "[95% Pointwise", 'Conf. Band]', '']
-    att_gt.columns = name_attgt_df
-    att_gt = att_gt.round(n)
-    self.summary2 = att_gt
-    return self
-
-  def aggte(
-    self, 
-    typec         = "group",
-    balance_e     = None,
-    min_e         = float('-inf'),
-    max_e         = float('inf'),
-    na_rm         = False,
-    bstrap        = None,
-    biters        = None,
-    cband         = None,
-    alp           = None,
-    clustervars   = None,
-    ):
-    mp = self.MP
-    did_object = self.did_object
-    
-    did_object.update({
-      'type': typec
-      }
-    )
-
-
-    atte = agg_te(
-      mp, typec=typec, balance_e=balance_e, 
-      min_e=min_e, max_e=max_e, na_rm=na_rm, bstrap=bstrap, 
-      biters=biters, cband=cband, alp=alp, clustervars=clustervars
-    )
-
-    self.atte = atte
-    return self
-  def plot_attgt(self, ylim=None, 
-                xlab=None, 
-                ylab=None, 
-                title="Group",
-                xgap=1, 
-                ncol=1, 
-                legend=True, 
-                group=None, 
-                ref_line=0,
-                theming=True, 
-                grtitle="Group"
-                ):
-
-    did_object = self.did_object
-
-    grp = did_object['group']
-    t_i = did_object['t']
-
-    G = len(np.unique(grp))
-    Y = len(np.unique(t_i))
-    g = np.unique(grp)[np.argsort(np.unique(grp))].astype(int)
-    y = np.unique(t_i)
-
-    results = pd.DataFrame({'year': np.tile(y, G)})
-    results['group'] = np.repeat(g, Y)
-    results['grtitle'] = grtitle + ' ' + results['group'].astype(str)
-    results['att'] = did_object['att']
-    results['att_se'] = did_object['se']
-    results['post'] = np.where(results['year'] >= grp, 1, 0)
-    results['year'] = results['year']
-    results['c'] = did_object['c']
-
-    if group is None:
-      group = g
-      if any(group not in g for group in group):
-        raise ValueError("Some of the specified groups do not exist in the data. Reporting all available groups.")
-
-
-    results = results.query(
-      'group in @group'
-      )
-    
-    self.data_plot_attgt = results
-
-    mplots = gplot(results, ylim, xlab, ylab, title, xgap, legend, ref_line, theming) + \
-              facet_wrap('~ grtitle', ncol=ncol, scales='free')
-
-    return mplots 
-  def plot_aggte(self, ylim=None, 
-                   xlab=None, 
-                   ylab=None, 
-                   title="", 
-                   xgap=1, 
-                   legend=True, 
-                   ref_line=0, 
-                   theming=True,
-                   **kwargs):
-
-    did_object = self.atte
-
-    post_treat = 1 * (np.asarray(did_object["egt"]).astype(int) >= 0)
-    
-    results = {
-        "year": list(map(int, did_object["egt"])),
-        "att": did_object["att_egt"],
-        "att_se": did_object["se_egt"][0],
-        "post": post_treat
-    }
-    
-    results = pd.DataFrame(results)
-    
-    if did_object['crit_val_egt'] is None:
-        results['c'] = abs(norm.ppf(0.025))
-    else:
-        results['c'] = did_object['crit_val_egt']
-
-    if title == "":
-        title = "Average Effect by Group" if\
-          did_object["type"] == "group" else\
-            "Average Effect by Length of Exposure"
-
-    if did_object['type'] == 'group':
-        p = splot(results, ylim, xlab, ylab, title, legend, ref_line, theming)
-    else:
-        p = gplot(results, ylim, xlab, ylab, title, xgap, legend, ref_line, theming)
-    # p
-    # print(p) 
-    return p
+# from aggte import AGGte
+from csdid.aggte_fnc.aggte import aggte as agg_te
+
+from csdid.attgt_fnc.preprocess_did import pre_process_did
+from csdid.attgt_fnc.compute_att_gt import compute_att_gt
+
+from csdid.utils.mboot import mboot
+
+from csdid.plots.gplot import gplot, splot
+
+
+from plotnine import ggplot, facet_wrap
+
+
+import numpy as np, pandas as pd
+
+# class ATTgt(AGGte):
+class ATTgt:
+  def __init__(self, yname, tname, idname, gname, data, control_group = ['nevertreated', 'notyertreated'], 
+  xformla: str = None, panel = True, allow_unbalanced_panel = True, 
+  clustervar = None, weights_name = None, anticipation = 0, 
+  cband = False, biters = 1000, alp = 0.05
+  ):
+    dp = pre_process_did(
+      yname=yname, tname = tname, idname=idname, gname = gname,
+      data = data, control_group=control_group, anticipation=anticipation,
+      xformla=xformla, panel=panel, allow_unbalanced_panel=allow_unbalanced_panel, cband=cband, clustervar=None, weights_name=None
+    )
+
+    dp['biters'] = biters
+    dp['alp'] = alp
+    dp['true_repeated_cross_sections'] = dp['true_rep_cross_section']
+    dp['cband'] = cband
+    self.dp = dp
+
+  def fit(self, est_method = 'dr', base_period = 'varying', bstrap = True):
+    # print(self.dp)
+    dp = self.dp
+    result, inffunc = compute_att_gt(dp)
+    att = result['att']
+    if bstrap:
+      ref_se = mboot(inffunc.T, dp)
+      crit_val, se = ref_se['crit_val'], ref_se['se']
+      V = ref_se['V']
+    
+    ############# aggte input
+    group = result['group']
+    att = result['att']
+    tt = result['year']
+    inf_fnc = {'inffunc': inffunc.T}
+
+    dp['bstrap'] = bstrap
+    dp['est_method'] = est_method
+    dp['base_period'] = base_period
+    self.dp = dp
+    n = dp['n']
+
+    mp = {
+      'group': group, 'att': att, 't': tt,
+      'DIDparams': dp, 'inffunc': inf_fnc, 
+      'n': n
+    }
+    self.MP = mp
+
+
+    cband_lower = att - crit_val * se
+    cband_upper = att + crit_val * se
+    sig = (cband_upper < 0) | (cband_lower > 0)
+    sig[np.isnan(sig)] = False
+    sig_text = np.where(sig, "*", "")
+
+    result.update(
+      {
+        'se': se, 'l_se': cband_lower,
+        'c': crit_val,
+        'u_se': cband_upper, 'sig': sig_text
+       })
+    
+    self.results = result
+
+    rst = result
+    did_object = {
+      'group': mp['group'],
+      't': mp['t'],
+      'att': rst['att'],
+      'se': rst['se'],
+      'c': rst['c'],
+    }
+    self.did_object = did_object
+    return self
+  def summ_attgt(self, n = 4):
+    result = self.results
+    att_gt = pd.DataFrame(result)
+    att_gt = att_gt.drop('c', axis=1)
+    name_attgt_df = ['Group', 'Time', 'ATT(g, t)', 'Post', "Std. Error", "[95% Pointwise", 'Conf. Band]', '']
+    att_gt.columns = name_attgt_df
+    att_gt = att_gt.round(n)
+    self.summary2 = att_gt
+    return self
+
+  def aggte(
+    self, 
+    typec         = "group",
+    balance_e     = None,
+    min_e         = float('-inf'),
+    max_e         = float('inf'),
+    na_rm         = False,
+    bstrap        = None,
+    biters        = None,
+    cband         = None,
+    alp           = None,
+    clustervars   = None,
+    ):
+    mp = self.MP
+    did_object = self.did_object
+    
+    did_object.update({
+      'type': typec
+      }
+    )
+
+
+    atte = agg_te(
+      mp, typec=typec, balance_e=balance_e, 
+      min_e=min_e, max_e=max_e, na_rm=na_rm, bstrap=bstrap, 
+      biters=biters, cband=cband, alp=alp, clustervars=clustervars
+    )
+
+    self.atte = atte
+    return self
+  def plot_attgt(self, ylim=None, 
+                xlab=None, 
+                ylab=None, 
+                title="Group",
+                xgap=1, 
+                ncol=1, 
+                legend=True, 
+                group=None, 
+                ref_line=0,
+                theming=True, 
+                grtitle="Group"
+                ):
+
+    did_object = self.did_object
+
+    grp = did_object['group']
+    t_i = did_object['t']
+
+    G = len(np.unique(grp))
+    Y = len(np.unique(t_i))
+    g = np.unique(grp)[np.argsort(np.unique(grp))].astype(int)
+    y = np.unique(t_i)
+
+    results = pd.DataFrame({'year': np.tile(y, G)})
+    results['group'] = np.repeat(g, Y)
+    results['grtitle'] = grtitle + ' ' + results['group'].astype(str)
+    results['att'] = did_object['att']
+    results['att_se'] = did_object['se']
+    results['post'] = np.where(results['year'] >= grp, 1, 0)
+    results['year'] = results['year']
+    results['c'] = did_object['c']
+
+    if group is None:
+      group = g
+      if any(group not in g for group in group):
+        raise ValueError("Some of the specified groups do not exist in the data. Reporting all available groups.")
+
+
+    results = results.query(
+      'group in @group'
+      )
+    
+    self.data_plot_attgt = results
+
+    mplots = gplot(results, ylim, xlab, ylab, title, xgap, legend, ref_line, theming) + \
+              facet_wrap('~ grtitle', ncol=ncol, scales='free')
+
+    return mplots 
+  def plot_aggte(self, ylim=None, 
+                   xlab=None, 
+                   ylab=None, 
+                   title="", 
+                   xgap=1, 
+                   legend=True, 
+                   ref_line=0, 
+                   theming=True,
+                   **kwargs):
+
+    did_object = self.atte
+
+    post_treat = 1 * (np.asarray(did_object["egt"]).astype(int) >= 0)
+    
+    results = {
+        "year": list(map(int, did_object["egt"])),
+        "att": did_object["att_egt"],
+        "att_se": did_object["se_egt"][0],
+        "post": post_treat
+    }
+    
+    results = pd.DataFrame(results)
+    
+    if did_object['crit_val_egt'] is None:
+        results['c'] = abs(norm.ppf(0.025))
+    else:
+        results['c'] = did_object['crit_val_egt']
+
+    if title == "":
+        title = "Average Effect by Group" if\
+          did_object["type"] == "group" else\
+            "Average Effect by Length of Exposure"
+
+    if did_object['type'] == 'group':
+        p = splot(results, ylim, xlab, ylab, title, legend, ref_line, theming)
+    else:
+        p = gplot(results, ylim, xlab, ylab, title, xgap, legend, ref_line, theming)
+    # p
+    # print(p) 
+    return p
```

### Comparing `csdid-0.1.81/csdid/attgt_fnc/compute_att_gt.py` & `csdid-0.1.82/csdid/attgt_fnc/compute_att_gt.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,195 +1,195 @@
-import numpy as np, pandas as pd
-import patsy 
-from drdid import drdid, reg_did
-
-from csdid.utils.bmisc import panel2cs2
-
-fml = patsy.dmatrices
-
-
-# data Struct
-# output = {
-#   "att" : []
-#   'group': []
-#   'year': []
-#   'post ': []
-# }
-
-
-def compute_att_gt(dp, est_method = "dr", base_period = 'varying'):
-  yname = dp['yname']
-  tname = dp['tname']
-  idname = dp['idname']
-  xformla = dp['xformla']
-  data = dp['data']
-  weights_name = dp['weights_name']
-  # base_period = dp['base_period']
-  panel = dp['panel']
-  true_rep_cross_section = dp['true_rep_cross_section']
-  control_group = dp['control_group']
-  anticipation = dp['anticipation']
-  gname = dp['gname']
-  n = dp['n']
-  nT = dp['nT']
-  nG = dp['nG']
-  tlist = dp['tlist']
-  glist = dp['glist']
-  tlist_len, tfac = len(tlist), 0
-  if base_period != 'universal':
-    tlist_len = tlist_len - 1
-    tfac = 1
-
-  inf_func = []
-
-  att_est, group, year, post_array = [], [], [], []
-
-  def add_att_data(att = 0, pst = 0, inf_f = []):
-    inf_func.append(inf_f)
-    att_est.append(att)
-    group.append(g)
-    year.append(tn)
-    post_array.append(pst)
-
-  never_treated = control_group == 'nevertreated'
-  if never_treated:
-    data = data.assign(C = 1 * (data[gname] == 0))
-  data = data.assign(y_main = data[yname])
-
-  # g, t = glist[0], tlist[0]
-
-  for _, g, in enumerate(glist):
-    # g = glist[1]
-    G_main = (data[gname] == g)
-    data = data.assign(G_m = 1 * G_main)
-
-    for t_i in range(tlist_len):
-      pret = t_i
-      tn = tlist[t_i + tfac]
-      if base_period == 'universal' or g < tn:
-        try:
-          pret = np.where(tlist + anticipation < g)[0][-1]
-        except:
-          raise f"There are no pre-treatment periods for the group first treated at {g}\nUnits from this group are dropped"
-          # break
-
-
-      if base_period == 'universal':
-        if pret == tn:
-          add_att_data()
-
-      if not never_treated:
-        n1 = data[gname] == 0
-        n2 = (data[gname] > (tlist[np.max([t, pret]) + tfac]) + anticipation)
-        n3 = np.where(data[gname] != glist[g], True, False)
-        row_eval = n1 | n2 & n3
-        data = data.assign(C = 1 * row_eval)
-
-      post_treat = 1 * (g <= tn)
-      disdat = data[(data[tname] == tn) | (data[tname] == tlist[pret])]
-
-      if panel: 
-        #! delete
-        est_method = "reg"
-        disdat = panel2cs2(disdat, yname, idname, tname)
-        disdat = disdat.dropna()
-        n = len(disdat)
-        dis_idx = np.array(disdat.G_m == 1) | np.array(disdat.C == 1)
-        disdat = disdat.loc[dis_idx, :]
-        n1 = len(disdat)
-        G = disdat.G_m
-        C = disdat.C
-        w = disdat.w
-
-        ypre = disdat.y0 if tn > pret else disdat.y1
-        ypost = disdat.y0 if tn < pret else disdat.y1
-        _, covariates = fml(xformla, data = disdat, return_type = 'dataframe')
-
-        G, C, w, ypre = map(np.array, [G, C, w, ypre])
-        ypost, covariates = map(np.array, [ypost, covariates])
-
-        if callable(est_method):
-          est_att_f = est_method
-        elif est_method == "reg":
-          est_att_f = reg_did.reg_did_panel
-        elif est_method == "dr":
-          est_att_f = drdid.drdid_panel
-
-        att_gt, att_inf_func = est_att_f(ypost, ypre, G, i_weights=w, covariates=covariates)
-
-        inf_zeros = np.zeros(n)
-        att_inf = n / n1 * att_inf_func
-        inf_zeros[dis_idx] = att_inf
-
-        add_att_data(att_gt, inf_f=inf_zeros)
-
-      if not panel:
-        right_ids = np.array(disdat.query('(G_m == 1) or (C == 1)').rowid)
-        dis_idx = (data['rowid'].isin(right_ids)) &\
-          ((data[tname] == tlist[t_i + tfac]) |\
-            (data[tname] == tlist[pret]))
-
-        disdat = data.loc[dis_idx]
-
-        G = disdat.G_m
-        C = disdat.C
-        Y = disdat[yname]
-        post = 1 * (disdat[tname] == tlist[t_i + tfac])
-        w = disdat.w
-
-        G, C, Y, post, w = map(np.array, [G, C, Y, post, w])
-
-        n1 = sum(G + C)
-
-        skip_this_att_gt = False
-        if np.sum(G * post) == 0:
-          print(f"No units in group {g} in time period {tn}")
-          skip_this_att_gt = True 
-
-        if np.sum(G * (1 - post)) == 0:
-          print(f"No units in group {g} in time period {t}")
-          skip_this_att_gt = True 
-
-        if np.sum(C * post) == 0:
-          print(f"No available control units for group {g} in time period {tn}")
-          skip_this_att_gt = True 
-
-        if np.sum(C * (1 - post)) == 0:
-          print(f"No available control units for group {g} in time period {t}")
-          skip_this_att_gt = True 
-
-        if skip_this_att_gt:
-          add_att_data()
-
-        _, covariates = fml(xformla, data = disdat, return_type = 'dataframe')
-        covariates = np.array(covariates)
-        #! todo estmedho
-
-        if callable(est_method):
-          est_att_f = est_method
-        elif est_method == "reg":
-          est_att_f = reg_did.reg_did_rc
-        elif est_method == "dr":
-          est_att_f = drdid.drdid_rc
-        att_gt, att_inf_func = est_att_f(y=Y, post=post, D = G, i_weights=w, covariates=covariates)
-
-        inf_func_df = pd.DataFrame(
-          {
-            "inf_func": att_inf_func,
-            "right_ids": right_ids
-          }
-        )
-        inf_zeros = np.zeros(n)
-        aggte_infffuc = inf_func_df.groupby('right_ids').inf_func.sum()
-        dis_idx1 = np.isin(data['rowid'].unique(), aggte_infffuc.index)
-        inf_zeros[dis_idx1] = np.array(aggte_infffuc)
-
-        add_att_data(att_gt, pst = post_treat, inf_f=inf_zeros)
-        # print(att_est)
-
-  output = {
-    'group': group ,
-    'year': year,
-    "att" : att_est,
-    'post ': post_array
-  }
+import numpy as np, pandas as pd
+import patsy 
+from drdid import drdid, reg_did
+
+from csdid.utils.bmisc import panel2cs2
+
+fml = patsy.dmatrices
+
+
+# data Struct
+# output = {
+#   "att" : []
+#   'group': []
+#   'year': []
+#   'post ': []
+# }
+
+
+def compute_att_gt(dp, est_method = "dr", base_period = 'varying'):
+  yname = dp['yname']
+  tname = dp['tname']
+  idname = dp['idname']
+  xformla = dp['xformla']
+  data = dp['data']
+  weights_name = dp['weights_name']
+  # base_period = dp['base_period']
+  panel = dp['panel']
+  true_rep_cross_section = dp['true_rep_cross_section']
+  control_group = dp['control_group']
+  anticipation = dp['anticipation']
+  gname = dp['gname']
+  n = dp['n']
+  nT = dp['nT']
+  nG = dp['nG']
+  tlist = dp['tlist']
+  glist = dp['glist']
+  tlist_len, tfac = len(tlist), 0
+  if base_period != 'universal':
+    tlist_len = tlist_len - 1
+    tfac = 1
+
+  inf_func = []
+
+  att_est, group, year, post_array = [], [], [], []
+
+  def add_att_data(att = 0, pst = 0, inf_f = []):
+    inf_func.append(inf_f)
+    att_est.append(att)
+    group.append(g)
+    year.append(tn)
+    post_array.append(pst)
+
+  never_treated = control_group == 'nevertreated'
+  if never_treated:
+    data = data.assign(C = 1 * (data[gname] == 0))
+  data = data.assign(y_main = data[yname])
+
+  # g, t = glist[0], tlist[0]
+
+  for _, g, in enumerate(glist):
+    # g = glist[1]
+    G_main = (data[gname] == g)
+    data = data.assign(G_m = 1 * G_main)
+
+    for t_i in range(tlist_len):
+      pret = t_i
+      tn = tlist[t_i + tfac]
+      if base_period == 'universal' or g < tn:
+        try:
+          pret = np.where(tlist + anticipation < g)[0][-1]
+        except:
+          raise f"There are no pre-treatment periods for the group first treated at {g}\nUnits from this group are dropped"
+          # break
+
+
+      if base_period == 'universal':
+        if pret == tn:
+          add_att_data()
+
+      if not never_treated:
+        n1 = data[gname] == 0
+        n2 = (data[gname] > (tlist[np.max([t, pret]) + tfac]) + anticipation)
+        n3 = np.where(data[gname] != glist[g], True, False)
+        row_eval = n1 | n2 & n3
+        data = data.assign(C = 1 * row_eval)
+
+      post_treat = 1 * (g <= tn)
+      disdat = data[(data[tname] == tn) | (data[tname] == tlist[pret])]
+
+      if panel: 
+        #! delete
+        est_method = "reg"
+        disdat = panel2cs2(disdat, yname, idname, tname)
+        disdat = disdat.dropna()
+        n = len(disdat)
+        dis_idx = np.array(disdat.G_m == 1) | np.array(disdat.C == 1)
+        disdat = disdat.loc[dis_idx, :]
+        n1 = len(disdat)
+        G = disdat.G_m
+        C = disdat.C
+        w = disdat.w
+
+        ypre = disdat.y0 if tn > pret else disdat.y1
+        ypost = disdat.y0 if tn < pret else disdat.y1
+        _, covariates = fml(xformla, data = disdat, return_type = 'dataframe')
+
+        G, C, w, ypre = map(np.array, [G, C, w, ypre])
+        ypost, covariates = map(np.array, [ypost, covariates])
+
+        if callable(est_method):
+          est_att_f = est_method
+        elif est_method == "reg":
+          est_att_f = reg_did.reg_did_panel
+        elif est_method == "dr":
+          est_att_f = drdid.drdid_panel
+
+        att_gt, att_inf_func = est_att_f(ypost, ypre, G, i_weights=w, covariates=covariates)
+
+        inf_zeros = np.zeros(n)
+        att_inf = n / n1 * att_inf_func
+        inf_zeros[dis_idx] = att_inf
+
+        add_att_data(att_gt, inf_f=inf_zeros)
+
+      if not panel:
+        right_ids = np.array(disdat.query('(G_m == 1) or (C == 1)').rowid)
+        dis_idx = (data['rowid'].isin(right_ids)) &\
+          ((data[tname] == tlist[t_i + tfac]) |\
+            (data[tname] == tlist[pret]))
+
+        disdat = data.loc[dis_idx]
+
+        G = disdat.G_m
+        C = disdat.C
+        Y = disdat[yname]
+        post = 1 * (disdat[tname] == tlist[t_i + tfac])
+        w = disdat.w
+
+        G, C, Y, post, w = map(np.array, [G, C, Y, post, w])
+
+        n1 = sum(G + C)
+
+        skip_this_att_gt = False
+        if np.sum(G * post) == 0:
+          print(f"No units in group {g} in time period {tn}")
+          skip_this_att_gt = True 
+
+        if np.sum(G * (1 - post)) == 0:
+          print(f"No units in group {g} in time period {t}")
+          skip_this_att_gt = True 
+
+        if np.sum(C * post) == 0:
+          print(f"No available control units for group {g} in time period {tn}")
+          skip_this_att_gt = True 
+
+        if np.sum(C * (1 - post)) == 0:
+          print(f"No available control units for group {g} in time period {t}")
+          skip_this_att_gt = True 
+
+        if skip_this_att_gt:
+          add_att_data()
+
+        _, covariates = fml(xformla, data = disdat, return_type = 'dataframe')
+        covariates = np.array(covariates)
+        #! todo estmedho
+
+        if callable(est_method):
+          est_att_f = est_method
+        elif est_method == "reg":
+          est_att_f = reg_did.reg_did_rc
+        elif est_method == "dr":
+          est_att_f = drdid.drdid_rc
+        att_gt, att_inf_func = est_att_f(y=Y, post=post, D = G, i_weights=w, covariates=covariates)
+
+        inf_func_df = pd.DataFrame(
+          {
+            "inf_func": att_inf_func,
+            "right_ids": right_ids
+          }
+        )
+        inf_zeros = np.zeros(n)
+        aggte_infffuc = inf_func_df.groupby('right_ids').inf_func.sum()
+        dis_idx1 = np.isin(data['rowid'].unique(), aggte_infffuc.index)
+        inf_zeros[dis_idx1] = np.array(aggte_infffuc)
+
+        add_att_data(att_gt, pst = post_treat, inf_f=inf_zeros)
+        # print(att_est)
+
+  output = {
+    'group': group ,
+    'year': year,
+    "att" : att_est,
+    'post ': post_array
+  }
   return (output, np.array(inf_func))
```

### Comparing `csdid-0.1.81/csdid/attgt_fnc/preprocess_did.py` & `csdid-0.1.82/csdid/attgt_fnc/preprocess_did.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,337 +1,327 @@
-00000000: 0d0a 696d 706f 7274 2070 616e 6461 7320  ..import pandas 
-00000010: 6173 2070 642c 206e 756d 7079 2061 7320  as pd, numpy as 
-00000020: 6e70 0d0a 696d 706f 7274 2070 6174 7379  np..import patsy
-00000030: 200d 0a66 726f 6d20 6373 6469 642e 7574   ..from csdid.ut
-00000040: 696c 732e 626d 6973 6320 696d 706f 7274  ils.bmisc import
-00000050: 206d 616b 6542 616c 616e 6365 6450 616e   makeBalancedPan
-00000060: 656c 0d0a 0d0a 666d 6c20 3d20 7061 7473  el....fml = pats
-00000070: 792e 646d 6174 7269 6365 730d 0a0d 0a64  y.dmatrices....d
-00000080: 6566 2070 7265 5f70 726f 6365 7373 5f64  ef pre_process_d
-00000090: 6964 2879 6e61 6d65 2c20 746e 616d 652c  id(yname, tname,
-000000a0: 2069 646e 616d 652c 2067 6e61 6d65 2c20   idname, gname, 
-000000b0: 6461 7461 3a20 7064 2e44 6174 6146 7261  data: pd.DataFra
-000000c0: 6d65 2c20 0d0a 2020 636f 6e74 726f 6c5f  me, ..  control_
-000000d0: 6772 6f75 7020 3d20 5b27 6e65 7665 7274  group = ['nevert
-000000e0: 7265 6174 6564 272c 2027 6e6f 7479 6574  reated', 'notyet
-000000f0: 7472 6561 7465 6427 5d2c 200d 0a20 2061  treated'], ..  a
-00000100: 6e74 6963 6970 6174 696f 6e20 3d20 302c  nticipation = 0,
-00000110: 2078 666f 726d 6c61 203a 2073 7472 203d   xformla : str =
-00000120: 204e 6f6e 652c 0d0a 2020 7061 6e65 6c20   None,..  panel 
-00000130: 3d20 5472 7565 2c20 616c 6c6f 775f 756e  = True, allow_un
-00000140: 6261 6c61 6e63 6564 5f70 616e 656c 203d  balanced_panel =
-00000150: 2054 7275 652c 2063 6261 6e64 203d 2046   True, cband = F
-00000160: 616c 7365 2c0d 0a20 2063 6c75 7374 6572  alse,..  cluster
-00000170: 7661 7220 3d20 4e6f 6e65 2c20 2077 6569  var = None,  wei
-00000180: 6768 7473 5f6e 616d 6520 3d20 4e6f 6e65  ghts_name = None
-00000190: 0d0a 2020 2920 2d3e 2064 6963 743a 0d0a  ..  ) -> dict:..
-000001a0: 0d0a 2020 6e2c 2074 203d 2064 6174 612e  ..  n, t = data.
-000001b0: 7368 6170 650d 0a20 2063 6f6e 7472 6f6c  shape..  control
-000001c0: 5f67 726f 7570 203d 2063 6f6e 7472 6f6c  _group = control
-000001d0: 5f67 726f 7570 5b30 5d0d 0a20 2063 6f6c  _group[0]..  col
-000001e0: 756d 6e73 203d 205b 6964 6e61 6d65 2c20  umns = [idname, 
-000001f0: 746e 616d 652c 2079 6e61 6d65 2c20 676e  tname, yname, gn
-00000200: 616d 655d 0d0a 2020 2320 7072 696e 7428  ame]..  # print(
-00000210: 636f 6c75 6d6e 7329 0d0a 2020 2320 436f  columns)..  # Co
-00000220: 6c75 6d6e 730d 0a20 2069 6620 636c 7573  lumns..  if clus
-00000230: 7465 7276 6172 2069 7320 6e6f 7420 4e6f  tervar is not No
-00000240: 6e65 3a0d 0a20 2020 2063 6f6c 756d 6e73  ne:..    columns
-00000250: 202b 3d20 5b63 6c75 7374 6572 7661 725d   += [clustervar]
-00000260: 0d0a 2020 6966 2077 6569 6768 7473 5f6e  ..  if weights_n
-00000270: 616d 6520 6973 206e 6f74 204e 6f6e 653a  ame is not None:
-00000280: 0d0a 2020 2020 636f 6c75 6d6e 7320 2b3d  ..    columns +=
-00000290: 205b 7765 6967 6874 735f 6e61 6d65 5d0d   [weights_name].
-000002a0: 0a20 2020 2077 203d 2064 6174 615b 7765  .    w = data[we
-000002b0: 6967 6874 735f 6e61 6d65 5d0d 0a20 2065  ights_name]..  e
-000002c0: 6c73 653a 0d0a 2020 2020 7720 3d20 6e70  lse:..    w = np
-000002d0: 2e6f 6e65 7328 6e29 0d0a 0d0a 0d0a 2020  .ones(n)......  
-000002e0: 6966 2078 666f 726d 6c61 2069 7320 4e6f  if xformla is No
-000002f0: 6e65 3a0d 0a20 2020 2078 666f 726d 6c61  ne:..    xformla
-00000300: 203d 2066 277b 796e 616d 657d 207e 2031   = f'{yname} ~ 1
-00000310: 270d 0a20 205f 2c20 785f 636f 7620 3d20  '..  _, x_cov = 
-00000320: 666d 6c28 7866 6f72 6d6c 612c 2064 6174  fml(xformla, dat
-00000330: 6120 3d20 6461 7461 2c20 7265 7475 726e  a = data, return
-00000340: 5f74 7970 653d 2764 6174 6166 7261 6d65  _type='dataframe
-00000350: 2729 0d0a 2020 5f2c 206e 5f63 6f76 203d  ')..  _, n_cov =
-00000360: 2078 5f63 6f76 2e73 6861 7065 0d0a 0d0a   x_cov.shape....
-00000370: 0d0a 2020 6461 7461 203d 2070 642e 636f  ..  data = pd.co
-00000380: 6e63 6174 285b 6461 7461 5b63 6f6c 756d  ncat([data[colum
-00000390: 6e73 5d2c 2078 5f63 6f76 5d2c 2061 7869  ns], x_cov], axi
-000003a0: 733d 3129 0d0a 2020 6461 7461 203d 2064  s=1)..  data = d
-000003b0: 6174 612e 6173 7369 676e 2877 203d 2077  ata.assign(w = w
-000003c0: 290d 0a20 2064 6174 6120 3d20 6461 7461  )..  data = data
-000003d0: 2e64 726f 706e 6128 290d 0a20 206e 6469  .dropna()..  ndi
-000003e0: 6666 203d 206e 202d 206c 656e 2864 6174  ff = n - len(dat
-000003f0: 6129 200d 0a20 2069 6620 6e64 6966 6620  a) ..  if ndiff 
-00000400: 213d 2030 3a20 0d0a 2020 2020 7072 696e  != 0: ..    prin
-00000410: 7428 6627 6472 6f70 7065 642c 207b 6e64  t(f'dropped, {nd
-00000420: 6966 667d 2c20 726f 7773 2066 726f 6d20  iff}, rows from 
-00000430: 6f72 6967 696e 616c 2064 6174 6120 6475  original data du
-00000440: 6520 746f 206d 6973 7369 6e67 2064 6174  e to missing dat
-00000450: 6127 290d 0a0d 0a20 2074 6c69 7374 203d  a')....  tlist =
-00000460: 206e 702e 736f 7274 2864 6174 615b 746e   np.sort(data[tn
-00000470: 616d 655d 2e75 6e69 7175 6528 2929 0d0a  ame].unique())..
-00000480: 2020 676c 6973 7420 3d20 6e70 2e73 6f72    glist = np.sor
-00000490: 7428 6461 7461 5b67 6e61 6d65 5d2e 756e  t(data[gname].un
-000004a0: 6971 7565 2829 290d 0a0d 0a20 2061 7369  ique())....  asi
-000004b0: 665f 6e65 765f 7472 6561 7465 6420 3d20  f_nev_treated = 
-000004c0: 6461 7461 5b67 6e61 6d65 5d20 3e20 6e70  data[gname] > np
-000004d0: 2e6d 6178 2874 6c69 7374 290d 0a20 2061  .max(tlist)..  a
-000004e0: 7369 665f 6e65 765f 7472 6561 7465 642e  sif_nev_treated.
-000004f0: 6669 6c6c 6e61 2846 616c 7365 2c20 696e  fillna(False, in
-00000500: 706c 6163 653d 5472 7565 290d 0a20 2064  place=True)..  d
-00000510: 6174 612e 6c6f 635b 6173 6966 5f6e 6576  ata.loc[asif_nev
-00000520: 5f74 7265 6174 6564 2c20 676e 616d 655d  _treated, gname]
-00000530: 203d 2030 0d0a 0d0a 2020 6966 206c 656e   = 0....  if len
-00000540: 2867 6c69 7374 5b67 6c69 7374 203d 3d20  (glist[glist == 
-00000550: 305d 2920 3d3d 2030 3a0d 0a20 2020 2069  0]) == 0:..    i
-00000560: 6620 636f 6e74 726f 6c5f 6772 6f75 7020  f control_group 
-00000570: 3d3d 2022 6e65 7665 7274 7265 6174 6564  == "nevertreated
-00000580: 223a 0d0a 2020 2020 2020 7261 6973 6520  ":..      raise 
-00000590: 5661 6c75 6545 7272 6f72 2822 5468 6572  ValueError("Ther
-000005a0: 6520 6973 206e 6f20 6176 6169 6c61 626c  e is no availabl
-000005b0: 6520 6e65 7665 722d 7472 6561 7465 6420  e never-treated 
-000005c0: 6772 6f75 7022 290d 0a20 2020 2065 6c73  group")..    els
-000005d0: 653a 0d0a 2020 2020 2020 7661 6c75 6520  e:..      value 
-000005e0: 3d20 6e70 2e6d 6178 2867 6c69 7374 2920  = np.max(glist) 
-000005f0: 2d20 616e 7469 6369 7061 7469 6f6e 0d0a  - anticipation..
-00000600: 2020 2020 2020 6461 7461 203d 2064 6174        data = dat
-00000610: 612e 7175 6572 7928 6627 7b74 6e61 6d65  a.query(f'{tname
-00000620: 7d20 3c20 4076 616c 7565 2729 0d0a 2020  } < @value')..  
-00000630: 2020 2020 746c 6973 7420 3d20 6e70 2e73      tlist = np.s
-00000640: 6f72 7428 6461 7461 5f6e 6f6e 615b 746e  ort(data_nona[tn
-00000650: 616d 655d 2e75 6e69 7175 6528 2929 0d0a  ame].unique())..
-00000660: 2020 2020 2020 676c 6973 7420 3d20 6e70        glist = np
-00000670: 2e73 6f72 7428 6461 7461 5f6e 6f6e 615b  .sort(data_nona[
-00000680: 676e 616d 655d 2e75 6e69 7175 6528 2929  gname].unique())
-00000690: 0d0a 2020 2020 2020 676c 6973 7420 3d20  ..      glist = 
-000006a0: 676c 6973 745b 676c 6973 7420 3c20 6e70  glist[glist < np
-000006b0: 2e6d 6178 2867 6c69 7374 295d 0d0a 0d0a  .max(glist)]....
-000006c0: 2020 676c 6973 7420 3d20 676c 6973 745b    glist = glist[
-000006d0: 676c 6973 7420 3e20 305d 0d0a 2020 2320  glist > 0]..  # 
-000006e0: 6669 7273 7420 7072 6572 696f 7320 0d0a  first prerios ..
-000006f0: 2020 6670 203d 2074 6c69 7374 5b30 5d0d    fp = tlist[0].
-00000700: 0a20 2067 6c69 7374 203d 2067 6c69 7374  .  glist = glist
-00000710: 5b67 6c69 7374 203e 2066 7020 2b20 616e  [glist > fp + an
-00000720: 7469 6369 7061 7469 6f6e 5d0d 0a0d 0a20  ticipation].... 
-00000730: 2074 7265 6174 6564 5f66 7020 3d20 2864   treated_fp = (d
-00000740: 6174 615b 676e 616d 655d 203c 3d20 6670  ata[gname] <= fp
-00000750: 2920 2620 7e28 6461 7461 5b67 6e61 6d65  ) & ~(data[gname
-00000760: 5d20 3d3d 2030 290d 0a20 2074 7265 6174  ] == 0)..  treat
-00000770: 6564 5f66 702e 6669 6c6c 6e61 2846 616c  ed_fp.fillna(Fal
-00000780: 7365 2c20 696e 706c 6163 653d 5472 7565  se, inplace=True
-00000790: 290d 0a0d 0a20 206e 6669 7273 745f 7065  )....  nfirst_pe
-000007a0: 7269 6f64 203d 206e 702e 7375 6d28 7472  riod = np.sum(tr
-000007b0: 6561 7465 645f 6670 2920 6966 2070 616e  eated_fp) if pan
-000007c0: 656c 205c 0d0a 2020 2020 656c 7365 206c  el \..    else l
-000007d0: 656e 2864 6174 612e 6c6f 635b 7472 6561  en(data.loc[trea
-000007e0: 7465 645f 6670 2c20 6964 6e61 6d65 5d2e  ted_fp, idname].
-000007f0: 756e 6971 7565 2829 290d 0a0d 0a20 2069  unique())....  i
-00000800: 6620 6e66 6972 7374 5f70 6572 696f 6420  f nfirst_period 
-00000810: 3e20 303a 0d0a 2020 2020 7761 726e 696e  > 0:..    warnin
-00000820: 675f 6d65 7373 6167 6520 3d20 6622 4472  g_message = f"Dr
-00000830: 6f70 7065 6420 7b6e 6669 7273 7470 6572  opped {nfirstper
-00000840: 696f 647d 2075 6e69 7473 2074 6861 7420  iod} units that 
-00000850: 7765 7265 2061 6c72 6561 6479 2074 7265  were already tre
-00000860: 6174 6564 2069 6e20 7468 6520 6669 7273  ated in the firs
-00000870: 7420 7065 7269 6f64 2e22 0d0a 2020 2020  t period."..    
-00000880: 7072 696e 7428 7761 726e 696e 675f 6d65  print(warning_me
-00000890: 7373 6167 6529 0d0a 2020 2020 676c 6973  ssage)..    glis
-000008a0: 745f 696e 203d 206e 702e 6170 7065 6e64  t_in = np.append
-000008b0: 2867 6c69 7374 2c20 5b30 5d29 0d0a 2020  (glist, [0])..  
-000008c0: 2020 6461 7461 203d 2064 6174 612e 7175    data = data.qu
-000008d0: 6572 7928 6627 7b67 6e61 6d65 7d20 696e  ery(f'{gname} in
-000008e0: 2040 676c 6973 745f 696e 2729 0d0a 2020   @glist_in')..  
-000008f0: 2020 746c 6973 7420 3d20 6e70 2e73 6f72    tlist = np.sor
-00000900: 7428 6461 7461 5f6e 6f6e 615b 746e 616d  t(data_nona[tnam
-00000910: 655d 2e75 6e69 7175 6528 2929 0d0a 2020  e].unique())..  
-00000920: 2020 676c 6973 7420 3d20 6e70 2e73 6f72    glist = np.sor
-00000930: 7428 6461 7461 5f6e 6f6e 615b 676e 616d  t(data_nona[gnam
-00000940: 655d 2e75 6e69 7175 6528 2929 0d0a 2020  e].unique())..  
-00000950: 2020 676c 6973 7420 3d20 676c 6973 745b    glist = glist[
-00000960: 676c 6973 7420 3e20 305d 0d0a 2020 2020  glist > 0]..    
-00000970: 6670 203d 2074 6c69 7374 5b30 5d0d 0a20  fp = tlist[0].. 
-00000980: 2020 2067 6c69 7374 203d 2067 6c69 7374     glist = glist
-00000990: 5b67 6c69 7374 203e 2066 7020 2b20 616e  [glist > fp + an
-000009a0: 7469 6369 7061 7469 6f6e 5d0d 0a0d 0a20  ticipation].... 
-000009b0: 2023 746f 646f 3a20 6964 6e61 6d65 206d   #todo: idname m
-000009c0: 7573 7420 6265 206e 756d 6572 6963 0d0a  ust be numeric..
-000009d0: 2020 7472 7565 5f72 6570 5f63 726f 7373    true_rep_cross
-000009e0: 5f73 6563 7469 6f6e 203d 2046 616c 7365  _section = False
-000009f0: 0d0a 2020 6966 206e 6f74 2070 616e 656c  ..  if not panel
-00000a00: 3a0d 0a20 2020 2074 7275 655f 7265 705f  :..    true_rep_
-00000a10: 6372 6f73 735f 7365 6374 696f 6e20 3d20  cross_section = 
-00000a20: 5472 7565 0d0a 0d0a 2020 6966 2070 616e  True....  if pan
-00000a30: 656c 3a0d 0a20 2020 2069 6620 616c 6c6f  el:..    if allo
-00000a40: 775f 756e 6261 6c61 6e63 6564 5f70 616e  w_unbalanced_pan
-00000a50: 656c 3a20 0d0a 2020 2020 2020 7061 6e65  el: ..      pane
-00000a60: 6c20 3d20 4661 6c73 650d 0a20 2020 2020  l = False..     
-00000a70: 2074 7275 655f 7265 705f 6372 6f73 735f   true_rep_cross_
-00000a80: 7365 6374 696f 6e20 3d20 4661 6c73 650d  section = False.
-00000a90: 0a20 2020 2065 6c73 653a 0d0a 2020 2020  .    else:..    
-00000aa0: 2020 6b65 6570 6572 7320 3d20 6461 7461    keepers = data
-00000ab0: 2e64 726f 706e 6128 292e 696e 6465 780d  .dropna().index.
-00000ac0: 0a20 2020 2020 206e 203d 206c 656e 2864  .      n = len(d
-00000ad0: 6174 615b 6964 6e61 6d65 5d2e 756e 6971  ata[idname].uniq
-00000ae0: 7565 290d 0a20 2020 2020 2070 7269 6e74  ue)..      print
-00000af0: 286e 290d 0a20 2020 2020 206e 5f6b 6565  (n)..      n_kee
-00000b00: 7020 3d20 6c65 6e28 6461 7461 2e69 6c6f  p = len(data.ilo
-00000b10: 635b 6b65 6570 6572 732c 2069 646e 616d  c[keepers, idnam
-00000b20: 655d 2e75 6e69 7175 6528 2929 0d0a 0d0a  e].unique())....
-00000b30: 2020 2020 2020 6966 206c 656e 2864 6174        if len(dat
-00000b40: 612e 6c6f 635b 6b65 6570 6572 735d 203c  a.loc[keepers] <
-00000b50: 206c 656e 2864 6174 6129 293a 0d0a 2020   len(data)):..  
-00000b60: 2020 2020 2020 7072 696e 7428 6622 4472        print(f"Dr
-00000b70: 6f70 7065 6420 7b6e 2d6e 5f6b 6565 707d  opped {n-n_keep}
-00000b80: 206f 6273 6572 7661 7469 6f6e 7320 7468   observations th
-00000b90: 6174 2068 6164 206d 6973 7369 6e67 2064  at had missing d
-00000ba0: 6174 612e 2229 0d0a 2020 2020 2020 2020  ata.")..        
-00000bb0: 6461 7461 203d 2064 6174 612e 6c6f 635b  data = data.loc[
-00000bc0: 6b65 6570 6572 735d 0d0a 2020 2020 2020  keepers]..      
-00000bd0: 2320 6d61 6b65 2062 616c 616e 6365 6420  # make balanced 
-00000be0: 6461 7461 2073 6574 0d0a 2020 2020 2020  data set..      
-00000bf0: 6e5f 6f6c 6420 3d20 6c65 6e28 6461 7461  n_old = len(data
-00000c00: 5b69 646e 616d 655d 2e75 6e69 7175 6528  [idname].unique(
-00000c10: 2929 0d0a 2020 2020 2020 6461 7461 203d  ))..      data =
-00000c20: 206d 616b 6542 616c 616e 6365 6450 616e   makeBalancedPan
-00000c30: 656c 2864 6174 612c 2069 646e 616d 653d  el(data, idname=
-00000c40: 6964 6e61 6d65 2c20 746e 616d 653d 746e  idname, tname=tn
-00000c50: 616d 6529 0d0a 2020 2020 2020 6e20 3d20  ame)..      n = 
-00000c60: 6c65 6e28 6461 7461 5b69 646e 616d 655d  len(data[idname]
-00000c70: 2e75 6e69 7175 6528 2929 0d0a 2020 2020  .unique())..    
-00000c80: 2020 6966 206c 656e 2864 6174 6129 203d    if len(data) =
-00000c90: 3d20 303a 0d0a 2020 2020 2020 2020 7261  = 0:..        ra
-00000ca0: 6973 6520 5661 6c75 6545 7272 6f72 2822  ise ValueError("
-00000cb0: 416c 6c20 6f62 7365 7276 6174 696f 6e73  All observations
-00000cc0: 2064 726f 7070 6564 2074 6f20 636f 6e76   dropped to conv
-00000cd0: 6572 7420 6461 7461 2074 6f20 6261 6c61  ert data to bala
-00000ce0: 6e63 6564 2070 616e 656c 2e20 436f 6e73  nced panel. Cons
-00000cf0: 6964 6572 2073 6574 7469 6e67 2060 7061  ider setting `pa
-00000d00: 6e65 6c3d 4661 6c73 6560 2061 6e64 2f6f  nel=False` and/o
-00000d10: 7220 7265 7669 7369 7420 2769 646e 616d  r revisit 'idnam
-00000d20: 6527 2e22 290d 0a20 2020 2020 2069 6620  e'.")..      if 
-00000d30: 6e20 3c20 6e5f 6f6c 643a 0d0a 2020 2020  n < n_old:..    
-00000d40: 2020 2020 7761 726e 696e 6773 2e77 6172      warnings.war
-00000d50: 6e28 6622 4472 6f70 7065 6420 7b6e 5f6f  n(f"Dropped {n_o
-00000d60: 6c64 2d6e 7d20 6f62 7365 7276 6174 696f  ld-n} observatio
-00000d70: 6e73 2077 6869 6c65 2063 6f6e 7665 7274  ns while convert
-00000d80: 696e 6720 746f 2062 616c 616e 6365 6420  ing to balanced 
-00000d90: 7061 6e65 6c2e 2229 0d0a 2020 2020 2020  panel.")..      
-00000da0: 746e 203d 2074 6c69 7374 5b30 5d0d 0a20  tn = tlist[0].. 
-00000db0: 2020 2020 206e 203d 206c 656e 2864 6174       n = len(dat
-00000dc0: 612e 7175 6572 7928 6627 7b74 6e61 6d65  a.query(f'{tname
-00000dd0: 7d20 3d3d 2040 746e 2729 290d 0a20 2023  } == @tn'))..  #
-00000de0: 2061 6464 2072 6f77 6964 0d0a 2020 6966   add rowid..  if
-00000df0: 206e 6f74 2070 616e 656c 3a0d 0a20 2020   not panel:..   
-00000e00: 206b 6565 7065 7273 203d 2064 6174 612e   keepers = data.
-00000e10: 6472 6f70 6e61 2829 2e69 6e64 6578 0d0a  dropna().index..
-00000e20: 2020 2020 6e64 6966 6620 3d20 6c65 6e28      ndiff = len(
-00000e30: 6461 7461 2e6c 6f63 5b6b 6565 7065 7273  data.loc[keepers
-00000e40: 5d29 202d 206c 656e 2864 6174 6129 0d0a  ]) - len(data)..
-00000e50: 2020 2020 6966 206c 656e 286b 6565 7065      if len(keepe
-00000e60: 7273 2920 3d3d 2030 3a0d 0a20 2020 2020  rs) == 0:..     
-00000e70: 2072 6169 7365 2022 416c 6c20 6f62 7365   raise "All obse
-00000e80: 7276 6174 696f 6e73 2064 726f 7070 6564  rvations dropped
-00000e90: 2064 7565 2074 6f20 6d69 7373 696e 6720   due to missing 
-00000ea0: 6461 7461 2070 726f 626c 656d 732e 220d  data problems.".
-00000eb0: 0a20 2020 2069 6620 6e64 6966 6620 3c20  .    if ndiff < 
-00000ec0: 303a 0d0a 2020 2020 2020 6d73 7367 203d  0:..      mssg =
-00000ed0: 2066 2244 726f 7070 6564 207b 6e64 6966   f"Dropped {ndif
-00000ee0: 667d 206f 6273 6572 7661 7469 6f6e 7320  f} observations 
-00000ef0: 7468 6174 2068 6164 206d 6973 7369 6e67  that had missing
-00000f00: 2064 6174 612e 220d 0a20 2020 2020 2064   data."..      d
-00000f10: 6174 6120 3d20 6461 7461 2e6c 6f63 5b6b  ata = data.loc[k
-00000f20: 6565 7065 7273 5d0d 0a20 2020 2069 6620  eepers]..    if 
-00000f30: 7472 7565 5f72 6570 5f63 726f 7373 5f73  true_rep_cross_s
-00000f40: 6563 7469 6f6e 3a20 0d0a 2020 2020 2020  ection: ..      
-00000f50: 6461 7461 203d 2064 6174 612e 6173 7369  data = data.assi
-00000f60: 676e 2872 6f77 6964 203d 2072 616e 6765  gn(rowid = range
-00000f70: 286c 656e 2864 6174 6129 2929 0d0a 2020  (len(data)))..  
-00000f80: 2020 2020 6964 6e61 6d65 203d 2027 726f      idname = 'ro
-00000f90: 7769 6427 0d0a 2020 2020 656c 7365 3a0d  wid'..    else:.
-00000fa0: 0a20 2020 2020 2072 5f69 6420 3d20 6e70  .      r_id = np
-00000fb0: 2e61 7272 6179 2864 6174 615b 6964 6e61  .array(data[idna
-00000fc0: 6d65 5d29 0d0a 2020 2020 2020 6461 7461  me])..      data
-00000fd0: 203d 2064 6174 612e 6173 7369 676e 2872   = data.assign(r
-00000fe0: 6f77 6964 203d 2072 5f69 6429 0d0a 2020  owid = r_id)..  
-00000ff0: 2020 0d0a 2020 2020 6e20 3d20 6c65 6e28    ..    n = len(
-00001000: 6461 7461 5b69 646e 616d 655d 2e75 6e69  data[idname].uni
-00001010: 7175 6528 2929 0d0a 0d0a 2020 6461 7461  que())....  data
-00001020: 203d 2064 6174 612e 736f 7274 5f76 616c   = data.sort_val
-00001030: 7565 7328 5b69 646e 616d 652c 2074 6e61  ues([idname, tna
-00001040: 6d65 5d29 0d0a 2020 6461 7461 2e6c 6f63  me])..  data.loc
-00001050: 5b3a 2c20 222e 7722 5d20 3d20 6461 7461  [:, ".w"] = data
-00001060: 5b27 7727 5d0d 0a20 2069 6620 6c65 6e28  ['w']..  if len(
-00001070: 676c 6973 7429 203d 3d20 303a 0d0a 2020  glist) == 0:..  
-00001080: 2020 7261 6973 6520 6622 4e6f 2076 616c    raise f"No val
-00001090: 6964 2067 726f 7570 732e 2054 6865 2076  id groups. The v
-000010a0: 6172 6961 626c 6520 696e 2027 7b67 6e61  ariable in '{gna
-000010b0: 6d65 7d27 2073 686f 756c 6420 6265 2065  me}' should be e
-000010c0: 7870 7265 7373 6564 2061 7320 7468 6520  xpressed as the 
-000010d0: 7469 6d65 2061 2075 6e69 7420 6973 2066  time a unit is f
-000010e0: 6972 7374 2074 7265 6174 6564 2028 3020  irst treated (0 
-000010f0: 6966 206e 6576 6572 2d74 7265 6174 6564  if never-treated
-00001100: 292e 220d 0a20 2069 6620 6c65 6e28 746c  )."..  if len(tl
-00001110: 6973 7429 203d 3d20 323a 0d0a 2020 2020  ist) == 2:..    
-00001120: 6362 616e 6420 3d20 4661 6c73 650d 0a20  cband = False.. 
-00001130: 2067 7369 7a65 203d 2064 6174 612e 6772   gsize = data.gr
-00001140: 6f75 7062 7928 6461 7461 5b67 6e61 6d65  oupby(data[gname
-00001150: 5d29 2e73 697a 6528 292e 7265 7365 745f  ]).size().reset_
-00001160: 696e 6465 7828 6e61 6d65 3d22 636f 756e  index(name="coun
-00001170: 7422 290d 0a20 2067 7369 7a65 5b22 636f  t")..  gsize["co
-00001180: 756e 7422 5d20 2f3d 206c 656e 2874 6c69  unt"] /= len(tli
-00001190: 7374 290d 0a0d 0a20 2072 6571 7369 7a65  st)....  reqsize
-000011a0: 203d 206e 5f63 6f76 202b 2035 0d0a 2020   = n_cov + 5..  
-000011b0: 6773 697a 6520 3d20 6773 697a 655b 6773  gsize = gsize[gs
-000011c0: 697a 655b 2263 6f75 6e74 225d 203c 2072  ize["count"] < r
-000011d0: 6571 7369 7a65 5d0d 0a0d 0a20 2069 6620  eqsize]....  if 
-000011e0: 6c65 6e28 6773 697a 6529 203e 2030 3a0d  len(gsize) > 0:.
-000011f0: 0a20 2020 2067 7061 7374 6520 3d20 222c  .    gpaste = ",
-00001200: 222e 6a6f 696e 286d 6170 2873 7472 2c20  ".join(map(str, 
-00001210: 6773 697a 655b 676e 616d 655d 2929 0d0a  gsize[gname]))..
-00001220: 2020 2020 7761 726e 696e 6773 2e77 6172      warnings.war
-00001230: 6e28 6622 4265 2061 7761 7265 2074 6861  n(f"Be aware tha
-00001240: 7420 7468 6572 6520 6172 6520 736f 6d65  t there are some
-00001250: 2073 6d61 6c6c 2067 726f 7570 7320 696e   small groups in
-00001260: 2079 6f75 7220 6461 7461 7365 742e 5c6e   your dataset.\n
-00001270: 2020 4368 6563 6b20 6772 6f75 7073 3a20    Check groups: 
-00001280: 7b67 7061 7374 657d 2e22 290d 0a0d 0a20  {gpaste}.").... 
-00001290: 2020 2069 6620 3020 696e 2067 7369 7a65     if 0 in gsize
-000012a0: 5b67 6e61 6d65 5d2e 746f 6c69 7374 2829  [gname].tolist()
-000012b0: 2061 6e64 2063 6f6e 7472 6f6c 5f67 726f   and control_gro
-000012c0: 7570 203d 3d20 226e 6576 6572 7472 6561  up == "nevertrea
-000012d0: 7465 6422 3a0d 0a20 2020 2020 2072 6169  ted":..      rai
-000012e0: 7365 2022 4e65 7665 722d 7472 6561 7465  se "Never-treate
-000012f0: 6420 6772 6f75 7020 6973 2074 6f6f 2073  d group is too s
-00001300: 6d61 6c6c 2c20 7472 7920 7365 7474 696e  mall, try settin
-00001310: 6720 636f 6e74 726f 6c5f 6772 6f75 703d  g control_group=
-00001320: 276e 6f74 7965 7474 7265 6174 6564 272e  'notyettreated'.
-00001330: 220d 0a20 206e 542c 206e 4720 3d20 6d61  "..  nT, nG = ma
-00001340: 7028 6c65 6e2c 205b 746c 6973 742c 2067  p(len, [tlist, g
-00001350: 6c69 7374 5d29 0d0a 2020 6469 645f 7061  list])..  did_pa
-00001360: 7261 6d73 203d 207b 0d0a 2020 2020 2779  rams = {..    'y
-00001370: 6e61 6d65 2720 3a20 796e 616d 652c 2027  name' : yname, '
-00001380: 746e 616d 6527 3a20 746e 616d 652c 0d0a  tname': tname,..
-00001390: 2020 2020 2769 646e 616d 6527 203a 2069      'idname' : i
-000013a0: 646e 616d 652c 2027 676e 616d 6527 3a20  dname, 'gname': 
-000013b0: 676e 616d 652c 0d0a 2020 2020 2778 666f  gname,..    'xfo
-000013c0: 726d 6c61 273a 2078 666f 726d 6c61 2c20  rmla': xformla, 
-000013d0: 2764 6174 6127 3a20 6461 7461 2c0d 0a20  'data': data,.. 
-000013e0: 2020 2027 746c 6973 7427 3a20 746c 6973     'tlist': tlis
-000013f0: 742c 2027 676c 6973 7427 3a20 676c 6973  t, 'glist': glis
-00001400: 742c 0d0a 2020 2020 276e 273a 206e 2c20  t,..    'n': n, 
-00001410: 276e 4727 3a20 6e47 2c20 276e 5427 3a20  'nG': nG, 'nT': 
-00001420: 6e54 2c0d 0a20 2020 2027 636f 6e74 726f  nT,..    'contro
-00001430: 6c5f 6772 6f75 7027 3a20 636f 6e74 726f  l_group': contro
-00001440: 6c5f 6772 6f75 702c 2027 616e 7469 6369  l_group, 'antici
-00001450: 7061 7469 6f6e 273a 2061 6e74 6963 6970  pation': anticip
-00001460: 6174 696f 6e2c 0d0a 2020 2020 2777 6569  ation,..    'wei
-00001470: 6768 7473 5f6e 616d 6527 3a20 7765 6967  ghts_name': weig
-00001480: 6874 735f 6e61 6d65 2c20 2770 616e 656c  hts_name, 'panel
-00001490: 273a 2070 616e 656c 2c0d 0a20 2020 2027  ': panel,..    '
-000014a0: 7472 7565 5f72 6570 5f63 726f 7373 5f73  true_rep_cross_s
-000014b0: 6563 7469 6f6e 273a 2074 7275 655f 7265  ection': true_re
-000014c0: 705f 6372 6f73 735f 7365 6374 696f 6e2c  p_cross_section,
-000014d0: 0d0a 2020 2020 2763 6c75 7374 6572 7661  ..    'clusterva
-000014e0: 7273 273a 2063 6c75 7374 6572 7661 720d  rs': clustervar.
-000014f0: 0a20 207d 0d0a 2020 7265 7475 726e 2064  .  }..  return d
-00001500: 6964 5f70 6172 616d 730d 0a0d 0a         id_params....
+00000000: 0a69 6d70 6f72 7420 7061 6e64 6173 2061  .import pandas a
+00000010: 7320 7064 2c20 6e75 6d70 7920 6173 206e  s pd, numpy as n
+00000020: 700a 696d 706f 7274 2070 6174 7379 200a  p.import patsy .
+00000030: 6672 6f6d 2063 7364 6964 2e75 7469 6c73  from csdid.utils
+00000040: 2e62 6d69 7363 2069 6d70 6f72 7420 6d61  .bmisc import ma
+00000050: 6b65 4261 6c61 6e63 6564 5061 6e65 6c0a  keBalancedPanel.
+00000060: 0a66 6d6c 203d 2070 6174 7379 2e64 6d61  .fml = patsy.dma
+00000070: 7472 6963 6573 0a0a 6465 6620 7072 655f  trices..def pre_
+00000080: 7072 6f63 6573 735f 6469 6428 796e 616d  process_did(ynam
+00000090: 652c 2074 6e61 6d65 2c20 6964 6e61 6d65  e, tname, idname
+000000a0: 2c20 676e 616d 652c 2064 6174 613a 2070  , gname, data: p
+000000b0: 642e 4461 7461 4672 616d 652c 200a 2020  d.DataFrame, .  
+000000c0: 636f 6e74 726f 6c5f 6772 6f75 7020 3d20  control_group = 
+000000d0: 5b27 6e65 7665 7274 7265 6174 6564 272c  ['nevertreated',
+000000e0: 2027 6e6f 7479 6574 7472 6561 7465 6427   'notyettreated'
+000000f0: 5d2c 200a 2020 616e 7469 6369 7061 7469  ], .  anticipati
+00000100: 6f6e 203d 2030 2c20 7866 6f72 6d6c 6120  on = 0, xformla 
+00000110: 3a20 7374 7220 3d20 4e6f 6e65 2c0a 2020  : str = None,.  
+00000120: 7061 6e65 6c20 3d20 5472 7565 2c20 616c  panel = True, al
+00000130: 6c6f 775f 756e 6261 6c61 6e63 6564 5f70  low_unbalanced_p
+00000140: 616e 656c 203d 2054 7275 652c 2063 6261  anel = True, cba
+00000150: 6e64 203d 2046 616c 7365 2c0a 2020 636c  nd = False,.  cl
+00000160: 7573 7465 7276 6172 203d 204e 6f6e 652c  ustervar = None,
+00000170: 2020 7765 6967 6874 735f 6e61 6d65 203d    weights_name =
+00000180: 204e 6f6e 650a 2020 2920 2d3e 2064 6963   None.  ) -> dic
+00000190: 743a 0a0a 2020 6e2c 2074 203d 2064 6174  t:..  n, t = dat
+000001a0: 612e 7368 6170 650a 2020 636f 6e74 726f  a.shape.  contro
+000001b0: 6c5f 6772 6f75 7020 3d20 636f 6e74 726f  l_group = contro
+000001c0: 6c5f 6772 6f75 705b 305d 0a20 2063 6f6c  l_group[0].  col
+000001d0: 756d 6e73 203d 205b 6964 6e61 6d65 2c20  umns = [idname, 
+000001e0: 746e 616d 652c 2079 6e61 6d65 2c20 676e  tname, yname, gn
+000001f0: 616d 655d 0a20 2023 2070 7269 6e74 2863  ame].  # print(c
+00000200: 6f6c 756d 6e73 290a 2020 2320 436f 6c75  olumns).  # Colu
+00000210: 6d6e 730a 2020 6966 2063 6c75 7374 6572  mns.  if cluster
+00000220: 7661 7220 6973 206e 6f74 204e 6f6e 653a  var is not None:
+00000230: 0a20 2020 2063 6f6c 756d 6e73 202b 3d20  .    columns += 
+00000240: 5b63 6c75 7374 6572 7661 725d 0a20 2069  [clustervar].  i
+00000250: 6620 7765 6967 6874 735f 6e61 6d65 2069  f weights_name i
+00000260: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00000270: 636f 6c75 6d6e 7320 2b3d 205b 7765 6967  columns += [weig
+00000280: 6874 735f 6e61 6d65 5d0a 2020 2020 7720  hts_name].    w 
+00000290: 3d20 6461 7461 5b77 6569 6768 7473 5f6e  = data[weights_n
+000002a0: 616d 655d 0a20 2065 6c73 653a 0a20 2020  ame].  else:.   
+000002b0: 2077 203d 206e 702e 6f6e 6573 286e 290a   w = np.ones(n).
+000002c0: 0a0a 2020 6966 2078 666f 726d 6c61 2069  ..  if xformla i
+000002d0: 7320 4e6f 6e65 3a0a 2020 2020 7866 6f72  s None:.    xfor
+000002e0: 6d6c 6120 3d20 6627 7b79 6e61 6d65 7d20  mla = f'{yname} 
+000002f0: 7e20 3127 0a20 205f 2c20 785f 636f 7620  ~ 1'.  _, x_cov 
+00000300: 3d20 666d 6c28 7866 6f72 6d6c 612c 2064  = fml(xformla, d
+00000310: 6174 6120 3d20 6461 7461 2c20 7265 7475  ata = data, retu
+00000320: 726e 5f74 7970 653d 2764 6174 6166 7261  rn_type='datafra
+00000330: 6d65 2729 0a20 205f 2c20 6e5f 636f 7620  me').  _, n_cov 
+00000340: 3d20 785f 636f 762e 7368 6170 650a 0a0a  = x_cov.shape...
+00000350: 2020 6461 7461 203d 2070 642e 636f 6e63    data = pd.conc
+00000360: 6174 285b 6461 7461 5b63 6f6c 756d 6e73  at([data[columns
+00000370: 5d2c 2078 5f63 6f76 5d2c 2061 7869 733d  ], x_cov], axis=
+00000380: 3129 0a20 2064 6174 6120 3d20 6461 7461  1).  data = data
+00000390: 2e61 7373 6967 6e28 7720 3d20 7729 0a20  .assign(w = w). 
+000003a0: 2064 6174 6120 3d20 6461 7461 2e64 726f   data = data.dro
+000003b0: 706e 6128 290a 2020 6e64 6966 6620 3d20  pna().  ndiff = 
+000003c0: 6e20 2d20 6c65 6e28 6461 7461 2920 0a20  n - len(data) . 
+000003d0: 2069 6620 6e64 6966 6620 213d 2030 3a20   if ndiff != 0: 
+000003e0: 0a20 2020 2070 7269 6e74 2866 2764 726f  .    print(f'dro
+000003f0: 7070 6564 2c20 7b6e 6469 6666 7d2c 2072  pped, {ndiff}, r
+00000400: 6f77 7320 6672 6f6d 206f 7269 6769 6e61  ows from origina
+00000410: 6c20 6461 7461 2064 7565 2074 6f20 6d69  l data due to mi
+00000420: 7373 696e 6720 6461 7461 2729 0a0a 2020  ssing data')..  
+00000430: 746c 6973 7420 3d20 6e70 2e73 6f72 7428  tlist = np.sort(
+00000440: 6461 7461 5b74 6e61 6d65 5d2e 756e 6971  data[tname].uniq
+00000450: 7565 2829 290a 2020 676c 6973 7420 3d20  ue()).  glist = 
+00000460: 6e70 2e73 6f72 7428 6461 7461 5b67 6e61  np.sort(data[gna
+00000470: 6d65 5d2e 756e 6971 7565 2829 290a 0a20  me].unique()).. 
+00000480: 2061 7369 665f 6e65 765f 7472 6561 7465   asif_nev_treate
+00000490: 6420 3d20 6461 7461 5b67 6e61 6d65 5d20  d = data[gname] 
+000004a0: 3e20 6e70 2e6d 6178 2874 6c69 7374 290a  > np.max(tlist).
+000004b0: 2020 6173 6966 5f6e 6576 5f74 7265 6174    asif_nev_treat
+000004c0: 6564 2e66 696c 6c6e 6128 4661 6c73 652c  ed.fillna(False,
+000004d0: 2069 6e70 6c61 6365 3d54 7275 6529 0a20   inplace=True). 
+000004e0: 2064 6174 612e 6c6f 635b 6173 6966 5f6e   data.loc[asif_n
+000004f0: 6576 5f74 7265 6174 6564 2c20 676e 616d  ev_treated, gnam
+00000500: 655d 203d 2030 0a0a 2020 6966 206c 656e  e] = 0..  if len
+00000510: 2867 6c69 7374 5b67 6c69 7374 203d 3d20  (glist[glist == 
+00000520: 305d 2920 3d3d 2030 3a0a 2020 2020 6966  0]) == 0:.    if
+00000530: 2063 6f6e 7472 6f6c 5f67 726f 7570 203d   control_group =
+00000540: 3d20 226e 6576 6572 7472 6561 7465 6422  = "nevertreated"
+00000550: 3a0a 2020 2020 2020 7261 6973 6520 5661  :.      raise Va
+00000560: 6c75 6545 7272 6f72 2822 5468 6572 6520  lueError("There 
+00000570: 6973 206e 6f20 6176 6169 6c61 626c 6520  is no available 
+00000580: 6e65 7665 722d 7472 6561 7465 6420 6772  never-treated gr
+00000590: 6f75 7022 290a 2020 2020 656c 7365 3a0a  oup").    else:.
+000005a0: 2020 2020 2020 7661 6c75 6520 3d20 6e70        value = np
+000005b0: 2e6d 6178 2867 6c69 7374 2920 2d20 616e  .max(glist) - an
+000005c0: 7469 6369 7061 7469 6f6e 0a20 2020 2020  ticipation.     
+000005d0: 2064 6174 6120 3d20 6461 7461 2e71 7565   data = data.que
+000005e0: 7279 2866 277b 746e 616d 657d 203c 2040  ry(f'{tname} < @
+000005f0: 7661 6c75 6527 290a 2020 2020 2020 746c  value').      tl
+00000600: 6973 7420 3d20 6e70 2e73 6f72 7428 6461  ist = np.sort(da
+00000610: 7461 5f6e 6f6e 615b 746e 616d 655d 2e75  ta_nona[tname].u
+00000620: 6e69 7175 6528 2929 0a20 2020 2020 2067  nique()).      g
+00000630: 6c69 7374 203d 206e 702e 736f 7274 2864  list = np.sort(d
+00000640: 6174 615f 6e6f 6e61 5b67 6e61 6d65 5d2e  ata_nona[gname].
+00000650: 756e 6971 7565 2829 290a 2020 2020 2020  unique()).      
+00000660: 676c 6973 7420 3d20 676c 6973 745b 676c  glist = glist[gl
+00000670: 6973 7420 3c20 6e70 2e6d 6178 2867 6c69  ist < np.max(gli
+00000680: 7374 295d 0a0a 2020 676c 6973 7420 3d20  st)]..  glist = 
+00000690: 676c 6973 745b 676c 6973 7420 3e20 305d  glist[glist > 0]
+000006a0: 0a20 2023 2066 6972 7374 2070 7265 7269  .  # first preri
+000006b0: 6f73 200a 2020 6670 203d 2074 6c69 7374  os .  fp = tlist
+000006c0: 5b30 5d0a 2020 676c 6973 7420 3d20 676c  [0].  glist = gl
+000006d0: 6973 745b 676c 6973 7420 3e20 6670 202b  ist[glist > fp +
+000006e0: 2061 6e74 6963 6970 6174 696f 6e5d 0a0a   anticipation]..
+000006f0: 2020 7472 6561 7465 645f 6670 203d 2028    treated_fp = (
+00000700: 6461 7461 5b67 6e61 6d65 5d20 3c3d 2066  data[gname] <= f
+00000710: 7029 2026 207e 2864 6174 615b 676e 616d  p) & ~(data[gnam
+00000720: 655d 203d 3d20 3029 0a20 2074 7265 6174  e] == 0).  treat
+00000730: 6564 5f66 702e 6669 6c6c 6e61 2846 616c  ed_fp.fillna(Fal
+00000740: 7365 2c20 696e 706c 6163 653d 5472 7565  se, inplace=True
+00000750: 290a 0a20 206e 6669 7273 745f 7065 7269  )..  nfirst_peri
+00000760: 6f64 203d 206e 702e 7375 6d28 7472 6561  od = np.sum(trea
+00000770: 7465 645f 6670 2920 6966 2070 616e 656c  ted_fp) if panel
+00000780: 205c 0a20 2020 2065 6c73 6520 6c65 6e28   \.    else len(
+00000790: 6461 7461 2e6c 6f63 5b74 7265 6174 6564  data.loc[treated
+000007a0: 5f66 702c 2069 646e 616d 655d 2e75 6e69  _fp, idname].uni
+000007b0: 7175 6528 2929 0a0a 2020 6966 206e 6669  que())..  if nfi
+000007c0: 7273 745f 7065 7269 6f64 203e 2030 3a0a  rst_period > 0:.
+000007d0: 2020 2020 7761 726e 696e 675f 6d65 7373      warning_mess
+000007e0: 6167 6520 3d20 6622 4472 6f70 7065 6420  age = f"Dropped 
+000007f0: 7b6e 6669 7273 7470 6572 696f 647d 2075  {nfirstperiod} u
+00000800: 6e69 7473 2074 6861 7420 7765 7265 2061  nits that were a
+00000810: 6c72 6561 6479 2074 7265 6174 6564 2069  lready treated i
+00000820: 6e20 7468 6520 6669 7273 7420 7065 7269  n the first peri
+00000830: 6f64 2e22 0a20 2020 2070 7269 6e74 2877  od.".    print(w
+00000840: 6172 6e69 6e67 5f6d 6573 7361 6765 290a  arning_message).
+00000850: 2020 2020 676c 6973 745f 696e 203d 206e      glist_in = n
+00000860: 702e 6170 7065 6e64 2867 6c69 7374 2c20  p.append(glist, 
+00000870: 5b30 5d29 0a20 2020 2064 6174 6120 3d20  [0]).    data = 
+00000880: 6461 7461 2e71 7565 7279 2866 277b 676e  data.query(f'{gn
+00000890: 616d 657d 2069 6e20 4067 6c69 7374 5f69  ame} in @glist_i
+000008a0: 6e27 290a 2020 2020 746c 6973 7420 3d20  n').    tlist = 
+000008b0: 6e70 2e73 6f72 7428 6461 7461 5f6e 6f6e  np.sort(data_non
+000008c0: 615b 746e 616d 655d 2e75 6e69 7175 6528  a[tname].unique(
+000008d0: 2929 0a20 2020 2067 6c69 7374 203d 206e  )).    glist = n
+000008e0: 702e 736f 7274 2864 6174 615f 6e6f 6e61  p.sort(data_nona
+000008f0: 5b67 6e61 6d65 5d2e 756e 6971 7565 2829  [gname].unique()
+00000900: 290a 2020 2020 676c 6973 7420 3d20 676c  ).    glist = gl
+00000910: 6973 745b 676c 6973 7420 3e20 305d 0a20  ist[glist > 0]. 
+00000920: 2020 2066 7020 3d20 746c 6973 745b 305d     fp = tlist[0]
+00000930: 0a20 2020 2067 6c69 7374 203d 2067 6c69  .    glist = gli
+00000940: 7374 5b67 6c69 7374 203e 2066 7020 2b20  st[glist > fp + 
+00000950: 616e 7469 6369 7061 7469 6f6e 5d0a 0a20  anticipation].. 
+00000960: 2023 746f 646f 3a20 6964 6e61 6d65 206d   #todo: idname m
+00000970: 7573 7420 6265 206e 756d 6572 6963 0a20  ust be numeric. 
+00000980: 2074 7275 655f 7265 705f 6372 6f73 735f   true_rep_cross_
+00000990: 7365 6374 696f 6e20 3d20 4661 6c73 650a  section = False.
+000009a0: 2020 6966 206e 6f74 2070 616e 656c 3a0a    if not panel:.
+000009b0: 2020 2020 7472 7565 5f72 6570 5f63 726f      true_rep_cro
+000009c0: 7373 5f73 6563 7469 6f6e 203d 2054 7275  ss_section = Tru
+000009d0: 650a 0a20 2069 6620 7061 6e65 6c3a 0a20  e..  if panel:. 
+000009e0: 2020 2069 6620 616c 6c6f 775f 756e 6261     if allow_unba
+000009f0: 6c61 6e63 6564 5f70 616e 656c 3a20 0a20  lanced_panel: . 
+00000a00: 2020 2020 2070 616e 656c 203d 2046 616c       panel = Fal
+00000a10: 7365 0a20 2020 2020 2074 7275 655f 7265  se.      true_re
+00000a20: 705f 6372 6f73 735f 7365 6374 696f 6e20  p_cross_section 
+00000a30: 3d20 4661 6c73 650a 2020 2020 656c 7365  = False.    else
+00000a40: 3a0a 2020 2020 2020 6b65 6570 6572 7320  :.      keepers 
+00000a50: 3d20 6461 7461 2e64 726f 706e 6128 292e  = data.dropna().
+00000a60: 696e 6465 780a 2020 2020 2020 6e20 3d20  index.      n = 
+00000a70: 6c65 6e28 6461 7461 5b69 646e 616d 655d  len(data[idname]
+00000a80: 2e75 6e69 7175 6529 0a20 2020 2020 2070  .unique).      p
+00000a90: 7269 6e74 286e 290a 2020 2020 2020 6e5f  rint(n).      n_
+00000aa0: 6b65 6570 203d 206c 656e 2864 6174 612e  keep = len(data.
+00000ab0: 696c 6f63 5b6b 6565 7065 7273 2c20 6964  iloc[keepers, id
+00000ac0: 6e61 6d65 5d2e 756e 6971 7565 2829 290a  name].unique()).
+00000ad0: 0a20 2020 2020 2069 6620 6c65 6e28 6461  .      if len(da
+00000ae0: 7461 2e6c 6f63 5b6b 6565 7065 7273 5d20  ta.loc[keepers] 
+00000af0: 3c20 6c65 6e28 6461 7461 2929 3a0a 2020  < len(data)):.  
+00000b00: 2020 2020 2020 7072 696e 7428 6622 4472        print(f"Dr
+00000b10: 6f70 7065 6420 7b6e 2d6e 5f6b 6565 707d  opped {n-n_keep}
+00000b20: 206f 6273 6572 7661 7469 6f6e 7320 7468   observations th
+00000b30: 6174 2068 6164 206d 6973 7369 6e67 2064  at had missing d
+00000b40: 6174 612e 2229 0a20 2020 2020 2020 2064  ata.").        d
+00000b50: 6174 6120 3d20 6461 7461 2e6c 6f63 5b6b  ata = data.loc[k
+00000b60: 6565 7065 7273 5d0a 2020 2020 2020 2320  eepers].      # 
+00000b70: 6d61 6b65 2062 616c 616e 6365 6420 6461  make balanced da
+00000b80: 7461 2073 6574 0a20 2020 2020 206e 5f6f  ta set.      n_o
+00000b90: 6c64 203d 206c 656e 2864 6174 615b 6964  ld = len(data[id
+00000ba0: 6e61 6d65 5d2e 756e 6971 7565 2829 290a  name].unique()).
+00000bb0: 2020 2020 2020 6461 7461 203d 206d 616b        data = mak
+00000bc0: 6542 616c 616e 6365 6450 616e 656c 2864  eBalancedPanel(d
+00000bd0: 6174 612c 2069 646e 616d 653d 6964 6e61  ata, idname=idna
+00000be0: 6d65 2c20 746e 616d 653d 746e 616d 6529  me, tname=tname)
+00000bf0: 0a20 2020 2020 206e 203d 206c 656e 2864  .      n = len(d
+00000c00: 6174 615b 6964 6e61 6d65 5d2e 756e 6971  ata[idname].uniq
+00000c10: 7565 2829 290a 2020 2020 2020 6966 206c  ue()).      if l
+00000c20: 656e 2864 6174 6129 203d 3d20 303a 0a20  en(data) == 0:. 
+00000c30: 2020 2020 2020 2072 6169 7365 2056 616c         raise Val
+00000c40: 7565 4572 726f 7228 2241 6c6c 206f 6273  ueError("All obs
+00000c50: 6572 7661 7469 6f6e 7320 6472 6f70 7065  ervations droppe
+00000c60: 6420 746f 2063 6f6e 7665 7274 2064 6174  d to convert dat
+00000c70: 6120 746f 2062 616c 616e 6365 6420 7061  a to balanced pa
+00000c80: 6e65 6c2e 2043 6f6e 7369 6465 7220 7365  nel. Consider se
+00000c90: 7474 696e 6720 6070 616e 656c 3d46 616c  tting `panel=Fal
+00000ca0: 7365 6020 616e 642f 6f72 2072 6576 6973  se` and/or revis
+00000cb0: 6974 2027 6964 6e61 6d65 272e 2229 0a20  it 'idname'."). 
+00000cc0: 2020 2020 2069 6620 6e20 3c20 6e5f 6f6c       if n < n_ol
+00000cd0: 643a 0a20 2020 2020 2020 2077 6172 6e69  d:.        warni
+00000ce0: 6e67 732e 7761 726e 2866 2244 726f 7070  ngs.warn(f"Dropp
+00000cf0: 6564 207b 6e5f 6f6c 642d 6e7d 206f 6273  ed {n_old-n} obs
+00000d00: 6572 7661 7469 6f6e 7320 7768 696c 6520  ervations while 
+00000d10: 636f 6e76 6572 7469 6e67 2074 6f20 6261  converting to ba
+00000d20: 6c61 6e63 6564 2070 616e 656c 2e22 290a  lanced panel.").
+00000d30: 2020 2020 2020 746e 203d 2074 6c69 7374        tn = tlist
+00000d40: 5b30 5d0a 2020 2020 2020 6e20 3d20 6c65  [0].      n = le
+00000d50: 6e28 6461 7461 2e71 7565 7279 2866 277b  n(data.query(f'{
+00000d60: 746e 616d 657d 203d 3d20 4074 6e27 2929  tname} == @tn'))
+00000d70: 0a20 2023 2061 6464 2072 6f77 6964 0a20  .  # add rowid. 
+00000d80: 2069 6620 6e6f 7420 7061 6e65 6c3a 0a20   if not panel:. 
+00000d90: 2020 206b 6565 7065 7273 203d 2064 6174     keepers = dat
+00000da0: 612e 6472 6f70 6e61 2829 2e69 6e64 6578  a.dropna().index
+00000db0: 0a20 2020 206e 6469 6666 203d 206c 656e  .    ndiff = len
+00000dc0: 2864 6174 612e 6c6f 635b 6b65 6570 6572  (data.loc[keeper
+00000dd0: 735d 2920 2d20 6c65 6e28 6461 7461 290a  s]) - len(data).
+00000de0: 2020 2020 6966 206c 656e 286b 6565 7065      if len(keepe
+00000df0: 7273 2920 3d3d 2030 3a0a 2020 2020 2020  rs) == 0:.      
+00000e00: 7261 6973 6520 2241 6c6c 206f 6273 6572  raise "All obser
+00000e10: 7661 7469 6f6e 7320 6472 6f70 7065 6420  vations dropped 
+00000e20: 6475 6520 746f 206d 6973 7369 6e67 2064  due to missing d
+00000e30: 6174 6120 7072 6f62 6c65 6d73 2e22 0a20  ata problems.". 
+00000e40: 2020 2069 6620 6e64 6966 6620 3c20 303a     if ndiff < 0:
+00000e50: 0a20 2020 2020 206d 7373 6720 3d20 6622  .      mssg = f"
+00000e60: 4472 6f70 7065 6420 7b6e 6469 6666 7d20  Dropped {ndiff} 
+00000e70: 6f62 7365 7276 6174 696f 6e73 2074 6861  observations tha
+00000e80: 7420 6861 6420 6d69 7373 696e 6720 6461  t had missing da
+00000e90: 7461 2e22 0a20 2020 2020 2064 6174 6120  ta.".      data 
+00000ea0: 3d20 6461 7461 2e6c 6f63 5b6b 6565 7065  = data.loc[keepe
+00000eb0: 7273 5d0a 2020 2020 6966 2074 7275 655f  rs].    if true_
+00000ec0: 7265 705f 6372 6f73 735f 7365 6374 696f  rep_cross_sectio
+00000ed0: 6e3a 200a 2020 2020 2020 6461 7461 203d  n: .      data =
+00000ee0: 2064 6174 612e 6173 7369 676e 2872 6f77   data.assign(row
+00000ef0: 6964 203d 2072 616e 6765 286c 656e 2864  id = range(len(d
+00000f00: 6174 6129 2929 0a20 2020 2020 2069 646e  ata))).      idn
+00000f10: 616d 6520 3d20 2772 6f77 6964 270a 2020  ame = 'rowid'.  
+00000f20: 2020 656c 7365 3a0a 2020 2020 2020 725f    else:.      r_
+00000f30: 6964 203d 206e 702e 6172 7261 7928 6461  id = np.array(da
+00000f40: 7461 5b69 646e 616d 655d 290a 2020 2020  ta[idname]).    
+00000f50: 2020 6461 7461 203d 2064 6174 612e 6173    data = data.as
+00000f60: 7369 676e 2872 6f77 6964 203d 2072 5f69  sign(rowid = r_i
+00000f70: 6429 0a20 2020 200a 2020 2020 6e20 3d20  d).    .    n = 
+00000f80: 6c65 6e28 6461 7461 5b69 646e 616d 655d  len(data[idname]
+00000f90: 2e75 6e69 7175 6528 2929 0a0a 2020 6461  .unique())..  da
+00000fa0: 7461 203d 2064 6174 612e 736f 7274 5f76  ta = data.sort_v
+00000fb0: 616c 7565 7328 5b69 646e 616d 652c 2074  alues([idname, t
+00000fc0: 6e61 6d65 5d29 0a20 2064 6174 612e 6c6f  name]).  data.lo
+00000fd0: 635b 3a2c 2022 2e77 225d 203d 2064 6174  c[:, ".w"] = dat
+00000fe0: 615b 2777 275d 0a20 2069 6620 6c65 6e28  a['w'].  if len(
+00000ff0: 676c 6973 7429 203d 3d20 303a 0a20 2020  glist) == 0:.   
+00001000: 2072 6169 7365 2066 224e 6f20 7661 6c69   raise f"No vali
+00001010: 6420 6772 6f75 7073 2e20 5468 6520 7661  d groups. The va
+00001020: 7269 6162 6c65 2069 6e20 277b 676e 616d  riable in '{gnam
+00001030: 657d 2720 7368 6f75 6c64 2062 6520 6578  e}' should be ex
+00001040: 7072 6573 7365 6420 6173 2074 6865 2074  pressed as the t
+00001050: 696d 6520 6120 756e 6974 2069 7320 6669  ime a unit is fi
+00001060: 7273 7420 7472 6561 7465 6420 2830 2069  rst treated (0 i
+00001070: 6620 6e65 7665 722d 7472 6561 7465 6429  f never-treated)
+00001080: 2e22 0a20 2069 6620 6c65 6e28 746c 6973  .".  if len(tlis
+00001090: 7429 203d 3d20 323a 0a20 2020 2063 6261  t) == 2:.    cba
+000010a0: 6e64 203d 2046 616c 7365 0a20 2067 7369  nd = False.  gsi
+000010b0: 7a65 203d 2064 6174 612e 6772 6f75 7062  ze = data.groupb
+000010c0: 7928 6461 7461 5b67 6e61 6d65 5d29 2e73  y(data[gname]).s
+000010d0: 697a 6528 292e 7265 7365 745f 696e 6465  ize().reset_inde
+000010e0: 7828 6e61 6d65 3d22 636f 756e 7422 290a  x(name="count").
+000010f0: 2020 6773 697a 655b 2263 6f75 6e74 225d    gsize["count"]
+00001100: 202f 3d20 6c65 6e28 746c 6973 7429 0a0a   /= len(tlist)..
+00001110: 2020 7265 7173 697a 6520 3d20 6e5f 636f    reqsize = n_co
+00001120: 7620 2b20 350a 2020 6773 697a 6520 3d20  v + 5.  gsize = 
+00001130: 6773 697a 655b 6773 697a 655b 2263 6f75  gsize[gsize["cou
+00001140: 6e74 225d 203c 2072 6571 7369 7a65 5d0a  nt"] < reqsize].
+00001150: 0a20 2069 6620 6c65 6e28 6773 697a 6529  .  if len(gsize)
+00001160: 203e 2030 3a0a 2020 2020 6770 6173 7465   > 0:.    gpaste
+00001170: 203d 2022 2c22 2e6a 6f69 6e28 6d61 7028   = ",".join(map(
+00001180: 7374 722c 2067 7369 7a65 5b67 6e61 6d65  str, gsize[gname
+00001190: 5d29 290a 2020 2020 7761 726e 696e 6773  ])).    warnings
+000011a0: 2e77 6172 6e28 6622 4265 2061 7761 7265  .warn(f"Be aware
+000011b0: 2074 6861 7420 7468 6572 6520 6172 6520   that there are 
+000011c0: 736f 6d65 2073 6d61 6c6c 2067 726f 7570  some small group
+000011d0: 7320 696e 2079 6f75 7220 6461 7461 7365  s in your datase
+000011e0: 742e 5c6e 2020 4368 6563 6b20 6772 6f75  t.\n  Check grou
+000011f0: 7073 3a20 7b67 7061 7374 657d 2e22 290a  ps: {gpaste}.").
+00001200: 0a20 2020 2069 6620 3020 696e 2067 7369  .    if 0 in gsi
+00001210: 7a65 5b67 6e61 6d65 5d2e 746f 6c69 7374  ze[gname].tolist
+00001220: 2829 2061 6e64 2063 6f6e 7472 6f6c 5f67  () and control_g
+00001230: 726f 7570 203d 3d20 226e 6576 6572 7472  roup == "nevertr
+00001240: 6561 7465 6422 3a0a 2020 2020 2020 7261  eated":.      ra
+00001250: 6973 6520 224e 6576 6572 2d74 7265 6174  ise "Never-treat
+00001260: 6564 2067 726f 7570 2069 7320 746f 6f20  ed group is too 
+00001270: 736d 616c 6c2c 2074 7279 2073 6574 7469  small, try setti
+00001280: 6e67 2063 6f6e 7472 6f6c 5f67 726f 7570  ng control_group
+00001290: 3d27 6e6f 7479 6574 7472 6561 7465 6427  ='notyettreated'
+000012a0: 2e22 0a20 206e 542c 206e 4720 3d20 6d61  .".  nT, nG = ma
+000012b0: 7028 6c65 6e2c 205b 746c 6973 742c 2067  p(len, [tlist, g
+000012c0: 6c69 7374 5d29 0a20 2064 6964 5f70 6172  list]).  did_par
+000012d0: 616d 7320 3d20 7b0a 2020 2020 2779 6e61  ams = {.    'yna
+000012e0: 6d65 2720 3a20 796e 616d 652c 2027 746e  me' : yname, 'tn
+000012f0: 616d 6527 3a20 746e 616d 652c 0a20 2020  ame': tname,.   
+00001300: 2027 6964 6e61 6d65 2720 3a20 6964 6e61   'idname' : idna
+00001310: 6d65 2c20 2767 6e61 6d65 273a 2067 6e61  me, 'gname': gna
+00001320: 6d65 2c0a 2020 2020 2778 666f 726d 6c61  me,.    'xformla
+00001330: 273a 2078 666f 726d 6c61 2c20 2764 6174  ': xformla, 'dat
+00001340: 6127 3a20 6461 7461 2c0a 2020 2020 2774  a': data,.    't
+00001350: 6c69 7374 273a 2074 6c69 7374 2c20 2767  list': tlist, 'g
+00001360: 6c69 7374 273a 2067 6c69 7374 2c0a 2020  list': glist,.  
+00001370: 2020 276e 273a 206e 2c20 276e 4727 3a20    'n': n, 'nG': 
+00001380: 6e47 2c20 276e 5427 3a20 6e54 2c0a 2020  nG, 'nT': nT,.  
+00001390: 2020 2763 6f6e 7472 6f6c 5f67 726f 7570    'control_group
+000013a0: 273a 2063 6f6e 7472 6f6c 5f67 726f 7570  ': control_group
+000013b0: 2c20 2761 6e74 6963 6970 6174 696f 6e27  , 'anticipation'
+000013c0: 3a20 616e 7469 6369 7061 7469 6f6e 2c0a  : anticipation,.
+000013d0: 2020 2020 2777 6569 6768 7473 5f6e 616d      'weights_nam
+000013e0: 6527 3a20 7765 6967 6874 735f 6e61 6d65  e': weights_name
+000013f0: 2c20 2770 616e 656c 273a 2070 616e 656c  , 'panel': panel
+00001400: 2c0a 2020 2020 2774 7275 655f 7265 705f  ,.    'true_rep_
+00001410: 6372 6f73 735f 7365 6374 696f 6e27 3a20  cross_section': 
+00001420: 7472 7565 5f72 6570 5f63 726f 7373 5f73  true_rep_cross_s
+00001430: 6563 7469 6f6e 2c0a 2020 2020 2763 6c75  ection,.    'clu
+00001440: 7374 6572 7661 7273 273a 2063 6c75 7374  stervars': clust
+00001450: 6572 7661 720a 2020 7d0a 2020 7265 7475  ervar.  }.  retu
+00001460: 726e 2064 6964 5f70 6172 616d 730a 0a    rn did_params..
```

### Comparing `csdid-0.1.81/csdid/plots/gplot.py` & `csdid-0.1.82/csdid/plots/gplot.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,103 +1,103 @@
-# -*- coding: utf-8 -*-
-"""
-Created on Sun Jun 11 16:17:07 2023
-
-@author: Carlos Guevara
-"""
-
-from plotnine import ggplot, aes, geom_point, geom_errorbar, scale_y_continuous, scale_x_continuous, \
-    scale_color_manual, labs, geom_hline, theme, element_text, element_rect, element_line, \
-    scale_x_discrete
-
-# get_ipython().run_line_magic('matplotlib', 'qt') # To aopen separate window
-# get_ipython().run_line_magic('matplotlib', 'inline') # In line graph
-
-def gplot(ssresults, ylim=None, xlab=None, ylab=None, title="Group", xgap=1,
-           legend=True, ref_line=0, theming=True):
-    if ylab is None:
-        ylab = 'ATT'
-    dabreaks = ssresults['year'][::xgap]
-    ssresults['post'] = ssresults['post'].astype('category')
-
-    post_levels = list(ssresults['post'].unique().categories)
-    
-    if 0 in post_levels:
-        color_values = ["#e87d72", "#56bcc2"]
-        label_values = ['Pre', 'Post']
-    else:
-        color_values = ["#56bcc2"]
-        label_values = ['Post']
-    
-    p = ggplot(ssresults,
-               aes(x='year', y='att', ymin='att - c * att_se', ymax='att + c * att_se')) + \
-        geom_point(aes(colour='post'), size=2) + \
-        geom_errorbar(aes(colour='post'), width=0.15 , size=0.8 ) + \
-        scale_y_continuous(limits=ylim) + \
-        scale_x_continuous(breaks=list(dabreaks), labels=list(map(str, dabreaks))) + \
-        scale_color_manual(drop=False, values=color_values, breaks=post_levels, labels=label_values) + \
-        labs(x=xlab, y=ylab, title=title, color='') 
-        
-    if ref_line is not None:
-        p += geom_hline(aes(yintercept=ref_line), linetype='dashed')
-
-    if theming:
-        p += theme(
-                panel_background=element_rect(fill='white'),
-                plot_title=element_text(color='#1F1F1F', fontweight='bold', size=10),
-                axis_text=element_text(color='#1F1F1F'),
-                axis_line=element_line(color='#1F1F1F'),
-                strip_background=element_rect(fill='white'),
-                legend_position=(.55, -.025),
-                strip_text=element_text(color='#1F1F1F', fontweight='bold', size=9)
-        ) 
-
-    if not legend:
-        p += theme(legend_position='none')
-
-    return p
-
-
-def splot(ssresults, ylim=None, xlab=None, ylab=None, title="Group",
-          legend=True, ref_line=0, theming=True):
-    if ylab is None:
-        ylab = 'ATT'
-    if xlab is None:
-        xlab = 'Group'
-    ssresults['year'] = ssresults['year'].astype('category')
-    ssresults['post'] = ssresults['post'].astype('category')
-    
-    post_levels = list(ssresults['post'].unique().categories)  
-   
-    if 0 in post_levels:
-        color_values = ["#e87d72", "#56bcc2"]
-        label_values = ['Pre', 'Post']
-    else:
-        color_values = ["#56bcc2"]
-        label_values = ['Post']
-
-    p = ggplot(ssresults,
-               aes(y='att', x='year', ymin='att - c * att_se', ymax='att + c * att_se')) + \
-        geom_point(aes(colour='post'), size=2) + \
-        geom_errorbar(aes(colour='post'), width=0.15 , size=0.8) + \
-        scale_y_continuous(limits=ylim) + \
-        scale_x_discrete(breaks=list(ssresults['year']))  + \
-        scale_color_manual(drop=False, values=color_values,breaks=list(post_levels) , labels=label_values) + \
-        labs(x=xlab, y=ylab, title=title, color='')
-    
-    if ref_line is not None:
-        p += geom_hline(aes(yintercept=ref_line), linetype='dashed')
-    
-    if theming:
-        p += theme(
-                panel_background=element_rect(fill='white'),
-                plot_title=element_text(color='#1F1F1F', fontweight='bold', size=10),
-                axis_text=element_text(color='#1F1F1F'),
-                axis_line=element_line(color='#1F1F1F'),
-                strip_background=element_rect(fill='white'),
-                legend_position=(.55, -.025)
-            )
-    
-    if not legend:
-        p += theme(legend_position='none')
-    
+# -*- coding: utf-8 -*-
+"""
+Created on Sun Jun 11 16:17:07 2023
+
+@author: Carlos Guevara
+"""
+
+from plotnine import ggplot, aes, geom_point, geom_errorbar, scale_y_continuous, scale_x_continuous, \
+    scale_color_manual, labs, geom_hline, theme, element_text, element_rect, element_line, \
+    scale_x_discrete
+
+# get_ipython().run_line_magic('matplotlib', 'qt') # To aopen separate window
+# get_ipython().run_line_magic('matplotlib', 'inline') # In line graph
+
+def gplot(ssresults, ylim=None, xlab=None, ylab=None, title="Group", xgap=1,
+           legend=True, ref_line=0, theming=True):
+    if ylab is None:
+        ylab = 'ATT'
+    dabreaks = ssresults['year'][::xgap]
+    ssresults['post'] = ssresults['post'].astype('category')
+
+    post_levels = list(ssresults['post'].unique().categories)
+    
+    if 0 in post_levels:
+        color_values = ["#e87d72", "#56bcc2"]
+        label_values = ['Pre', 'Post']
+    else:
+        color_values = ["#56bcc2"]
+        label_values = ['Post']
+    
+    p = ggplot(ssresults,
+               aes(x='year', y='att', ymin='att - c * att_se', ymax='att + c * att_se')) + \
+        geom_point(aes(colour='post'), size=2) + \
+        geom_errorbar(aes(colour='post'), width=0.15 , size=0.8 ) + \
+        scale_y_continuous(limits=ylim) + \
+        scale_x_continuous(breaks=list(dabreaks), labels=list(map(str, dabreaks))) + \
+        scale_color_manual(drop=False, values=color_values, breaks=post_levels, labels=label_values) + \
+        labs(x=xlab, y=ylab, title=title, color='') 
+        
+    if ref_line is not None:
+        p += geom_hline(aes(yintercept=ref_line), linetype='dashed')
+
+    if theming:
+        p += theme(
+                panel_background=element_rect(fill='white'),
+                plot_title=element_text(color='#1F1F1F', fontweight='bold', size=10),
+                axis_text=element_text(color='#1F1F1F'),
+                axis_line=element_line(color='#1F1F1F'),
+                strip_background=element_rect(fill='white'),
+                legend_position=(.55, -.025),
+                strip_text=element_text(color='#1F1F1F', fontweight='bold', size=9)
+        ) 
+
+    if not legend:
+        p += theme(legend_position='none')
+
+    return p
+
+
+def splot(ssresults, ylim=None, xlab=None, ylab=None, title="Group",
+          legend=True, ref_line=0, theming=True):
+    if ylab is None:
+        ylab = 'ATT'
+    if xlab is None:
+        xlab = 'Group'
+    ssresults['year'] = ssresults['year'].astype('category')
+    ssresults['post'] = ssresults['post'].astype('category')
+    
+    post_levels = list(ssresults['post'].unique().categories)  
+   
+    if 0 in post_levels:
+        color_values = ["#e87d72", "#56bcc2"]
+        label_values = ['Pre', 'Post']
+    else:
+        color_values = ["#56bcc2"]
+        label_values = ['Post']
+
+    p = ggplot(ssresults,
+               aes(y='att', x='year', ymin='att - c * att_se', ymax='att + c * att_se')) + \
+        geom_point(aes(colour='post'), size=2) + \
+        geom_errorbar(aes(colour='post'), width=0.15 , size=0.8) + \
+        scale_y_continuous(limits=ylim) + \
+        scale_x_discrete(breaks=list(ssresults['year']))  + \
+        scale_color_manual(drop=False, values=color_values,breaks=list(post_levels) , labels=label_values) + \
+        labs(x=xlab, y=ylab, title=title, color='')
+    
+    if ref_line is not None:
+        p += geom_hline(aes(yintercept=ref_line), linetype='dashed')
+    
+    if theming:
+        p += theme(
+                panel_background=element_rect(fill='white'),
+                plot_title=element_text(color='#1F1F1F', fontweight='bold', size=10),
+                axis_text=element_text(color='#1F1F1F'),
+                axis_line=element_line(color='#1F1F1F'),
+                strip_background=element_rect(fill='white'),
+                legend_position=(.55, -.025)
+            )
+    
+    if not legend:
+        p += theme(legend_position='none')
+    
     return p
```

### Comparing `csdid-0.1.81/csdid/utils/bmisc.py` & `csdid-0.1.82/csdid/utils/bmisc.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,55 +1,55 @@
-import pandas as pd
-def makeBalancedPanel(data, idname, tname):
-  data = data.sort_values([idname, tname]).reset_index(drop = True)
-  nt = len(data[tname].unique())
-  data = data.groupby(idname)\
-    .filter(lambda x: len(x) == nt)
-  return data
-
-
-def panel2cs2(data: pd.DataFrame, yname, idname, tname):
-  if len(data[tname].unique()) != 2:
-    raise ValueError('panel2cs2 only for 2 perios of apnel data')
-
-  data = data.sort_values([idname, tname])
-  y1 = data.groupby(idname)[yname].shift(-1)
-  y0 = data[yname]
-  dy = y1 - y0
-  data = data.assign(
-    y1 = y1, y0 = y0, dy = dy
-  )
-  return data.dropna()
-
-# -*- coding: utf-8 -*-
-"""
-Created on Wed May 31 18:58:35 2023
-
-@author: Carlos Guevara
-"""
-import numpy as np
-
-def TorF(cond, use_isTRUE=False):
-
-    if not isinstance(cond, np.ndarray) or cond.dtype != bool:
-        raise ValueError("cond should be a logical vector")
-    if use_isTRUE:
-        cond = np.array([x is True for x in cond])
-    else:
-        cond[np.isnan(cond)] = False
-    return cond
-
-def multiplier_bootstrap(inf_func, biters): # This function comes from c++
-    n, K = inf_func.shape
-    biters = int(biters)
-    innerMat = np.zeros((n, K))
-    Ub = np.zeros(n)
-    outMat = np.zeros((biters,K))
-
-    for b in range(biters):
-        # draw Rademechar weights
-        # Ub = ( np.ones(n) - 2 * np.round(np.random.rand(n)) )[:, np.newaxis]
-        Ub = np.random.choice([1, -1], size=(n, 1))
-        innerMat = inf_func * Ub
-        outMat[b] = np.mean(innerMat, axis=0)
-
+import pandas as pd
+def makeBalancedPanel(data, idname, tname):
+  data = data.sort_values([idname, tname]).reset_index(drop = True)
+  nt = len(data[tname].unique())
+  data = data.groupby(idname)\
+    .filter(lambda x: len(x) == nt)
+  return data
+
+
+def panel2cs2(data: pd.DataFrame, yname, idname, tname):
+  if len(data[tname].unique()) != 2:
+    raise ValueError('panel2cs2 only for 2 perios of apnel data')
+
+  data = data.sort_values([idname, tname])
+  y1 = data.groupby(idname)[yname].shift(-1)
+  y0 = data[yname]
+  dy = y1 - y0
+  data = data.assign(
+    y1 = y1, y0 = y0, dy = dy
+  )
+  return data.dropna()
+
+# -*- coding: utf-8 -*-
+"""
+Created on Wed May 31 18:58:35 2023
+
+@author: Carlos Guevara
+"""
+import numpy as np
+
+def TorF(cond, use_isTRUE=False):
+
+    if not isinstance(cond, np.ndarray) or cond.dtype != bool:
+        raise ValueError("cond should be a logical vector")
+    if use_isTRUE:
+        cond = np.array([x is True for x in cond])
+    else:
+        cond[np.isnan(cond)] = False
+    return cond
+
+def multiplier_bootstrap(inf_func, biters): # This function comes from c++
+    n, K = inf_func.shape
+    biters = int(biters)
+    innerMat = np.zeros((n, K))
+    Ub = np.zeros(n)
+    outMat = np.zeros((biters,K))
+
+    for b in range(biters):
+        # draw Rademechar weights
+        # Ub = ( np.ones(n) - 2 * np.round(np.random.rand(n)) )[:, np.newaxis]
+        Ub = np.random.choice([1, -1], size=(n, 1))
+        innerMat = inf_func * Ub
+        outMat[b] = np.mean(innerMat, axis=0)
+
     return outMat
```

### Comparing `csdid-0.1.81/csdid/utils/mboot.py` & `csdid-0.1.82/csdid/utils/mboot.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,112 +1,112 @@
-import numpy as np
-from scipy.stats import mstats, norm
-from joblib import Parallel, delayed
-import pandas as pd
-
-from csdid.utils.bmisc import multiplier_bootstrap
-
-def mboot(inf_func, DIDparams, pl=False, cores=1):
-    # Setup needed variables
-    data            = pd.DataFrame( DIDparams['data'] )
-    idname          = DIDparams['idname']
-    clustervars     = DIDparams['clustervars']
-    biters          = DIDparams['biters']
-    tname           = DIDparams['tname']
-    tlist           = np.sort( np.unique(data[tname]) )
-    alp             = DIDparams['alp']
-    panel           = DIDparams['panel']
-    true_repeated_cross_sections = DIDparams['true_repeated_cross_sections']
-
-    # Get n observations (for clustering below)
-    if panel:
-        dta = data[ data[tname] == tlist[0] ]
-    else:
-        dta = data.copy()
-
-    # Convert inf_func to matrix
-    inf_func = np.asarray(inf_func)
-
-    # Set correct number of units
-    n = inf_func.shape[0]
-
-    # Drop idname if it is in clustervars
-    if clustervars is not None and idname in clustervars:
-        clustervars.remove(idname)
-
-    if clustervars is not None:
-        if isinstance(clustervars, list) and isinstance(clustervars[0], str):
-            raise ValueError("clustervars need to be the name of the clustering variable.")
-
-    # We can only handle up to 2-way clustering
-    if clustervars is not None and len(clustervars) > 1:
-        raise ValueError("Can't handle that many cluster variables")
-
-    if clustervars is not None:
-        # Check that cluster variable does not vary over time within unit
-        clust_tv = dta.groupby(idname)[clustervars[0]].nunique() == 1
-        if not clust_tv.all():
-            raise ValueError("Can't handle time-varying cluster variables")
-    # clustervars='year'    
-    # Multiplier bootstrap
-    n_clusters = n
-    if not clustervars:
-        bres = np.sqrt(n) * run_multiplier_bootstrap(inf_func, biters, pl, cores)
-    else:
-        n_clusters = len(data[clustervars].drop_duplicates())
-        cluster = dta[[idname, clustervars]].drop_duplicates().values[:, 1]
-        cluster_n = dta.groupby(cluster).size().values
-        cluster_mean_if = pd.DataFrame(inf_func).groupby(cluster).sum().values / cluster_n
-        bres = np.sqrt(n_clusters) * run_multiplier_bootstrap(cluster_mean_if, biters, pl, cores)
-
-    # Handle vector and matrix case differently to get nxk matrix
-    if isinstance(bres, np.ndarray) and bres.ndim == 1:
-        bres = np.expand_dims(bres, axis=0)
-    elif isinstance(bres, np.ndarray) and bres.ndim > 2:
-        bres = bres.transpose()
-
-    # Non-degenerate dimensions
-    ndg_dim = np.logical_and(~np.isnan(np.sum(bres, axis=0)), np.sum(bres ** 2, axis=0) > np.sqrt(np.finfo(float).eps) * 10)
-    bres = bres[:, ndg_dim]
-
-    # Bootstrap variance matrix (this matrix can be defective because of degenerate cases)
-    V = np.cov(bres, rowvar=False)
-
-    # Bootstrap standard error
-    quantile_75 = np.quantile(bres, 0.75, axis=0, method="inverted_cdf")
-    quantile_25 = np.quantile(bres, 0.25, axis=0, method="inverted_cdf")
-    qnorm_75 = norm.ppf(0.75)
-    qnorm_25 = norm.ppf(0.25)   
-    bSigma = (quantile_75 - quantile_25) / (qnorm_75 - qnorm_25)
-        
-    # Critical value for uniform confidence band
-    bT = np.max(np.abs(bres / bSigma), axis=1)
-    bT = bT[np.isfinite(bT)]
-    crit_val = np.quantile(bT, 1 - alp, method="inverted_cdf")
-    
-    # Standard error
-    se = np.full(ndg_dim.shape, np.nan)
-    se[ndg_dim] = bSigma / np.sqrt(n_clusters)
-
-    return {'bres': bres, 'V': V, 'se': se, 'crit_val': crit_val}
-
-def run_multiplier_bootstrap(inf_func, biters, pl=False, cores=1):
-    ngroups = int(np.ceil(biters / cores))
-    chunks = [ngroups] * cores
-    chunks[0] += biters - sum(chunks)
-
-    n = inf_func.shape[0]
-
-    def parallel_function(biters):
-        return multiplier_bootstrap(inf_func, biters)
-
-    if n > 2500 and pl and cores > 1:
-        results = Parallel(n_jobs=cores)(
-            delayed(parallel_function)(biters) for biters in chunks
-        )
-        results = np.vstack(results)
-    else:
-        results = multiplier_bootstrap(inf_func, biters)
-
-    return results
-
-
+import numpy as np
+from scipy.stats import mstats, norm
+from joblib import Parallel, delayed
+import pandas as pd
+
+from csdid.utils.bmisc import multiplier_bootstrap
+
+def mboot(inf_func, DIDparams, pl=False, cores=1):
+    # Setup needed variables
+    data            = pd.DataFrame( DIDparams['data'] )
+    idname          = DIDparams['idname']
+    clustervars     = DIDparams['clustervars']
+    biters          = DIDparams['biters']
+    tname           = DIDparams['tname']
+    tlist           = np.sort( np.unique(data[tname]) )
+    alp             = DIDparams['alp']
+    panel           = DIDparams['panel']
+    true_repeated_cross_sections = DIDparams['true_repeated_cross_sections']
+
+    # Get n observations (for clustering below)
+    if panel:
+        dta = data[ data[tname] == tlist[0] ]
+    else:
+        dta = data.copy()
+
+    # Convert inf_func to matrix
+    inf_func = np.asarray(inf_func)
+
+    # Set correct number of units
+    n = inf_func.shape[0]
+
+    # Drop idname if it is in clustervars
+    if clustervars is not None and idname in clustervars:
+        clustervars.remove(idname)
+
+    if clustervars is not None:
+        if isinstance(clustervars, list) and isinstance(clustervars[0], str):
+            raise ValueError("clustervars need to be the name of the clustering variable.")
+
+    # We can only handle up to 2-way clustering
+    if clustervars is not None and len(clustervars) > 1:
+        raise ValueError("Can't handle that many cluster variables")
+
+    if clustervars is not None:
+        # Check that cluster variable does not vary over time within unit
+        clust_tv = dta.groupby(idname)[clustervars[0]].nunique() == 1
+        if not clust_tv.all():
+            raise ValueError("Can't handle time-varying cluster variables")
+    # clustervars='year'    
+    # Multiplier bootstrap
+    n_clusters = n
+    if not clustervars:
+        bres = np.sqrt(n) * run_multiplier_bootstrap(inf_func, biters, pl, cores)
+    else:
+        n_clusters = len(data[clustervars].drop_duplicates())
+        cluster = dta[[idname, clustervars]].drop_duplicates().values[:, 1]
+        cluster_n = dta.groupby(cluster).size().values
+        cluster_mean_if = pd.DataFrame(inf_func).groupby(cluster).sum().values / cluster_n
+        bres = np.sqrt(n_clusters) * run_multiplier_bootstrap(cluster_mean_if, biters, pl, cores)
+
+    # Handle vector and matrix case differently to get nxk matrix
+    if isinstance(bres, np.ndarray) and bres.ndim == 1:
+        bres = np.expand_dims(bres, axis=0)
+    elif isinstance(bres, np.ndarray) and bres.ndim > 2:
+        bres = bres.transpose()
+
+    # Non-degenerate dimensions
+    ndg_dim = np.logical_and(~np.isnan(np.sum(bres, axis=0)), np.sum(bres ** 2, axis=0) > np.sqrt(np.finfo(float).eps) * 10)
+    bres = bres[:, ndg_dim]
+
+    # Bootstrap variance matrix (this matrix can be defective because of degenerate cases)
+    V = np.cov(bres, rowvar=False)
+
+    # Bootstrap standard error
+    quantile_75 = np.quantile(bres, 0.75, axis=0, method="inverted_cdf")
+    quantile_25 = np.quantile(bres, 0.25, axis=0, method="inverted_cdf")
+    qnorm_75 = norm.ppf(0.75)
+    qnorm_25 = norm.ppf(0.25)   
+    bSigma = (quantile_75 - quantile_25) / (qnorm_75 - qnorm_25)
+        
+    # Critical value for uniform confidence band
+    bT = np.max(np.abs(bres / bSigma), axis=1)
+    bT = bT[np.isfinite(bT)]
+    crit_val = np.quantile(bT, 1 - alp, method="inverted_cdf")
+    
+    # Standard error
+    se = np.full(ndg_dim.shape, np.nan)
+    se[ndg_dim] = bSigma / np.sqrt(n_clusters)
+
+    return {'bres': bres, 'V': V, 'se': se, 'crit_val': crit_val}
+
+def run_multiplier_bootstrap(inf_func, biters, pl=False, cores=1):
+    ngroups = int(np.ceil(biters / cores))
+    chunks = [ngroups] * cores
+    chunks[0] += biters - sum(chunks)
+
+    n = inf_func.shape[0]
+
+    def parallel_function(biters):
+        return multiplier_bootstrap(inf_func, biters)
+
+    if n > 2500 and pl and cores > 1:
+        results = Parallel(n_jobs=cores)(
+            delayed(parallel_function)(biters) for biters in chunks
+        )
+        results = np.vstack(results)
+    else:
+        results = multiplier_bootstrap(inf_func, biters)
+
+    return results
+
+
```

### Comparing `csdid-0.1.81/csdid.egg-info/SOURCES.txt` & `csdid-0.1.82/csdid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `csdid-0.1.81/setup.py` & `csdid-0.1.82/setup.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-from setuptools import setup, find_packages
-
-# with open('requirements.txt') as f:
-#     required = f.read().splitlines()
-# print(required)
-from csdid._version import __version
-print(__version)
-
-setup(
-  name = 'csdid',
-  version=__version,
-  url='https://github.com/d2cml-ai/csdid',
-  author='D2CML Team, Alexander Quispe, Carlos Guevara, Jhon Flroes',
-  keywords=['Causal inference', 'Research'],
-  license="MIT",
-  description='Difference in Difference in Python',
-  classifiers=[
-        "Intended Audience :: Developers",
-        "Intended Audience :: Education",
-        "Intended Audience :: Science/Research",
-        "License :: OSI Approved :: Apache Software License",
-        "Topic :: Scientific/Engineering",
-    ],
-  install_requires=[
-        'pandas',
-        'numpy<=1.24.3',
-        'scipy',
-        'patsy',
-        'plotnine',
-        'twine'
-  ],
-  packages=find_packages(),
-  package_data={
-    'data': ['data/*'],
-    'configs': ['configs/*']
-  }
+from setuptools import setup, find_packages
+
+# with open('requirements.txt') as f:
+#     required = f.read().splitlines()
+# print(required)
+from csdid._version import __version
+print(__version)
+
+setup(
+  name = 'csdid',
+  version=__version,
+  url='https://github.com/d2cml-ai/csdid',
+  author='D2CML Team, Alexander Quispe, Carlos Guevara, Jhon Flroes',
+  keywords=['Causal inference', 'Research'],
+  license="MIT",
+  description='Difference in Difference in Python',
+  classifiers=[
+        "Intended Audience :: Developers",
+        "Intended Audience :: Education",
+        "Intended Audience :: Science/Research",
+        "License :: OSI Approved :: Apache Software License",
+        "Topic :: Scientific/Engineering",
+    ],
+  install_requires=[
+        'pandas',
+        'numpy<=1.24.3',
+        'scipy',
+        'patsy',
+        'plotnine',
+        'twine'
+  ],
+  packages=find_packages(),
+  package_data={
+    'data': ['data/*'],
+    'configs': ['configs/*']
+  }
 )
```

