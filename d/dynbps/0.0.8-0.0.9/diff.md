# Comparing `tmp/dynbps-0.0.8.tar.gz` & `tmp/dynbps-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dynbps-0.0.8.tar", last modified: Mon May 22 22:17:46 2023, max compression
+gzip compressed data, was "dist/dynbps-0.0.9.tar", last modified: Wed Jun 14 16:42:04 2023, max compression
```

## Comparing `dynbps-0.0.8.tar` & `dynbps-0.0.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 josephrilling   (501) staff       (20)        0 2023-05-22 22:17:46.353302 dynbps-0.0.8/
--rw-r--r--   0 josephrilling   (501) staff       (20)    11357 2023-05-16 21:26:28.000000 dynbps-0.0.8/LICENSE
--rw-rw-r--   0 josephrilling   (501) staff       (20)      111 2023-04-27 10:12:58.000000 dynbps-0.0.8/MANIFEST.in
--rw-r--r--   0 josephrilling   (501) staff       (20)     7337 2023-05-22 22:17:46.351531 dynbps-0.0.8/PKG-INFO
--rw-r--r--   0 josephrilling   (501) staff       (20)     6570 2023-05-22 22:10:05.000000 dynbps-0.0.8/README.md
-drwxr-xr-x   0 josephrilling   (501) staff       (20)        0 2023-05-22 22:17:46.332153 dynbps-0.0.8/dynbps/
--rw-r--r--   0 josephrilling   (501) staff       (20)     8905 2023-05-22 22:17:36.000000 dynbps-0.0.8/dynbps/BPS.py
--rw-r--r--   0 josephrilling   (501) staff       (20)       22 2023-05-22 22:17:36.000000 dynbps-0.0.8/dynbps/__init__.py
--rw-r--r--   0 josephrilling   (501) staff       (20)      763 2023-05-22 22:17:36.000000 dynbps-0.0.8/dynbps/_modidx.py
-drwxr-xr-x   0 josephrilling   (501) staff       (20)        0 2023-05-22 22:17:46.348316 dynbps-0.0.8/dynbps/datasets/
--rw-r--r--   0 josephrilling   (501) staff       (20)    41999 2023-05-17 22:21:27.000000 dynbps-0.0.8/dynbps/datasets/data.xlsx
--rw-r--r--   0 josephrilling   (501) staff       (20)      747 2023-05-22 22:17:36.000000 dynbps-0.0.8/dynbps/loadData.py
-drwxr-xr-x   0 josephrilling   (501) staff       (20)        0 2023-05-22 22:17:46.347249 dynbps-0.0.8/dynbps.egg-info/
--rw-r--r--   0 josephrilling   (501) staff       (20)     7337 2023-05-22 22:17:46.000000 dynbps-0.0.8/dynbps.egg-info/PKG-INFO
--rw-r--r--   0 josephrilling   (501) staff       (20)      358 2023-05-22 22:17:46.000000 dynbps-0.0.8/dynbps.egg-info/SOURCES.txt
--rw-r--r--   0 josephrilling   (501) staff       (20)        1 2023-05-22 22:17:46.000000 dynbps-0.0.8/dynbps.egg-info/dependency_links.txt
--rw-r--r--   0 josephrilling   (501) staff       (20)       34 2023-05-22 22:17:46.000000 dynbps-0.0.8/dynbps.egg-info/entry_points.txt
--rw-r--r--   0 josephrilling   (501) staff       (20)        1 2023-05-16 21:36:56.000000 dynbps-0.0.8/dynbps.egg-info/not-zip-safe
--rw-r--r--   0 josephrilling   (501) staff       (20)       44 2023-05-22 22:17:46.000000 dynbps-0.0.8/dynbps.egg-info/requires.txt
--rw-r--r--   0 josephrilling   (501) staff       (20)        7 2023-05-22 22:17:46.000000 dynbps-0.0.8/dynbps.egg-info/top_level.txt
--rw-r--r--   0 josephrilling   (501) staff       (20)      839 2023-05-22 22:17:36.000000 dynbps-0.0.8/settings.ini
--rw-r--r--   0 josephrilling   (501) staff       (20)       38 2023-05-22 22:17:46.353588 dynbps-0.0.8/setup.cfg
--rw-rw-r--   0 josephrilling   (501) staff       (20)     2640 2023-05-17 22:24:08.000000 dynbps-0.0.8/setup.py
+drwxr-xr-x   0 josephrilling   (501) staff       (20)        0 2023-06-14 16:42:04.032320 dynbps-0.0.9/
+-rw-r--r--   0 josephrilling   (501) staff       (20)    11357 2023-05-16 21:26:28.000000 dynbps-0.0.9/LICENSE
+-rw-rw-r--   0 josephrilling   (501) staff       (20)      111 2023-04-27 10:12:58.000000 dynbps-0.0.9/MANIFEST.in
+-rw-r--r--   0 josephrilling   (501) staff       (20)     7337 2023-06-14 16:42:04.031797 dynbps-0.0.9/PKG-INFO
+-rw-r--r--   0 josephrilling   (501) staff       (20)     6570 2023-06-14 15:17:50.000000 dynbps-0.0.9/README.md
+drwxr-xr-x   0 josephrilling   (501) staff       (20)        0 2023-06-14 16:42:04.022832 dynbps-0.0.9/dynbps/
+-rw-r--r--   0 josephrilling   (501) staff       (20)     9546 2023-06-14 16:39:09.000000 dynbps-0.0.9/dynbps/BPS.py
+-rw-r--r--   0 josephrilling   (501) staff       (20)       22 2023-06-14 16:39:09.000000 dynbps-0.0.9/dynbps/__init__.py
+-rw-r--r--   0 josephrilling   (501) staff       (20)      763 2023-06-14 16:39:09.000000 dynbps-0.0.9/dynbps/_modidx.py
+drwxr-xr-x   0 josephrilling   (501) staff       (20)        0 2023-06-14 16:42:04.029879 dynbps-0.0.9/dynbps/datasets/
+-rw-r--r--   0 josephrilling   (501) staff       (20)    41999 2023-05-17 22:21:27.000000 dynbps-0.0.9/dynbps/datasets/data.xlsx
+-rw-r--r--   0 josephrilling   (501) staff       (20)      747 2023-06-14 16:39:09.000000 dynbps-0.0.9/dynbps/loadData.py
+drwxr-xr-x   0 josephrilling   (501) staff       (20)        0 2023-06-14 16:42:04.029165 dynbps-0.0.9/dynbps.egg-info/
+-rw-r--r--   0 josephrilling   (501) staff       (20)     7337 2023-06-14 16:42:03.000000 dynbps-0.0.9/dynbps.egg-info/PKG-INFO
+-rw-r--r--   0 josephrilling   (501) staff       (20)      358 2023-06-14 16:42:03.000000 dynbps-0.0.9/dynbps.egg-info/SOURCES.txt
+-rw-r--r--   0 josephrilling   (501) staff       (20)        1 2023-06-14 16:42:03.000000 dynbps-0.0.9/dynbps.egg-info/dependency_links.txt
+-rw-r--r--   0 josephrilling   (501) staff       (20)       34 2023-06-14 16:42:03.000000 dynbps-0.0.9/dynbps.egg-info/entry_points.txt
+-rw-r--r--   0 josephrilling   (501) staff       (20)        1 2023-05-16 21:36:56.000000 dynbps-0.0.9/dynbps.egg-info/not-zip-safe
+-rw-r--r--   0 josephrilling   (501) staff       (20)       44 2023-06-14 16:42:03.000000 dynbps-0.0.9/dynbps.egg-info/requires.txt
+-rw-r--r--   0 josephrilling   (501) staff       (20)        7 2023-06-14 16:42:03.000000 dynbps-0.0.9/dynbps.egg-info/top_level.txt
+-rw-r--r--   0 josephrilling   (501) staff       (20)      839 2023-06-14 16:39:00.000000 dynbps-0.0.9/settings.ini
+-rw-r--r--   0 josephrilling   (501) staff       (20)       38 2023-06-14 16:42:04.032479 dynbps-0.0.9/setup.cfg
+-rw-rw-r--   0 josephrilling   (501) staff       (20)     2640 2023-05-17 22:24:08.000000 dynbps-0.0.9/setup.py
```

### Comparing `dynbps-0.0.8/LICENSE` & `dynbps-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dynbps-0.0.8/PKG-INFO` & `dynbps-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynbps
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python code for Dynamic BPS
 Home-page: https://github.com/josephrilling/dynbps
 Author: josephrilling
 Author-email: tun52698@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dynbps-0.0.8/README.md` & `dynbps-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `dynbps-0.0.8/dynbps/BPS.py` & `dynbps-0.0.9/dynbps/BPS.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,32 +13,51 @@
 class BPS:
     "Bayesian Predictive Synthesis: A latent ensemble forecasting method"
     
     def __init__(self, 
                  y:list, #The true values
                  a_j:'T by J matrix', #Each agent's predicted mean
                  A_j:'T by J matrix', #Each agent's predicted variance
-                 n_j:'T by J matrix', #Each agent's predicted degrees of freedom
-                 delta:list, #Discount factor on [state, observation]
-                 m_0:list, #Prior for coefficients of agent's
-                 C_0:"J by J matrix", #Prior for covariance of agent's
-                 n_0:list, #Prior for degrees of freedom
-                 s_0:float, #Prior for observation variance
-                 burn_in:int, #Iterations for burn in
-                 mcmc_iter:int): #Iterations to keep
+                 n_j:'T by J matrix'=None, #Each agent's predicted degrees of freedom
+                 delta:list = None, #Discount factor on [state, observation]
+                 m_0:list = None, #Prior for coefficients of agent's
+                 C_0:"J by J matrix"= None, #Prior for covariance of agent's
+                 n_0:list= None, #Prior for degrees of freedom
+                 s_0:float = None, #Prior for observation variance
+                 burn_in:int = None, #Iterations for burn in
+                 mcmc_iter:int = None): #Iterations to keep
         self.y = y
         self.a_j = a_j
         self.A_j = A_j
+        self.p_x = A_j.shape[1]
+        self.p = self.p_x+1
+        if n_j is None:
+            n_j = np.full(A_j.shape, 30)
         self.n_j = n_j
+        if delta is None:
+            delta = [0.95,0.99]
         self.delta = delta
+        if m_0 is None:
+            m0 = [0]*(self.p)
+            m0[1:] = [1/self.p_x]*(self.p_x)
         self.m_0 = m_0
+        if C_0 is None:
+            C_0 = np.eye(self.p) * 1 
         self.C_0 = C_0
+        if n_0 is None:
+            n_0 = 1/(1 - delta[1]) # prior on BPS degrees of freedom
         self.n_0 = n_0
+        if s_0 is None:
+            s_0 = 0.01 # prior on BPS observation variance 
         self.s_0 = s_0
+        if burn_in is None:
+            burn_in = 2000
         self.burn_in = burn_in
+        if mcmc_iter is None:
+            mcmc_iter = 3000
         self.mcmc_iter = mcmc_iter
     def fit(self):
                 
         def std_var(x):
             return (x + np.transpose(x))/2
 
         def chol(A):
@@ -50,22 +69,20 @@
         A_j =self.A_j
         n_j =self.n_j 
         delta =self.delta 
         m_0 = self.m_0
         C_0 =self.C_0
         n_0 =self.n_0 
         s_0 =self.s_0 
+        p = self.p
+        p_x = self.p_x
         burn_in = self.burn_in
         mcmc_iter = self.mcmc_iter
         mcmc_iter = self.burn_in + self.mcmc_iter
         T = y.shape[0]
-        p_x = a_j.shape[1]
-        p = p_x + 1
-        self.p = p
-        self.p_x= p_x
         m_t = np.zeros(shape = [T + 1, p])
         C_t = np.zeros(shape = [(T + 1) * p, p])
         n_t = np.zeros(shape = [T + 1, 1])
         s_t = np.zeros(shape = [T + 1, mcmc_iter])
         v_t = np.zeros(shape = [T, mcmc_iter])
         a_t = np.zeros(shape = [T, p])
         R_t = np.zeros(shape = [T * p, p])
```

### Comparing `dynbps-0.0.8/dynbps/_modidx.py` & `dynbps-0.0.9/dynbps/_modidx.py`

 * *Files identical despite different names*

### Comparing `dynbps-0.0.8/dynbps/datasets/data.xlsx` & `dynbps-0.0.9/dynbps/datasets/data.xlsx`

 * *Files identical despite different names*

### Comparing `dynbps-0.0.8/dynbps/loadData.py` & `dynbps-0.0.9/dynbps/loadData.py`

 * *Files identical despite different names*

### Comparing `dynbps-0.0.8/dynbps.egg-info/PKG-INFO` & `dynbps-0.0.9/dynbps.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynbps
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python code for Dynamic BPS
 Home-page: https://github.com/josephrilling/dynbps
 Author: josephrilling
 Author-email: tun52698@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dynbps-0.0.8/settings.ini` & `dynbps-0.0.9/settings.ini`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = dynbps
 lib_name = dynbps
-version = 0.0.8
+version = 0.0.9
 min_python = 3.7
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = dynbps
 nbs_path = nbs
 recursive = True
```

### Comparing `dynbps-0.0.8/setup.py` & `dynbps-0.0.9/setup.py`

 * *Files identical despite different names*

