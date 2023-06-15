# Comparing `tmp/mlbi_at_dku_lib-0.1.4.tar.gz` & `tmp/mlbi_at_dku_lib-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlbi_at_dku_lib-0.1.4.tar", last modified: Thu Jun  8 06:54:08 2023, max compression
+gzip compressed data, was "mlbi_at_dku_lib-0.1.5.tar", last modified: Thu Jun 15 02:08:06 2023, max compression
```

## Comparing `mlbi_at_dku_lib-0.1.4.tar` & `mlbi_at_dku_lib-0.1.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-06-08 06:54:08.909526 mlbi_at_dku_lib-0.1.4/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    35821 2023-05-23 01:43:50.000000 mlbi_at_dku_lib-0.1.4/LICENSE
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       60 2023-05-23 01:43:50.000000 mlbi_at_dku_lib-0.1.4/MANIFEST.in
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      832 2023-06-08 06:54:08.909526 mlbi_at_dku_lib-0.1.4/PKG-INFO
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      175 2023-05-23 01:43:50.000000 mlbi_at_dku_lib-0.1.4/README.md
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-06-08 06:54:08.909526 mlbi_at_dku_lib-0.1.4/mlbi_at_dku_lib/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      163 2023-05-22 09:19:00.000000 mlbi_at_dku_lib-0.1.4/mlbi_at_dku_lib/__init__.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)     9379 2023-05-23 01:44:36.000000 mlbi_at_dku_lib-0.1.4/mlbi_at_dku_lib/cpdb.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)     5445 2023-06-08 06:50:28.000000 mlbi_at_dku_lib-0.1.4/mlbi_at_dku_lib/deiso.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    12716 2023-05-23 01:44:36.000000 mlbi_at_dku_lib-0.1.4/mlbi_at_dku_lib/gsea.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    30883 2023-05-23 01:44:36.000000 mlbi_at_dku_lib-0.1.4/mlbi_at_dku_lib/icnv.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    32659 2023-05-23 08:25:18.000000 mlbi_at_dku_lib-0.1.4/mlbi_at_dku_lib/misc.py
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-06-08 06:54:08.909526 mlbi_at_dku_lib-0.1.4/mlbi_at_dku_lib.egg-info/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      832 2023-06-08 06:54:08.000000 mlbi_at_dku_lib-0.1.4/mlbi_at_dku_lib.egg-info/PKG-INFO
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      447 2023-06-08 06:54:08.000000 mlbi_at_dku_lib-0.1.4/mlbi_at_dku_lib.egg-info/SOURCES.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)        1 2023-06-08 06:54:08.000000 mlbi_at_dku_lib-0.1.4/mlbi_at_dku_lib.egg-info/dependency_links.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)        1 2023-06-08 06:54:08.000000 mlbi_at_dku_lib-0.1.4/mlbi_at_dku_lib.egg-info/not-zip-safe
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       27 2023-06-08 06:54:08.000000 mlbi_at_dku_lib-0.1.4/mlbi_at_dku_lib.egg-info/requires.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       22 2023-06-08 06:54:08.000000 mlbi_at_dku_lib-0.1.4/mlbi_at_dku_lib.egg-info/top_level.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       79 2023-06-08 06:54:08.909526 mlbi_at_dku_lib-0.1.4/setup.cfg
--rw-rw-r--   0 syoon     (1001) syoon     (1001)     2823 2023-06-08 06:51:51.000000 mlbi_at_dku_lib-0.1.4/setup.py
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-06-08 06:54:08.909526 mlbi_at_dku_lib-0.1.4/tests/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      124 2023-05-22 09:19:00.000000 mlbi_at_dku_lib-0.1.4/tests/__init__.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-06-15 02:08:06.478702 mlbi_at_dku_lib-0.1.5/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    35821 2023-05-23 01:43:50.000000 mlbi_at_dku_lib-0.1.5/LICENSE
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       60 2023-05-23 01:43:50.000000 mlbi_at_dku_lib-0.1.5/MANIFEST.in
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      832 2023-06-15 02:08:06.478702 mlbi_at_dku_lib-0.1.5/PKG-INFO
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      175 2023-05-23 01:43:50.000000 mlbi_at_dku_lib-0.1.5/README.md
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-06-15 02:08:06.474702 mlbi_at_dku_lib-0.1.5/mlbi_at_dku_lib/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      163 2023-05-22 09:19:00.000000 mlbi_at_dku_lib-0.1.5/mlbi_at_dku_lib/__init__.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)     9385 2023-06-12 09:03:17.000000 mlbi_at_dku_lib-0.1.5/mlbi_at_dku_lib/cpdb.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)     5445 2023-06-08 06:50:28.000000 mlbi_at_dku_lib-0.1.5/mlbi_at_dku_lib/deiso.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    12716 2023-05-23 01:44:36.000000 mlbi_at_dku_lib-0.1.5/mlbi_at_dku_lib/gsea.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    30883 2023-05-23 01:44:36.000000 mlbi_at_dku_lib-0.1.5/mlbi_at_dku_lib/icnv.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    37174 2023-06-15 02:06:24.000000 mlbi_at_dku_lib-0.1.5/mlbi_at_dku_lib/misc.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-06-15 02:08:06.478702 mlbi_at_dku_lib-0.1.5/mlbi_at_dku_lib.egg-info/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      832 2023-06-15 02:08:06.000000 mlbi_at_dku_lib-0.1.5/mlbi_at_dku_lib.egg-info/PKG-INFO
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      447 2023-06-15 02:08:06.000000 mlbi_at_dku_lib-0.1.5/mlbi_at_dku_lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)        1 2023-06-15 02:08:06.000000 mlbi_at_dku_lib-0.1.5/mlbi_at_dku_lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)        1 2023-06-08 06:54:08.000000 mlbi_at_dku_lib-0.1.5/mlbi_at_dku_lib.egg-info/not-zip-safe
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       27 2023-06-15 02:08:06.000000 mlbi_at_dku_lib-0.1.5/mlbi_at_dku_lib.egg-info/requires.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       22 2023-06-15 02:08:06.000000 mlbi_at_dku_lib-0.1.5/mlbi_at_dku_lib.egg-info/top_level.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       79 2023-06-15 02:08:06.478702 mlbi_at_dku_lib-0.1.5/setup.cfg
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)     2823 2023-06-15 02:07:40.000000 mlbi_at_dku_lib-0.1.5/setup.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-06-15 02:08:06.478702 mlbi_at_dku_lib-0.1.5/tests/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      124 2023-05-22 09:19:00.000000 mlbi_at_dku_lib-0.1.5/tests/__init__.py
```

### Comparing `mlbi_at_dku_lib-0.1.4/LICENSE` & `mlbi_at_dku_lib-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mlbi_at_dku_lib-0.1.4/PKG-INFO` & `mlbi_at_dku_lib-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlbi_at_dku_lib
-Version: 0.1.4
+Version: 0.1.5
 Summary: Toolkits for single-cell RNA-Seq data analysis. (Wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)
 Home-page: https://github.com/combio-dku
 Download-URL: https://github.com/combio-dku
 Author: Seokhyun Yoon
 Author-email: syoon@dku.edu
 Keywords: pypi mlbi_at_dku_lib
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mlbi_at_dku_lib-0.1.4/mlbi_at_dku_lib/cpdb.py` & `mlbi_at_dku_lib-0.1.5/mlbi_at_dku_lib/cpdb.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
                     
         exit_code = p.poll()
     return exit_code
 
 
 def cpdb_run( df_cell_by_gene, cell_types, out_dir,
               gene_id_type = 'gene_name', db = None, 
-              n_iter = None, pval_th = None, mean_th = None):
+              n_iter = None, pval_th = None, threshold = None):
     
     start = time.time()
     print('Running CellPhoneDB .. ')    
     X = df_cell_by_gene.astype(int) 
     ## X = (X.div(X.sum(axis = 1), axis=0)*1e6).astype(int)
     
     if out_dir[-1] == '/':
