# Comparing `tmp/peakachu-2.2.tar.gz` & `tmp/peakachu-2.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peakachu-2.2.tar", last modified: Mon May 22 01:34:10 2023, max compression
+gzip compressed data, was "peakachu-2.2.post1.tar", last modified: Thu Jun 15 01:24:53 2023, max compression
```

## Comparing `peakachu-2.2.tar` & `peakachu-2.2.post1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 xiaotaowang   (501) staff       (20)        0 2023-05-22 01:34:10.342982 peakachu-2.2/
--rw-r--r--   0 xiaotaowang   (501) staff       (20)     1063 2023-05-22 01:34:00.000000 peakachu-2.2/LICENSE
--rw-r--r--   0 xiaotaowang   (501) staff       (20)    81407 2023-05-22 01:34:10.342850 peakachu-2.2/PKG-INFO
--rw-r--r--   0 xiaotaowang   (501) staff       (20)    80675 2023-05-22 01:34:00.000000 peakachu-2.2/README.md
-drwxr-xr-x   0 xiaotaowang   (501) staff       (20)        0 2023-05-22 01:34:10.342148 peakachu-2.2/peakachu/
--rwxr-xr-x   0 xiaotaowang   (501) staff       (20)      103 2023-05-22 01:34:00.000000 peakachu-2.2/peakachu/__init__.py
--rwxr-xr-x   0 xiaotaowang   (501) staff       (20)     2316 2023-05-22 01:34:00.000000 peakachu-2.2/peakachu/calculate_depth.py
--rw-r--r--   0 xiaotaowang   (501) staff       (20)      850 2023-05-22 01:34:00.000000 peakachu-2.2/peakachu/call_loops.py
--rwxr-xr-x   0 xiaotaowang   (501) staff       (20)     5829 2023-05-22 01:34:00.000000 peakachu-2.2/peakachu/peakacluster.py
--rw-r--r--   0 xiaotaowang   (501) staff       (20)     5166 2023-05-22 01:34:00.000000 peakachu-2.2/peakachu/scoreUtils.py
--rwxr-xr-x   0 xiaotaowang   (501) staff       (20)     2755 2023-05-22 01:34:00.000000 peakachu-2.2/peakachu/score_chromosome.py
--rwxr-xr-x   0 xiaotaowang   (501) staff       (20)     3250 2023-05-22 01:34:00.000000 peakachu-2.2/peakachu/score_genome.py
--rwxr-xr-x   0 xiaotaowang   (501) staff       (20)     4843 2023-05-22 01:34:00.000000 peakachu-2.2/peakachu/trainUtils.py
--rwxr-xr-x   0 xiaotaowang   (501) staff       (20)     3642 2023-05-22 01:34:00.000000 peakachu-2.2/peakachu/train_models.py
--rw-r--r--   0 xiaotaowang   (501) staff       (20)     6417 2023-05-22 01:34:00.000000 peakachu-2.2/peakachu/utils.py
-drwxr-xr-x   0 xiaotaowang   (501) staff       (20)        0 2023-05-22 01:34:10.342594 peakachu-2.2/peakachu.egg-info/
--rw-r--r--   0 xiaotaowang   (501) staff       (20)    81407 2023-05-22 01:34:10.000000 peakachu-2.2/peakachu.egg-info/PKG-INFO
--rw-r--r--   0 xiaotaowang   (501) staff       (20)      411 2023-05-22 01:34:10.000000 peakachu-2.2/peakachu.egg-info/SOURCES.txt
--rw-r--r--   0 xiaotaowang   (501) staff       (20)        1 2023-05-22 01:34:10.000000 peakachu-2.2/peakachu.egg-info/dependency_links.txt
--rw-r--r--   0 xiaotaowang   (501) staff       (20)        9 2023-05-22 01:34:10.000000 peakachu-2.2/peakachu.egg-info/top_level.txt
-drwxr-xr-x   0 xiaotaowang   (501) staff       (20)        0 2023-05-22 01:34:10.342699 peakachu-2.2/scripts/
--rwxr-xr-x   0 xiaotaowang   (501) staff       (20)     4945 2023-05-22 01:34:10.000000 peakachu-2.2/scripts/peakachu
--rw-r--r--   0 xiaotaowang   (501) staff       (20)       38 2023-05-22 01:34:10.343026 peakachu-2.2/setup.cfg
--rw-r--r--   0 xiaotaowang   (501) staff       (20)     1649 2023-05-22 01:34:00.000000 peakachu-2.2/setup.py
+drwxr-xr-x   0 xiaotaowang   (501) staff       (20)        0 2023-06-15 01:24:53.770492 peakachu-2.2.post1/
+-rw-r--r--   0 xiaotaowang   (501) staff       (20)     1063 2023-06-15 01:24:22.000000 peakachu-2.2.post1/LICENSE
+-rw-r--r--   0 xiaotaowang   (501) staff       (20)    81413 2023-06-15 01:24:53.770360 peakachu-2.2.post1/PKG-INFO
+-rw-r--r--   0 xiaotaowang   (501) staff       (20)    80675 2023-06-15 01:24:22.000000 peakachu-2.2.post1/README.md
+drwxr-xr-x   0 xiaotaowang   (501) staff       (20)        0 2023-06-15 01:24:53.769560 peakachu-2.2.post1/peakachu/
+-rwxr-xr-x   0 xiaotaowang   (501) staff       (20)      106 2023-06-15 01:24:22.000000 peakachu-2.2.post1/peakachu/__init__.py
+-rwxr-xr-x   0 xiaotaowang   (501) staff       (20)     2316 2023-06-15 01:24:22.000000 peakachu-2.2.post1/peakachu/calculate_depth.py
+-rw-r--r--   0 xiaotaowang   (501) staff       (20)      850 2023-06-15 01:24:22.000000 peakachu-2.2.post1/peakachu/call_loops.py
+-rwxr-xr-x   0 xiaotaowang   (501) staff       (20)     5831 2023-06-15 01:24:22.000000 peakachu-2.2.post1/peakachu/peakacluster.py
+-rw-r--r--   0 xiaotaowang   (501) staff       (20)     5166 2023-06-15 01:24:22.000000 peakachu-2.2.post1/peakachu/scoreUtils.py
+-rwxr-xr-x   0 xiaotaowang   (501) staff       (20)     2755 2023-06-15 01:24:22.000000 peakachu-2.2.post1/peakachu/score_chromosome.py
+-rwxr-xr-x   0 xiaotaowang   (501) staff       (20)     3250 2023-06-15 01:24:22.000000 peakachu-2.2.post1/peakachu/score_genome.py
+-rwxr-xr-x   0 xiaotaowang   (501) staff       (20)     4843 2023-06-15 01:24:22.000000 peakachu-2.2.post1/peakachu/trainUtils.py
+-rwxr-xr-x   0 xiaotaowang   (501) staff       (20)     3642 2023-06-15 01:24:22.000000 peakachu-2.2.post1/peakachu/train_models.py
+-rw-r--r--   0 xiaotaowang   (501) staff       (20)     6417 2023-06-15 01:24:22.000000 peakachu-2.2.post1/peakachu/utils.py
+drwxr-xr-x   0 xiaotaowang   (501) staff       (20)        0 2023-06-15 01:24:53.770037 peakachu-2.2.post1/peakachu.egg-info/
+-rw-r--r--   0 xiaotaowang   (501) staff       (20)    81413 2023-06-15 01:24:53.000000 peakachu-2.2.post1/peakachu.egg-info/PKG-INFO
+-rw-r--r--   0 xiaotaowang   (501) staff       (20)      411 2023-06-15 01:24:53.000000 peakachu-2.2.post1/peakachu.egg-info/SOURCES.txt
+-rw-r--r--   0 xiaotaowang   (501) staff       (20)        1 2023-06-15 01:24:53.000000 peakachu-2.2.post1/peakachu.egg-info/dependency_links.txt
+-rw-r--r--   0 xiaotaowang   (501) staff       (20)        9 2023-06-15 01:24:53.000000 peakachu-2.2.post1/peakachu.egg-info/top_level.txt
+drwxr-xr-x   0 xiaotaowang   (501) staff       (20)        0 2023-06-15 01:24:53.770165 peakachu-2.2.post1/scripts/
+-rwxr-xr-x   0 xiaotaowang   (501) staff       (20)     4945 2023-06-15 01:24:53.000000 peakachu-2.2.post1/scripts/peakachu
+-rw-r--r--   0 xiaotaowang   (501) staff       (20)       38 2023-06-15 01:24:53.770522 peakachu-2.2.post1/setup.cfg
+-rw-r--r--   0 xiaotaowang   (501) staff       (20)     1649 2023-06-15 01:24:22.000000 peakachu-2.2.post1/setup.py
```

### Comparing `peakachu-2.2/LICENSE` & `peakachu-2.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `peakachu-2.2/PKG-INFO` & `peakachu-2.2.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peakachu
-Version: 2.2
+Version: 2.2.post1
 Summary: A supervised learning framework for chromatin loop detection in genome-wide contact maps.
 Home-page: https://github.com/tariks/peakachu/
 Author: Xiaotao Wang and Tarik Salameh
 Author-email: wangxiaotao686@gmail.com
 Keywords: Hi-C chromatin interaction contact loop peak cooler
 Classifier: Programming Language :: Python :: 3.6
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `peakachu-2.2/README.md` & `peakachu-2.2.post1/README.md`

 * *Files identical despite different names*

### Comparing `peakachu-2.2/peakachu/calculate_depth.py` & `peakachu-2.2.post1/peakachu/calculate_depth.py`

 * *Files identical despite different names*

### Comparing `peakachu-2.2/peakachu/call_loops.py` & `peakachu-2.2.post1/peakachu/call_loops.py`

 * *Files identical despite different names*

### Comparing `peakachu-2.2/peakachu/peakacluster.py` & `peakachu-2.2.post1/peakachu/peakacluster.py`

 * *Files 0% similar despite different names*

```diff
@@ -119,15 +119,15 @@
                         out.append(tuple(q))
                 if len(out)==ini:
                     break
                 ini = len(out)
                 tmp = np.r_[Local]
                 # assign centroid to a certain pixel
                 cen = tuple(tmp.mean(axis=0).round().astype(int))
