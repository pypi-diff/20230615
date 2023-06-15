# Comparing `tmp/rots-py-1.0.3.tar.gz` & `tmp/rots-py-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rots-py-1.0.3.tar", last modified: Wed Apr 26 17:17:29 2023, max compression
+gzip compressed data, was "rots-py-1.1.0.tar", last modified: Thu Jun 15 14:23:00 2023, max compression
```

## Comparing `rots-py-1.0.3.tar` & `rots-py-1.1.0.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-04-26 17:17:29.739342 rots-py-1.0.3/
--rw-rw-rw-   0        0        0     1097 2023-04-18 12:29:22.000000 rots-py-1.0.3/LICENSE
--rw-rw-rw-   0        0        0     2070 2023-04-26 17:17:29.738347 rots-py-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      273 2023-04-18 14:24:25.000000 rots-py-1.0.3/README.md
--rw-rw-rw-   0        0        0      724 2023-04-26 17:16:08.000000 rots-py-1.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-26 17:17:29.740340 rots-py-1.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-26 17:17:29.658219 rots-py-1.0.3/src/
--rw-rw-rw-   0        0        0        0 2023-04-18 12:38:29.000000 rots-py-1.0.3/src/__init__.py
--rw-rw-rw-   0        0        0      164 2023-04-18 12:48:35.000000 rots-py-1.0.3/src/__main__.py
--rw-rw-rw-   0        0        0     3101 2023-04-26 17:07:58.000000 rots-py-1.0.3/src/calculateOverlaps1.py
--rw-rw-rw-   0        0        0     2816 2023-04-26 17:08:25.000000 rots-py-1.0.3/src/calculateOverlaps2.py
--rw-rw-rw-   0        0        0     8416 2023-04-26 17:11:26.000000 rots-py-1.0.3/src/helpers.py
--rw-rw-rw-   0        0        0    11266 2023-04-19 22:18:42.000000 rots-py-1.0.3/src/rots.py
-drwxrwxrwx   0        0        0        0 2023-04-26 17:17:29.735353 rots-py-1.0.3/src/rots_py.egg-info/
--rw-rw-rw-   0        0        0     2070 2023-04-26 17:17:29.000000 rots-py-1.0.3/src/rots_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      355 2023-04-26 17:17:29.000000 rots-py-1.0.3/src/rots_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-26 17:17:29.000000 rots-py-1.0.3/src/rots_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-04-26 17:17:29.000000 rots-py-1.0.3/src/rots_py.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       40 2023-04-26 17:17:29.000000 rots-py-1.0.3/src/rots_py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       69 2023-04-26 17:17:29.000000 rots-py-1.0.3/src/rots_py.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-15 14:23:00.094057 rots-py-1.1.0/
+-rw-rw-rw-   0        0        0     1097 2023-04-18 12:29:22.000000 rots-py-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     4815 2023-06-15 14:23:00.092056 rots-py-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3018 2023-06-15 14:04:54.000000 rots-py-1.1.0/README.md
+-rw-rw-rw-   0        0        0      724 2023-06-15 14:07:22.000000 rots-py-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-15 14:23:00.094057 rots-py-1.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-15 14:22:59.888403 rots-py-1.1.0/src/
+-rw-rw-rw-   0        0        0        0 2023-04-18 12:38:29.000000 rots-py-1.1.0/src/__init__.py
+-rw-rw-rw-   0        0        0      164 2023-04-18 12:48:35.000000 rots-py-1.1.0/src/__main__.py
+-rw-rw-rw-   0        0        0     3101 2023-04-26 17:07:58.000000 rots-py-1.1.0/src/calculateOverlaps1.py
+-rw-rw-rw-   0        0        0     2816 2023-04-26 17:08:25.000000 rots-py-1.1.0/src/calculateOverlaps2.py
+-rw-rw-rw-   0        0        0     8531 2023-06-14 11:03:17.000000 rots-py-1.1.0/src/helpers.py
+drwxrwxrwx   0        0        0        0 2023-06-15 14:22:59.895388 rots-py-1.1.0/src/optim_cy/
+-rw-rw-rw-   0        0        0      173 2023-06-13 17:42:24.000000 rots-py-1.1.0/src/optim_cy/setup.py
+-rw-rw-rw-   0        0        0    11162 2023-06-15 13:24:45.000000 rots-py-1.1.0/src/rots.py
+drwxrwxrwx   0        0        0        0 2023-06-15 14:23:00.057860 rots-py-1.1.0/src/rots_py.egg-info/
+-rw-rw-rw-   0        0        0     4815 2023-06-15 14:22:59.000000 rots-py-1.1.0/src/rots_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      377 2023-06-15 14:22:59.000000 rots-py-1.1.0/src/rots_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 14:22:59.000000 rots-py-1.1.0/src/rots_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-06-15 14:22:59.000000 rots-py-1.1.0/src/rots_py.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       40 2023-06-15 14:22:59.000000 rots-py-1.1.0/src/rots_py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       78 2023-06-15 14:22:59.000000 rots-py-1.1.0/src/rots_py.egg-info/top_level.txt
```

### Comparing `rots-py-1.0.3/LICENSE` & `rots-py-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rots-py-1.0.3/pyproject.toml` & `rots-py-1.1.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # pyproject.toml
 
 [project]
 name = "rots-py"