@@ -47,15 +47,15 @@
                                index = X.index.values)    
     df_celltype.to_csv(file_meta, sep = '\t')
     
     cmd = 'cellphonedb method statistical_analysis '
     cmd = cmd + '%s %s ' % (file_meta, file_cpm)
     cmd = cmd + '--counts-data=%s ' % gene_id_type
     if pval_th is not None: cmd = cmd + '--pvalue=%f ' % pval_th
-    if mean_th is not None: cmd = cmd + '--threshold=%f ' % mean_th
+    if threshold is not None: cmd = cmd + '--threshold=%f ' % threshold
     if n_iter is not None: cmd = cmd + '--iterations=%i ' % n_iter
     if db is not None: '--database %s ' % db
     cmd = cmd + '--output-path %s ' % out_dir
 
     with warnings.catch_warnings():
         warnings.simplefilter("ignore")
         run_command(cmd)
```

### Comparing `mlbi_at_dku_lib-0.1.4/mlbi_at_dku_lib/deiso.py` & `mlbi_at_dku_lib-0.1.5/mlbi_at_dku_lib/deiso.py`

 * *Files identical despite different names*

### Comparing `mlbi_at_dku_lib-0.1.4/mlbi_at_dku_lib/gsea.py` & `mlbi_at_dku_lib-0.1.5/mlbi_at_dku_lib/gsea.py`

 * *Files identical despite different names*

### Comparing `mlbi_at_dku_lib-0.1.4/mlbi_at_dku_lib/icnv.py` & `mlbi_at_dku_lib-0.1.5/mlbi_at_dku_lib/icnv.py`

 * *Files identical despite different names*

### Comparing `mlbi_at_dku_lib-0.1.4/mlbi_at_dku_lib/misc.py` & `mlbi_at_dku_lib-0.1.5/mlbi_at_dku_lib/misc.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import time, os, copy, datetime, math, random, warnings
 import numpy as np
 import pandas as pd
 import scanpy as sc
