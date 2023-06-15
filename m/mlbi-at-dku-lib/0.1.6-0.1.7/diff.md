# Comparing `tmp/mlbi_at_dku_lib-0.1.6.tar.gz` & `tmp/mlbi_at_dku_lib-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlbi_at_dku_lib-0.1.6.tar", last modified: Thu Jun 15 04:25:33 2023, max compression
+gzip compressed data, was "mlbi_at_dku_lib-0.1.7.tar", last modified: Thu Jun 15 08:57:00 2023, max compression
```

## Comparing `mlbi_at_dku_lib-0.1.6.tar` & `mlbi_at_dku_lib-0.1.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-06-15 04:25:33.547876 mlbi_at_dku_lib-0.1.6/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    35821 2023-05-23 01:43:50.000000 mlbi_at_dku_lib-0.1.6/LICENSE
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       60 2023-05-23 01:43:50.000000 mlbi_at_dku_lib-0.1.6/MANIFEST.in
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      832 2023-06-15 04:25:33.547876 mlbi_at_dku_lib-0.1.6/PKG-INFO
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      175 2023-05-23 01:43:50.000000 mlbi_at_dku_lib-0.1.6/README.md
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-06-15 04:25:33.547876 mlbi_at_dku_lib-0.1.6/mlbi_at_dku_lib/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      163 2023-05-22 09:19:00.000000 mlbi_at_dku_lib-0.1.6/mlbi_at_dku_lib/__init__.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)     9385 2023-06-12 09:03:17.000000 mlbi_at_dku_lib-0.1.6/mlbi_at_dku_lib/cpdb.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)     5445 2023-06-08 06:50:28.000000 mlbi_at_dku_lib-0.1.6/mlbi_at_dku_lib/deiso.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    12716 2023-05-23 01:44:36.000000 mlbi_at_dku_lib-0.1.6/mlbi_at_dku_lib/gsea.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    30883 2023-05-23 01:44:36.000000 mlbi_at_dku_lib-0.1.6/mlbi_at_dku_lib/icnv.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    37323 2023-06-15 04:24:26.000000 mlbi_at_dku_lib-0.1.6/mlbi_at_dku_lib/misc.py
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-06-15 04:25:33.547876 mlbi_at_dku_lib-0.1.6/mlbi_at_dku_lib.egg-info/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      832 2023-06-15 04:25:33.000000 mlbi_at_dku_lib-0.1.6/mlbi_at_dku_lib.egg-info/PKG-INFO
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      447 2023-06-15 04:25:33.000000 mlbi_at_dku_lib-0.1.6/mlbi_at_dku_lib.egg-info/SOURCES.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)        1 2023-06-15 04:25:33.000000 mlbi_at_dku_lib-0.1.6/mlbi_at_dku_lib.egg-info/dependency_links.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)        1 2023-06-08 06:54:08.000000 mlbi_at_dku_lib-0.1.6/mlbi_at_dku_lib.egg-info/not-zip-safe
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       27 2023-06-15 04:25:33.000000 mlbi_at_dku_lib-0.1.6/mlbi_at_dku_lib.egg-info/requires.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       22 2023-06-15 04:25:33.000000 mlbi_at_dku_lib-0.1.6/mlbi_at_dku_lib.egg-info/top_level.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       79 2023-06-15 04:25:33.547876 mlbi_at_dku_lib-0.1.6/setup.cfg
--rw-rw-r--   0 syoon     (1001) syoon     (1001)     2823 2023-06-15 04:25:27.000000 mlbi_at_dku_lib-0.1.6/setup.py
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-06-15 04:25:33.547876 mlbi_at_dku_lib-0.1.6/tests/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      124 2023-05-22 09:19:00.000000 mlbi_at_dku_lib-0.1.6/tests/__init__.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-06-15 08:57:00.805514 mlbi_at_dku_lib-0.1.7/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    35821 2023-05-23 01:43:50.000000 mlbi_at_dku_lib-0.1.7/LICENSE
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       60 2023-05-23 01:43:50.000000 mlbi_at_dku_lib-0.1.7/MANIFEST.in
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      832 2023-06-15 08:57:00.805514 mlbi_at_dku_lib-0.1.7/PKG-INFO
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      175 2023-05-23 01:43:50.000000 mlbi_at_dku_lib-0.1.7/README.md
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-06-15 08:57:00.805514 mlbi_at_dku_lib-0.1.7/mlbi_at_dku_lib/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      163 2023-05-22 09:19:00.000000 mlbi_at_dku_lib-0.1.7/mlbi_at_dku_lib/__init__.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)     9385 2023-06-12 09:03:17.000000 mlbi_at_dku_lib-0.1.7/mlbi_at_dku_lib/cpdb.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)     6012 2023-06-15 08:56:21.000000 mlbi_at_dku_lib-0.1.7/mlbi_at_dku_lib/deiso.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    12716 2023-05-23 01:44:36.000000 mlbi_at_dku_lib-0.1.7/mlbi_at_dku_lib/gsea.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    30883 2023-05-23 01:44:36.000000 mlbi_at_dku_lib-0.1.7/mlbi_at_dku_lib/icnv.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    37323 2023-06-15 04:24:26.000000 mlbi_at_dku_lib-0.1.7/mlbi_at_dku_lib/misc.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-06-15 08:57:00.805514 mlbi_at_dku_lib-0.1.7/mlbi_at_dku_lib.egg-info/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      832 2023-06-15 08:57:00.000000 mlbi_at_dku_lib-0.1.7/mlbi_at_dku_lib.egg-info/PKG-INFO
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      447 2023-06-15 08:57:00.000000 mlbi_at_dku_lib-0.1.7/mlbi_at_dku_lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)        1 2023-06-15 08:57:00.000000 mlbi_at_dku_lib-0.1.7/mlbi_at_dku_lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)        1 2023-06-08 06:54:08.000000 mlbi_at_dku_lib-0.1.7/mlbi_at_dku_lib.egg-info/not-zip-safe
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       27 2023-06-15 08:57:00.000000 mlbi_at_dku_lib-0.1.7/mlbi_at_dku_lib.egg-info/requires.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       22 2023-06-15 08:57:00.000000 mlbi_at_dku_lib-0.1.7/mlbi_at_dku_lib.egg-info/top_level.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       79 2023-06-15 08:57:00.805514 mlbi_at_dku_lib-0.1.7/setup.cfg
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)     2823 2023-06-15 08:56:42.000000 mlbi_at_dku_lib-0.1.7/setup.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-06-15 08:57:00.805514 mlbi_at_dku_lib-0.1.7/tests/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      124 2023-05-22 09:19:00.000000 mlbi_at_dku_lib-0.1.7/tests/__init__.py
```

### Comparing `mlbi_at_dku_lib-0.1.6/LICENSE` & `mlbi_at_dku_lib-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `mlbi_at_dku_lib-0.1.6/PKG-INFO` & `mlbi_at_dku_lib-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlbi_at_dku_lib
-Version: 0.1.6
+Version: 0.1.7
 Summary: Toolkits for single-cell RNA-Seq data analysis. (Wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)
 Home-page: https://github.com/combio-dku
 Download-URL: https://github.com/combio-dku
 Author: Seokhyun Yoon
 Author-email: syoon@dku.edu
 Keywords: pypi mlbi_at_dku_lib
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mlbi_at_dku_lib-0.1.6/mlbi_at_dku_lib/cpdb.py` & `mlbi_at_dku_lib-0.1.7/mlbi_at_dku_lib/cpdb.py`

 * *Files identical despite different names*