-version = "1.0.3"
+version = "1.1.0"
 description = "ROTS gene ranking implementation in Python"
 readme = "README.md"
 authors = [{ name = "F.Mamadbekov, M.Shakya, A.Montoya, I.Ul-Haq", email = "fmamadbe@abo.fi" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `rots-py-1.0.3/src/calculateOverlaps1.py` & `rots-py-1.1.0/src/calculateOverlaps1.py`

 * *Files identical despite different names*

### Comparing `rots-py-1.0.3/src/calculateOverlaps2.py` & `rots-py-1.1.0/src/calculateOverlaps2.py`

 * *Files identical despite different names*

### Comparing `rots-py-1.0.3/src/helpers.py` & `rots-py-1.1.0/src/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import numpy as np
 from numba import njit, jit
 import pandas as pd
 from tqdm import tqdm
 
+from optim_cy import optim
+
 @jit(nopython=True, error_model='numpy')
 def bootstrapSamples(B, labels, paired):
-  samples = np.zeros((B, len(labels)))#matrix(nrow=B, ncol=length(labels))
+  samples = np.zeros((B, len(labels)))
   
   for i in range(B):
     for label in np.unique(labels):
       pos = np.where(labels == label)[0]
       #samples[i, pos] = np.random.choice(pos, size=len(pos), replace=True)            
       _samp = samples[i]
       _samp[pos] = np.random.choice(pos, size=len(pos), replace=True)
@@ -129,17 +131,19 @@
   # Store order for later use
   observed_order = sorted(range(len(observed)), key=lambda k: abs(observed[k]), reverse=True) # order(abs(observed), decreasing=TRUE)
   
   # Sort observed and permuted values
   observed = -np.sort(-abs(observed)) #sort(abs(observed), decreasing=TRUE)
   permuted = -np.sort(-np.abs(permuted.flatten())) #sort(abs(as.vector(permuted)), decreasing=TRUE)
   
+  print("observed shape: ", observed.shape)
+  print("permuted shape: ", permuted.shape)
   # Get p-values from C++ code
   # (expects ordered vectors)
-  p = pvalue(observed, permuted)        
+  p = optim.pvalue(observed, permuted)
   
   # Revert to original ordering
   results = np.zeros(len(p)) #vector(mode="numeric", length=length(p))
   for i in range(len(results)):
     results[observed_order[i]] =  p[i]
   
   return results
@@ -193,14 +197,15 @@
   # d = matches
   #ipdb.set_trace(context=10)   ## BREAKPOINT
   d = np.array([np.where(z == v)[0][0] if v in z else None for v in x])
   res = d - a + b
 
   return res
 
+# Replaced by *optim_cy.pvalue*
 @jit(nopython=True, error_model='numpy')
 def pvalue(a, b):
   observed = a.ravel()
   permuted = b.ravel()
   pvalues = np.zeros(len(observed))
 
   j = 0
```

### Comparing `rots-py-1.0.3/src/rots.py` & `rots-py-1.1.0/src/rots.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,53 +3,64 @@
 import pandas as pd
 from tqdm import tqdm
 import random
 
 from helpers import bootstrapSamples, permutatedSamples, testStatistic, calculateP, calculateFDR
 from calculateOverlaps1 import calculateOverlaps1
 from calculateOverlaps2 import calculateOverlaps2
+from optim_cy import optim
 
-def rots(data, groups, B=1000, K=None, paired=False, seed=None, a1=None, a2=None, log=None, progress=False, verbose=True):
-  if isinstance(data, pd.DataFrame):
-    data_val = data.values    
+def rots(data, groups, B=500, K=None, paired=False, seed=None, a1=None, a2=None, log=False, progress=False, verbose=True):
+  #if isinstance(data, pd.DataFrame):
+  #  data_val = data.values    
+  
+  ## Set random number generator seed for reproducibility
   if seed is not None:
     random.seed(seed)
+
+  ## Check groups
   if data.shape[1] != len(groups):
     raise ValueError("Number of samples in the data does not match the groups.")
+  
+  ## If data.index == NULL, use integers as index. Summary function requires that
+  ## the data matrix has index.
   if not data.index.any():
-    data.index = np.arange(1, data.shape[0]+1)
+    data.index = np.arange(1, data.shape[0]+1)  
 
+  ##  The reproducibility values in a dense lattice
   ssq = np.concatenate((
     np.arange(0, 0.21, 0.01), 
     np.arange(0.22, 1.01, 0.02),
     np.arange(1.2, 5.2, 0.2)
   ))
   N = np.concatenate([
     np.arange(1, 21) * 5,
     np.arange(11, 51) * 10,
     np.arange(21, 41) * 25, 
     np.arange(11, 1001) * 100
   ])
-  
-  #ipdb.set_trace(context=6)   ## BREAKPOINT
-
+    
+  ## Check for top list size K
   if K is None:
     K = data.shape[0] // 4
     if (verbose):
       print("No top list size K given, using ", K)
 
+  ## The top list size cannot be larger than the total number of genes
   K = min(K, data.shape[0])
   N = N[N < K]
 
+  # handle the situation if the groups is character
   if isinstance(groups[0], str):
     groups = pd.factorize(groups)[0]
     groups_levels = pd.factorize(groups)[1]
   else:
     groups_levels = None
 
+  ## Reorder the data according to the group labels and check for NA rows.
   data = data.iloc[:, np.argsort(groups)]
   groups = np.sort(groups)
   
   for i in np.unique(groups):
     if np.any(np.sum(np.isnan(data.iloc[:, np.where(groups == i)[0]]), axis=1) >= len(np.where(groups == i)[0]) - 1):
       if groups_levels is None:
         target = i
@@ -57,24 +68,24 @@
         target = groups_levels[i]
       raise ValueError("The data matrix of group " + str(target) + " contains rows with less than two non-missing values, please remove these rows.")
 
   cl = groups + (1-np.min(groups))
 
   ## Check number of samples for paired test
   if paired:
-    for i in np.unique(cl)[-1]:
+    for i in np.unique(cl)[1:]:
       if len(np.where(cl == 1)[0]) != len(np.where(cl == i)[0]):
         raise ValueError("Uneven number of samples for paired test.")
 
   ## Calculate fold change
   if len(np.unique(cl)) == 2:
     if log:
-      logfc = np.mean(data.iloc[:, np.where(cl==1)[0]], axis=1) - np.mean(data.iloc[:, np.where(cl==2)[0]], axis=1)
+      logfc = np.nanmean(data.iloc[:, np.where(cl==1)[0]], axis=1) - np.nanmean(data.iloc[:, np.where(cl==2)[0]], axis=1)
     else:
-      logfc = np.mean(np.log2(data.iloc[:,np.where(cl==1)[0]]+1), axis=1) - np.mean(np.log2(data.iloc[:,np.where(cl==2)[0]]+1), axis=1)
+      logfc = np.nanmean(np.log2(data.iloc[:,np.where(cl==1)[0]]+1), axis=1) - np.nanmean(np.log2(data.iloc[:,np.where(cl==2)[0]]+1), axis=1)
   else:
     logfc = np.repeat(np.nan, data.shape[0])
 
   ## ---------------------------------------------------------------------------
 
   ## Bootstrap samples
   if (verbose): 
@@ -114,18 +125,14 @@
     
     if progress: 
       pb.update()
     
   if progress: 
     pb.close()
 
-  ## Free up memory
-  ##del samples
-  ##del pSamples
-    
   ## ---------------------------------------------------------------------------
 
   if  a1==None or a2==None:
     ## Optimize the parameters
     if verbose:
       print("Optimizing parameters")
     
@@ -149,32 +156,30 @@
     ## data): the rows correspond to the a1-values given in ssq (+ 1 for signal
     ## log-ratio only: a1=1, a2=0), the columns correspond to the different
     ## top list sizes
     reprotable_sd = pd.DataFrame(index=np.append(ssq, "slr"),columns=N)
 
     # Progress bar
     if progress:
-        pb = tqdm(total=len(ssq)) #txtProgressBar(min=0, max=length(ssq), style=3)      
+        pb = tqdm(total=len(ssq))
 
     for i in range(len(ssq)):
       ## The overlaps between bootstrap samples. Rows correspond to different
       ## bootrsrap samples and columns corrospond to different top list size.
       ## Repeat for each parameter combination a1 and a2.
       overlaps = np.zeros((B,len(N)))
       overlaps_P = np.zeros((B,len(N)))      
 
-      ## Call the custom c++-loop 1.
-      cResults = calculateOverlaps1(D, S, pD, pS, len(D), N.astype(int), len(N),
+      
+      cResults = optim.calculateOverlaps1(D, S, pD, pS, len(D), N.astype(int), len(N),
                         ssq[i], int(B), overlaps, overlaps_P)
       
       ## Colmeans & rowMeans are a lot faster than apply
       #         reprotable[i, ] <- colMeans(overlaps)
-      #         reprotable.P[i, ] <- colMeans(overlaps.P)
-      
-      
+      #         reprotable.P[i, ] <- colMeans(overlaps.P)            
       reprotable.iloc[i] = np.mean(cResults["overlaps"], axis=0)
       reprotable_P.iloc[i] = np.mean(cResults["overlaps_P"], axis=0)
       
       ## Standard deviation for each column
       ## same as reprotable.sd[i, ] <- apply(overlaps, 2, sd)
       ## or just sd(overlaps), but a lot faster.
       #         reprotable.sd[i,] <- sqrt(rowSums((t(overlaps) - reprotable[i,])^2) /
@@ -189,76 +194,56 @@
 
     if progress: 
       pb.close()
 
     i = len(ssq)
     overlaps = np.zeros((B,len(N)))
     overlaps_P = np.zeros((B,len(N)))
-
-    ## Call the custom c++-loop 2.
-    cResults = calculateOverlaps2(D, pD, len(D), N.astype(int), len(N),
+    
+    cResults = optim.calculateOverlaps2(D, pD, len(D), N.astype(int), len(N),
                     int(B), overlaps, overlaps_P)
 
-    ## Free up memory
-    #rm(D, S)
-    #del D
-    #del S
-
     #ipdb.set_trace(context=6)   ## BREAKPOINT
-    reprotable.iloc[i] = np.mean(cResults["overlaps"], axis=0) #colMeans(cResults[["overlaps"]])
-    reprotable_P.iloc[i] = np.mean(cResults["overlaps_P"], axis=0) #colMeans(cResults[["overlaps_P"]])
+    
+    reprotable.iloc[i] = np.mean(cResults["overlaps"], axis=0) 
+    reprotable_P.iloc[i] = np.mean(cResults["overlaps_P"], axis=0)
     ## Standard deviation for each column
     #sqrt(rowSums((t(cResults[["overlaps"]]) - reprotable[i,])^2) / (nrow(cResults[["overlaps"]]) - 1))
     #reprotable_sd.iloc[i] = np.std(cResults["overlaps"])
     reprotable_sd.iloc[i] = np.sqrt(np.sum((cResults["overlaps"].T - reprotable.iloc[i].values[0])**2, axis=1) / 
                                       (cResults["overlaps"].shape[0] - 1))[0]
 
-    ## Free up memory
-    ##del overlaps
-    #del overlaps_P
-    #del cResults
-
     ## -------------------------------------------------------------------------
 
     ## Calculate the Z-statistic and find the top list size and the
     ## (a1,a2)-combination giving the maximal Z-value
-    ztable = (reprotable - reprotable_P) / reprotable_sd
     ## Rownames of ztable are c(ssq, "slr") and colnames are N
-
-    ztable = ztable.infer_objects()
-
-    ## Free up memory
-    #del reprotable_P
-    #del reprotable_sd
+    ztable = (reprotable - reprotable_P) / reprotable_sd    
+    ztable = ztable.infer_objects()    
     
     sel = np.unravel_index(np.argmax(ztable[np.isfinite(ztable)]), ztable.shape) #np.where(ztable == max(ztable[is.finite(ztable)]), arr.ind=TRUE)
     ## Sel is a matrix containing the location(s) of the largest value (row,
     ## col). If the location of the largest value is not unique then nrow(sel)
     ## > 2 (length(sel) > 2)
-
-    #ipdb.set_trace(context=6)   ## BREAKPOINT
+    
     if len(sel) > 2:
       sel = sel[0:2]
 
     if sel[0] < len(reprotable)-1:
       a1 = float(reprotable.index[sel[0]])
       a2 = 1
     
     if sel[0] == len(reprotable)-1:
       a1 = 1
       a2 = 0
     
     k = int(reprotable.columns[sel[1]])
     R = reprotable.iloc[sel[0],sel[1]]
     Z = ztable.iloc[sel[0],sel[1]]
-    
-    ## Free up memory
-    #del reprotable
-    
-    #ipdb.set_trace(context=6)   ## BREAKPOINT
+   
     ## Calculate the reproducibility-optimized test statistic based on the
     ## reproducibility-maximizing a1, a2 and k values and the corresponding FDR      
     #fit = testStatistic(paired, lapply(split(1:len(cl), cl), function(x) data[:,x]))
     fit = testStatistic(paired, np.split(data.to_numpy(), np.where(np.diff(cl) != 0)[0] + 1, axis=1))
     d = fit['d'] / (a1 + a2 * fit['s'])
     pD = pD/(a1 + a2 * pS)
```