+import seaborn as sns
+from statannot import add_stat_annotation
 import matplotlib.pyplot as plt
 from matplotlib import cm
 from MarkerCount.hicat import get_markers_cell_type, get_markers_minor_type2, get_markers_major_type
 
 try:
     import plotly.graph_objects as go
 except ImportError:
@@ -172,34 +174,159 @@
         b = np.array(pids) == pid
         ct_sel = np.array(cts)[b]
 
         for ct in celltype_lst:
             bx = ct_sel == ct
             df_celltype_cnt.loc[pid, ct] = np.sum(bx)
 
-    df_celltype_pct = df_celltype_cnt.div(df_celltype_cnt.sum(axis = 1), axis = 0)*100
+    df_celltype_pct = (df_celltype_cnt.div(df_celltype_cnt.sum(axis = 1), axis = 0)*100).astype(float)
     
     if len(sort_by) > 0:
         df_celltype_pct.sort_values(by = sort_by, inplace = True)
 
     return df_celltype_cnt, df_celltype_pct
 
 
-def plot_population(df_celltype_pct, figsize=(5, 3), dpi = 80, return_fig = False):    
-
-    # sc.settings.set_figure_params(figsize=figsize, dpi=dpi, facecolor='white')
-    ax = df_celltype_pct.plot.bar(stacked = True, rot = 90)
-    ax.legend( df_celltype_pct.columns.values, bbox_to_anchor=(1, 1) )
+def plot_population(df_celltype_pct, title = None, title_fs = 12, 
+                    label_fs = 11, tick_fs = 10, tick_rot = 45,
+                    legend_fs = 10, legend_loc = 'upper left', bbox_to_anchor = (1,1), 
+                    figsize=(5, 3), return_fig = False):    
+
+    ax = df_celltype_pct.plot.bar(stacked = True, rot = tick_rot, figsize = figsize)
+    ax.legend( df_celltype_pct.columns.values, bbox_to_anchor=bbox_to_anchor, 
+               loc = legend_loc, fontsize = legend_fs )
+    plt.xticks(fontsize=tick_fs)
+    plt.yticks(fontsize=tick_fs)
+    plt.ylabel('Percentage [%]', fontsize = label_fs)
+    plt.title(title, fontsize = title_fs)
     if return_fig:
         return ax
     else:
         plt.show()
         return
     return
 