### Comparing `mlbi_at_dku_lib-0.1.6/mlbi_at_dku_lib/deiso.py` & `mlbi_at_dku_lib-0.1.7/mlbi_at_dku_lib/deiso.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import time, os, sys
+import time, os, sys, warnings
 import numpy as np
 import pandas as pd
 from scipy import stats
 
 SKLEARN = True
 try:
     from sklearn.decomposition import PCA
@@ -16,14 +16,21 @@
     rownames = ['PC%i' % (i+1) for i in range(int(n_comp))]
     pca_obj = PCA(n_components=int(n_comp))
     X_pca = pca_obj.fit_transform(dfs.transpose()).transpose()  
     df_pca = pd.DataFrame(X_pca, index = rownames, columns = dfs.columns.values)
     return df_pca
 
 
+def get_mean_and_cov(dfx):
+    m = dfx.mean(axis = 1)
+    dfy = dfx.sub(m, axis = 0)
+    C = dfy.dot(dfy.transpose())/(dfy.shape[1]-1)    
+    return m, C 
+
+
 def DEiso_anal_per_gene( dfs_in, groups, gr, norm = False, log = False,
                          n_pca_comp = 0, cn_th = 1e-10, ro = 0.1, nth = 0.8 ):
     
     dfs = dfs_in.copy(deep = True)
     if norm:
         dfs = dfs.div(dfs.sum(axis = 0), axis = 1)*100
         if log:
@@ -45,48 +52,45 @@
     b = np.array(groups) == gr
     ssel = list(samples[b])
     
     bt = ((dfs[ssel] > 0).sum(axis = 0) > 0)
     if bt.sum() < dfs[ssel].shape[1]*nth:
         return None
 
-    Cr = dfs[ssel].transpose().cov()
-    mr = dfs[ssel].mean(axis = 1)
+    # Cr = np.array( dfs[ssel].transpose().cov() )
+    # mr = np.array( dfs[ssel].mean(axis = 1) )
+    mr, Cr = get_mean_and_cov(dfs[ssel])
     
     res = {}
     for i, g in enumerate(glst):
         b = np.array(groups) == g
         ssel = list(samples[b])
         
         bt = ((dfs[ssel] > 0).sum(axis = 0) > 0)
         if bt.sum() >= dfs[ssel].shape[1]*nth:
         
