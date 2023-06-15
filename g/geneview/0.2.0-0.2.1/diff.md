# Comparing `tmp/geneview-0.2.0.tar.gz` & `tmp/geneview-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/geneview-0.2.0.tar", last modified: Wed Jun 14 02:16:55 2023, max compression
+gzip compressed data, was "dist/geneview-0.2.1.tar", last modified: Thu Jun 15 02:42:35 2023, max compression
```

## Comparing `geneview-0.2.0.tar` & `geneview-0.2.1.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 huangshujia   (501) staff       (20)        0 2023-06-14 02:16:55.975234 geneview-0.2.0/
--rw-r--r--   0 huangshujia   (501) staff       (20)    15671 2023-06-14 02:16:55.974323 geneview-0.2.0/PKG-INFO
--rw-r--r--   0 huangshujia   (501) staff       (20)    11957 2023-06-14 02:12:24.000000 geneview-0.2.0/README.md
-drwxr-xr-x   0 huangshujia   (501) staff       (20)        0 2023-06-14 02:16:55.831253 geneview-0.2.0/geneview/
--rw-r--r--   0 huangshujia   (501) staff       (20)      508 2023-06-14 01:55:50.000000 geneview-0.2.0/geneview/__init__.py
-drwxr-xr-x   0 huangshujia   (501) staff       (20)        0 2023-06-14 02:16:55.851199 geneview-0.2.0/geneview/algorithm/
--rw-r--r--   0 huangshujia   (501) staff       (20)       42 2021-04-30 15:11:56.000000 geneview-0.2.0/geneview/algorithm/__init__.py
--rw-r--r--   0 huangshujia   (501) staff       (20)     4790 2021-06-02 00:32:31.000000 geneview-0.2.0/geneview/algorithm/_cluster.py
-drwxr-xr-x   0 huangshujia   (501) staff       (20)        0 2023-06-14 02:16:55.864070 geneview-0.2.0/geneview/baseplot/
--rw-r--r--   0 huangshujia   (501) staff       (20)       47 2021-05-06 07:48:03.000000 geneview-0.2.0/geneview/baseplot/__init__.py
--rw-r--r--   0 huangshujia   (501) staff       (20)        0 2021-05-13 09:00:18.000000 geneview-0.2.0/geneview/baseplot/_forest.py
--rw-r--r--   0 huangshujia   (501) staff       (20)    21012 2021-05-27 09:15:06.000000 geneview-0.2.0/geneview/baseplot/_venn.py
--rw-r--r--   0 huangshujia   (501) staff       (20)     5443 2021-05-13 02:30:08.000000 geneview-0.2.0/geneview/conftest.py
-drwxr-xr-x   0 huangshujia   (501) staff       (20)        0 2023-06-14 02:16:55.868054 geneview-0.2.0/geneview/genome_tracks/
--rw-r--r--   0 huangshujia   (501) staff       (20)      209 2021-05-25 08:54:56.000000 geneview-0.2.0/geneview/genome_tracks/__init__.py
-drwxr-xr-x   0 huangshujia   (501) staff       (20)        0 2023-06-14 02:16:55.894755 geneview-0.2.0/geneview/gwas/
--rw-r--r--   0 huangshujia   (501) staff       (20)       70 2021-05-11 03:58:13.000000 geneview-0.2.0/geneview/gwas/__init__.py
--rw-r--r--   0 huangshujia   (501) staff       (20)       78 2021-05-13 09:06:32.000000 geneview-0.2.0/geneview/gwas/_locuszoom.py
--rw-r--r--   0 huangshujia   (501) staff       (20)    15669 2022-08-18 13:19:47.000000 geneview-0.2.0/geneview/gwas/_manhattan.py
--rw-r--r--   0 huangshujia   (501) staff       (20)    11066 2022-01-10 13:44:21.000000 geneview-0.2.0/geneview/gwas/_qq.py
-drwxr-xr-x   0 huangshujia   (501) staff       (20)        0 2023-06-14 02:16:55.901201 geneview-0.2.0/geneview/karyotype/
--rw-r--r--   0 huangshujia   (501) staff       (20)       34 2021-02-04 01:48:57.000000 geneview-0.2.0/geneview/karyotype/__init__.py
--rw-r--r--   0 huangshujia   (501) staff       (20)     3149 2021-05-13 05:13:25.000000 geneview-0.2.0/geneview/karyotype/_karyotype.py
-drwxr-xr-x   0 huangshujia   (501) staff       (20)        0 2023-06-14 02:16:55.914605 geneview-0.2.0/geneview/palette/
--rw-r--r--   0 huangshujia   (501) staff       (20)      234 2021-05-02 15:17:42.000000 geneview-0.2.0/geneview/palette/__init__.py
--rw-r--r--   0 huangshujia   (501) staff       (20)     6932 2021-02-04 01:48:57.000000 geneview-0.2.0/geneview/palette/_circos.py
--rw-r--r--   0 huangshujia   (501) staff       (20)      494 2021-05-05 03:00:12.000000 geneview-0.2.0/geneview/palette/_palettes.py
--rw-r--r--   0 huangshujia   (501) staff       (20)    35446 2021-02-04 01:48:57.000000 geneview-0.2.0/geneview/palette/_xkcd_rgb.py
-drwxr-xr-x   0 huangshujia   (501) staff       (20)        0 2023-06-14 02:16:55.937636 geneview-0.2.0/geneview/popgene/
--rw-r--r--   0 huangshujia   (501) staff       (20)       38 2023-06-13 16:36:36.000000 geneview-0.2.0/geneview/popgene/__init__.py
--rw-r--r--   0 huangshujia   (501) staff       (20)    13782 2023-06-14 01:50:37.000000 geneview-0.2.0/geneview/popgene/_admixture.py
--rw-r--r--   0 huangshujia   (501) staff       (20)        0 2021-06-03 02:43:17.000000 geneview-0.2.0/geneview/popgene/_ldblock.py
-drwxr-xr-x   0 huangshujia   (501) staff       (20)        0 2023-06-14 02:16:55.940419 geneview-0.2.0/geneview/tests/
--rw-r--r--   0 huangshujia   (501) staff       (20)        0 2021-02-04 01:48:57.000000 geneview-0.2.0/geneview/tests/__init__.py
--rw-r--r--   0 huangshujia   (501) staff       (20)        0 2021-05-11 03:56:07.000000 geneview-0.2.0/geneview/tests/test_algorithms.py
--rw-r--r--   0 huangshujia   (501) staff       (20)     2370 2021-05-11 03:54:37.000000 geneview-0.2.0/geneview/tests/test_decorators.py
-drwxr-xr-x   0 huangshujia   (501) staff       (20)        0 2023-06-14 02:16:55.968981 geneview-0.2.0/geneview/utils/
--rw-r--r--   0 huangshujia   (501) staff       (20)      612 2021-05-14 06:52:45.000000 geneview-0.2.0/geneview/utils/__init__.py
--rw-r--r--   0 huangshujia   (501) staff       (20)    26871 2021-04-27 08:42:56.000000 geneview-0.2.0/geneview/utils/_adjust_text.py
--rw-r--r--   0 huangshujia   (501) staff       (20)     2842 2021-05-14 06:18:34.000000 geneview-0.2.0/geneview/utils/_dataset.py
--rw-r--r--   0 huangshujia   (501) staff       (20)     2153 2021-05-14 06:43:50.000000 geneview-0.2.0/geneview/utils/_decorators.py
--rw-r--r--   0 huangshujia   (501) staff       (20)      922 2021-05-14 06:41:43.000000 geneview-0.2.0/geneview/utils/_misc.py
-drwxr-xr-x   0 huangshujia   (501) staff       (20)        0 2023-06-14 02:16:55.841642 geneview-0.2.0/geneview.egg-info/
--rw-r--r--   0 huangshujia   (501) staff       (20)    15671 2023-06-14 02:16:54.000000 geneview-0.2.0/geneview.egg-info/PKG-INFO
--rw-r--r--   0 huangshujia   (501) staff       (20)     1009 2023-06-14 02:16:54.000000 geneview-0.2.0/geneview.egg-info/SOURCES.txt
--rw-r--r--   0 huangshujia   (501) staff       (20)        1 2023-06-14 02:16:54.000000 geneview-0.2.0/geneview.egg-info/dependency_links.txt
--rw-r--r--   0 huangshujia   (501) staff       (20)       38 2023-06-14 02:16:54.000000 geneview-0.2.0/geneview.egg-info/requires.txt
--rw-r--r--   0 huangshujia   (501) staff       (20)        9 2023-06-14 02:16:54.000000 geneview-0.2.0/geneview.egg-info/top_level.txt
--rw-r--r--   0 huangshujia   (501) staff       (20)       38 2023-06-14 02:16:55.975676 geneview-0.2.0/setup.cfg
--rw-r--r--   0 huangshujia   (501) staff       (20)     2325 2023-06-14 02:13:16.000000 geneview-0.2.0/setup.py
+drwxr-xr-x   0 huangshujia   (501) staff       (20)        0 2023-06-15 02:42:35.839734 geneview-0.2.1/
+-rw-r--r--   0 huangshujia   (501) staff       (20)    15671 2023-06-15 02:42:35.838936 geneview-0.2.1/PKG-INFO
+-rw-r--r--   0 huangshujia   (501) staff       (20)    11957 2023-06-14 02:12:24.000000 geneview-0.2.1/README.md
+drwxr-xr-x   0 huangshujia   (501) staff       (20)        0 2023-06-15 02:42:35.735700 geneview-0.2.1/geneview/
+-rw-r--r--   0 huangshujia   (501) staff       (20)      508 2023-06-14 01:55:50.000000 geneview-0.2.1/geneview/__init__.py
+drwxr-xr-x   0 huangshujia   (501) staff       (20)        0 2023-06-15 02:42:35.747370 geneview-0.2.1/geneview/algorithm/
+-rw-r--r--   0 huangshujia   (501) staff       (20)       42 2021-04-30 15:11:56.000000 geneview-0.2.1/geneview/algorithm/__init__.py
+-rw-r--r--   0 huangshujia   (501) staff       (20)     4790 2021-06-02 00:32:31.000000 geneview-0.2.1/geneview/algorithm/_cluster.py
+drwxr-xr-x   0 huangshujia   (501) staff       (20)        0 2023-06-15 02:42:35.755756 geneview-0.2.1/geneview/baseplot/
+-rw-r--r--   0 huangshujia   (501) staff       (20)       47 2021-05-06 07:48:03.000000 geneview-0.2.1/geneview/baseplot/__init__.py
+-rw-r--r--   0 huangshujia   (501) staff       (20)        0 2021-05-13 09:00:18.000000 geneview-0.2.1/geneview/baseplot/_forest.py
+-rw-r--r--   0 huangshujia   (501) staff       (20)    21012 2021-05-27 09:15:06.000000 geneview-0.2.1/geneview/baseplot/_venn.py
+-rw-r--r--   0 huangshujia   (501) staff       (20)     5443 2021-05-13 02:30:08.000000 geneview-0.2.1/geneview/conftest.py
+drwxr-xr-x   0 huangshujia   (501) staff       (20)        0 2023-06-15 02:42:35.760952 geneview-0.2.1/geneview/genome_tracks/
+-rw-r--r--   0 huangshujia   (501) staff       (20)      209 2021-05-25 08:54:56.000000 geneview-0.2.1/geneview/genome_tracks/__init__.py
+drwxr-xr-x   0 huangshujia   (501) staff       (20)        0 2023-06-15 02:42:35.781701 geneview-0.2.1/geneview/gwas/
+-rw-r--r--   0 huangshujia   (501) staff       (20)       70 2021-05-11 03:58:13.000000 geneview-0.2.1/geneview/gwas/__init__.py
+-rw-r--r--   0 huangshujia   (501) staff       (20)       78 2021-05-13 09:06:32.000000 geneview-0.2.1/geneview/gwas/_locuszoom.py
+-rw-r--r--   0 huangshujia   (501) staff       (20)    15669 2022-08-18 13:19:47.000000 geneview-0.2.1/geneview/gwas/_manhattan.py
+-rw-r--r--   0 huangshujia   (501) staff       (20)    11066 2022-01-10 13:44:21.000000 geneview-0.2.1/geneview/gwas/_qq.py
+drwxr-xr-x   0 huangshujia   (501) staff       (20)        0 2023-06-15 02:42:35.788903 geneview-0.2.1/geneview/karyotype/
+-rw-r--r--   0 huangshujia   (501) staff       (20)       34 2021-02-04 01:48:57.000000 geneview-0.2.1/geneview/karyotype/__init__.py
+-rw-r--r--   0 huangshujia   (501) staff       (20)     3149 2021-05-13 05:13:25.000000 geneview-0.2.1/geneview/karyotype/_karyotype.py
+drwxr-xr-x   0 huangshujia   (501) staff       (20)        0 2023-06-15 02:42:35.804866 geneview-0.2.1/geneview/palette/
+-rw-r--r--   0 huangshujia   (501) staff       (20)      234 2021-05-02 15:17:42.000000 geneview-0.2.1/geneview/palette/__init__.py
+-rw-r--r--   0 huangshujia   (501) staff       (20)     6932 2021-02-04 01:48:57.000000 geneview-0.2.1/geneview/palette/_circos.py
+-rw-r--r--   0 huangshujia   (501) staff       (20)      494 2021-05-05 03:00:12.000000 geneview-0.2.1/geneview/palette/_palettes.py
+-rw-r--r--   0 huangshujia   (501) staff       (20)    35446 2021-02-04 01:48:57.000000 geneview-0.2.1/geneview/palette/_xkcd_rgb.py
+drwxr-xr-x   0 huangshujia   (501) staff       (20)        0 2023-06-15 02:42:35.816511 geneview-0.2.1/geneview/popgene/
+-rw-r--r--   0 huangshujia   (501) staff       (20)       38 2023-06-13 16:36:36.000000 geneview-0.2.1/geneview/popgene/__init__.py
+-rw-r--r--   0 huangshujia   (501) staff       (20)    14211 2023-06-15 02:31:44.000000 geneview-0.2.1/geneview/popgene/_admixture.py
+-rw-r--r--   0 huangshujia   (501) staff       (20)        0 2021-06-03 02:43:17.000000 geneview-0.2.1/geneview/popgene/_ldblock.py
+drwxr-xr-x   0 huangshujia   (501) staff       (20)        0 2023-06-15 02:42:35.818363 geneview-0.2.1/geneview/tests/
+-rw-r--r--   0 huangshujia   (501) staff       (20)        0 2021-02-04 01:48:57.000000 geneview-0.2.1/geneview/tests/__init__.py
+-rw-r--r--   0 huangshujia   (501) staff       (20)        0 2021-05-11 03:56:07.000000 geneview-0.2.1/geneview/tests/test_algorithms.py
+-rw-r--r--   0 huangshujia   (501) staff       (20)     2370 2021-05-11 03:54:37.000000 geneview-0.2.1/geneview/tests/test_decorators.py
+drwxr-xr-x   0 huangshujia   (501) staff       (20)        0 2023-06-15 02:42:35.833394 geneview-0.2.1/geneview/utils/
+-rw-r--r--   0 huangshujia   (501) staff       (20)      612 2021-05-14 06:52:45.000000 geneview-0.2.1/geneview/utils/__init__.py
+-rw-r--r--   0 huangshujia   (501) staff       (20)    26871 2021-04-27 08:42:56.000000 geneview-0.2.1/geneview/utils/_adjust_text.py
+-rw-r--r--   0 huangshujia   (501) staff       (20)     2842 2021-05-14 06:18:34.000000 geneview-0.2.1/geneview/utils/_dataset.py
+-rw-r--r--   0 huangshujia   (501) staff       (20)     2153 2021-05-14 06:43:50.000000 geneview-0.2.1/geneview/utils/_decorators.py
+-rw-r--r--   0 huangshujia   (501) staff       (20)      922 2021-05-14 06:41:43.000000 geneview-0.2.1/geneview/utils/_misc.py
+drwxr-xr-x   0 huangshujia   (501) staff       (20)        0 2023-06-15 02:42:35.745270 geneview-0.2.1/geneview.egg-info/
+-rw-r--r--   0 huangshujia   (501) staff       (20)    15671 2023-06-15 02:42:34.000000 geneview-0.2.1/geneview.egg-info/PKG-INFO
+-rw-r--r--   0 huangshujia   (501) staff       (20)     1009 2023-06-15 02:42:34.000000 geneview-0.2.1/geneview.egg-info/SOURCES.txt
+-rw-r--r--   0 huangshujia   (501) staff       (20)        1 2023-06-15 02:42:34.000000 geneview-0.2.1/geneview.egg-info/dependency_links.txt
+-rw-r--r--   0 huangshujia   (501) staff       (20)       38 2023-06-15 02:42:34.000000 geneview-0.2.1/geneview.egg-info/requires.txt
+-rw-r--r--   0 huangshujia   (501) staff       (20)        9 2023-06-15 02:42:34.000000 geneview-0.2.1/geneview.egg-info/top_level.txt
+-rw-r--r--   0 huangshujia   (501) staff       (20)       38 2023-06-15 02:42:35.840027 geneview-0.2.1/setup.cfg
+-rw-r--r--   0 huangshujia   (501) staff       (20)     2325 2023-06-15 02:41:43.000000 geneview-0.2.1/setup.py
```

### Comparing `geneview-0.2.0/PKG-INFO` & `geneview-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geneview
-Version: 0.2.0
+Version: 0.2.1
 Summary: Geneview: A python package for genomics data visualization.
 Home-page: https://github.com/ShujiaHuang/geneview
 Author: Shujia Huang
 Author-email: huangshujia9@gmail.com
 Maintainer: Shujia Huang
 Maintainer-email: huangshujia9@gmail.com
 License: BSD (3-clause)