+
+def plot_population_g(df_pct, sg_map, sort_by = [], title = None, title_y = 1.05, title_fs = 14, 
+                    title_fs2 = 12, label_fs = 11, tick_fs = 10, tick_rot = 45,
+                    legend_fs = 10, legend_loc = 'upper left', bbox_to_anchor = (1,1), 
+                    figsize=(5, 3), return_fig = False):    
+    
+    df = df_pct.copy(deep = True)
+
+    items = list(df.columns.values)
+
+    df['Group'] = list(df.index.values)
+    df['Group'].replace(sg_map, inplace = True)
+
+    num_p = []
+
+    glst = list(df['Group'].unique())
+    glst.sort()
+
+    cnt = df['Group'].value_counts()
+    for g in glst:
+        num_p.append(cnt.loc[g])
+
+    nr, nc = 1, len(glst)
+    fig, axes = plt.subplots(nrows=nr, ncols=nc, constrained_layout=True, 
+                             gridspec_kw={'width_ratios': num_p})
+    fig.tight_layout() 
+    if title is not None: 
+        fig.suptitle(title, x = 0.5, y = title_y, fontsize = title_fs, ha = 'center')
+    plt.subplots_adjust(left=None, bottom=None, right=None, top=None, wspace=0.06, hspace=0.25)
+
+    cnt = 0
+    for j, g in enumerate(glst):
+        b = df['Group'] == g
+        dft = df.loc[b,:]
+        if len(sort_by) > 0:
+            dft = dft.sort_values(sort_by)
+        ax = dft.plot.bar(width = 0.75, stacked = True, ax = axes[j+cnt], 
+                          figsize = figsize, legend = None)
+        ax.set_title('%s' % (g), fontsize = title_fs2)
+        if j == 2: 
+            plt.legend(loc = 'upper left', bbox_to_anchor = (1,1), fontsize = legend_fs)  
+        else:
+            pass
+        if j != 0:
+            ax.set_yticks([])
+        else:
+            ax.set_ylabel('Proportion', fontsize = label_fs)
+
+        ax.tick_params(axis='x', labelsize=tick_fs, rotation = tick_rot)
+        ax.tick_params(axis='y', labelsize=tick_fs)
+            
+    plt.show()
+    
+    return
+
+
+def get_sample_to_group_dict( samples, conditions ):
+    slst = list(set(list(samples)))
+    slst.sort()
+    glst = []
+    for s in slst:
+        b = samples == s
+        g = conditions[b][0]
+        glst.append(g)
+        
+    dct = dict(zip(slst, glst))
+    return dct
+
+
+def plot_pct_box(df_pct, sg_map, nr_nc, figsize = None, dpi = 100,
+                 title = None, title_y = 1.05, title_fs = 14, 
+                 title_fs2 = 12, label_fs = 11, tick_fs = 10, tick_rot = 0, 
+                 annot_fs = 10, ws_hs = (0.3, 0.3)):
+    
+    df = df_pct.copy(deep = True)
+    nr, nc = nr_nc
+    ws, hs = ws_hs
+    fig, axes = plt.subplots(figsize=figsize, dpi=dpi, nrows=nr, ncols=nc, constrained_layout=True)
+    fig.tight_layout() # Or equivalently,  "plt.tight_layout()"
+    if title is not None:
+        fig.suptitle('%s' % title, x = 0.5, y = title_y, fontsize = title_fs, ha = 'center')
+    plt.subplots_adjust(left=None, bottom=None, right=None, top=None, wspace=ws, hspace=hs)
+
+    items = list(df.columns.values)
+
+    df['Group'] = list(df.index.values)
+    df['Group'].replace(sg_map, inplace = True)
+
+    lst = df['Group'].unique()
+    lst_pair = []
+    for k, l1 in enumerate(lst):
+        for j, l2 in enumerate(lst):
+            if j >  k:
+                lst_pair.append((l1, l2))
+
+    for k, item in enumerate(items):
+        plt.subplot(nr,nc,k+1)
+        ax = sns.boxplot(data = df, x = 'Group', y = item) #, order=['HC', 'CC', 'AC'])
+        if k%nc == 0: plt.ylabel('Percentage', fontsize = label_fs)
+        else: plt.ylabel(None)
+        if k >= nc*(nr-1): plt.xlabel('Condition', fontsize = label_fs)
+        else: plt.xlabel(None)
+        plt.title(item, fontsize = title_fs2)
+        if k < (nr*nc - nc):
+            plt.xticks([])
+            plt.yticks(fontsize = tick_fs)
+        else:
+            plt.xticks(rotation = 0, ha = 'center', fontsize = tick_fs)
+            plt.yticks(fontsize = tick_fs)
+
+        add_stat_annotation(ax, data=df, x = 'Group', y = item, # order=['HC', 'CC', 'AC'],
+                        box_pairs=lst_pair, loc='inside', fontsize = annot_fs,
+                        test='t-test_ind', text_format='simple', verbose=0)
+        #'''
+    plt.show()
+    return
+
+
 def plot_composition_bar( adata_t,  pid_field = 'pid', cell_type_field = 'cell_type_major_pred',
                           sort_by = [] ):
     
     pid_lst = list(adata_t.obs[pid_field].unique())
 
     ct_idx = cell_type_field
     celltype_lst = list(adata_t.obs[ct_idx].unique())