-            Ct = dfs[ssel].transpose().cov()
-            mt = dfs[ssel].mean(axis = 1)
+            # Ct = np.array( dfs[ssel].transpose().cov() )
+            # mt = np.array( dfs[ssel].mean(axis = 1) )
+            mt, Ct = get_mean_and_cov(dfs[ssel])
+            
             m = mt - mr    
 
             C = Cr + Ct
             C = C + (np.diag(C).mean()*ro)*np.eye(C.shape[0])
             if np.linalg.det(C) < cn_th:
                 c1 = 0
             else:
                 C = np.linalg.inv(C)
-                c1 = m.transpose().dot(C.dot(m))
+                c1 = m.dot(C.dot(m))
                 c1 = np.sqrt(c1)
 
                 p1 = stats.t.sf(c1, df = dfs.shape[1])*2
-                res[g] = (c1, p1)
+                res['%s_vs_%s' % (g, gr)] = (c1, p1)
 
-    if len(glst) == 1:
-        if g in list(res.keys()):
-            return res
-        else:
-            return None
-    else:
-        return res    
+    return res    
     
 
 def DEiso_anal( df, gene_names, groups, ref_group, norm = True, log = False, 
                 n_pca_comp = 0, rho = 0.1, nth = 0.8, verbose = True ):
     
     if not SKLEARN:
         print('DEiso ERROR: scikit-learn not installed.', flush=True)
@@ -159,21 +163,35 @@
             b = df_res['pval_adj'] > 1
             df_res.loc[b, 'pval_adj'] = 1
             df_res = df_res.sort_values(['stat'], ascending = False)
        
     return df_res
 
 
-def save_to_excel(df_res_all, file_out):
+def save_to_excel(df_res_all, file_out, pv_cutoff = 0.1):
 
     cnt = 0
     for key in df_res_all.keys():
 
         if cnt == 0: 
             with pd.ExcelWriter(file_out, mode='w') as writer:
-                df_res_all[key].to_excel(writer, sheet_name = key)
+                b = df_res_all[key]['pval'] <= pv_cutoff
+                df_res_all[key].loc[b,:].to_excel(writer, sheet_name = key)
         else: 
             with pd.ExcelWriter(file_out, mode='a', if_sheet_exists = 'replace') as writer:
-                df_res_all[key].to_excel(writer, sheet_name = key)
+                b = df_res_all[key]['pval'] <= pv_cutoff
+                df_res_all[key].loc[b,:].to_excel(writer, sheet_name = key)
         cnt += 1
 
     return
+
+
+def load_excel(file):
+    
+    xls = pd.ExcelFile(file)
+    lst = xls.sheet_names
+    df_res_all = {}
+    for s in lst:
+        df_res_all[s] = pd.read_excel(xls, s, index_col = 0) 
+        
+    return df_res_all
+
```

### Comparing `mlbi_at_dku_lib-0.1.6/mlbi_at_dku_lib/gsea.py` & `mlbi_at_dku_lib-0.1.7/mlbi_at_dku_lib/gsea.py`

 * *Files identical despite different names*

### Comparing `mlbi_at_dku_lib-0.1.6/mlbi_at_dku_lib/icnv.py` & `mlbi_at_dku_lib-0.1.7/mlbi_at_dku_lib/icnv.py`

 * *Files identical despite different names*

### Comparing `mlbi_at_dku_lib-0.1.6/mlbi_at_dku_lib/misc.py` & `mlbi_at_dku_lib-0.1.7/mlbi_at_dku_lib/misc.py`

 * *Files identical despite different names*

### Comparing `mlbi_at_dku_lib-0.1.6/mlbi_at_dku_lib.egg-info/PKG-INFO` & `mlbi_at_dku_lib-0.1.7/mlbi_at_dku_lib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlbi-at-dku-lib
-Version: 0.1.6
+Version: 0.1.7
 Summary: Toolkits for single-cell RNA-Seq data analysis. (Wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)
 Home-page: https://github.com/combio-dku
 Download-URL: https://github.com/combio-dku
 Author: Seokhyun Yoon
 Author-email: syoon@dku.edu
 Keywords: pypi mlbi_at_dku_lib
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mlbi_at_dku_lib-0.1.6/setup.py` & `mlbi_at_dku_lib-0.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 setup(
     # 배포할 패키지의 이름을 적어줍니다. setup.py파일을 가지는 폴더 이름과 동일하게 합니다.
     name                = 'mlbi_at_dku_lib',
     # 배포할 패키지의 버전을 적어줍니다. 첫 등록이므로 0.1 또는 0.0.1을 사용합니다.
-    version             = '0.1.6',
+    version             = '0.1.7',
     # 배포할 패키지에 대한 설명을 작성합니다.
     description         = 'Toolkits for single-cell RNA-Seq data analysis. (Wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)',
     # 배포하는 사람의 이름을 작성합니다.
     author              = 'Seokhyun Yoon',
     # 배포하는 사람의 메일주소를 작성합니다.
     author_email        = 'syoon@dku.edu',
     # 배포하는 패키지의 url을 적어줍니다. 보통 github 링크를 적습니다.
```