```

### Comparing `geneview-0.2.0/README.md` & `geneview-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `geneview-0.2.0/geneview/algorithm/_cluster.py` & `geneview-0.2.1/geneview/algorithm/_cluster.py`

 * *Files identical despite different names*

### Comparing `geneview-0.2.0/geneview/baseplot/_venn.py` & `geneview-0.2.1/geneview/baseplot/_venn.py`

 * *Files identical despite different names*

### Comparing `geneview-0.2.0/geneview/conftest.py` & `geneview-0.2.1/geneview/conftest.py`

 * *Files identical despite different names*

### Comparing `geneview-0.2.0/geneview/gwas/_manhattan.py` & `geneview-0.2.1/geneview/gwas/_manhattan.py`

 * *Files identical despite different names*

### Comparing `geneview-0.2.0/geneview/gwas/_qq.py` & `geneview-0.2.1/geneview/gwas/_qq.py`

 * *Files identical despite different names*

### Comparing `geneview-0.2.0/geneview/karyotype/_karyotype.py` & `geneview-0.2.1/geneview/karyotype/_karyotype.py`

 * *Files identical despite different names*

### Comparing `geneview-0.2.0/geneview/palette/_circos.py` & `geneview-0.2.1/geneview/palette/_circos.py`

 * *Files identical despite different names*