-                rad = np.int(np.round(max([euclidean(cen,q) for q in Local]))) + r
+                rad = np.int64(np.round(max([euclidean(cen,q) for q in Local]))) + r
                 sub = np.r_[out]
             for q in Local:
                 pool.add(q)
             final_list.append((p[1], cen, rad))
         
         visited.update(pool)
```

### Comparing `peakachu-2.2/peakachu/scoreUtils.py` & `peakachu-2.2.post1/peakachu/scoreUtils.py`

 * *Files identical despite different names*

### Comparing `peakachu-2.2/peakachu/score_chromosome.py` & `peakachu-2.2.post1/peakachu/score_chromosome.py`

 * *Files identical despite different names*

### Comparing `peakachu-2.2/peakachu/score_genome.py` & `peakachu-2.2.post1/peakachu/score_genome.py`

 * *Files identical despite different names*

### Comparing `peakachu-2.2/peakachu/trainUtils.py` & `peakachu-2.2.post1/peakachu/trainUtils.py`

 * *Files identical despite different names*

### Comparing `peakachu-2.2/peakachu/train_models.py` & `peakachu-2.2.post1/peakachu/train_models.py`

 * *Files identical despite different names*

### Comparing `peakachu-2.2/peakachu/utils.py` & `peakachu-2.2.post1/peakachu/utils.py`

 * *Files identical despite different names*

### Comparing `peakachu-2.2/peakachu.egg-info/PKG-INFO` & `peakachu-2.2.post1/peakachu.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peakachu
-Version: 2.2
+Version: 2.2.post1
 Summary: A supervised learning framework for chromatin loop detection in genome-wide contact maps.
 Home-page: https://github.com/tariks/peakachu/
 Author: Xiaotao Wang and Tarik Salameh
 Author-email: wangxiaotao686@gmail.com
 Keywords: Hi-C chromatin interaction contact loop peak cooler
 Classifier: Programming Language :: Python :: 3.6
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `peakachu-2.2/scripts/peakachu` & `peakachu-2.2.post1/scripts/peakachu`

 * *Files identical despite different names*

### Comparing `peakachu-2.2/setup.py` & `peakachu-2.2.post1/setup.py`

 * *Files identical despite different names*