@@ -216,20 +343,21 @@
             df_celltype_cnt.loc[pid, ct] = np.sum(bx)
 
     df_celltype_pct = df_celltype_cnt.div(df_celltype_cnt.sum(axis = 1), axis = 0)*100
     
     if len(sort_by) > 0:
         df_celltype_pct.sort_values(by = sort_by, inplace = True)
 
-    # sc.settings.set_figure_params(figsize=(5, 3), dpi=80, facecolor='white')
+    sc.settings.set_figure_params(figsize=(5, 3), dpi=80, facecolor='white')
     ax = df_celltype_pct.plot.bar(stacked = True, rot = 90)
     ax.legend( df_celltype_pct.columns.values, bbox_to_anchor=(1, 1) )
     
     return df_celltype_cnt
 
+
 '''
 ### DigitalCellSorter
 
 ## df_ann = cell_type_id_using_DCS( df, name = 'DCS_tmp', batch = None, mkr = 'CIBERSORT_LM22_7', n_clust = 30 )
 
 import urllib.request
 import DigitalCellSorter
```

### Comparing `mlbi_at_dku_lib-0.1.4/mlbi_at_dku_lib.egg-info/PKG-INFO` & `mlbi_at_dku_lib-0.1.5/mlbi_at_dku_lib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlbi-at-dku-lib
-Version: 0.1.4
+Version: 0.1.5
 Summary: Toolkits for single-cell RNA-Seq data analysis. (Wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)
 Home-page: https://github.com/combio-dku
 Download-URL: https://github.com/combio-dku
 Author: Seokhyun Yoon
 Author-email: syoon@dku.edu
 Keywords: pypi mlbi_at_dku_lib
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mlbi_at_dku_lib-0.1.4/setup.py` & `mlbi_at_dku_lib-0.1.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 setup(
     # 배포할 패키지의 이름을 적어줍니다. setup.py파일을 가지는 폴더 이름과 동일하게 합니다.
     name                = 'mlbi_at_dku_lib',
     # 배포할 패키지의 버전을 적어줍니다. 첫 등록이므로 0.1 또는 0.0.1을 사용합니다.
-    version             = '0.1.4',
+    version             = '0.1.5',
     # 배포할 패키지에 대한 설명을 작성합니다.
     description         = 'Toolkits for single-cell RNA-Seq data analysis. (Wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)',
     # 배포하는 사람의 이름을 작성합니다.
     author              = 'Seokhyun Yoon',
     # 배포하는 사람의 메일주소를 작성합니다.
     author_email        = 'syoon@dku.edu',
     # 배포하는 패키지의 url을 적어줍니다. 보통 github 링크를 적습니다.
```