### Comparing `geneview-0.2.0/geneview/palette/_xkcd_rgb.py` & `geneview-0.2.1/geneview/palette/_xkcd_rgb.py`

 * *Files identical despite different names*

### Comparing `geneview-0.2.0/geneview/popgene/_admixture.py` & `geneview-0.2.1/geneview/popgene/_admixture.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,14 +21,15 @@
         edgewidth=1.0,
         palette="tab10",
         xticklabels=None,
         xticklabel_kws=None,
         ylabel=None,
         ylabel_kws=None,
         hierarchical_kws=None,
+        set_xticklabel_top=False,
         ax=None
 ):
     """Plot admixture.
 
     Parameters
     ----------
     data : dict.
@@ -102,14 +103,17 @@
         ax.axvline(x=g_pos, color="k", lw=linewidth)
 
     ax.spines["left"].set_linewidth(edgewidth)
     ax.spines["top"].set_linewidth(edgewidth)
     ax.spines["right"].set_linewidth(edgewidth)
     ax.spines["bottom"].set_linewidth(edgewidth)
 
+    if set_xticklabel_top:
+        ax.xaxis.tick_top()
+
     ax.set_xlim([x[0], x[-1]+bar_width])
     ax.set_ylim([0, 1.0])
     ax.tick_params(bottom=False, top=False, left=False, right=False)
 
     if xticklabel_kws is None:
         xticklabel_kws = {}
 
@@ -170,14 +174,15 @@
         edgewidth=1.0,
         palette="tab10",
         xticklabels=None,
         xticklabel_kws=None,
         ylabel=None,
         ylabel_kws=None,
         hierarchical_kws=None,
+        set_xticklabel_top=False,
         ax=None
 ):
     """Plot admixture.
 
         Parameters
         ----------
         data : a file path to the admixture output(.Q) or a dict.
@@ -224,14 +229,17 @@
             Other keyword arguments are passed to set y label in
             ``maplotlib.axis.Axes.set_ylabel``.
 
         hierarchical_kws : key, value pairings, or None, optional
             Other keyword arguments are passed to set the hierarchical clustering in
             ``geneview.algorithm.hierarchical_cluster``.
 
+        set_xticklabel_top : bool, optional
+            Place the x-axis ticklabels at the top of the image. Default: False
+
         ax : matplotlib axis, optional
             Axis to plot on, otherwise define a subplot by ``admixtureplot()``.
 
         Returns
         -------
         ax : matplotlib Axes
             Axes object with the admixtureplot.
@@ -244,14 +252,15 @@
         .. plot::
             :context: close-figs
 
             >>> from geneview.utils import load_dataset
             >>> from geneview import admixtureplot
             >>> admixture_fn = load_dataset("admixture_output.Q")
             >>> population_fn = load_dataset("admixture_population.info")
+            >>> ax = admixtureplot(data=admixture_fn, population_info=population_fn, set_xticklabel_top=True)
             >>> ax = admixtureplot(data=admixture_fn, population_info=population_fn)
 
         Plot the admixture by a specify population order
 
         .. plot::
             :context: close-figs
 
@@ -346,8 +355,9 @@
                                edgewidth=edgewidth,
                                palette=palette,
                                xticklabels=xticklabels,
                                xticklabel_kws=xticklabel_kws,
                                ylabel=ylabel,
                                ylabel_kws=ylabel_kws,
                                hierarchical_kws=hierarchical_kws,
+                               set_xticklabel_top=set_xticklabel_top,
                                ax=ax)
```

### Comparing `geneview-0.2.0/geneview/tests/test_decorators.py` & `geneview-0.2.1/geneview/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `geneview-0.2.0/geneview/utils/__init__.py` & `geneview-0.2.1/geneview/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `geneview-0.2.0/geneview/utils/_adjust_text.py` & `geneview-0.2.1/geneview/utils/_adjust_text.py`

 * *Files identical despite different names*

### Comparing `geneview-0.2.0/geneview/utils/_dataset.py` & `geneview-0.2.1/geneview/utils/_dataset.py`

 * *Files identical despite different names*

### Comparing `geneview-0.2.0/geneview/utils/_decorators.py` & `geneview-0.2.1/geneview/utils/_decorators.py`

 * *Files identical despite different names*

### Comparing `geneview-0.2.0/geneview/utils/_misc.py` & `geneview-0.2.1/geneview/utils/_misc.py`

 * *Files identical despite different names*

### Comparing `geneview-0.2.0/geneview.egg-info/PKG-INFO` & `geneview-0.2.1/geneview.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geneview
-Version: 0.2.0
+Version: 0.2.1
 Summary: Geneview: A python package for genomics data visualization.
 Home-page: https://github.com/ShujiaHuang/geneview
 Author: Shujia Huang
 Author-email: huangshujia9@gmail.com
 Maintainer: Shujia Huang
 Maintainer-email: huangshujia9@gmail.com
 License: BSD (3-clause)
```

### Comparing `geneview-0.2.0/geneview.egg-info/SOURCES.txt` & `geneview-0.2.1/geneview.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `geneview-0.2.0/setup.py` & `geneview-0.2.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 meta = Namespace(
     __DISTNAME__     = "geneview",
     __AUTHOR__       = "Shujia Huang",
     __AUTHOR_EMAIL__ = "huangshujia9@gmail.com",
     __URL__          = "https://github.com/ShujiaHuang/geneview",
     __LICENSE__      = "BSD (3-clause)",
     __DOWNLOAD_URL__ = "https://github.com/ShujiaHuang/geneview",
-    __VERSION__      = "0.2.0",
+    __VERSION__      = "0.2.1",
 )
 
 try:
     from setuptools import setup, find_packages
     _has_setuptools = True
 except ImportError:
     from distutils.core import setup, find_packages
```

